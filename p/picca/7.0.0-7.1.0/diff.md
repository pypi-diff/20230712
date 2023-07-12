# Comparing `tmp/picca-7.0.0.tar.gz` & `tmp/picca-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picca-7.0.0.tar", last modified: Fri Jun  2 13:23:49 2023, max compression
+gzip compressed data, was "picca-7.1.0.tar", last modified: Wed Jul 12 15:20:10 2023, max compression
```

## Comparing `picca-7.0.0.tar` & `picca-7.1.0.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.968002 picca-7.0.0/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    35141 2021-11-29 16:42:40.000000 picca-7.0.0/LICENSE
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6155 2023-06-02 13:23:49.964002 picca-7.0.0/PKG-INFO
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5828 2023-03-10 09:08:48.000000 picca-7.0.0/README.md
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.952002 picca-7.0.0/bin/
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    24135 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_Pk1D.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10849 2023-06-02 13:08:37.000000 picca-7.0.0/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16058 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_cf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11731 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_cf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11265 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_cf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12071 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14263 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_coadd_zint.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9312 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5833 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     3480 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_convert_transmission.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1908 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_delta_extraction.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15850 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12239 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_export.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14187 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_export_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     4728 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19846 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_metal_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18174 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    27530 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_nersc_submit.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     2201 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_pk2fits.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5870 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1251 2023-03-10 09:08:44.000000 picca-7.0.0/bin/picca_reduce_spall.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19061 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_wick.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16708 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_xcf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12008 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_xcf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    13810 2023-04-14 09:44:54.000000 picca-7.0.0/bin/picca_xcf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15413 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17951 2023-06-01 08:57:46.000000 picca-7.0.0/bin/picca_xwick.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.948002 picca-7.0.0/py/
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.952002 picca-7.0.0/py/picca/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       46 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       22 2023-06-02 13:19:03.000000 picca-7.0.0/py/picca/_version.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3364 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bal_tools.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.956002 picca-7.0.0/py/picca/bin/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)        0 2022-02-03 13:41:19.000000 picca-7.0.0/py/picca/bin/__init__.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.956002 picca-7.0.0/py/picca/bin/old/
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    43689 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_deltas.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      722 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_fitter2.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      575 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_fitter2_control.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)      614 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/old/picca_fitter2_control_mpi.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    24135 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_Pk1D.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    10849 2023-06-02 13:08:37.000000 picca-7.0.0/py/picca/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16058 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_cf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11731 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_cf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    11265 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_cf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12071 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14263 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_coadd_zint.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     9312 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5833 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     3480 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_convert_transmission.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1908 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_delta_extraction.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15850 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12239 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_export.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    14187 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_export_co.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     4728 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19846 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_metal_dmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    18174 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    27530 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_nersc_submit.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     2201 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_pk2fits.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     5870 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     1251 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/bin/picca_reduce_spall.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    19061 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_wick.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    16708 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_xcf.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    12008 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_xcf1d.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    13810 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/bin/picca_xcf_angl.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    15413 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_xdmat.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)    17951 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/bin/picca_xwick.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    64077 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/cf.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7828 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/co.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10611 2023-05-31 16:28:55.000000 picca-7.0.0/py/picca/constants.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    12823 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/converters.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    51080 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/data.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.956002 picca-7.0.0/py/picca/delta_extraction/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5067 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_object.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5729 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9213 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25713 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11372 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5955 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1170 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    27062 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/config.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      941 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/correction.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/corrections/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/corrections/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4062 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/corrections/calibration_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5974 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/corrections/dust_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3454 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/corrections/ivar_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4115 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    22238 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/data.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/data_catalogues/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    14819 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8585 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8906 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2145 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10874 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1131 2023-03-10 09:08:48.000000 picca-7.0.0/py/picca/delta_extraction/errors.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16433 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/expected_flux.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    30238 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3794 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1688 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1718 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2620 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3875 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3970 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1729 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    21268 2022-03-31 16:50:19.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    15906 2022-03-31 16:50:19.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19543 2022-03-31 16:50:19.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19675 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4628 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/expected_fluxes/utils.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/least_squares/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/least_squares/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6416 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7476 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2026 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/delta_extraction/mask.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/masks/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/masks/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     4303 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/delta_extraction/masks/absorber_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8367 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/masks/bal_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9918 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/masks/dla_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3286 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/delta_extraction/masks/lines_mask.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2996 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogue.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8146 2023-03-10 09:08:48.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    12201 2023-03-10 09:08:48.000000 picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1817 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/rejection_log.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.960002 picca-7.0.0/py/picca/delta_extraction/rejection_logs/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/rejection_logs/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     2716 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3275 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8733 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/survey.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11272 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/delta_extraction/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10817 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/delta_extraction/utils_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5953 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/dla.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)        0 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19385 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/chi2.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1031 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/control.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    13706 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/control_mpi.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    20123 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/data.py
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     6784 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/effective-bins.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.948002 picca-7.0.0/py/picca/fitter2/models/
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_large/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_small/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/DR9LyaMocks/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25920 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/Planck18/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2023-01-23 16:50:46.000000 picca-7.0.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/PlanckDR12/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    25920 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/fitter2/models/PlanckDR16/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2021-11-29 16:42:41.000000 picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    28800 2022-02-03 13:41:20.000000 picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1556 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/myGamma.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     8089 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/parser.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16465 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/pk.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      554 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/priors.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     5369 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/sampler.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3921 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10748 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/fitter2/xi.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    64892 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/io.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/pk1d/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19994 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/pk1d/compute_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    38897 2023-06-02 13:08:37.000000 picca-7.0.0/py/picca/pk1d/postproc_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     9245 2023-06-02 13:08:37.000000 picca-7.0.0/py/picca/pk1d/prep_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1071 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/pk1d/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    13939 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/prep_del.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    19665 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/raw_io.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/tests/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      250 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/__init__.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/tests/delta_extraction/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      116 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/__init__.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10670 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/delta_extraction/abstract_test.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    88977 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    23177 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/config_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    10454 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/tests/delta_extraction/correction_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    63846 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/delta_extraction/data_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    81274 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    31778 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/tests/delta_extraction/mask_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    18721 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     6230 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/delta_extraction/scripts_tests.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     7957 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/delta_extraction/test_utils.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.964002 picca-7.0.0/py/picca/tests/old/
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    17429 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/old/test_1_deltas.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3651 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/old/test_4_fitter2.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     3337 2023-05-17 07:27:52.000000 picca-7.0.0/py/picca/tests/test_2_pk1d.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    42559 2023-04-14 09:44:54.000000 picca-7.0.0/py/picca/tests/test_3_cor.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    11334 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/tests/test_helpers.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    16216 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/utils.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1504 2023-03-10 09:08:44.000000 picca-7.0.0/py/picca/wedgize.py
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)    40856 2023-06-01 08:57:46.000000 picca-7.0.0/py/picca/xcf.py
-drwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        0 2023-06-02 13:23:49.952002 picca-7.0.0/py/picca.egg-info/
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     6155 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/PKG-INFO
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)     7168 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/SOURCES.txt
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        1 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/dependency_links.txt
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)       82 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/requires.txt
--rwxr-xr-x   0 michael.walther (24410) ls-gruen (11769)        6 2023-06-02 13:23:49.000000 picca-7.0.0/py/picca.egg-info/top_level.txt
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)      133 2022-03-31 16:50:20.000000 picca-7.0.0/pyproject.toml
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)       38 2023-06-02 13:23:49.968002 picca-7.0.0/setup.cfg
--rw-r--r--   0 michael.walther (24410) ls-gruen (11769)     1236 2023-03-10 09:08:44.000000 picca-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.729496 picca-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-12 15:19:58.000000 picca-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-12 15:20:10.729496 picca-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-12 15:19:58.000000 picca-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.709495 picca-7.1.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12008 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xwick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.705495 picca-7.1.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.713495 picca-7.1.0/py/picca/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bal_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/bin/old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43689 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_deltas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_fitter2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_fitter2_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_fitter2_control_mpi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12008 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xwick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/calibration_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/dust_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/ivar_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/data_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/least_squares/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/least_squares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/masks/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/absorber_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/bal_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/dla_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/lines_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/rejection_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/utils_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/dla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/chi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/control_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/effective-bins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.705495 picca-7.1.0/py/picca/fitter2/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_large/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_small/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/DR9LyaMocks/
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/Planck18/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/PlanckDR12/
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/PlanckDR16/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/myGamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/xi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64892 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/pk1d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/compute_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38897 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/postproc_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/prep_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/prep_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/raw_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.729496 picca-7.1.0/py/picca/tests/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/correction_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81274 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/mask_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/scripts_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.729496 picca-7.1.0/py/picca/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (123)    17429 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/old/test_1_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/old/test_4_fitter2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/test_2_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/test_3_cor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/wedgize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/xcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.713495 picca-7.1.0/py/picca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 15:20:01.000000 picca-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:20:10.729496 picca-7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 15:20:01.000000 picca-7.1.0/setup.py
```

### Comparing `picca-7.0.0/LICENSE` & `picca-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/PKG-INFO` & `picca-7.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: picca
-Version: 7.0.0
-Summary: Package for Igm Cosmological-Correlations Analyses
-Home-page: https://github.com/igmhub/picca
-Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols et al
-Author-email: iprafols@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # picca
 [![Coverage Status](https://coveralls.io/repos/github/igmhub/picca/badge.svg?branch=master)](https://coveralls.io/github/igmhub/picca?branch=master)
 
 Package for Igm Cosmological-Correlations Analyses.
 
 This package contains tools used for the analysis of the Lyman-alpha forest sample from the extended Baryon Oscillation Spectroscopic Survey (eBOSS) and the Dark Energy Spectroscopic Instrument (DESI). Here you will find tools to
 
@@ -169,7 +159,13 @@
    to ensure the coding styles are maintained.
 4. Consider using pylint to help in the debug process. From the repo folder run
    ```
    pylint py/picca/delta_extraction/
    pylint py/picca/pk1d/
    ```
    depending on the module you are working on.
+   
+When merging PRs (or committing to master directly):
+- by default the patch version is increased via a github action, so every change of master will generate a new version
+This behaviour can be changed by adding one of the following to the commit-msg of the merge commit:
+- by specifying [bump minor] or [bump major] a new minor or major version will be generated instead, but tags and releases need to be created manually (and are auto-pushed to pypi when they are created)
+- by specifying [no bump] the version bump can be circumvented altogether when some other behaviour is wanted, in that case bump2version should be run manually
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `picca-7.0.0/README.md` & `picca-7.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: picca
+Version: 7.1.0
+Summary: Package for Igm Cosmological-Correlations Analyses
+Home-page: https://github.com/igmhub/picca
+Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
+Author-email: iprafols@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # picca
 [![Coverage Status](https://coveralls.io/repos/github/igmhub/picca/badge.svg?branch=master)](https://coveralls.io/github/igmhub/picca?branch=master)
 
 Package for Igm Cosmological-Correlations Analyses.
 
 This package contains tools used for the analysis of the Lyman-alpha forest sample from the extended Baryon Oscillation Spectroscopic Survey (eBOSS) and the Dark Energy Spectroscopic Instrument (DESI). Here you will find tools to
 
@@ -159,7 +169,13 @@
    to ensure the coding styles are maintained.
 4. Consider using pylint to help in the debug process. From the repo folder run
    ```
    pylint py/picca/delta_extraction/
    pylint py/picca/pk1d/
    ```
    depending on the module you are working on.
+   
+When merging PRs (or committing to master directly):
+- by default the patch version is increased via a github action, so every change of master will generate a new version
+This behaviour can be changed by adding one of the following to the commit-msg of the merge commit:
+- by specifying [bump minor] or [bump major] a new minor or major version will be generated instead, but tags and releases need to be created manually (and are auto-pushed to pypi when they are created)
+- by specifying [no bump] the version bump can be circumvented altogether when some other behaviour is wanted, in that case bump2version should be run manually
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `picca-7.0.0/bin/picca_Pk1D.py` & `picca-7.1.0/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_Pk1D_postprocess.py` & `picca-7.1.0/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_cf.py` & `picca-7.1.0/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_cf1d.py` & `picca-7.1.0/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_cf_angl.py` & `picca-7.1.0/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_co.py` & `picca-7.1.0/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_coadd_zint.py` & `picca-7.1.0/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_compute_fvoigt.py` & `picca-7.1.0/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_compute_pk_pksb.py` & `picca-7.1.0/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_convert_transmission.py` & `picca-7.1.0/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_delta_extraction.py` & `picca-7.1.0/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_dmat.py` & `picca-7.1.0/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_export.py` & `picca-7.1.0/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_export_co.py` & `picca-7.1.0/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_export_cross_covariance.py` & `picca-7.1.0/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_metal_dmat.py` & `picca-7.1.0/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_metal_xdmat.py` & `picca-7.1.0/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_nersc_submit.py` & `picca-7.1.0/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_pk2fits.py` & `picca-7.1.0/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_plot_pk1d.py` & `picca-7.1.0/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_reduce_spall.py` & `picca-7.1.0/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_wick.py` & `picca-7.1.0/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_xcf.py` & `picca-7.1.0/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_xcf1d.py` & `picca-7.1.0/bin/picca_xcf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_xcf_angl.py` & `picca-7.1.0/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_xdmat.py` & `picca-7.1.0/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/bin/picca_xwick.py` & `picca-7.1.0/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bal_tools.py` & `picca-7.1.0/py/picca/bal_tools.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/old/picca_deltas.py` & `picca-7.1.0/py/picca/bin/old/picca_deltas.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/old/picca_fitter2.py` & `picca-7.1.0/py/picca/bin/old/picca_fitter2.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/old/picca_fitter2_control.py` & `picca-7.1.0/py/picca/bin/old/picca_fitter2_control.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/old/picca_fitter2_control_mpi.py` & `picca-7.1.0/py/picca/bin/old/picca_fitter2_control_mpi.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_Pk1D.py` & `picca-7.1.0/py/picca/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_Pk1D_postprocess.py` & `picca-7.1.0/py/picca/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_cf.py` & `picca-7.1.0/py/picca/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_cf1d.py` & `picca-7.1.0/py/picca/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_cf_angl.py` & `picca-7.1.0/py/picca/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_co.py` & `picca-7.1.0/py/picca/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_coadd_zint.py` & `picca-7.1.0/py/picca/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_compute_fvoigt.py` & `picca-7.1.0/py/picca/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_compute_pk_pksb.py` & `picca-7.1.0/py/picca/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_convert_transmission.py` & `picca-7.1.0/py/picca/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_delta_extraction.py` & `picca-7.1.0/py/picca/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_dmat.py` & `picca-7.1.0/py/picca/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_export.py` & `picca-7.1.0/py/picca/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_export_co.py` & `picca-7.1.0/py/picca/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_export_cross_covariance.py` & `picca-7.1.0/py/picca/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_metal_dmat.py` & `picca-7.1.0/py/picca/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_metal_xdmat.py` & `picca-7.1.0/py/picca/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_nersc_submit.py` & `picca-7.1.0/py/picca/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_pk2fits.py` & `picca-7.1.0/py/picca/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_plot_pk1d.py` & `picca-7.1.0/py/picca/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_reduce_spall.py` & `picca-7.1.0/py/picca/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_wick.py` & `picca-7.1.0/py/picca/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_xcf.py` & `picca-7.1.0/py/picca/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_xcf1d.py` & `picca-7.1.0/py/picca/bin/picca_xcf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_xcf_angl.py` & `picca-7.1.0/py/picca/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_xdmat.py` & `picca-7.1.0/py/picca/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/bin/picca_xwick.py` & `picca-7.1.0/py/picca/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/cf.py` & `picca-7.1.0/py/picca/cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/co.py` & `picca-7.1.0/py/picca/co.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/constants.py` & `picca-7.1.0/py/picca/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,31 +250,34 @@
 
 ### Absorber names and wavelengths [Angstrom]
 ABSORBER_IGM = {
     "Halpha"      : 6562.8,
     "Hbeta"       : 4862.68,
     "MgI(2853)"   : 2852.96,
     "MgII(2804)"  : 2803.5324,
+    "MgII(eff)"   : 2798.75,
     "MgII(2796)"  : 2796.3511,
     "FeII(2600)"  : 2600.1724835,
     "FeII(2587)"  : 2586.6495659,
     "MnII(2577)"  : 2576.877,
     "FeII(2383)"  : 2382.7641781,
     "FeII(2374)"  : 2374.4603294,
     "FeII(2344)"  : 2344.2129601,
+    "CIII(1908)"  : 1908.73,
     "AlIII(1863)" : 1862.79113,
     "AlIII(1855)" : 1854.71829,
     "AlII(1671)"  : 1670.7886,
     "FeII(1608)"  : 1608.4511,
     "CIV(1551)"   : 1550.77845,
     "CIV(eff)"    : 1549.06,
     "CIV(1548)"   : 1548.2049,
     "SiII(1527)"  : 1526.70698,
     "NiII(1455)"  : 1454.842,
     "SiIV(1403)"  : 1402.77291,
+    "SiIV(eff)"   : 1396.76,
     "SiIV(1394)"  : 1393.76018,
     "NiII(1370)"  : 1370.132,
     "CII(1335)"   : 1334.5323,
     "NiII(1317)"  : 1317.217,
     "SiII(1304)"  : 1304.3702,
     "OI(1302)"    : 1302.1685,
     "SiII(1260)"  : 1260.4221,
```

### Comparing `picca-7.0.0/py/picca/converters.py` & `picca-7.1.0/py/picca/converters.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/data.py` & `picca-7.1.0/py/picca/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_object.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_object.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/forest.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py` & `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/config.py` & `picca-7.1.0/py/picca/delta_extraction/config.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/correction.py` & `picca-7.1.0/py/picca/delta_extraction/correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/corrections/calibration_correction.py` & `picca-7.1.0/py/picca/delta_extraction/corrections/calibration_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/corrections/dust_correction.py` & `picca-7.1.0/py/picca/delta_extraction/corrections/dust_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/corrections/ivar_correction.py` & `picca-7.1.0/py/picca/delta_extraction/corrections/ivar_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py` & `picca-7.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/data.py` & `picca-7.1.0/py/picca/delta_extraction/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py` & `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py` & `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py` & `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py` & `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py` & `picca-7.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,22 @@
             try:
                 hdul = fitsio.FITS(filename)
             except IOError:
                 self.logger.warning(f"Error reading {filename}. Ignoring file")
                 continue
             self.logger.progress(f"Read {filename}")
 
-            log_lambda = np.array(hdul[1]["loglam"][:], dtype=np.float64)
-            flux = np.array(hdul[1]["flux"][:], dtype=np.float64)
-            ivar = (np.array(hdul[1]["ivar"][:], dtype=np.float64) *
-                    hdul[1]["and_mask"][:] == 0)
+            try:
+                log_lambda = np.array(hdul[1]["loglam"][:], dtype=np.float64)
+                flux = np.array(hdul[1]["flux"][:], dtype=np.float64)
+                ivar = (np.array(hdul[1]["ivar"][:], dtype=np.float64) *
+                        hdul[1]["and_mask"][:] == 0)
+            except OSError:
+                self.logger.warning(f"Error reading HDU for {filename}. Ignoring file")
+                continue
 
             if self.analysis_type == "BAO 3D":
                 forest = SdssForest(
                     **{
                         "log_lambda": log_lambda,
                         "flux": flux,
                         "ivar": ivar,
```

### Comparing `picca-7.0.0/py/picca/delta_extraction/errors.py` & `picca-7.1.0/py/picca/delta_extraction/errors.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/expected_fluxes/utils.py` & `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py` & `picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py` & `picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/mask.py` & `picca-7.1.0/py/picca/delta_extraction/mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/masks/absorber_mask.py` & `picca-7.1.0/py/picca/delta_extraction/masks/absorber_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/masks/bal_mask.py` & `picca-7.1.0/py/picca/delta_extraction/masks/bal_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/masks/dla_mask.py` & `picca-7.1.0/py/picca/delta_extraction/masks/dla_mask.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This module defines the classes DlaMask and Dla used in the
 masking of DLAs"""
 import logging
 
 from astropy.table import Table
 import fitsio
 import numpy as np
-from numba import njit
+from scipy.constants import speed_of_light as SPEED_LIGHT
+from scipy.special import voigt_profile
 
 from picca.delta_extraction.astronomical_objects.forest import Forest
 from picca.delta_extraction.errors import MaskError
 from picca.delta_extraction.mask import Mask, accepted_options, defaults
 from picca.delta_extraction.utils import (
     ABSORBER_IGM, update_accepted_options, update_default_options)
 
@@ -19,20 +20,21 @@
 
 defaults = update_default_options(
     defaults, {
         "dla mask limit": 0.8,
         "los_id name": "THING_ID",
     })
 
-np.random.seed(0)
-NUM_POINTS = 10000
-GAUSSIAN_DIST = np.random.normal(size=NUM_POINTS) * np.sqrt(2)
-
+LAMBDA_LYA = float(ABSORBER_IGM["LYA"]) ## Lya wavelength [A]
+LAMBDA_LYB = float(ABSORBER_IGM["LYB"]) ## Lyb wavelength [A]
+OSCILLATOR_STRENGTH_LYA = 0.41641
+OSCILLATOR_STRENGTH_LYB = 0.079142
+GAMMA_LYA = 6.2648e08  # s^-1 damping constant
+GAMMA_LYB = 1.6725e8  # s^-1 damping constant
 
-@njit
 def dla_profile(lambda_, z_abs, nhi):
     """Compute DLA profile
 
     Arguments
     ---------
     lambda_: array of floats
     Wavelength (in Angs)
@@ -40,127 +42,102 @@
     z_abs: float
     Redshift of the absorption
 
     nhi: float
     DLA column density in log10(cm^-2)
     """
     transmission = np.exp(
-        -tau_lya(lambda_, z_abs, nhi)
-        -tau_lyb(lambda_, z_abs, nhi))
+        -compute_tau(lambda_, z_abs, nhi, LAMBDA_LYA, OSCILLATOR_STRENGTH_LYA, GAMMA_LYA)
+        -compute_tau(lambda_, z_abs, nhi, LAMBDA_LYB, OSCILLATOR_STRENGTH_LYB, GAMMA_LYB)
+    )
     return transmission
 
-### Implementation of Pasquier code,
-###     also in Rutten 2003 at 3.3.3
-LAMBDA_LYA = float(ABSORBER_IGM["LYA"]) ## Lya wavelength [A]
-@njit
-def tau_lya(lambda_, z_abs, nhi):
-    """Compute the optical depth for Lyman-alpha absorption.
-
-    Arguments
-    ---------
-    lambda_: array of floats
-    Wavelength (in Angs)
+# constants to compute the optical depth of the DLA absoprtion
+ELEMENTARY_CHARGE = 1.6021e-19  # C
+EPSILON_0 = 8.8541e-12  # C^2.s^2.kg^-1.m^-3
+PROTON_MASS = 1.6726e-27  # kg
+ELECTRON_MASS = 9.109e-31  # kg
+BOLTZMAN_CONSTANT_K = 1.3806e-23  # m^2.kg.s^-2.K-1
+GAS_TEMP = 5 * 1e4  # K
+
+# precomputed factors to save time
+# compared to equation 36 of Garnett et al 2017 there is a sqrt(2) missing
+# this is because otherwise we need to divide this quantity by sqrt(2)
+# when calling scipy.special.voigt
+GAUSSIAN_BROADENING_B = np.sqrt(BOLTZMAN_CONSTANT_K * GAS_TEMP / PROTON_MASS)
+# the 1e-10 appears as the wavelengths are given in Angstroms
+LORENTZIAN_BROADENING_GAMMA_PREFACTOR = 1e-10 / (4 * np.pi)
+TAU_PREFACTOR = (
+    ELEMENTARY_CHARGE**2 * 1e-10 / ELECTRON_MASS / SPEED_LIGHT / 4 / EPSILON_0)
+
+def compute_tau(lambda_, z_abs, log_nhi, lambda_t, oscillator_strength_f, gamma):
+    r"""Compute the optical depth for DLA absorption.
+
+    Tau is computed using equations 34 to 36 of Garnett et al. 2017. We add
+    a factor 4pi\epsion_0 in the denominator of their equation 34 so that
+    dimensions match. The equations we use are:
+
+    \tau(\lambda, z_{abs}, N_{HI}) = N_{HI} \frac {e^{2} f\lambda_{t} }
+        {4 \epsion_0 m_{e} c } \phi{\nu, b, \gamma}
+
+    where e is the elementary charge, \lambda_{t} is the transition wavelength
+    and f is the oscillator strength of the transition. The line profile
+    function \phi is a Voigt profile, where \nu is ther elative velocity
+
+    \nu = c ( \frac{ \lambda } { \lambda_{t}* (1+z_{DLA}) }  ) ,
+
+    b / \sqrt{2} is the standard deviation of the Gaussian (Maxwellian)
+    broadening contribution:
 
-    z_abs: float
-    Redshift of the absorption
+    b = \sqrt{ \frac{ 2kT }{ m_{p} } }
 
-    nhi: float
-    DLA column density in log10(cm^-2)
+    and \gamma is the width of the Lorenztian broadening contribution:
 
-    Return
-    ------
-    tau: array of float
-    The optical depth.
-    """
-    gamma = 6.625e8  ## damping constant of the transition [s^-1]
-    osc_strength = 0.4164  ## oscillator strength of the atomic transition
-    speed_light = 3e8  ## speed of light [m/s]
-    thermal_velocity = 30000.  ## sqrt(2*k*T/m_proton) with
-    ## T = 5*10^4 ## [m.s^-1]
-    nhi_cm2 = 10**nhi  ## column density [cm^-2]
-    lambda_rest_frame = lambda_ / (1 + z_abs)
-    ## wavelength at DLA restframe [A]
-
-    u_voight = ((speed_light / thermal_velocity) *
-                (LAMBDA_LYA / lambda_rest_frame - 1))
-    ## dimensionless frequency offset in Doppler widths.
-    a_voight = LAMBDA_LYA * 1e-10 * gamma / (4 * np.pi * thermal_velocity)
-    ## Voigt damping parameter
-    voigt_profile = voigt(a_voight, u_voight)
-    thermal_velocity /= 1000.
-    ## 1.497e-16 = e**2/(4*sqrt(pi)*epsilon0*m_electron*c)*1e-10
-    ## [m^2.s^-1.m/]
-    ## we have b/1000 & 1.497e-15 to convert
-    ## 1.497e-15*osc_strength*lambda_rest_frame*h/n to cm^2
-    tau = (1.497e-15 * nhi_cm2 * osc_strength * lambda_rest_frame * voigt_profile /
-           thermal_velocity)
-    return tau
+    \gamma = \frac { \Gamma \lambda_{t} } { 4\pi }
 
-LAMBDA_LYB = float(ABSORBER_IGM["LYB"])
-@njit
-def tau_lyb(lambda_, z_abs, nhi):
-    """Compute the optical depth for Lyman-beta absorption.
+    where \Gamma is a damping constant
 
     Arguments
     ---------
     lambda_: array of floats
     Wavelength (in Angs)
 
     z_abs: float
     Redshift of the absorption
 
-    nhi: float
+    log_nhi: float
     DLA column density in log10(cm^-2)
 
-    Return
-    ------
-    tau: array of float
-    The optical depth.
-    """
-    gamma = 0.079120
-    osc_strength = 1.897e8
-    speed_light = 3e8  ## speed of light m/s
-    thermal_velocity = 30000.
-    nhi_cm2 = 10**nhi
-    lambda_rest_frame = lambda_ / (1 + z_abs)
-
-    u_voight = ((speed_light / thermal_velocity) *
-                (LAMBDA_LYB / lambda_rest_frame - 1))
-    a_voight = LAMBDA_LYB * 1e-10 * gamma / (4 * np.pi * thermal_velocity)
-    voigt_profile = voigt(a_voight, u_voight)
-    thermal_velocity /= 1000.
-    tau = (1.497e-15 * nhi_cm2 * osc_strength * lambda_rest_frame * voigt_profile /
-           thermal_velocity)
-    return tau
-
-# maybe we should replace this by scipy.special.voigt_profile?
-# if it is in numba
-@njit
-def voigt(a_voight, u_voight):
-    """Compute the classical Voigt function
+    lambda_t: float
+    Transition wavelength, in Angstroms, e.g. for Lya 1215.67
 
-    Arguments
-    ---------
-    a_voight: float
-    Voigt damping parameter.
+    oscillator_strength_f: float
+    Oscillator strength, e.g. f = 0.41611 for Lya
 
-    u_voight: array of floats
-    Dimensionless frequency offset in Doppler widths.
+    gamma: float
+    Damping constant (in s^-1)
 
     Return
     ------
-    voigt: array of float
-    The Voigt function for each element in a, u
+    tau: array of float
+    The optical depth.
     """
-    unnormalized_voigt = np.zeros_like(u_voight)
-    for index in range(unnormalized_voigt.shape[0]):
-        unnormalized_voigt[index] = np.mean(
-            1.0 / (a_voight**2 + (GAUSSIAN_DIST - u_voight[index])**2)
-        )
-    return unnormalized_voigt * a_voight / np.sqrt(np.pi)
+    # compute broadenings for the voight profile
+    relative_velocity_nu = SPEED_LIGHT * (lambda_ / (1 + z_abs) / lambda_t - 1)
+    lorentzian_broadening_gamma = (
+        LORENTZIAN_BROADENING_GAMMA_PREFACTOR * gamma * lambda_t)
+
+    # convert column density to m^2
+    nhi = 10**log_nhi * 1e4
+
+    # the 1e-10 converts the wavelength from Angstroms to meters
+    tau = TAU_PREFACTOR * nhi * oscillator_strength_f * lambda_t * voigt_profile(
+        relative_velocity_nu, GAUSSIAN_BROADENING_B, lorentzian_broadening_gamma)
+
+    return tau
 
 class DlaMask(Mask):
     """Class to mask DLAs
 
     Methods
     -------
     __init__
```

### Comparing `picca-7.0.0/py/picca/delta_extraction/masks/lines_mask.py` & `picca-7.1.0/py/picca/delta_extraction/masks/lines_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/quasar_catalogue.py` & `picca-7.1.0/py/picca/delta_extraction/quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py` & `picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py` & `picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/rejection_log.py` & `picca-7.1.0/py/picca/delta_extraction/rejection_log.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py` & `picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py` & `picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/survey.py` & `picca-7.1.0/py/picca/delta_extraction/survey.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/delta_extraction/utils.py` & `picca-7.1.0/py/picca/delta_extraction/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,40 +7,43 @@
 
 from numba import njit
 import numpy as np
 from scipy.constants import speed_of_light as speed_light
 
 from picca.delta_extraction.errors import DeltaExtractionError
 
-module_logger = logging.getLogger(__name__)
-
 SPEED_LIGHT = speed_light / 1000.  # [km/s]
 
+module_logger = logging.getLogger(__name__)
+
 ABSORBER_IGM = {
     "Halpha": 6562.8,
     "Hbeta": 4862.68,
     "MgI(2853)": 2852.96,
     "MgII(2804)": 2803.5324,
     "MgII(2796)": 2796.3511,
+    "MgII(eff)" : 2798.75,
     "FeII(2600)": 2600.1724835,
     "FeII(2587)": 2586.6495659,
     "MnII(2577)": 2576.877,
     "FeII(2383)": 2382.7641781,
     "FeII(2374)": 2374.4603294,
     "FeII(2344)": 2344.2129601,
+    "CIII(1908)"  : 1908.73,
     "AlIII(1863)": 1862.79113,
     "AlIII(1855)": 1854.71829,
     "AlII(1671)": 1670.7886,
     "FeII(1608)": 1608.4511,
     "CIV(1551)": 1550.77845,
     "CIV(eff)": 1549.06,
     "CIV(1548)": 1548.2049,
     "SiII(1527)": 1526.70698,
     "NiII(1455)": 1454.842,
     "SiIV(1403)": 1402.77291,
+    "SiIV(eff)" : 1396.76,
     "SiIV(1394)": 1393.76018,
     "NiII(1370)": 1370.132,
     "CII(1335)": 1334.5323,
     "NiII(1317)": 1317.217,
     "SiII(1304)": 1304.3702,
     "OI(1302)": 1302.1685,
     "SiII(1260)": 1260.4221,
```

### Comparing `picca-7.0.0/py/picca/delta_extraction/utils_pk1d.py` & `picca-7.1.0/py/picca/delta_extraction/utils_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/chi2.py` & `picca-7.1.0/py/picca/fitter2/chi2.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/control.py` & `picca-7.1.0/py/picca/fitter2/control.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/control_mpi.py` & `picca-7.1.0/py/picca/fitter2/control_mpi.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/data.py` & `picca-7.1.0/py/picca/fitter2/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/effective-bins.py` & `picca-7.1.0/py/picca/fitter2/effective-bins.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits` & `picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits` & `picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits` & `picca-7.1.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits` & `picca-7.1.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits` & `picca-7.1.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits` & `picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits` & `picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/myGamma.py` & `picca-7.1.0/py/picca/fitter2/myGamma.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/parser.py` & `picca-7.1.0/py/picca/fitter2/parser.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/pk.py` & `picca-7.1.0/py/picca/fitter2/pk.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/priors.py` & `picca-7.1.0/py/picca/fitter2/priors.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/sampler.py` & `picca-7.1.0/py/picca/fitter2/sampler.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/utils.py` & `picca-7.1.0/py/picca/fitter2/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/fitter2/xi.py` & `picca-7.1.0/py/picca/fitter2/xi.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/io.py` & `picca-7.1.0/py/picca/io.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/pk1d/compute_pk1d.py` & `picca-7.1.0/py/picca/pk1d/compute_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/pk1d/postproc_pk1d.py` & `picca-7.1.0/py/picca/pk1d/postproc_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/pk1d/prep_pk1d.py` & `picca-7.1.0/py/picca/pk1d/prep_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/pk1d/utils.py` & `picca-7.1.0/py/picca/pk1d/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/prep_del.py` & `picca-7.1.0/py/picca/prep_del.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/raw_io.py` & `picca-7.1.0/py/picca/raw_io.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/abstract_test.py` & `picca-7.1.0/py/picca/tests/delta_extraction/abstract_test.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/config_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/config_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/correction_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/correction_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/data_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/data_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/mask_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/mask_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -464,14 +464,16 @@
         DlaMask when masked pixels are removed
 
         Load a DlaMask instace and check that it is
         correctly initialized.
         """
         in_file = f"{THIS_DIR}/data/dummy_absorbers_cat.fits.gz"
         out_file = f"{THIS_DIR}/results/dla_mask_print.txt"
+        out_file_forest1 = f"{THIS_DIR}/results/dla_mask_forest1_remove.txt"
+        out_file_forest2 = f"{THIS_DIR}/results/dla_mask_forest2_remove.txt"
         test_file = f"{THIS_DIR}/data/dla_mask_print.txt"
         test_file_forest1 = f"{THIS_DIR}/data/dla_mask_forest1_remove.txt"
         test_file_forest2 = f"{THIS_DIR}/data/dla_mask_forest2_remove.txt"
 
         # setup printing
         setup_logger(log_file=out_file)
 
@@ -486,42 +488,46 @@
                 config["mask"][key] = str(value)
         mask = DlaMask(config["mask"])
         self.assertTrue(isinstance(mask, Mask))
 
         # apply mask to forest with 1 DLA
         forest = copy.deepcopy(forest1)
         mask.apply_mask(forest)
+
+        # save the results
+        f = open(out_file_forest1, "w")
+        f.write("# log_lambda flux ivar transmission_correction\n")
+        for log_lambda, flux, ivar, transmission_correction in zip(
+            forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
+                f.write(f"{log_lambda} {flux} {ivar} {transmission_correction}\n")
+        f.close()
+
+        # load expected values and compare
         forest_masked = np.genfromtxt(test_file_forest1, names=True)
         self.assertEqual(forest.flux.size, forest_masked["flux"].size)
         self.assertTrue(np.allclose(forest.flux, forest_masked["flux"]))
         self.assertTrue(np.allclose(forest.log_lambda, forest_masked["log_lambda"]))
         self.assertTrue(np.allclose(forest.ivar, forest_masked["ivar"]))
         self.assertTrue(np.allclose(forest.transmission_correction,
                                     forest_masked["transmission_correction"]))
 
 
         # apply mask to forest with 2 DLAs
         forest = copy.deepcopy(forest2)
-        """
-        print("Forest2, remove, before masking ")
-        print("------------------------")
-        print(forest.flux.size)
-        for log_lambda, flux, ivar, transmission_correction in zip(forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
-            print(f"{log_lambda} {flux} {ivar} {transmission_correction}")
-        print("------------------------")
-        """
         mask.apply_mask(forest)
-        """
-        print("Forest2, remove, after masking ")
-        print("------------------------")
-        print(forest.flux.size)
-        for log_lambda, flux, ivar, transmission_correction in zip(forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
-            print(f"{log_lambda} {flux} {ivar} {transmission_correction}")
-        print("------------------------")
-        """
+
+        # save the results
+        f = open(out_file_forest2, "w")
+        f.write("# log_lambda flux ivar transmission_correction\n")
+        for log_lambda, flux, ivar, transmission_correction in zip(
+            forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
+                f.write(f"{log_lambda} {flux} {ivar} {transmission_correction}\n")
+        f.close()
+
+        # load expected values and compare
         forest_masked = np.genfromtxt(test_file_forest2, names=True)
         self.assertEqual(forest.flux.size, forest_masked["flux"].size)
         self.assertTrue(np.allclose(forest.flux, forest_masked["flux"]))
         self.assertTrue(np.allclose(forest.log_lambda, forest_masked["log_lambda"]))
         self.assertTrue(np.allclose(forest.ivar, forest_masked["ivar"]))
         self.assertTrue(np.allclose(forest.transmission_correction,
                                     forest_masked["transmission_correction"]))
@@ -543,14 +549,16 @@
         the inverse variance to zero
 
         Load a DlaMask instace and check that it is
         correctly initialized.
         """
         in_file = f"{THIS_DIR}/data/dummy_absorbers_cat.fits.gz"
         out_file = f"{THIS_DIR}/results/dla_mask_print.txt"
+        out_file_forest1 = f"{THIS_DIR}/results/dla_mask_forest1_set_ivar.txt"
+        out_file_forest2 = f"{THIS_DIR}/results/dla_mask_forest2_set_ivar.txt"
         test_file = f"{THIS_DIR}/data/dla_mask_print.txt"
         test_file_forest1 = f"{THIS_DIR}/data/dla_mask_forest1_set_ivar.txt"
         test_file_forest2 = f"{THIS_DIR}/data/dla_mask_forest2_set_ivar.txt"
 
         # setup printing
         setup_logger(log_file=out_file)
 
@@ -564,59 +572,48 @@
             if key not in config["mask"]:
                 config["mask"][key] = str(value)
         mask = DlaMask(config["mask"])
         self.assertTrue(isinstance(mask, Mask))
 
         # apply mask to forest with 1 DLA
         forest = copy.deepcopy(forest1)
-        """
-        print("Forest1, set ivar, before masking ")
-        print("------------------------")
-        print(forest1.flux.size)
-        for log_lambda, flux, ivar, transmission_correction in zip(forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
-            print(f"{log_lambda} {flux} {ivar} {transmission_correction}")
-        print("------------------------")
-        """
         mask.apply_mask(forest)
-        """
-        print("Forest1, set ivar, after masking ")
-        print("------------------------")
-        print(forest.flux.size)
-        for log_lambda, flux, ivar, transmission_correction in zip(forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
-            print(f"{log_lambda} {flux} {ivar} {transmission_correction}")
-        print("------------------------")
-        """
+
+        # save the results
+        f = open(out_file_forest1, "w")
+        f.write("# log_lambda flux ivar transmission_correction\n")
+        for log_lambda, flux, ivar, transmission_correction in zip(
+            forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
+                f.write(f"{log_lambda} {flux} {ivar} {transmission_correction}\n")
+        f.close()
+
+        # load expected values and compare
         forest_masked = np.genfromtxt(test_file_forest1, names=True)
         self.assertEqual(forest.flux.size, forest_masked["flux"].size)
         self.assertTrue(np.allclose(forest.flux, forest_masked["flux"]))
         self.assertTrue(np.allclose(forest.log_lambda, forest_masked["log_lambda"]))
         self.assertTrue(np.allclose(forest.ivar, forest_masked["ivar"]))
         self.assertTrue(np.allclose(forest.transmission_correction,
                                     forest_masked["transmission_correction"]))
 
 
         # apply mask to forest with 2 DLAs
         forest = copy.deepcopy(forest2)
-        """
-        print("Forest2, set ivar, before masking ")
-        print("------------------------")
-        print(forest.flux.size)
-        for log_lambda, flux, ivar, transmission_correction in zip(forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
-            print(f"{log_lambda} {flux} {ivar} {transmission_correction}")
-        print("------------------------")
-        """
         mask.apply_mask(forest)
-        """
-        print("Forest2, set ivar, after masking ")
-        print("------------------------")
-        print(forest.flux.size)
-        for log_lambda, flux, ivar, transmission_correction in zip(forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
-            print(f"{log_lambda} {flux} {ivar} {transmission_correction}")
-        print("------------------------")
-        """
+
+        # save the results
+        f = open(out_file_forest2, "w")
+        f.write("# log_lambda flux ivar transmission_correction\n")
+        for log_lambda, flux, ivar, transmission_correction in zip(
+            forest.log_lambda, forest.flux, forest.ivar, forest.transmission_correction):
+                f.write(f"{log_lambda} {flux} {ivar} {transmission_correction}\n")
+        f.close()
+
+        # load expected values and compare
+
         forest_masked = np.genfromtxt(test_file_forest2, names=True)
         self.assertEqual(forest.flux.size, forest_masked["flux"].size)
         self.assertTrue(np.allclose(forest.flux, forest_masked["flux"]))
         self.assertTrue(np.allclose(forest.log_lambda, forest_masked["log_lambda"]))
         self.assertTrue(np.allclose(forest.ivar, forest_masked["ivar"]))
         self.assertTrue(np.allclose(forest.transmission_correction,
                                     forest_masked["transmission_correction"]))
```

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/scripts_tests.py` & `picca-7.1.0/py/picca/tests/delta_extraction/scripts_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/delta_extraction/test_utils.py` & `picca-7.1.0/py/picca/tests/delta_extraction/test_utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/old/test_1_deltas.py` & `picca-7.1.0/py/picca/tests/old/test_1_deltas.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/old/test_4_fitter2.py` & `picca-7.1.0/py/picca/tests/old/test_4_fitter2.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/test_2_pk1d.py` & `picca-7.1.0/py/picca/tests/test_2_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/test_3_cor.py` & `picca-7.1.0/py/picca/tests/test_3_cor.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/tests/test_helpers.py` & `picca-7.1.0/py/picca/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/utils.py` & `picca-7.1.0/py/picca/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/wedgize.py` & `picca-7.1.0/py/picca/wedgize.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca/xcf.py` & `picca-7.1.0/py/picca/xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/py/picca.egg-info/PKG-INFO` & `picca-7.1.0/py/picca.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 7.0.0
+Version: 7.1.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
-Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols et al
+Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # picca
 [![Coverage Status](https://coveralls.io/repos/github/igmhub/picca/badge.svg?branch=master)](https://coveralls.io/github/igmhub/picca?branch=master)
 
@@ -169,7 +169,13 @@
    to ensure the coding styles are maintained.
 4. Consider using pylint to help in the debug process. From the repo folder run
    ```
    pylint py/picca/delta_extraction/
    pylint py/picca/pk1d/
    ```
    depending on the module you are working on.
+   
+When merging PRs (or committing to master directly):
+- by default the patch version is increased via a github action, so every change of master will generate a new version
+This behaviour can be changed by adding one of the following to the commit-msg of the merge commit:
+- by specifying [bump minor] or [bump major] a new minor or major version will be generated instead, but tags and releases need to be created manually (and are auto-pushed to pypi when they are created)
+- by specifying [no bump] the version bump can be circumvented altogether when some other behaviour is wanted, in that case bump2version should be run manually
```

### Comparing `picca-7.0.0/py/picca.egg-info/SOURCES.txt` & `picca-7.1.0/py/picca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picca-7.0.0/setup.py` & `picca-7.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,23 +13,22 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 exec(open('py/picca/_version.py').read())
 version = __version__
 
 setup(name="picca",
-    version=version,
-    description=description,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url="https://github.com/igmhub/picca",
-    author="Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols et al",
-    author_email="iprafols@gmail.com",
-    packages=find_namespace_packages(where='py'),
+    version = version,
+    description = description,
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
+    url = "https://github.com/igmhub/picca",
+    author = "Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al",
+    author_email = "iprafols@gmail.com",
+    packages = find_namespace_packages(where='py'),
     package_dir = {'': 'py'},
     package_data = {'picca': ['fitter2/models/*/*.fits', 'delta_extraction/expected_fluxes/raw_stats/*fits.gz']},
-    install_requires=['numpy', 'scipy', 'iminuit', 'healpy', 'fitsio',
-                      'llvmlite', 'numba', 'h5py', 'future', 'setuptools',
-                      'gitpython'],
-    #test_suite='picca.test',
+    install_requires = ['numpy', 'scipy', 'iminuit', 'healpy', 'fitsio',
+                        'llvmlite', 'numba', 'h5py', 'future', 'setuptools',
+                        'gitpython'],
     scripts = scripts
     )
```

