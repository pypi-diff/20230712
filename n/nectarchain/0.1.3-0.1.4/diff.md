# Comparing `tmp/nectarchain-0.1.3.tar.gz` & `tmp/nectarchain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nectarchain-0.1.3.tar", last modified: Fri Mar 17 11:45:26 2023, max compression
+gzip compressed data, was "nectarchain-0.1.4.tar", last modified: Wed Jul 12 15:49:38 2023, max compression
```

## Comparing `nectarchain-0.1.3.tar` & `nectarchain-0.1.4.tar`

### file list

```diff
@@ -1,101 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-17 11:45:22.000000 nectarchain-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-17 11:45:26.897018 nectarchain-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-17 11:45:22.000000 nectarchain-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-17 11:45:22.000000 nectarchain-0.1.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.885017 nectarchain-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-03-17 11:45:22.000000 nectarchain-0.1.3/examples/waveform_animation_highGain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.885017 nectarchain-0.1.3/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-17 11:45:22.000000 nectarchain-0.1.3/licenses/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-17 11:45:22.000000 nectarchain-0.1.3/licenses/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.889017 nectarchain-0.1.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   114080 2023-03-17 11:45:22.000000 nectarchain-0.1.3/notebooks/Access NectarCAM data using DIRAC API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-03-17 11:45:22.000000 nectarchain-0.1.3/notebooks/Read_NectarCAM_events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   832042 2023-03-17 11:45:22.000000 nectarchain-0.1.3/notebooks/calculate_calibration_coefficients.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1718551 2023-03-17 11:45:22.000000 nectarchain-0.1.3/notebooks/calculate_pedestals.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-17 11:45:22.000000 nectarchain-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-17 11:45:26.897018 nectarchain-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 11:45:22.000000 nectarchain-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.889017 nectarchain-0.1.3/singularity/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-17 11:45:22.000000 nectarchain-0.1.3/singularity/Singularity
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.885017 nectarchain-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.889017 nectarchain-0.1.3/src/nectarchain/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.889017 nectarchain-0.1.3/src/nectarchain/calibration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.889017 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.893018 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/PhotoStat/
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/PhotoStat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.893018 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py
--rw-r--r--   0 runner    (1001) docker     (123)    48372 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters_ped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signalStd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_fromHHVFit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.893018 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.893018 nectarchain-0.1.3/src/nectarchain/calibration/container/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21469 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/container/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/container/charge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/container/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/calibration/container/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.893018 nectarchain-0.1.3/src/nectarchain/dqm/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/README
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/ReadPickleFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/camera_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/charge_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/dqm_summary_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/mean_camera_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/mean_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/start_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/dqm/trigger_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.893018 nectarchain-0.1.3/src/nectarchain/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/src/nectarchain/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/tools/write_camera_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/tools/write_camera_calibration_param.json
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/tools/write_pedestals.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/tools/write_pedestals_param.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.885017 nectarchain-0.1.3/src/nectarchain/user_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/src/nectarchain/user_scripts/fbradascio/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/fbradascio/fbradascio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/src/nectarchain/user_scripts/fbrun/
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/fbrun/fbrun_scripts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.897018 nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2394 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4576 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-17 11:45:22.000000 nectarchain-0.1.3/src/nectarchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 11:45:26.889017 nectarchain-0.1.3/src/nectarchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 11:45:26.000000 nectarchain-0.1.3/src/nectarchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.426652 nectarchain-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 15:49:28.000000 nectarchain-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 15:49:28.000000 nectarchain-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-12 15:49:38.426652 nectarchain-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-12 15:49:28.000000 nectarchain-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-12 15:49:28.000000 nectarchain-0.1.4/Singularity
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 15:49:28.000000 nectarchain-0.1.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.410652 nectarchain-0.1.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-12 15:49:28.000000 nectarchain-0.1.4/examples/waveform_animation_highGain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   208363 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/Access NectarCAM data using DIRAC API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/Read_NectarCAM_events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   832042 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/calculate_calibration_coefficients.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1718551 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/calculate_pedestals.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-12 15:49:28.000000 nectarchain-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:49:38.426652 nectarchain-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.410652 nectarchain-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/calibration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_ped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signalStd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_fromHHVFit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/calibration/container/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26120 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/charge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/dqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/camera_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/charge_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/dqm_summary_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/mean_camera_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/mean_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/start_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/trigger_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration_param.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_pedestals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_pedestals_param.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.410652 nectarchain-0.1.4/src/nectarchain/user_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/fbradascio/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/fbradascio/fbradascio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/fbrun_scripts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3154 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3833 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/GainFitter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/submitGainFitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.426652 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/
+-rw-r--r--   0 runner    (1001) docker     (123)    26016 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/CalibrationData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/CalibrationEvoData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/DBHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/DataUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ExtractInformation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/PedestalEstimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ShowDataContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ShowPedestalEvolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/Stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/top_level.txt
```

### Comparing `nectarchain-0.1.3/examples/waveform_animation_highGain.py` & `nectarchain-0.1.4/examples/waveform_animation_highGain.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/notebooks/Read_NectarCAM_events.ipynb` & `nectarchain-0.1.4/notebooks/Read_NectarCAM_events.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/notebooks/calculate_calibration_coefficients.ipynb` & `nectarchain-0.1.4/notebooks/calculate_calibration_coefficients.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/notebooks/calculate_pedestals.ipynb` & `nectarchain-0.1.4/notebooks/calculate_pedestals.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 __all__ = ["PhotoStatGainFFandPed"]
 
 class PhotoStatGain(ABC):
 
     def _readFF(self,FFRun,maxevents: int = None,**kwargs) :
         log.info('reading FF data')
-        method = kwargs.get('method','std')
+        method = kwargs.get('method','FullWaveformSum')
         FFchargeExtractorWindowLength = kwargs.get('FFchargeExtractorWindowLength',None)
-        if method != 'std' :
+        if method != 'FullWaveformSum' :
             if FFchargeExtractorWindowLength is None : 
                 e = Exception(f"we have to specify FFchargeExtractorWindowLength argument if charge extractor method is not FullwaveformSum")
                 log.error(e,exc_info=True)
                 raise e
             else : 
                 self.__coefCharge_FF_Ped = FFchargeExtractorWindowLength / constants.N_SAMPLES
         else : 
@@ -64,15 +64,15 @@
         else : 
             e =  TypeError("FFRun must be int or ChargeContainer")
             log.error(e,exc_info = True)
             raise e
 
     def _readPed(self,PedRun,maxevents: int = None,**kwargs) :
         log.info('reading Ped data')
-        method = 'std'#kwargs.get('method','std')
+        method = 'FullWaveformSum'#kwargs.get('method','std')
         if isinstance(PedRun,int) : 
             try : 
                 self.Pedcharge = ChargeContainer.from_file(f"{os.environ['NECTARCAMDATA']}/charges/{method}",PedRun)
                 log.info(f'charges have ever been computed for Ped run {PedRun}')
             except Exception as e : 
                 log.error("charge have not been yet computed")
                 raise e
```

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from .parameters import Parameters
 from .utils import UtilsMinuit,weight_gaussian,Statistics
 
 __all__ = ['NectarGainSPE']
 
 class NectarGainSPE(ABC) :
     _Ncall = 4000000
+    _Windows_lenght = 40
+    _Order = 2
+
     def __init__(self) :
         #set parameters value for fit
         self.__parameters = Parameters()
                 
         #output
         self._output_table = QTable()
         #self.create_output_table() #need to be done in the child class __init__
@@ -100,16 +103,16 @@
                     self._parameters.parameters[i].max = dico.get("max",np.nan)
 
     @staticmethod
     def _get_mean_gaussian_fit(charge_in, histo_in ,extension = ""):
         charge = charge_in.data[~histo_in.mask]
         histo = histo_in.data[~histo_in.mask]
 
-        windows_lenght = 80
-        order = 2
+        windows_lenght = NectarGainSPE._Windows_lenght
+        order = NectarGainSPE._Order
         histo_smoothed = savgol_filter(histo, windows_lenght, order)
 
         peaks = find_peaks(histo_smoothed,10)
         peak_max = np.argmax(histo_smoothed[peaks[0]])
         peak_pos,peak_value = charge[peaks[0][peak_max]], histo[peaks[0][peak_max]]
 
         coeff, var_matrix = curve_fit(weight_gaussian, charge[:peaks[0][peak_max]], histo_smoothed[:peaks[0][peak_max]],p0 = [peak_value,peak_pos,1])
@@ -122,58 +125,60 @@
         peak_pos_mean,peak_value_mean = charge[mask][peaks_mean[0][peak_max_mean]], histo_smoothed[mask][peaks_mean[0][peak_max_mean]]
 
         mask = (charge > ((coeff[1]+peak_pos_mean)/2)) * (charge < (peak_pos_mean + (peak_pos_mean-coeff[1])/2))
         coeff_mean, var_matrix = curve_fit(weight_gaussian, charge[mask], histo_smoothed[mask],p0 = [peak_value_mean,peak_pos_mean,1])
 
         if log.getEffectiveLevel() == logging.DEBUG :
             log.debug('plotting figures with prefit parameters computation') 
-            fig,ax = plt.subplots(1,1,figsize = (8,8))
+            fig,ax = plt.subplots(1,1,figsize = (5,5))
             ax.errorbar(charge,histo,np.sqrt(histo),zorder=0,fmt=".",label = "data")
             ax.plot(charge,histo_smoothed,label = f'smoothed data with savgol filter (windows lenght : {windows_lenght}, order : {order})')
             ax.plot(charge,weight_gaussian(charge,coeff_mean[0],coeff_mean[1],coeff_mean[2]),label = 'gaussian fit of the SPE')
             ax.vlines(coeff_mean[1],0,peak_value,label = f'mean initial value = {coeff_mean[1] - coeff[1]:.0f}',color = "red")
             ax.add_patch(Rectangle((coeff_mean[1]-coeff_mean[2], 0), 2 * coeff_mean[2], peak_value_mean,fc=to_rgba('red', 0.5)))
+            ax.set_xlim([peak_pos - 500,None])
             ax.set_xlabel("Charge (ADC)", size=15)
             ax.set_ylabel("Events", size=15)
-            ax.legend(fontsize=15)
+            ax.legend(fontsize=7)
             os.makedirs(f"{os.environ.get('NECTARCHAIN_LOG')}/{os.getpid()}/figures/",exist_ok=True)
             fig.savefig(f"{os.environ.get('NECTARCHAIN_LOG')}/{os.getpid()}/figures/initialization_mean_pixel{extension}_{os.getpid()}.pdf")
             fig.clf()
             plt.close(fig)
             del fig,ax
         return coeff_mean,var_matrix
 
     @staticmethod
     def _get_pedestal_gaussian_fit(charge_in, histo_in ,extension = "") :
         #x = np.linspace(nectargain.charge[pixel].min(),nectargain.charge[pixel].max(),int(nectargain.charge[pixel].max()-nectargain.charge[pixel].min()))
         #interp = interp1d(nectargain.charge[pixel],nectargain.histo[pixel])
         charge = charge_in.data[~histo_in.mask]
         histo = histo_in.data[~histo_in.mask]
 
-        windows_lenght = 80
-        order = 2
+        windows_lenght = NectarGainSPE._Windows_lenght
+        order = NectarGainSPE._Order
         histo_smoothed = savgol_filter(histo, windows_lenght, order)
 
         peaks = find_peaks(histo_smoothed,10)
         peak_max = np.argmax(histo_smoothed[peaks[0]])
         peak_pos,peak_value = charge[peaks[0][peak_max]], histo[peaks[0][peak_max]]
 
         coeff, var_matrix = curve_fit(weight_gaussian, charge[:peaks[0][peak_max]], histo_smoothed[:peaks[0][peak_max]],p0 = [peak_value,peak_pos,1])
 
         if log.getEffectiveLevel() == logging.DEBUG :
             log.debug('plotting figures with prefit parameters computation') 
-            fig,ax = plt.subplots(1,1,figsize = (8,8))
+            fig,ax = plt.subplots(1,1,figsize = (5,5))
             ax.errorbar(charge,histo,np.sqrt(histo),zorder=0,fmt=".",label = "data")
             ax.plot(charge,histo_smoothed,label = f'smoothed data with savgol filter (windows lenght : {windows_lenght}, order : {order})')
             ax.plot(charge,weight_gaussian(charge,coeff[0],coeff[1],coeff[2]),label = 'gaussian fit of the pedestal, left tail only')
+            ax.set_xlim([peak_pos - 500,None])
             ax.vlines(coeff[1],0,peak_value,label = f'pedestal initial value = {coeff[1]:.0f}',color = 'red')
             ax.add_patch(Rectangle((coeff[1]-coeff[2], 0), 2 * coeff[2], peak_value,fc=to_rgba('red', 0.5)))
             ax.set_xlabel("Charge (ADC)", size=15)
             ax.set_ylabel("Events", size=15)
-            ax.legend(fontsize=15)
+            ax.legend(fontsize=7)
             os.makedirs(f"{os.environ.get('NECTARCHAIN_LOG')}/{os.getpid()}/figures/",exist_ok=True)
             fig.savefig(f"{os.environ.get('NECTARCHAIN_LOG')}/{os.getpid()}/figures/initialization_pedestal_pixel{extension}_{os.getpid()}.pdf")
             fig.clf()
             plt.close(fig)
             del fig,ax
         return coeff,var_matrix
```

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,25 +453,26 @@
             output['gain_error'] = np.empty(2)
             output['gain_error'][0] = gain[1] 
             output['gain_error'][1] = gain[2] 
 
 
 
             if kwargs.get('figpath',0) != 0 :
-                fig,ax = plt.subplots(1,1,figsize=(8, 6))
+                fig,ax = plt.subplots(1,1,figsize=(8, 8))
                 ax.errorbar(charge,histo,np.sqrt(histo),zorder=0,fmt=".",label = "data")
                 ax.plot(charge,
                     np.trapz(histo,charge)*MPE2(charge,parameters['pp'].value, parameters['resolution'].value, parameters['mean'].value, parameters['n'].value, parameters['pedestal'].value, parameters['pedestalWidth'].value, parameters['luminosity'].value),
                     zorder=1,
                     linewidth=2,
-                    label = f"SPE model fit \n gain : {gain[0] - gain[1]:.2f} < {gain[0]:.2f} < {gain[0] + gain[2]:.2f} ADC/pe, pvalue = {Statistics.chi2_pvalue(ndof,fit.fval)},\n likelihood = {fit.fval:.2f}")
+                    label = f"SPE model fit \n gain : {gain[0] - gain[1]:.2f} < {gain[0]:.2f} < {gain[0] + gain[2]:.2f} ADC/pe,\n pvalue = {Statistics.chi2_pvalue(ndof,fit.fval)},\n likelihood = {fit.fval:.2f}")
                 ax.set_xlabel("Charge (ADC)", size=15)
                 ax.set_ylabel("Events", size=15)
                 ax.set_title(f"SPE fit pixel {it} with pixel_id : {pixels_id}")
-                ax.legend(fontsize=15)
+                ax.set_xlim([parameters['pedestal'].value - 6 * parameters['pedestalWidth'].value, None])
+                ax.legend(fontsize=18)
                 os.makedirs(kwargs.get('figpath'),exist_ok = True)
                 fig.savefig(f"{kwargs.get('figpath')}/fit_SPE_pixel{pixels_id}.pdf")
                 fig.clf()
                 plt.close(fig)
                 del fig,ax
         else : 
             log.warning(f"fit pixel {it} with pixel_id = {pixels_id} is not valid")
@@ -499,25 +500,26 @@
             self._output_table['gain'][pixel] = self.__gain[pixel,0] 
             self._output_table['gain_error'][pixel][0] = self.__gain[pixel,1] 
             self._output_table['gain_error'][pixel][1] = self.__gain[pixel,2] 
 
 
 
             if kwargs.get('figpath',0) != 0 :
-                fig,ax = plt.subplots(1,1,figsize=(8, 6))
+                fig,ax = plt.subplots(1,1,figsize=(8, 8))
                 ax.errorbar(self.charge[pixel],self.histo[pixel],np.sqrt(self.histo[pixel]),zorder=0,fmt=".",label = "data")
                 ax.plot(self.charge[pixel],
                     np.trapz(self.histo[pixel],self.charge[pixel])*MPE2(self.charge[pixel],self.__pp.value,self.__resolution.value,self.__mean.value,self.__n.value,self.pedestal.value,self.__pedestalWidth.value,self.__luminosity.value),
                     zorder=1,
                     linewidth=2,
-                    label = f"SPE model fit \n gain : {self.__gain[pixel,0] - self.__gain[pixel,1]:.2f} < {self.__gain[pixel,0]:.2f} < {self.__gain[pixel,0] + self.__gain[pixel,2]:.2f} ADC/pe, pvalue = {Statistics.chi2_pvalue(ndof,fit.fval)},\n likelihood = {fit.fval:.2f}")
+                    label = f"SPE model fit \n gain : {self.__gain[pixel,0] - self.__gain[pixel,1]:.2f} < {self.__gain[pixel,0]:.2f} < {self.__gain[pixel,0] + self.__gain[pixel,2]:.2f} ADC/pe,\n pvalue = {Statistics.chi2_pvalue(ndof,fit.fval)},\n likelihood = {fit.fval:.2f}")
                 ax.set_xlabel("Charge (ADC)", size=15)
                 ax.set_ylabel("Events", size=15)
                 ax.set_title(f"SPE fit pixel : {pixel} (pixel id : {self.pixels_id[pixel]})")
-                ax.legend(fontsize=15)
+                ax.set_xlim([self.pedestal.value - 6 * self.pedestalWidth.value, None])
+                ax.legend(fontsize=18)
                 os.makedirs(kwargs.get('figpath'),exist_ok = True)
                 fig.savefig(f"{kwargs.get('figpath')}/fit_SPE_pixel{self.pixels_id[pixel]}.pdf")
                 fig.clf()
                 plt.close(fig)
                 del fig,ax
         else : 
             log.warning(f"fit pixel_id = {self.pixels_id[pixel]} is not valid")
@@ -567,15 +569,15 @@
         pedestal = parameters['pedestal']
         pedestalWidth = parameters["pedestalWidth"]
         pedestalWidth.value = pedestal.max - pedestal.value
         pedestalWidth.max = 3 * pedestalWidth.value
         log.debug(f"pedestalWidth updated : {pedestalWidth}")
         try : 
             coeff,var_matrix =  NectarGainSPE._get_mean_gaussian_fit(charge,histo,f'{it}_nominal')
-            if coeff[1] - pedestal.value < 0 : raise Exception("mean gaussian fit not good")
+            if (coeff[1] - pedestal.value < 0) or ((coeff[1] - coeff[2]) - pedestal.max < 0) : raise Exception("mean gaussian fit not good")
             mean = parameters['mean']
             mean.value = coeff[1] - pedestal.value
             mean.min = (coeff[1] - coeff[2]) - pedestal.max
             mean.max = (coeff[1] + coeff[2]) - pedestal.min
             log.debug(f"mean updated : {mean}")
         except Exception as e :
             log.warning(e,exc_info=True)
@@ -781,15 +783,15 @@
     def run(self,pixel : int = None,multiproc = False, **kwargs):
         kwargs['nectarGainSPEresult'] = copy.deepcopy(self.__nectarGainSPEresult)
         if multiproc :
             kwargs['same_luminosity'] = self.__same_luminosity
         super().run(pixel,multiproc,**kwargs)
 
     def _run_obs(self,pixel,prescan = False,**kwargs) : 
-        if self.__nectarGainSPEresult[pixel]['is_valid'].value : 
+        if self.__nectarGainSPEresult[pixel]['is_valid'] : 
             kwargs['pixel_id'] = self.pixels_id[pixel]
             super()._run_obs(pixel,prescan,**kwargs)
         else :
             log.warning(f"fit pixel {pixel} with pixel_id = {self.pixels_id[pixel]} is not valid")
             self.fill_table(pixel,False,0,0)
 
     @classmethod
```

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/NectarGain/SPEfit/utils.py` & `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/utils.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/container/charge.py` & `nectarchain-0.1.4/src/nectarchain/calibration/container/charge.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from argparse import ArgumentError
 import numpy as np
 import numpy.ma as ma
 from matplotlib import pyplot as plt
 import copy
 from pathlib import Path
+import glob
 import time
 import sys
 import os
 import logging
 logging.basicConfig(format='%(asctime)s %(name)s %(levelname)s %(message)s')
 log = logging.getLogger(__name__)
 log.handlers = logging.getLogger('__main__').handlers
@@ -29,14 +30,15 @@
 
 from astropy.table import Table
 from astropy.io import fits
 
 from numba import guvectorize, float64, int64, bool_
 
 from .waveforms import WaveformsContainer,WaveformsContainers
+from .utils import CtaPipeExtractor
 
 
 
 #from .charge_extractor import *
 
 __all__ = ['ChargeContainer','ChargeContainers']
 
@@ -112,28 +114,29 @@
     CAMERA = CameraGeometry.from_name("NectarCam-003")
 
     def __init__(self,charge_hg,charge_lg,peak_hg,peak_lg,run_number,pixels_id,nevents,npixels, method = "FullWaveformSum") : 
         self.charge_hg = charge_hg
         self.charge_lg = charge_lg
         self.peak_hg = peak_hg
         self.peak_lg = peak_lg
-        self.__run_number = run_number
-        self.__pixels_id = pixels_id
-        self.__method = method
-        self.__nevents = nevents
-        self.__npixels = npixels
+        self._run_number = run_number
+        self._pixels_id = pixels_id
+        self._method = method
+        self._nevents = nevents
+        self._npixels = npixels
 
 
         self.ucts_timestamp = np.zeros((self.nevents),dtype = np.uint64)
         self.ucts_busy_counter = np.zeros((self.nevents),dtype = np.uint16)
         self.ucts_event_counter = np.zeros((self.nevents),dtype = np.uint16)
         self.event_type = np.zeros((self.nevents),dtype = np.uint8)
         self.event_id = np.zeros((self.nevents),dtype = np.uint16)
         self.trig_pattern_all = np.zeros((self.nevents,self.CAMERA.n_pixels,4),dtype = bool)
 
+
     @classmethod
     def from_waveforms(cls,waveformContainer : WaveformsContainer,method : str = "FullWaveformSum",**kwargs) : 
         """ create a new ChargeContainer from a WaveformsContainer
         Args:
             waveformContainer (WaveformsContainer): the waveforms
             method (str, optional): Ctapipe ImageExtractor method. Defaults to "FullWaveformSum".
 
@@ -168,55 +171,55 @@
         suffix = kwargs.get("suffix","")
         if suffix != "" : suffix = f"_{suffix}"
 
         log.info(f"saving in {path}")
         os.makedirs(path,exist_ok = True)
 
         #table = Table(self.charge_hg)
-        #table.meta["pixels_id"] = self.__pixels_id
+        #table.meta["pixels_id"] = self._pixels_id
         #table.write(Path(path)/f"charge_hg_run{self.run_number}.ecsv",format='ascii.ecsv',overwrite=kwargs.get('overwrite',False))
         #
         #table = Table(self.charge_lg)
-        #table.meta["pixels_id"] = self.__pixels_id
+        #table.meta["pixels_id"] = self._pixels_id
         #table.write(Path(path)/f"charge_lg_run{self.run_number}.ecsv",format='ascii.ecsv',overwrite=kwargs.get('overwrite',False))
         #
         #table = Table(self.peak_hg)
-        #table.meta["pixels_id"] = self.__pixels_id
+        #table.meta["pixels_id"] = self._pixels_id
         #table.write(Path(path)/f"peak_hg_run{self.run_number}.ecsv",format='ascii.ecsv',overwrite=kwargs.get('overwrite',False))
         #
         #table = Table(self.peak_lg)
-        #table.meta["pixels_id"] = self.__pixels_id
+        #table.meta["pixels_id"] = self._pixels_id
         #table.write(Path(path)/f"peak_lg_run{self.run_number}.ecsv",format='ascii.ecsv',overwrite=kwargs.get('overwrite',False))
 
         hdr = fits.Header()
-        hdr['RUN'] = self.__run_number
+        hdr['RUN'] = self._run_number
         hdr['NEVENTS'] = self.nevents
         hdr['NPIXELS'] = self.npixels
-        hdr['COMMENT'] = f"The charge containeur for run {self.__run_number} with {self.__method} method : primary is the pixels id, then you can find HG charge, LG charge, HG peak and LG peak, 2 last HDU are composed of event properties and trigger patern"
+        hdr['COMMENT'] = f"The charge containeur for run {self._run_number} with {self._method} method : primary is the pixels id, then you can find HG charge, LG charge, HG peak and LG peak, 2 last HDU are composed of event properties and trigger patern"
 
         primary_hdu = fits.PrimaryHDU(self.pixels_id,header=hdr)
-        charge_hg_hdu = fits.ImageHDU(self.charge_hg)
-        charge_lg_hdu = fits.ImageHDU(self.charge_lg)
-        peak_hg_hdu = fits.ImageHDU(self.peak_hg)
-        peak_lg_hdu = fits.ImageHDU(self.peak_lg)
+        charge_hg_hdu = fits.ImageHDU(self.charge_hg,name = "HG charge")
+        charge_lg_hdu = fits.ImageHDU(self.charge_lg,name = "LG charge")
+        peak_hg_hdu = fits.ImageHDU(self.peak_hg, name = 'HG peak time')
+        peak_lg_hdu = fits.ImageHDU(self.peak_lg, name = 'LG peak time')
 
         col1 = fits.Column(array = self.event_id, name = "event_id", format = '1I')
         col2 = fits.Column(array = self.event_type, name = "event_type", format = '1I')
         col3 = fits.Column(array = self.ucts_timestamp, name = "ucts_timestamp", format = '1K')
         col4 = fits.Column(array = self.ucts_busy_counter, name = "ucts_busy_counter", format = '1I')
         col5 = fits.Column(array = self.ucts_event_counter, name = "ucts_event_counter", format = '1I')
         col6 = fits.Column(array = self.multiplicity, name = "multiplicity", format = '1I')
 
         coldefs = fits.ColDefs([col1, col2, col3, col4, col5, col6])
-        event_properties = fits.BinTableHDU.from_columns(coldefs)
+        event_properties = fits.BinTableHDU.from_columns(coldefs, name = 'event properties')
 
         col1 = fits.Column(array = self.trig_pattern_all, name = "trig_pattern_all", format = f'{4 * self.CAMERA.n_pixels}L',dim = f'({self.CAMERA.n_pixels},4)')
         col2 = fits.Column(array = self.trig_pattern, name = "trig_pattern", format = f'{self.CAMERA.n_pixels}L')
         coldefs = fits.ColDefs([col1, col2])
-        trigger_patern = fits.BinTableHDU.from_columns(coldefs)
+        trigger_patern = fits.BinTableHDU.from_columns(coldefs, name = 'trigger patern')
 
         hdul = fits.HDUList([primary_hdu, charge_hg_hdu, charge_lg_hdu,peak_hg_hdu,peak_lg_hdu,event_properties,trigger_patern])
         try : 
             hdul.writeto(Path(path)/f"charge_run{self.run_number}{suffix}.fits",overwrite=kwargs.get('overwrite',False))
             log.info(f"charge saved in {Path(path)}/charge_run{self.run_number}{suffix}.fits")
         except OSError as e : 
             log.warning(e)
@@ -229,53 +232,45 @@
 
     @staticmethod
     def from_file(path : Path,run_number : int,**kwargs) : 
         """load ChargeContainer from FITS file previously written with ChargeContainer.write() method  
         
         Args:
             path (str): path of the FITS file
+            run_number (int) : the run number
 
         Returns:
             ChargeContainer: ChargeContainer instance
         """
-        log.info(f"loading in {path} run number {run_number}")
+        if kwargs.get("explicit_filename",False) : 
+            filename = kwargs.get("explicit_filename")
+            log.info(f"loading {filename}")
+        else : 
+            log.info(f"loading in {path} run number {run_number}")
+            filename = Path(path)/f"charge_run{run_number}.fits"
         
-        #table = Table.read(Path(path)/f"charge_hg_run{run_number}.ecsv")
-        #pixels_id = table.meta['pixels_id']
-        #charge_hg = np.array([table[colname] for colname in table.colnames]).T
-        #
-        #table = Table.read(Path(path)/f"charge_lg_run{run_number}.ecsv")
-        #charge_lg = np.array([table[colname] for colname in table.colnames]).T
-        #
-        #table = Table.read(Path(path)/f"peak_hg_run{run_number}.ecsv")
-        #peak_hg = np.array([table[colname] for colname in table.colnames]).T
-        #
-        #table = Table.read(Path(path)/f"peak_lg_run{run_number}.ecsv")
-        #peak_lg = np.array([table[colname] for colname in table.colnames]).T
-        #
-        hdul = fits.open(Path(path)/f"charge_run{run_number}.fits")
-        pixels_id = hdul[0].data
-        nevents = hdul[0].header['NEVENTS'] 
-        npixels = hdul[0].header['NPIXELS'] 
-        charge_hg = hdul[1].data
-        charge_lg = hdul[2].data
-        peak_hg = hdul[3].data
-        peak_lg = hdul[4].data
-
-
-        cls = ChargeContainer(charge_hg,charge_lg,peak_hg,peak_lg,run_number,pixels_id,nevents,npixels)
-
-        cls.event_id = hdul[5].data["event_id"]
-        cls.event_type = hdul[5].data["event_type"]
-        cls.ucts_timestamp = hdul[5].data["ucts_timestamp"]
-        cls.ucts_busy_counter = hdul[5].data["ucts_busy_counter"]
-        cls.ucts_event_counter = hdul[5].data["ucts_event_counter"]
+        with fits.open(filename) as hdul :
+            pixels_id = hdul[0].data
+            nevents = hdul[0].header['NEVENTS'] 
+            npixels = hdul[0].header['NPIXELS'] 
+            charge_hg = hdul[1].data
+            charge_lg = hdul[2].data
+            peak_hg = hdul[3].data
+            peak_lg = hdul[4].data
+
+            cls = ChargeContainer(charge_hg,charge_lg,peak_hg,peak_lg,run_number,pixels_id,nevents,npixels)
+
+            cls.event_id = hdul[5].data["event_id"]
+            cls.event_type = hdul[5].data["event_type"]
+            cls.ucts_timestamp = hdul[5].data["ucts_timestamp"]
+            cls.ucts_busy_counter = hdul[5].data["ucts_busy_counter"]
+            cls.ucts_event_counter = hdul[5].data["ucts_event_counter"]
 
-        table_trigger = hdul[6].data
-        cls.trig_pattern_all = table_trigger["trig_pattern_all"]
+            table_trigger = hdul[6].data
+            cls.trig_pattern_all = table_trigger["trig_pattern_all"]
 
         return cls
 
         
     @staticmethod 
     def compute_charge(waveformContainer : WaveformsContainer,channel : int,method : str = "FullWaveformSum" ,**kwargs) : 
         """compute charge from waveforms 
@@ -292,22 +287,31 @@
         Returns:
             output of the extractor called on waveforms
         """
         
         if not(method in list_ctapipe_charge_extractor or method in list_nectarchain_charge_extractor) :
             raise ArgumentError(f"method must be in {list_ctapipe_charge_extractor}")
 
-        if "apply_integration_correction" in eval(method).class_traits() :
-            kwargs["apply_integration_correction"] = False
+        extractor_kwargs = {}
+        for key in eval(method).class_own_traits().keys() :
+            if key in kwargs.keys() :
+                extractor_kwargs[key] = kwargs[key]
+
+        if "apply_integration_correction" in eval(method).class_own_traits().keys() : #to change the default behavior of ctapipe extractor
+            extractor_kwargs["apply_integration_correction"] = kwargs.get("apply_integration_correction",False)
+
+        log.debug(f"Extracting charges with method {method} and extractor_kwargs {extractor_kwargs}")
+        ImageExtractor = eval(method)(waveformContainer.subarray,**extractor_kwargs)
 
-        ImageExtractor = eval(method)(waveformContainer.subarray,**kwargs)
         if channel == constants.HIGH_GAIN:
-            return ImageExtractor(waveformContainer.wfs_hg,waveformContainer.TEL_ID,channel)
+            out = np.array([CtaPipeExtractor.get_image_peak_time(ImageExtractor(waveformContainer.wfs_hg[i],waveformContainer.TEL_ID,channel,waveformContainer.broken_pixels_hg)) for i in range(len(waveformContainer.wfs_hg))]).transpose(1,0,2)
+            return out[0],out[1]
         elif channel == constants.LOW_GAIN:
-            return ImageExtractor(waveformContainer.wfs_lg,waveformContainer.TEL_ID,channel)
+            out = np.array([CtaPipeExtractor.get_image_peak_time(ImageExtractor(waveformContainer.wfs_lg[i],waveformContainer.TEL_ID,channel,waveformContainer.broken_pixels_lg)) for i in range(len(waveformContainer.wfs_lg))]).transpose(1,0,2)
+            return out[0],out[1]
         else :
             raise ArgumentError(f"channel must be {constants.LOW_GAIN} or {constants.HIGH_GAIN}")
 
     def histo_hg(self,n_bins : int = 1000,autoscale : bool = True) -> np.ndarray:
         """method to compute histogram of HG channel
         Numba is used to compute histograms in vectorized way
 
@@ -405,24 +409,27 @@
             (np.ndarray): charge array in the order of specified pixel_id
         """
         mask_contain_pixels_id = np.array([pixel in self.pixels_id for pixel in pixel_id],dtype = bool)
         for pixel in pixel_id[~mask_contain_pixels_id] : log.warning(f"You asked for pixel_id {pixel} but it is not present in this ChargeContainer, skip this one")
         return np.array([self.charge_lg.T[np.where(self.pixels_id == pixel)[0][0]] for pixel in pixel_id[mask_contain_pixels_id]]).T
 
     @property
-    def run_number(self) : return self.__run_number
+    def run_number(self) : return self._run_number
 
     @property
-    def pixels_id(self) : return self.__pixels_id
+    def pixels_id(self) : return self._pixels_id
 
     @property
-    def npixels(self) : return self.__npixels
+    def npixels(self) : return self._npixels
 
     @property
-    def nevents(self) : return self.__nevents
+    def nevents(self) : return self._nevents
+
+    @property
+    def method(self) : return self._method
 
 
     #physical properties
     @property
     def multiplicity(self) :  return np.uint16(np.count_nonzero(self.trig_pattern,axis = 1))
 
     @property
@@ -443,29 +450,103 @@
             waveformContainers (WaveformsContainers)
 
         Returns:
             chargeContainers (ChargeContainers)
         """
         chargeContainers = cls()
         for i in range(waveformContainers.nWaveformsContainer) : 
-            chargeContainers.append(ChargeContainer.from_waveforms(waveformContainers.waveformsContainer[i]))
+            chargeContainers.append(ChargeContainer.from_waveforms(waveformContainers.waveformsContainer[i],**kwargs))
         return chargeContainers
 
     def write(self,path : str, **kwargs) : 
         """write each ChargeContainer in ChargeContainers on disk 
 
         Args:
             path (str): path where data are saved
         """
         for i in range(self.__nChargeContainer) : 
             self.chargeContainers[i].write(path,suffix = f"{i:04d}" ,**kwargs)
 
+    @staticmethod
+    def from_file(path : Path,run_number : int,**kwargs) :
+        """load ChargeContainers from FITS file previously written with ChargeContainers.write() method 
+        This method will search all the fits files corresponding to {path}/charge_run{run_number}_*.fits scheme
+        
+        Args:
+            path (str): path with name of the FITS file without .fits extension
+            run_number (int) : the run number
+
+        Returns:
+            ChargeContainers: ChargeContainers instance
+        """
+        log.info(f"loading from {path}/charge_run{run_number}_*.fits")
+        files = glob.glob(f"{path}/charge_run{run_number}_*.fits")
+        if len(files) == 0 : 
+            e = FileNotFoundError(f"no files found corresponding to {path}_*.fits")
+            log.error(e)
+            raise e
+        else : 
+            cls = ChargeContainers.__new__(ChargeContainers)
+            cls.chargeContainers = []
+            cls.__nchargeContainers = len(files)
+            for file in files : 
+                cls.chargeContainers.append(ChargeContainer.from_file(path,run_number,explicit_filename = file))
+            return cls
+
     @property
-    def nChargeContainer(self) : return self.__nChargeContainer
+    def nChargeContainer(self) : 
+        """getter giving the number of chargeContainer into the ChargeContainers instance
+
+        Returns:
+            int: the number of chargeContainer
+        """
+        return self.__nChargeContainer
 
     @property
     def nevents(self) : 
+        """number of events into the whole ChargesContainers
+
+        Returns:
+            int: number of events
+        """
         return np.sum([self.chargeContainers[i].nevents for i in range(self.__nChargeContainer)])
 
-    def append(self,chargeContainer : ChargeContainer) : 
+    def append(self,chargeContainer : ChargeContainer) :
+        """method to stack a ChargeContainer into the ChargeContainers
+
+        Args:
+            chargeContainer (ChargeContainer): the data to be stacked into
+        """
         self.chargeContainers.append(chargeContainer)
-        self.__nChargeContainer += 1
+        self.__nChargeContainer += 1
+
+
+    def merge(self) -> ChargeContainer : 
+        """method to merge a ChargeContainers into one single ChargeContainer
+
+        Returns:
+            ChargeContainer: the merged object
+        """
+        cls  = ChargeContainer.__new__(ChargeContainer)
+        cls.charge_hg = np.concatenate([chargecontainer.charge_hg for chargecontainer in self.chargeContainers],axis = 0) 
+        cls.charge_lg = np.concatenate([chargecontainer.charge_lg for chargecontainer in self.chargeContainers],axis = 0) 
+        cls.peak_hg = np.concatenate([chargecontainer.peak_hg for chargecontainer in self.chargeContainers],axis = 0) 
+        cls.peak_lg = np.concatenate([chargecontainer.peak_lg for chargecontainer in self.chargeContainers],axis = 0) 
+
+        if np.all([chargecontainer.run_number == self.chargeContainers[0].run_number for chargecontainer in self.chargeContainers]) : 
+            cls._run_number = self.chargeContainers[0].run_number
+        if np.all([chargecontainer.pixels_id == self.chargeContainers[0].pixels_id for chargecontainer in self.chargeContainers]) : 
+            cls._pixels_id = self.chargeContainers[0].pixels_id
+        if np.all([chargecontainer.method == self.chargeContainers[0].method for chargecontainer in self.chargeContainers]):
+            cls._method = self.chargeContainers[0].method
+        cls._nevents = np.sum([chargecontainer.nevents for chargecontainer in self.chargeContainers])
+        if np.all([chargecontainer.npixels == self.chargeContainers[0].npixels for chargecontainer in self.chargeContainers]):
+            cls._npixels = self.chargeContainers[0].npixels
+
+
+        cls.ucts_timestamp = np.concatenate([chargecontainer.ucts_timestamp for chargecontainer in self.chargeContainers ])
+        cls.ucts_busy_counter = np.concatenate([chargecontainer.ucts_busy_counter for chargecontainer in self.chargeContainers ])
+        cls.ucts_event_counter = np.concatenate([chargecontainer.ucts_event_counter for chargecontainer in self.chargeContainers ])
+        cls.event_type = np.concatenate([chargecontainer.event_type for chargecontainer in self.chargeContainers ])
+        cls.event_id = np.concatenate([chargecontainer.event_id for chargecontainer in self.chargeContainers ])
+        cls.trig_pattern_all = np.concatenate([chargecontainer.trig_pattern_all for chargecontainer in self.chargeContainers ],axis = 0)
+        return cls
```

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/container/charge_extractor.py` & `nectarchain-0.1.4/src/nectarchain/calibration/container/charge_extractor.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/container/utils.py` & `nectarchain-0.1.4/src/nectarchain/calibration/container/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import requests
 import browser_cookie3
 
 from DIRAC.Interfaces.API.Dirac import Dirac
 from pathlib import Path
 from typing import List,Tuple
 
+from ctapipe.containers import DL1CameraContainer 
+
 
 import logging
 logging.basicConfig(format='%(asctime)s %(name)s %(levelname)s %(message)s')
 log = logging.getLogger(__name__)
 log.handlers = logging.getLogger('__main__').handlers
 
 __all__ = ['DataManagement','ChainGenerator']
@@ -86,41 +88,38 @@
             _type_: _description_
         """
 
         url = "http://nectarcam.in2p3.fr/elog/nectarcam-data-qm/?cmd=Find"
 
         url_run = f"http://nectarcam.in2p3.fr/elog/nectarcam-data-qm/?mode=full&reverse=0&reverse=1&npp=20&subtext=%23{run_number}"
 
-        #try to acces data by getting cookies from firefox and Chrome
-        log.debug('try to get data with cookies from Firefox abnd Chrome')
-        cookies = browser_cookie3.load()
-        req = requests.get(f'http://nectarcam.in2p3.fr/elog/nectarcam-data-qm/?jcmd=&mode=Raw&attach=1&printable=1&reverse=0&reverse=1&npp=20&ma=&da=&ya=&ha=&na=&ca=&last=&mb=&db=&yb=&hb=&nb=&cb=&Author=&Setup=&Category=&Keyword=&Subject=&ModuleCount=&subtext=%23{run_number}',cookies = cookies)
-        
-        if "<title>ELOG Login</title>" in req.text : 
-            log.debug('log to Elog with cookies impossible, try again with password')
+        if not(username is None or password is None) :  
+            log.debug('log to Elog with username and password')
             #log to Elog
             br = mechanize.Browser()
             br.open(url)
-
             form = br.select_form('form1')
-
             for i in range(4) : 
                 log.debug(br.form.find_control(nr=i).name)
-
             br.form['uname'] = username
             br.form['upassword'] = password
             br.method = "POST"
-
             req = br.submit()
             #html_page = req.get_data()
             cookies = br._ua_handlers['_cookies'].cookiejar
-
             #get data
-            req = requests.get(f'http://nectarcam.in2p3.fr/elog/nectarcam-data-qm/?jcmd=&mode=Raw&attach=1&printable=1&reverse=0&reverse=1&npp=20&ma=&da=&ya=&ha=&na=&ca=&last=&mb=&db=&yb=&hb=&nb=&cb=&Author=&Setup=&Category=&Keyword=&Subject=&ModuleCount=&subtext=%23{run_number}',cookies = cookies)
-
+            req = requests.get(f'http://nectarcam.in2p3.fr/elog/nectarcam-data-qm/?jcmd=&mode=Raw&attach=1&printable=1&reverse=0&reverse=1&npp=20&ma=&da=&ya=&ha=&na=&ca=&last=&mb=&db=&yb=&hb=&nb=&cb=&Author=&Setup=&Category=&Keyword=&Subject=%23{run_number}&ModuleCount=&subtext=',cookies = cookies)
+        
+        else : 
+            #try to acces data by getting cookies from firefox and Chrome
+            log.debug('try to get data with cookies from Firefox abnd Chrome')
+            cookies = browser_cookie3.load()
+            req = requests.get(f'http://nectarcam.in2p3.fr/elog/nectarcam-data-qm/?jcmd=&mode=Raw&attach=1&printable=1&reverse=0&reverse=1&npp=20&ma=&da=&ya=&ha=&na=&ca=&last=&mb=&db=&yb=&hb=&nb=&cb=&Author=&Setup=&Category=&Keyword=&Subject=%23{run_number}&ModuleCount=&subtext=',cookies = cookies)
+        
+        #if "<title>ELOG Login</title>" in req.text : 
 
         lines = req.text.split('\r\n')
 
         url_data = None
         for i,line in enumerate(lines) : 
             if '<p>' in line : 
                 url_data = line.split("</p>")[0].split('FC:')[1]
@@ -130,21 +129,22 @@
         if i == len(lines)-1 :
             e=Exception("lfns not found on GRID")
             log.error(e,exc_info=True)
             log.debug(lines)
             raise e
 
         if output_lfns : 
+            lfns = []
             try : 
                 #Dirac
                 dirac = Dirac()
                 loc = f"/vo.cta.in2p3.fr/nectarcam/{url_data.split('/')[-2]}/{url_data.split('/')[-1]}"
+                log.debug(f"searching in Dirac filecatalog at {loc}")
                 res = dirac.listCatalogDirectory(loc, printOutput=True)
 
-                lfns = []
                 for key in res['Value']['Successful'][loc]['Files'].keys():
                     if str(run_number) in key and "fits.fz" in key : 
                         lfns.append(key)
             except Exception as e : 
                 log.error(e,exc_info = True)
             return lfns
         else : 
@@ -178,7 +178,10 @@
             Generator: a generator which chains EventSource
         """
         if len(list) == 2 :
             return ChainGenerator.chain(list[0],list[1])
         else :
             return ChainGenerator.chain(list[0],ChainGenerator.chainEventSource(list[1:]))
 
+class CtaPipeExtractor():
+    def get_image_peak_time(cameraContainer : DL1CameraContainer) : 
+        return cameraContainer.image, cameraContainer.peak_time
```

### Comparing `nectarchain-0.1.3/src/nectarchain/calibration/container/waveforms.py` & `nectarchain-0.1.4/src/nectarchain/calibration/container/waveforms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from argparse import ArgumentError
 import numpy as np
 from matplotlib import pyplot as plt
 import copy
 import os
+import glob
 from pathlib import Path
 
 from enum import Enum
 
 from astropy.io import fits
 from astropy.table import QTable,Column,Table
 import astropy.units as u
@@ -35,27 +36,29 @@
     """
     TEL_ID = 0
     CAMERA = CameraGeometry.from_name("NectarCam-003")
     def __new__(cls,*args,**kwargs) : 
         obj = object.__new__(cls)
         return obj
 
-    def __init__(self,run_number : int,max_events : int = None,nevents : int = -1,run_file = None):
+    def __init__(self,run_number : int,max_events : int = None,nevents : int = -1,run_file = None, init_arrays : bool = False):
         """construtor
 
         Args:
             run_number (int): id of the run to be loaded
             maxevents (int, optional): max of events to be loaded. Defaults to 0, to load everythings.
             nevents (int, optional) : number of events in run if known (parameter used to save computing time)
             merge_file (optional) : if True will load all fits.fz files of the run, else merge_file can be integer to select the run fits.fz file according to this number
             
         """
 
         self.__run_number = run_number
-        #gerer ici le fait de traiter plusieurs fichiers ou simplement 1 par 1
+        self.__run_file = run_file
+        self.__max_events = max_events
+
         self.__reader = WaveformsContainer.load_run(run_number,max_events,run_file = run_file)
 
         #from reader members
         self.__npixels = self.__reader.camera_config.num_pixels
         self.__nsamples =  self.__reader.camera_config.num_samples
         self.__geometry = self.__reader.subarray.tel[WaveformsContainer.TEL_ID].camera
         self.__subarray =  self.__reader.subarray
@@ -63,46 +66,62 @@
         
         #set camera properties
         log.info(f"N pixels : {self.npixels}")
 
         #run properties
         if nevents != -1 :
             self.__nevents = nevents if max_events is None else min(max_events,nevents) #self.check_events()
+            self.__reader = None
         else :
             self.__nevents = self.check_events()
-            #reload file (bc check_events has drained reader generator)
-            self.__reader = WaveformsContainer.load_run(run_number,max_events,run_file = run_file)
+            
         log.info(f"N_events : {self.nevents}")
 
+        if init_arrays : 
+            self.__init_arrays()
+            
+    def __init_arrays(self,**kwargs) : 
+        log.debug('creation of the EventSource reader')
+        self.__reader = WaveformsContainer.load_run(self.__run_number,self.__max_events,run_file = self.__run_file)
+        
+        log.debug("create wfs, ucts, event properties and triger pattern arrays")
         #define zeros members which will be filled therafter
         self.wfs_hg = np.zeros((self.nevents,self.npixels,self.nsamples),dtype = np.uint16)
         self.wfs_lg = np.zeros((self.nevents,self.npixels,self.nsamples),dtype = np.uint16)
         self.ucts_timestamp = np.zeros((self.nevents),dtype = np.uint64)
         self.ucts_busy_counter = np.zeros((self.nevents),dtype = np.uint32)
         self.ucts_event_counter = np.zeros((self.nevents),dtype = np.uint32)
         self.event_type = np.zeros((self.nevents),dtype = np.uint8)
         self.event_id = np.zeros((self.nevents),dtype = np.uint32)
         self.trig_pattern_all = np.zeros((self.nevents,self.CAMERA.n_pixels,4),dtype = bool)
         #self.trig_pattern = np.zeros((self.nevents,self.npixels),dtype = bool)
         #self.multiplicity = np.zeros((self.nevents,self.npixels),dtype = np.uint16)
 
+        self.__broken_pixels_hg = np.zeros((self.npixels),dtype = bool)
+        self.__broken_pixels_lg = np.zeros((self.npixels),dtype = bool)
+
+
+    def __compute_broken_pixels(self,**kwargs) : 
+        log.warning("computation of broken pixels is not yet implemented")
+        self.__broken_pixels_hg = np.zeros((self.npixels),dtype = bool)
+        self.__broken_pixels_lg = np.zeros((self.npixels),dtype = bool)
 
     @staticmethod
     def load_run(run_number : int,max_events : int = None, run_file = None) : 
         """Static method to load from $NECTARCAMDATA directory data for specified run with max_events
 
         Args:
             run_number (int): run_id
             maxevents (int, optional): max of events to be loaded. Defaults to 0, to load everythings.
             merge_file (optional) : if True will load all fits.fz files of the run, else merge_file can be integer to select the run fits.fz file according to this number
         Returns:
             List[ctapipe_io_nectarcam.NectarCAMEventSource]: List of EventSource for each run files
         """
-        generic_filename,filenames = DataManagement.findrun(run_number)
         if run_file is None : 
+            generic_filename,_ = DataManagement.findrun(run_number)
             log.info(f"{str(generic_filename)} will be loaded")
             eventsource = NectarCAMEventSource(input_url=generic_filename,max_events=max_events)
         else :  
             log.info(f"{run_file} will be loaded")
             eventsource = NectarCAMEventSource(input_url=run_file,max_events=max_events)
         return eventsource
         
@@ -125,14 +144,22 @@
                 log.info(f"event {i} is {previous_trigger} : {previous_trigger.value} trigger type")
             n_events+=1
         return n_events
 
 
 
     def load_wfs(self,compute_trigger_patern = False):
+        """mathod to extract waveforms data from the EventSource 
+
+        Args:
+            compute_trigger_patern (bool, optional): To recompute on our side the trigger patern. Defaults to False.
+        """
+        if not(hasattr(self, "wfs_hg")) : 
+            self.__init_arrays()
+
         wfs_hg_tmp=np.zeros((self.npixels,self.nsamples),dtype = np.uint16)
         wfs_lg_tmp=np.zeros((self.npixels,self.nsamples),dtype = np.uint16)
 
         n_traited_events = 0
         for i,event in enumerate(self.__reader):
             if i%100 == 0:
                 log.info(f"reading event number {i}")
@@ -149,15 +176,15 @@
             for pix in range(self.npixels):
                 wfs_lg_tmp[pix]=event.r0.tel[0].waveform[1,self.pixels_id[pix]]
                 wfs_hg_tmp[pix]=event.r0.tel[0].waveform[0,self.pixels_id[pix]]
 
             self.wfs_hg[i] = wfs_hg_tmp
             self.wfs_lg[i] = wfs_lg_tmp
 
-
+        self.__compute_broken_pixels()
 
         #if compute_trigger_patern and np.max(self.trig_pattern) == 0:
         #    self.compute_trigger_patern()
 
 
     def write(self,path : str, **kwargs) : 
         """method to write in an output FITS file the WaveformsContainer. Two files are created, one FITS representing the data
@@ -175,41 +202,41 @@
         hdr = fits.Header()
         hdr['RUN'] = self.__run_number
         hdr['NEVENTS'] = self.nevents
         hdr['NPIXELS'] = self.npixels
         hdr['NSAMPLES'] = self.nsamples
         hdr['SUBARRAY'] = self.subarray.name
 
-        self.subarray.to_hdf(f"{Path(path)}/subarray_run{self.run_number}.hdf5",overwrite=kwargs.get('overwrite',False))
+        self.subarray.to_hdf(f"{Path(path)}/subarray_run{self.run_number}{suffix}.hdf5",overwrite=kwargs.get('overwrite',False))
 
 
 
         hdr['COMMENT'] = f"The waveforms containeur for run {self.__run_number} : primary is the pixels id, 2nd HDU : high gain waveforms, 3rd HDU : low gain waveforms, 4th HDU :  event properties and 5th HDU trigger paterns."
 
         primary_hdu = fits.PrimaryHDU(self.pixels_id,header=hdr)
 
-        wfs_hg_hdu = fits.ImageHDU(self.wfs_hg)
-        wfs_lg_hdu = fits.ImageHDU(self.wfs_lg)
+        wfs_hg_hdu = fits.ImageHDU(self.wfs_hg,name = "HG Waveforms")
+        wfs_lg_hdu = fits.ImageHDU(self.wfs_lg,name = "LG Waveforms")
 
 
         col1 = fits.Column(array = self.event_id, name = "event_id", format = '1J')
         col2 = fits.Column(array = self.event_type, name = "event_type", format = '1I')
         col3 = fits.Column(array = self.ucts_timestamp, name = "ucts_timestamp", format = '1K')
         col4 = fits.Column(array = self.ucts_busy_counter, name = "ucts_busy_counter", format = '1J')
         col5 = fits.Column(array = self.ucts_event_counter, name = "ucts_event_counter", format = '1J')
         col6 = fits.Column(array = self.multiplicity, name = "multiplicity", format = '1I')
 
         coldefs = fits.ColDefs([col1, col2, col3, col4, col5, col6])
-        event_properties = fits.BinTableHDU.from_columns(coldefs)
+        event_properties = fits.BinTableHDU.from_columns(coldefs,name = 'event properties')
 
         col1 = fits.Column(array = self.trig_pattern_all, name = "trig_pattern_all", format = f'{4 * self.CAMERA.n_pixels}L',dim = f'({self.CAMERA.n_pixels},4)')
         col2 = fits.Column(array = self.trig_pattern, name = "trig_pattern", format = f'{self.CAMERA.n_pixels}L')
         coldefs = fits.ColDefs([col1, col2])
-        trigger_patern = fits.BinTableHDU.from_columns(coldefs)
-        
+        trigger_patern = fits.BinTableHDU.from_columns(coldefs,name = 'trigger patern')
+
         hdul = fits.HDUList([primary_hdu, wfs_hg_hdu, wfs_lg_hdu,event_properties,trigger_patern])
         try : 
             hdul.writeto(Path(path)/f"waveforms_run{self.run_number}{suffix}.fits",overwrite=kwargs.get('overwrite',False))
             log.info(f"run saved in {Path(path)}/waveforms_run{self.run_number}{suffix}.fits")
         except OSError as e : 
             log.warning(e)
         except Exception as e :
@@ -227,63 +254,87 @@
         Args:
             path (str): path of the FITS file
 
         Returns:
             WaveformsContainer: WaveformsContainer instance
         """
         log.info(f"loading from {path}")
-        hdul = fits.open(Path(path))
+        with fits.open(Path(path)) as hdul : 
+            cls = WaveformsContainer.__new__(WaveformsContainer)
 
-        cls = WaveformsContainer.__new__(WaveformsContainer)
+            cls.__run_number = hdul[0].header['RUN'] 
+            cls.__nevents = hdul[0].header['NEVENTS'] 
+            cls.__npixels = hdul[0].header['NPIXELS'] 
+            cls.__nsamples = hdul[0].header['NSAMPLES'] 
 
-        cls.__run_number = hdul[0].header['RUN'] 
-        cls.__nevents = hdul[0].header['NEVENTS'] 
-        cls.__npixels = hdul[0].header['NPIXELS'] 
-        cls.__nsamples = hdul[0].header['NSAMPLES'] 
+            cls.__subarray = SubarrayDescription.from_hdf(Path(path.replace('waveforms_','subarray_').replace('fits','hdf5')))
 
-        cls.__subarray = SubarrayDescription.from_hdf(Path(path.replace('waveforms_','subarray_').replace('fits','hdf5')))
 
+            cls.__pixels_id = hdul[0].data
+            cls.wfs_hg = hdul[1].data
+            cls.wfs_lg = hdul[2].data
 
-        cls.__pixels_id = hdul[0].data
-        cls.wfs_hg = hdul[1].data
-        cls.wfs_lg = hdul[2].data
+            table_prop = hdul[3].data
+            cls.event_id = table_prop["event_id"]
+            cls.event_type = table_prop["event_type"]
+            cls.ucts_timestamp = table_prop["ucts_timestamp"]
+            cls.ucts_busy_counter = table_prop["ucts_busy_counter"]
+            cls.ucts_event_counter = table_prop["ucts_event_counter"]
 
-        table_prop = hdul[3].data
-        cls.event_id = table_prop["event_id"]
-        cls.event_type = table_prop["event_type"]
-        cls.ucts_timestamp = table_prop["ucts_timestamp"]
-        cls.ucts_busy_counter = table_prop["ucts_busy_counter"]
-        cls.ucts_event_counter = table_prop["ucts_event_counter"]
+            table_trigger = hdul[4].data
+            cls.trig_pattern_all = table_trigger["trig_pattern_all"]
 
-        table_trigger = hdul[4].data
-        cls.trig_pattern_all = table_trigger["trig_pattern_all"]
+        cls.__compute_broken_pixels()
 
         return cls
 
     
 
     
 
 
     def compute_trigger_patern(self) : 
+        """(preliminary) function to compute the trigger patern
+        """
         #mean.shape nevents * npixels
         mean,std =np.mean(self.wfs_hg,axis = 2),np.std(self.wfs_hg,axis = 2)
         self.trig_pattern = self.wfs_hg.max(axis = 2) > (mean + 3 * std)
 
 
 
     ##methods used to display
     def display(self,evt,cmap = 'gnuplot2') : 
+        """plot camera display
+
+        Args:
+            evt (int): event index
+            cmap (str, optional): colormap. Defaults to 'gnuplot2'.
+
+        Returns:
+            CameraDisplay: thoe cameraDisplay plot
+        """
         image = self.wfs_hg.sum(axis=2)
         disp = CameraDisplay(geometry=WaveformsContainer.CAMERA, image=image[evt], cmap=cmap)
         disp.add_colorbar()
         return disp
 
-    def plot_waveform(self,evt) :
-        fig,ax = plt.subplots(1,1)
+    def plot_waveform_hg(self,evt,**kwargs) :
+        """plot the waveform of the evt
+
+        Args:
+            evt (int): the event index
+
+        Returns:
+            tuple: the figure and axes
+        """
+        if 'figure' in kwargs.keys() and 'ax' in kwargs.keys() :
+            fig = kwargs.get('figure')
+            ax = kwargs.get('ax')
+        else : 
+            fig,ax = plt.subplots(1,1)
         ax.plot(self.wfs_hg[evt].T)
         return fig,ax
 
 
     def select_waveforms_hg(self,pixel_id : np.ndarray) : 
         """method to extract waveforms HG from a list of pixel ids 
         The output is the waveforms HG with a shape following the size of the input pixel_id argument
@@ -292,15 +343,15 @@
             pixel_id (np.ndarray): array of pixel ids you want to extract the waveforms
         Returns:
             (np.ndarray): waveforms array in the order of specified pixel_id
         """
         mask_contain_pixels_id = np.array([pixel in self.pixels_id for pixel in pixel_id],dtype = bool)
         for pixel in pixel_id[~mask_contain_pixels_id] : log.warning(f"You asked for pixel_id {pixel} but it is not present in this WaveformsContainer, skip this one")
         res = np.array([self.wfs_hg[:,np.where(self.pixels_id == pixel)[0][0],:] for pixel in pixel_id[mask_contain_pixels_id]])
-        res = res.reshape(res.shape[1],res.shape[0],res.shape[2])
+        res = res.transpose(res.shape[1],res.shape[0],res.shape[2])
         return res
 
 
     def select_waveforms_lg(self,pixel_id : np.ndarray) : 
         """method to extract waveforms LG from a list of pixel ids 
         The output is the waveforms LG with a shape following the size of the input pixel_id argument
         Pixel in pixel_id which are not present in the WaveformsContaineur pixels_id are skipped 
@@ -310,17 +361,24 @@
 
         Returns:
             (np.ndarray): waveforms array in the order of specified pixel_id
         """
         mask_contain_pixels_id = np.array([pixel in self.pixels_id for pixel in pixel_id],dtype = bool)
         for pixel in pixel_id[~mask_contain_pixels_id] : log.warning(f"You asked for pixel_id {pixel} but it is not present in this WaveformsContainer, skip this one")
         res =  np.array([self.wfs_lg[:,np.where(self.pixels_id == pixel)[0][0],:] for pixel in pixel_id[mask_contain_pixels_id]])
-        res = res.reshape(res.shape[1],res.shape[0],res.shape[2])
+        res = res.transpose(res.shape[1],res.shape[0],res.shape[2])
         return res
 
+
+    @property 
+    def _run_file(self) : return self.__run_file 
+
+    @property
+    def _max_events(self) : return self.__max_events
+
     @property
     def reader(self) : return self.__reader
 
     @property
     def npixels(self) : return self.__npixels
 
     @property
@@ -337,15 +395,20 @@
 
     @property
     def nevents(self) : return self.__nevents
 
     @property
     def run_number(self) : return self.__run_number
 
+    @property
+    def broken_pixels_hg(self) : return self.__broken_pixels_hg
 
+    @property
+    def broken_pixels_lg(self) : return self.__broken_pixels_lg
+    
     #physical properties
     @property
     def multiplicity(self) :  return np.uint16(np.count_nonzero(self.trig_pattern,axis = 1))
 
     @property
     def trig_pattern(self) :  return self.trig_pattern_all.any(axis = 1)
 
@@ -354,39 +417,128 @@
 
 
 
 
 class WaveformsContainers() : 
     """This class is to be used for computing waveforms of a run treating run files one by one
     """
+    def __new__(cls,*args,**kwargs) : 
+        """base class constructor
 
-    def __init__(self,run_number : int,max_events : int = None) :
+        Returns:
+            WaveformsContainers : the new object
+        """
+        obj = object.__new__(cls)
+        return obj
+    
+    def __init__(self,run_number : int,max_events : int = None, init_arrays : bool = False) :
+        """initialize the waveformsContainer list inside the main object
+
+        Args:
+            run_number (int): the run number
+            max_events (int, optional): max events we want to read. Defaults to None.
+        """
         log.info('Initialization of WaveformsContainers') 
         _,filenames = DataManagement.findrun(run_number)
         self.waveformsContainer = []
         self.__nWaveformsContainer = 0
         for i,file in enumerate(filenames) : 
-            self.waveformsContainer.append(WaveformsContainer(run_number,max_events=max_events,run_file=file))
+            self.waveformsContainer.append(WaveformsContainer(run_number,max_events=max_events,run_file=file, init_arrays= init_arrays))
             self.__nWaveformsContainer += 1
             if not(max_events is None) : max_events -= self.waveformsContainer[i].nevents
             log.info(f'WaveformsContainer number {i} is created')
-            if max_events <= 0 : break
+            if not(max_events is None) and max_events <= 0 : break
+
+    def load_wfs(self,compute_trigger_patern = False,index : int = None) : 
+        """load waveforms from the Eventsource reader
+
+        Args:
+            compute_trigger_patern (bool, optional): to compute manually the trigger patern. Defaults to False.
+            index (int, optional): to only load waveforms from EventSource for the waveformsContainer at index, this parameters
+            can be used to load, write or perform some work step by step. Thus all the event are not nessessary loaded at the same time 
+            In such case memory can be saved. Defaults to None.
+
+        Raises:
+            IndexError: the index is > nWaveformsContainer or < 0
+        """
+        if index is None : 
+            for i in range(self.__nWaveformsContainer) : 
+                self.waveformsContainer[i].load_wfs(compute_trigger_patern = compute_trigger_patern)
+        else : 
+            if index < self.__nWaveformsContainer and index >= 0 : 
+                self.waveformsContainer[index].load_wfs(compute_trigger_patern = compute_trigger_patern)
+            else : 
+                raise IndexError(f"index must be >= 0 and < {self.__nWaveformsContainer}")
+
+
+    def write(self,path : str, index : int = None, **kwargs) : 
+        """method to write on disk all the waveformsContainer in the list
+
+        Args:
+            path (str): path where to save the waveforms
+            index (int, optional): index of the waveforms list you want to write. Defaults to None.
+
+        Raises:
+            IndexError: the index is > nWaveformsContainer or < 0
+        """
+        if index is None : 
+            for i in range(self.__nWaveformsContainer) : 
+                self.waveformsContainer[i].write(path,suffix = f"{i:04d}" ,**kwargs)
+        else : 
+            if index < self.__nWaveformsContainer and index >= 0 : 
+                self.waveformsContainer[index].write(path,suffix = f"{index:04d}" ,**kwargs)
+            else : 
+                raise IndexError(f"index must be >= 0 and < {self.__nWaveformsContainer}")
+
+    @staticmethod
+    def load(path : str) :
+        """method to load the waveforms list from splited fits files
+
+        Args:
+            path (str): path where data should be, it contain filename without extension
+
+        Raises:
+            e: File not found
+
+        Returns:
+            WaveformsContainers:
+        """
+        log.info(f"loading from {path}")
+        files = glob.glob(f"{path}_*.fits")
+        if len(files) == 0 : 
+            e = FileNotFoundError(f"no files found corresponding to {path}_*.fits")
+            log.error(e)
+            raise e
+        else : 
+            cls = WaveformsContainers.__new__(WaveformsContainers)
+            cls.waveformsContainer = []
+            cls.__nWaveformsContainer = len(files)
+            for file in files : 
+                cls.waveformsContainer.append(WaveformsContainer.load(file))
+            return cls
+
 
-    def load_wfs(self,compute_trigger_patern = False) : 
-        for i in range(self.__nWaveformsContainer) : 
-            self.waveformsContainer[i].load_wfs(compute_trigger_patern = compute_trigger_patern)
 
-    def write(self,path : str, **kwargs) : 
-        for i in range(self.__nWaveformsContainer) : 
-            self.waveformsContainer[i].write(path,suffix = f"{i:04d}" ,**kwargs)
 
         
     @property
-    def nWaveformsContainer(self) : return self.__nWaveformsContainer
+    def nWaveformsContainer(self) : 
+        """getter giving the number of waveformsContainer into the waveformsContainers instance
+
+        Returns:
+            int: the number of waveformsContainer
+        """
+        return self.__nWaveformsContainer
 
     @property
     def nevents(self) : 
+        """getter giving the number of events in the waveformsContainers instance"""
         return np.sum([self.waveformsContainer[i].nevents for i in range(self.__nWaveformsContainer)])
 
     def append(self,waveformsContainer : WaveformsContainer) : 
-        self.waveforms.append(waveformsContainer)
+        """method to append WaveformsContainer to the waveforms list
+
+        Args:
+            waveformsContainer (WaveformsContainer): the waveformsContainer to stack
+        """
+        self.waveformsContainer.append(waveformsContainer)
         self.__nWaveformsContainer += 1
```

### Comparing `nectarchain-0.1.3/src/nectarchain/dqm/camera_monitoring.py` & `nectarchain-0.1.4/src/nectarchain/dqm/camera_monitoring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,156 +1,173 @@
-
-from dqm_summary_processor import *
-import math
+from dqm_summary_processor import dqm_summary
+from matplotlib import pyplot as plt
+from ctapipe.visualization import CameraDisplay
+from ctapipe.instrument import CameraGeometry
+from ctapipe.coordinates import EngineeringCameraFrame
+from astropy import time as astropytime
+import numpy as np
 import sqlite3
-import os
 
 
 class CameraMonitoring(dqm_summary):
-
     def __init__(self, gaink):
-
         self.k = gaink
         return None
 
-    def ConfigureForRun(self,path, Chan, Samp, Reader1):
-        #define number of channels and samples
+    def ConfigureForRun(self, path, Chan, Samp, Reader1):
+        # define number of channels and samples
         self.Chan = Chan
-        self.Samp= Samp
+        self.Samp = Samp
 
-
-        self.camera = CameraGeometry.from_name("NectarCam", 3)
-        self.cmap = 'gnuplot2'
+        self.camera = CameraGeometry.from_name("NectarCam-003").transform_to(EngineeringCameraFrame())#CameraGeometry.from_name("NectarCam", 3)
+        self.cmap = "gnuplot2"
 
         self.subarray = Reader1.subarray
 
         self.event_id = []
         self.event_times = []
 
         for i, evt1 in enumerate(Reader1):
-            self.run_start1= evt1.nectarcam.tel[0].svc.date 
+            self.run_start1 = evt1.nectarcam.tel[0].svc.date
 
-        SqlFileDate = (astropytime.Time(self.run_start1, format='unix').iso).split(" ")[0]
+        SqlFileDate = (astropytime.Time(self.run_start1, format="unix").iso).split(" ")[
+            0
+        ]
 
         SqlFilePath = ""
-        for i in range(len(path.split("/"))-1):
-            SqlFilePath = SqlFilePath  +  path.split("/")[i] + "/"
+        for i in range(len(path.split("/")) - 1):
+            SqlFilePath = SqlFilePath + path.split("/")[i] + "/"
 
         SqlFileName = SqlFilePath + "nectarcam_monitoring_db_" + SqlFileDate + ".sqlite"
         print("SqlFileName", SqlFileName)
-
         con = sqlite3.connect(SqlFileName) 
         cursor = con.cursor()  
-        #print(cursor.fetchall())
-        cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
-        TempData=cursor.execute('''SELECT * FROM monitoring_drawer_temperatures''')
-        #print(TempData.description)
+        try:
+            #print(cursor.fetchall())
+            cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
+            TempData=cursor.execute('''SELECT * FROM monitoring_drawer_temperatures''')
+            #print(TempData.description)
+            self.DrawerTemp = cursor.fetchall()
+            cursor.close()
+            
+        except sqlite3.Error as err:
+            print("Error Code: ", err)
+            print("DRAWER TEMPERATURE COULD NOT BE RETRIEVED!")
 
-        self.DrawerTemp = cursor.fetchall()
-        cursor.close()
 
-    def ProcessEvent(self, evt):
+    def ProcessEvent(self, evt, noped):
         trigger_time = evt.trigger.time.value
         trigger_id = evt.index.event_id
 
         self.event_times.append(trigger_time)
         self.event_id.append(trigger_id)
 
-
-
     def FinishRun(self):
+        try:
 
-        self.event_id = np.array(self.event_id)
-        self.event_times = np.array(self.event_times)
-
-        self.run_start = self.event_times[self.event_id == np.min(self.event_id)] - 100
-        self.run_end = np.max(self.event_times) + 100
-
-        self.DrawerTemp = np.array(self.DrawerTemp)
-        self.DrawerTimes = np.array(self.DrawerTemp[:,3])
-
-        for i in range(len(self.DrawerTimes)):
-            self.DrawerTimes[i] = astropytime.Time(self.DrawerTimes[i], format = 'iso').unix
-
-
-        self.DrawerTemp11 = self.DrawerTemp[:,4][self.DrawerTimes > self.run_start]
-        self.DrawerTemp21 = self.DrawerTemp[:,5][self.DrawerTimes > self.run_start]
-        self.DrawerNum1 = self.DrawerTemp[:,2][self.DrawerTimes > self.run_start]
-
-        self.DrawerTimes_new = self.DrawerTimes[self.DrawerTimes > self.run_start]
-
-        self.DrawerTemp12 = self.DrawerTemp11[self.DrawerTimes_new < self.run_end]
-        self.DrawerTemp22 = self.DrawerTemp21[self.DrawerTimes_new < self.run_end]
-        self.DrawerNum2 = self.DrawerNum1[self.DrawerTimes_new < self.run_end]   
-
-        self.DrawerTemp1_mean = []
-        self.DrawerTemp2_mean = []
-        TotalDrawers = np.max(self.DrawerNum2)
-
-        for i in range(TotalDrawers+1):
-            for j in range(7):
-                self.DrawerTemp1_mean.append(np.mean(self.DrawerTemp12[self.DrawerNum2 == i]))
-                self.DrawerTemp2_mean.append(np.mean(self.DrawerTemp22[self.DrawerNum2 == i]))
-        self.DrawerTemp1_mean = np.array(self.DrawerTemp1_mean)
-        self.DrawerTemp2_mean = np.array(self.DrawerTemp2_mean)
-
-        self.DrawerTemp_mean = (self.DrawerTemp1_mean + self.DrawerTemp2_mean)/2
+            self.event_id = np.array(self.event_id)
+            self.event_times = np.array(self.event_times)
+    
+            self.run_start = self.event_times[self.event_id == np.min(self.event_id)] - 100
+            self.run_end = np.max(self.event_times) + 100
+    
+            self.DrawerTemp = np.array(self.DrawerTemp)
+            self.DrawerTimes = np.array(self.DrawerTemp[:,3])
+    
+            for i in range(len(self.DrawerTimes)):
+                self.DrawerTimes[i] = astropytime.Time(self.DrawerTimes[i], format = 'iso').unix
+    
+    
+            self.DrawerTemp11 = self.DrawerTemp[:,4][self.DrawerTimes > self.run_start]
+            self.DrawerTemp21 = self.DrawerTemp[:,5][self.DrawerTimes > self.run_start]
+            self.DrawerNum1 = self.DrawerTemp[:,2][self.DrawerTimes > self.run_start]
+    
+            self.DrawerTimes_new = self.DrawerTimes[self.DrawerTimes > self.run_start]
+    
+            self.DrawerTemp12 = self.DrawerTemp11[self.DrawerTimes_new < self.run_end]
+            self.DrawerTemp22 = self.DrawerTemp21[self.DrawerTimes_new < self.run_end]
+            self.DrawerNum2 = self.DrawerNum1[self.DrawerTimes_new < self.run_end]   
+    
+            self.DrawerTemp1_mean = []
+            self.DrawerTemp2_mean = []
+            TotalDrawers = np.max(self.DrawerNum2)
+    
+            for i in range(TotalDrawers+1):
+                for j in range(7):
+                    self.DrawerTemp1_mean.append(np.mean(self.DrawerTemp12[self.DrawerNum2 == i]))
+                    self.DrawerTemp2_mean.append(np.mean(self.DrawerTemp22[self.DrawerNum2 == i]))
+            self.DrawerTemp1_mean = np.array(self.DrawerTemp1_mean)
+            self.DrawerTemp2_mean = np.array(self.DrawerTemp2_mean)
+    
+            self.DrawerTemp_mean = (self.DrawerTemp1_mean + self.DrawerTemp2_mean)/2
+        except Exception as err:
+            print("Error Code: ", err)
+            print("DRAWER TEMPERATURE COULD NOT BE RETRIEVED!")
 
 
     def GetResults(self):
         self.CameraMonitoring_Results_Dict = {}
-        self.CameraMonitoring_Results_Dict["CAMERA-TEMPERATURE-AVERAGE"] = self.DrawerTemp_mean
+        try:
+            self.CameraMonitoring_Results_Dict["CAMERA-TEMPERATURE-AVERAGE"] = self.DrawerTemp_mean
+        except Exception as err:
+            print("Error Code: ", err)
+            print("DRAWER TEMPERATURE COULD NOT BE RETRIEVED!")
 
         return self.CameraMonitoring_Results_Dict
 
-    def PlotResults(self,name,FigPath):
-        self.ChargeInt_Figures_Dict={}
+    def PlotResults(self, name, FigPath):
+        self.ChargeInt_Figures_Dict = {}
         self.ChargeInt_Figures_Names_Dict = {}
 
-        fig, disp = plt.subplots()
-        disp = CameraDisplay(self.camera)
-        disp.image = self.DrawerTemp_mean
-        disp.cmap = plt.cm.coolwarm
-        disp.axes.text(1.8, -0.3, 'Temperature', fontsize=12,rotation=90)
-        disp.add_colorbar()
-        plt.title("Camera temperature average")
-        full_name = name + '_CameraTemperature_Mean.png'
-        FullPath = FigPath +full_name
-        self.ChargeInt_Figures_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE"] = fig
-        self.ChargeInt_Figures_Names_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE"] = FullPath
-
-        plt.close()
-
-
-
-        fig1, disp = plt.subplots()
-        disp = CameraDisplay(self.camera)
-        disp.image = self.DrawerTemp1_mean
-        disp.cmap = plt.cm.coolwarm
-        disp.axes.text(1.8, -0.3, 'Temperature 1', fontsize=12,rotation=90)
-        disp.add_colorbar()
-        plt.title("Camera temperature average 1")
-        full_name = name + '_CameraTemperature_average1.png'
-        FullPath = FigPath +full_name
-        self.ChargeInt_Figures_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-1"] = fig1
-        self.ChargeInt_Figures_Names_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-1"] = FullPath
-
-        plt.close()
-
-
+        try:
 
-        fig2, disp = plt.subplots()
-        disp = CameraDisplay(self.camera)
-        disp.image = self.DrawerTemp2_mean
-        disp.cmap = plt.cm.coolwarm
-        disp.axes.text(1.8, -0.3, 'Temperature 2', fontsize=12,rotation=90)
-        disp.add_colorbar()
-        plt.title("Camera temperature average 2")
-        full_name = name + '_CameraTemperature_average2.png'
-        FullPath = FigPath +full_name
-        self.ChargeInt_Figures_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-2"] = fig2
-        self.ChargeInt_Figures_Names_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-2"] = FullPath
+            fig, disp = plt.subplots()
+            disp = CameraDisplay(self.camera)
+            disp.image = self.DrawerTemp_mean
+            disp.cmap = plt.cm.coolwarm
+            disp.axes.text(1.8, -0.3, 'Temperature', fontsize=12,rotation=90)
+            disp.add_colorbar()
+            plt.title("Camera temperature average")
+            full_name = name + '_CameraTemperature_Mean.png'
+            FullPath = FigPath +full_name
+            self.ChargeInt_Figures_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE"] = fig
+            self.ChargeInt_Figures_Names_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE"] = FullPath
+    
+            plt.close()
+    
+    
+    
+            fig1, disp = plt.subplots()
+            disp = CameraDisplay(self.camera)
+            disp.image = self.DrawerTemp1_mean
+            disp.cmap = plt.cm.coolwarm
+            disp.axes.text(1.8, -0.3, 'Temperature 1', fontsize=12,rotation=90)
+            disp.add_colorbar()
+            plt.title("Camera temperature average 1")
+            full_name = name + '_CameraTemperature_average1.png'
+            FullPath = FigPath +full_name
+            self.ChargeInt_Figures_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-1"] = fig1
+            self.ChargeInt_Figures_Names_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-1"] = FullPath
+    
+            plt.close()
+    
+    
+    
+            fig2, disp = plt.subplots()
+            disp = CameraDisplay(self.camera)
+            disp.image = self.DrawerTemp2_mean
+            disp.cmap = plt.cm.coolwarm
+            disp.axes.text(1.8, -0.3, 'Temperature 2', fontsize=12,rotation=90)
+            disp.add_colorbar()
+            plt.title("Camera temperature average 2")
+            full_name = name + '_CameraTemperature_average2.png'
+            FullPath = FigPath +full_name
+            self.ChargeInt_Figures_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-2"] = fig2
+            self.ChargeInt_Figures_Names_Dict["CAMERA-TEMPERATURE-IMAGE-AVERAGE-2"] = FullPath
+    
+            plt.close()
 
-        plt.close()
 
-        return  self.ChargeInt_Figures_Dict, self.ChargeInt_Figures_Names_Dict
+        except Exception as err:
+            print("Error Code: ", err)
 
+        return self.ChargeInt_Figures_Dict, self.ChargeInt_Figures_Names_Dict
```

### Comparing `nectarchain-0.1.3/src/nectarchain/dqm/charge_integration.py` & `nectarchain-0.1.4/src/nectarchain/dqm/charge_integration.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,303 +1,473 @@
+from dqm_summary_processor import dqm_summary
+from matplotlib import pyplot as plt
+import numpy as np
+from ctapipe.visualization import CameraDisplay
+from ctapipe.instrument import CameraGeometry
+from ctapipe.coordinates import EngineeringCameraFrame
+from traitlets.config.loader import Config
+import ctapipe.instrument.camera.readout
+from ctapipe.image import LocalPeakWindowSum
 
-from dqm_summary_processor import *
 
 class ChargeIntegration_HighLowGain(dqm_summary):
-
     def __init__(self, gaink):
+        self.k = gaink
+        return None
 
-    	self.k = gaink
-    	return None
-
-    def ConfigureForRun(self,path, Chan, Samp, Reader1):
-        #define number of channels and samples
+    def ConfigureForRun(self, path, Chan, Samp, Reader1):
+        # define number of channels and samples
         self.Chan = Chan
-        self.Samp= Samp
+        self.Samp = Samp
 
         self.counter_evt = 0
         self.counter_ped = 0
 
-        self.camera = CameraGeometry.from_name("NectarCam-003")
-        self.cmap = 'gnuplot2'
+        self.camera = CameraGeometry.from_name("NectarCam-003").transform_to(EngineeringCameraFrame())#CameraGeometry.from_name("NectarCam", 3)
+        self.cmap = "gnuplot2"
 
-        #reader1=EventSource(input_url=path, max_events = 1)
+        # reader1=EventSource(input_url=path, max_events = 1)
         self.subarray = Reader1.subarray
         subarray = Reader1.subarray
-        subarray.tel[0].camera.readout = ctapipe.instrument.camera.readout.CameraReadout.from_name("NectarCam")
-        config = Config({"LocalPeakWindowSum": {"window_shift": 4, "window_width": 12}})
+        subarray.tel[
+            0
+        ].camera.readout = ctapipe.instrument.camera.readout.CameraReadout.from_name(
+            "NectarCam"
+        )
+        config = Config(
+            {"LocalPeakWindowSum": {"window_shift": 4, "window_width": 12}}
+        )
 
         self.integrator = LocalPeakWindowSum(subarray, config=config)
 
         self.image_all = []
-        self.peakpos_all =  []
+        self.peakpos_all = []
 
         self.image_ped = []
         self.peakpos_ped = []
 
+        
+
 
-    def ProcessEvent(self, evt):
+    def ProcessEvent(self, evt, noped):
         #print("test", evt.r0.tel[0].waveform[0])
-        waveform=evt.r0.tel[0].waveform[0]
-        image, peakpos = self.integrator(waveform,0,np.zeros(self.Chan, dtype = int))
+        self.pixelBAD = evt.mon.tel[0].pixel_status.hardware_failing_pixels
+        pixel = evt.nectarcam.tel[0].svc.pixel_ids
+        pixel21 = np.arange(0, 21, 1, dtype=int)
+        pixel = list(pixel)
+        pixel21 = list(pixel21)
+        pixels = np.concatenate([pixel21, pixel])
+
+        waveform=evt.r0.tel[0].waveform[self.k]
+
+        if noped:
+            ped = np.mean(waveform[:, 20])
+            w_noped = waveform - ped
+            output = self.integrator(w_noped,0,np.zeros(self.Chan, dtype = int), self.pixelBAD)
+            image = output.image
+            peakpos = output.peak_time
+            image = image[pixels]
+            peakpos = peakpos[pixels]
+
+        else:
+            output = self.integrator(waveform,0,np.zeros(self.Chan, dtype = int), self.pixelBAD)
+            image = output.image
+            peakpos = output.peak_time
+            image = image[pixels]
+            peakpos = peakpos[pixels]
 
-        if evt.trigger.event_type.value == 32: #count peds 
+        if evt.trigger.event_type.value == 32:  # count peds
             self.counter_ped += 1
             self.image_ped.append(image)
             self.peakpos_ped.append(peakpos)
         else:
             self.counter_evt += 1
             self.image_all.append(image)
             self.peakpos_all.append(peakpos)
-    	
 
     def FinishRun(self):
-
-        self.peakpos_all = np.array(self.peakpos_all, dtype = float) 
+        self.peakpos_all = np.array(self.peakpos_all, dtype=float)
         if self.counter_ped > 0:
-            self.peakpos_ped = np.array(self.peakpos_ped, dtype = float)
+            self.peakpos_ped = np.array(self.peakpos_ped, dtype=float)
 
-        #rms, percentile, mean deviation, median, mean, 
-        self.image_all = np.array(self.image_all, dtype = float)       
+        # rms, percentile, mean deviation, median, mean,
+        self.image_all = np.array(self.image_all, dtype=float)
         self.image_all_median = np.median(self.image_all, axis=0)
         self.image_all_average = np.mean(self.image_all, axis=0)
         self.image_all_std = np.std(self.image_all, axis=0)
         self.image_all_rms = np.sqrt(np.sum(self.image_all**2, axis=0))
 
         if self.counter_ped > 0:
-            self.image_ped = np.array(self.image_ped, dtype = float)
+            self.image_ped = np.array(self.image_ped, dtype=float)
             self.image_ped_median = np.median(self.image_ped, axis=0)
             self.image_ped_average = np.mean(self.image_ped, axis=0)
             self.image_ped_std = np.std(self.image_ped, axis=0)
             self.image_ped_rms = np.sqrt(np.sum(self.image_ped**2, axis=0))
 
-
-    
     def GetResults(self):
-
         self.ChargeInt_Results_Dict = {}
 
-        if (self.k==0):
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-HIGH-GAIN"]  = self.image_all_average
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-HIGH-GAIN"]  = self.image_all_median
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-RMS-HIGH-GAIN"]  = self.image_all_rms
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-STD-HIGH-GAIN"]  = self.image_all_std
+        if self.k == 0:
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-HIGH-GAIN"
+            ] = self.image_all_average
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-HIGH-GAIN"
+            ] = self.image_all_median
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-RMS-HIGH-GAIN"
+            ] = self.image_all_rms
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-STD-HIGH-GAIN"
+            ] = self.image_all_std
 
             if self.counter_ped > 0:
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-AVERAGE-HIGH-GAIN"]  = self.image_ped_average
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-MEDIAN-HIGH-GAIN"]  = self.image_ped_median
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-RMS-HIGH-GAIN"]  = self.image_ped_rms
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-STD-HIGH-GAIN"]  = self.image_ped_std
-
-        if (self.k ==1):
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-LOW-GAIN"]  = self.image_all_average 
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-LOW-GAIN"]  = self.image_all_median
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-RMS-LOW-GAIN"]  = self.image_all_rms
-            self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-IMAGE-ALL-STD-LOW-GAIN"]  = self.image_all_std
-            
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-AVERAGE-HIGH-GAIN"
+                ] = self.image_ped_average
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-MEDIAN-HIGH-GAIN"
+                ] = self.image_ped_median
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-RMS-HIGH-GAIN"
+                ] = self.image_ped_rms
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-STD-HIGH-GAIN"
+                ] = self.image_ped_std
+
+        if self.k == 1:
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-LOW-GAIN"
+            ] = self.image_all_average
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-LOW-GAIN"
+            ] = self.image_all_median
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-RMS-LOW-GAIN"
+            ] = self.image_all_rms
+            self.ChargeInt_Results_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-STD-LOW-GAIN"
+            ] = self.image_all_std
+
             if self.counter_ped > 0:
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-AVERAGE-LOW-GAIN"]  = self.image_ped_average
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-MEDIAN-LOW-GAIN"]  = self.image_ped_median
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-RMS-LOW-GAIN"]  = self.image_ped_rms
-                self.ChargeInt_Results_Dict["CHARGE-INTEGRATION-PED-ALL-STD-LOW-GAIN"]  = self.image_ped_std
-        
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-AVERAGE-LOW-GAIN"
+                ] = self.image_ped_average
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-MEDIAN-LOW-GAIN"
+                ] = self.image_ped_median
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-RMS-LOW-GAIN"
+                ] = self.image_ped_rms
+                self.ChargeInt_Results_Dict[
+                    "CHARGE-INTEGRATION-PED-ALL-STD-LOW-GAIN"
+                ] = self.image_ped_std
 
         return self.ChargeInt_Results_Dict
 
-
-    def PlotResults(self,name,FigPath):
+    def PlotResults(self, name, FigPath):
         self.ChargeInt_Figures_Dict = {}
         self.ChargeInt_Figures_Names_Dict = {}
 
+        # titles = ['All', 'Pedestals']
+        if self.k == 0:
+            gain_c = "High"
+        if self.k == 1:
+            gain_c = "Low"
 
-        titles = ['All', 'Pedestals']
-        if (self.k==0):
-            gain_c = 'High'
-        if (self.k ==1):
-            gain_c = 'Low'
-
-
-        #Charge integration MEAN plot
+        # Charge integration MEAN plot
         if self.counter_evt > 0:
             fig1, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            #disp = CameraDisplay(self.subarray.tels[0].camera)
-            disp.image = self.image_all_average
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            # disp = CameraDisplay(self.subarray.tels[0].camera)
+            disp.image = self.image_all_average[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
 
-            plt.title("Charge Integration Mean %s Gain (ALL)" %gain_c)
+            plt.title("Charge Integration Mean %s Gain (ALL)" % gain_c)
 
-            full_name = name + '_ChargeInt_Mean_%sGain_All.png' %gain_c 
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-%s-GAIN" %gain_c] = fig1
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-%s-GAIN" %gain_c] = FullPath
+            full_name = name + "_ChargeInt_Mean_%sGain_All.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-%s-GAIN" % gain_c
+            ] = fig1
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-AVERAGE-%s-GAIN" % gain_c
+            ] = FullPath
 
             plt.close()
 
-
         if self.counter_ped > 0:
             fig2, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_ped_average
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_ped_average[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
 
-            plt.title("Charge Integration Mean %s Gain (PED)" %gain_c)
+            plt.title("Charge Integration Mean %s Gain (PED)" % gain_c)
 
-            full_name = name + '_ChargeInt_Mean_%sGain_Ped.png' %gain_c 
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-PED-AVERAGE-%s-GAIN" %gain_c] = fig2
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-PED-AVERAGE-%s-GAIN" %gain_c] = FullPath
+            full_name = name + "_ChargeInt_Mean_%sGain_Ped.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-AVERAGE-%s-GAIN" % gain_c
+            ] = fig2
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-AVERAGE-%s-GAIN" % gain_c
+            ] = FullPath
 
             plt.close()
 
-
-        #Charge integration MEDIAN plot
+        # Charge integration MEDIAN plot
         if self.counter_evt > 0:
             fig3, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_all_median
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_all_median[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
-    
-            plt.title("Charge Integration Median %s Gain (ALL)" %gain_c)
-    
-            full_name = name + '_ChargeInt_Median_%sGain_All.png' %gain_c 
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-%s-GAIN" %gain_c] = fig3
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-%s-GAIN" %gain_c] = FullPath
-    
-            plt.close()
 
+            plt.title("Charge Integration Median %s Gain (ALL)" % gain_c)
+
+            full_name = name + "_ChargeInt_Median_%sGain_All.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-%s-GAIN" % gain_c
+            ] = fig3
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-MEDIAN-%s-GAIN" % gain_c
+            ] = FullPath
+
+            plt.close()
 
         if self.counter_ped > 0:
             fig4, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_ped_median
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_ped_median[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
 
-            plt.title("Charge Integration Median %s Gain (PED)" %gain_c)
-            
-            full_name = name + '_ChargeInt_Median_%sGain_Ped.png' %gain_c
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-PED-MEDIAN-%s-GAIN" %gain_c] = fig4
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-PED-MEDIAN-%s-GAIN" %gain_c] = FullPath
+            plt.title("Charge Integration Median %s Gain (PED)" % gain_c)
 
-            plt.close()
+            full_name = name + "_ChargeInt_Median_%sGain_Ped.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-MEDIAN-%s-GAIN" % gain_c
+            ] = fig4
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-MEDIAN-%s-GAIN" % gain_c
+            ] = FullPath
 
+            plt.close()
 
-        #Charge integration STD plot
+        # Charge integration STD plot
         if self.counter_evt > 0:
             fig5, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_all_std
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_all_std[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
-    
-            plt.title("Charge Integration STD %s Gain (ALL)" %gain_c)
-                
-            full_name = name + '_ChargeInt_Std_%sGain_All.png' %gain_c
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-ALL-STD-%s-GAIN" %gain_c] = fig5
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-ALL-STD-%s-GAIN" %gain_c] = FullPath
-    
+
+            plt.title("Charge Integration STD %s Gain (ALL)" % gain_c)
+
+            full_name = name + "_ChargeInt_Std_%sGain_All.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-STD-%s-GAIN" % gain_c
+            ] = fig5
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-STD-%s-GAIN" % gain_c
+            ] = FullPath
+
             plt.close()
-        
+
         if self.counter_ped > 0:
             fig6, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_ped_std
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_ped_std[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
 
-            plt.title("Charge Integration STD %s Gain (PED)" %gain_c)
-            
-            full_name = name + '_ChargeInt_Std_%sGain_Ped.png' %gain_c
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-PED-STD-%s-GAIN" %gain_c] = fig6
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-PED-STD-%s-GAIN" %gain_c] = FullPath
+            plt.title("Charge Integration STD %s Gain (PED)" % gain_c)
 
-            plt.close()
+            full_name = name + "_ChargeInt_Std_%sGain_Ped.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-STD-%s-GAIN" % gain_c
+            ] = fig6
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-STD-%s-GAIN" % gain_c
+            ] = FullPath
 
+            plt.close()
 
-        
-        #Charge integration RMS plot
+        # Charge integration RMS plot
         if self.counter_evt > 0:
             fig7, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_all_rms
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_all_rms[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
-    
-            plt.title("Charge Integration RMS %s Gain (ALL)" %gain_c)
-                
-            full_name = name + '_ChargeInt_Rms_%sGain_All.png' %gain_c
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-ALL-RMS-%s-GAIN" %gain_c] = fig7
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-ALL-RMS-%s-GAIN" %gain_c] = FullPath
-    
+
+            plt.title("Charge Integration RMS %s Gain (ALL)" % gain_c)
+
+            full_name = name + "_ChargeInt_Rms_%sGain_All.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-RMS-%s-GAIN" % gain_c
+            ] = fig7
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-ALL-RMS-%s-GAIN" % gain_c
+            ] = FullPath
+
             plt.close()
-    
+
         if self.counter_ped > 0:
             fig8, disp = plt.subplots()
-            disp = CameraDisplay(self.camera)
-            disp.image = self.image_ped_rms
+            disp = CameraDisplay(self.camera[~self.pixelBAD[0]])
+            disp.image = self.image_ped_rms[~self.pixelBAD[0]]
             disp.cmap = plt.cm.coolwarm
-            disp.axes.text(2, -0.8, f'{gain_c} gain integrated charge (DC)', fontsize=12,rotation=90)
+            disp.axes.text(
+                2,
+                -0.8,
+                f"{gain_c} gain integrated charge (DC)",
+                fontsize=12,
+                rotation=90,
+            )
             disp.add_colorbar()
 
-            plt.title("Charge Integration RMS %s Gain (PED)" %gain_c)
-            
-            full_name = name + '_ChargeInt_Rms_%sGain_Ped.png' %gain_c
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-IMAGE-PED-RMS-%s-GAIN" %gain_c] = fig8
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-IMAGE-PED-RMS-%s-GAIN" %gain_c] = FullPath
+            plt.title("Charge Integration RMS %s Gain (PED)" % gain_c)
 
-            plt.close()
+            full_name = name + "_ChargeInt_Rms_%sGain_Ped.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-RMS-%s-GAIN" % gain_c
+            ] = fig8
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-IMAGE-PED-RMS-%s-GAIN" % gain_c
+            ] = FullPath
 
+            plt.close()
 
-        #Charge integration SPECTRUM
+        # Charge integration SPECTRUM
         if self.counter_evt > 0:
             fig9, disp = plt.subplots()
             for i in range(self.Chan):
-                plt.hist(self.image_all[:,i],100, fill=False, density = True, stacked=True, linewidth=1, log = True, alpha = 0.01)
-            plt.hist(np.mean(self.image_all, axis=1),100, color = 'r', linewidth=1, log = True, alpha = 1, label = 'Camera average')
+                plt.hist(
+                    self.image_all[:, i],
+                    100,
+                    fill=False,
+                    density=True,
+                    stacked=True,
+                    linewidth=1,
+                    log=True,
+                    alpha=0.01,
+                )
+            plt.hist(
+                np.mean(self.image_all, axis=1),
+                100,
+                color="r",
+                linewidth=1,
+                log=True,
+                alpha=1,
+                label="Camera average",
+            )
             plt.legend()
             plt.xlabel("Charge (DC)")
-            plt.title("Charge spectrum %s gain (ALL)" %gain_c)
-                
-            full_name = name + '_Charge_Spectrum_%sGain_All.png' %gain_c 
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-SPECTRUM-ALL-%s-GAIN" %gain_c] = fig9
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-SPECTRUM-ALL-%s-GAIN" %gain_c] = FullPath
-    
+            plt.title("Charge spectrum %s gain (ALL)" % gain_c)
+
+            full_name = name + "_Charge_Spectrum_%sGain_All.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-SPECTRUM-ALL-%s-GAIN" % gain_c
+            ] = fig9
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-SPECTRUM-ALL-%s-GAIN" % gain_c
+            ] = FullPath
+
             plt.close()
 
         if self.counter_ped > 0:
             fig10, disp = plt.subplots()
             for i in range(self.Chan):
-                plt.hist(self.image_ped[:,i],100, fill=False, density = True, stacked=True, linewidth=1, log = True, alpha = 0.01)
-            plt.hist(np.mean(self.image_ped, axis=1),100, color = 'r', linewidth=1, log = True, alpha = 1, label = 'Camera average')
+                plt.hist(
+                    self.image_ped[:, i],
+                    100,
+                    fill=False,
+                    density=True,
+                    stacked=True,
+                    linewidth=1,
+                    log=True,
+                    alpha=0.01,
+                )
+            plt.hist(
+                np.mean(self.image_ped, axis=1),
+                100,
+                color="r",
+                linewidth=1,
+                log=True,
+                alpha=1,
+                label="Camera average",
+            )
             plt.legend()
             plt.xlabel("Charge (DC)")
-            plt.title("Charge spectrum %s gain (PED)" %gain_c)
-                
-            full_name = name + '_Charge_Spectrum_%sGain_Ped.png' %gain_c  
-            FullPath = FigPath +full_name
-            self.ChargeInt_Figures_Dict["CHARGE-INTEGRATION-SPECTRUM-PED-%s-GAIN" %gain_c] = fig10
-            self.ChargeInt_Figures_Names_Dict["CHARGE-INTEGRATION-SPECTRUM-PED-%s-GAIN" %gain_c] = FullPath
-
-            plt.close()
-
-
-        return  self.ChargeInt_Figures_Dict, self.ChargeInt_Figures_Names_Dict
+            plt.title("Charge spectrum %s gain (PED)" % gain_c)
 
+            full_name = name + "_Charge_Spectrum_%sGain_Ped.png" % gain_c
+            FullPath = FigPath + full_name
+            self.ChargeInt_Figures_Dict[
+                "CHARGE-INTEGRATION-SPECTRUM-PED-%s-GAIN" % gain_c
+            ] = fig10
+            self.ChargeInt_Figures_Names_Dict[
+                "CHARGE-INTEGRATION-SPECTRUM-PED-%s-GAIN" % gain_c
+            ] = FullPath
 
+            plt.close()
 
+        return self.ChargeInt_Figures_Dict, self.ChargeInt_Figures_Names_Dict
```

### Comparing `nectarchain-0.1.3/src/nectarchain/dqm/mean_waveforms.py` & `nectarchain-0.1.4/src/nectarchain/dqm/mean_waveforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,188 @@
-
-from dqm_summary_processor import *
+from dqm_summary_processor import dqm_summary
+from matplotlib import pyplot as plt
+import numpy as np
 
 
 class MeanWaveForms_HighLowGain(dqm_summary):
-
     def __init__(self, gaink):
-
         self.k = gaink
         return None
 
-    def ConfigureForRun(self,path, Chan, Samp, Reader1):
-        #define number of channels and samples
+    def ConfigureForRun(self, path, Chan, Samp, Reader1):
+        # define number of channels and samples
         self.Chan = Chan
-        self.Samp= Samp
+        self.Samp = Samp
 
-        #redefine everything
-        self.Mwf = np.zeros((self.Chan,self.Samp))
-        self.Mwf_ped = np.zeros((self.Chan,self.Samp))
+        # redefine everything
+        self.Mwf = np.zeros((self.Chan, self.Samp))
+        self.Mwf_ped = np.zeros((self.Chan, self.Samp))
         self.counter_evt = 0
         self.counter_ped = 0
 
-        self.Mwf_average = np.zeros((self.Chan,self.Samp))
-        self.Mwf_ped_average = np.zeros((self.Chan,self.Samp))
+        self.Mwf_average = np.zeros((self.Chan, self.Samp))
+        self.Mwf_ped_average = np.zeros((self.Chan, self.Samp))
         self.Mwf_Mean_overChan = []
         self.Mwf_ped_Mean_overChan = []
 
-
-        self.wf_list_plot = list(range(1, self.Samp+1))#used for plotting later on
-
-        
+        self.wf_list_plot = list(range(1, self.Samp + 1))  # used for plotting later on
 
         return None
 
 
-    def ProcessEvent(self, evt):
+    def ProcessEvent(self, evt, noped):
         if evt.trigger.event_type.value == 32: #count peds 
             self.counter_ped += 1
         else:
             self.counter_evt += 1
-            
-        for ichan in range(self.Chan): #loop over channels # 1855 should be redefined as a variable
-            if evt.trigger.event_type.value == 32: #only peds now
-                self.Mwf_ped[ichan,:] += evt.r0.tel[0].waveform[self.k][ichan] # fill channels one by one and sum them for peds only
+
+        for ichan in range(self.Chan):
+            # loop over channels, 1855 should be redefined as a variable
+            if evt.trigger.event_type.value == 32:  # only peds now
+                self.Mwf_ped[ichan, :] += evt.r0.tel[0].waveform[self.k][
+                    ichan
+                ]  # fill channels one by one and sum them for peds only
             else:
-                self.Mwf[ichan,:] += evt.r0.tel[0].waveform[self.k][ichan] # fill channels one by one and sum them
+                self.Mwf[ichan, :] += evt.r0.tel[0].waveform[self.k][
+                    ichan
+                ]  # fill channels one by one and sum them
         return None
 
-
     def FinishRun(self):
-        if (self.k==0):
-            gain_c = 'High'
-        if (self.k ==1):
-            gain_c = 'Low'
+        # if (self.k == 0):
+        #   gain_c = 'High'
+        # if (self.k == 1):
+        #    gain_c = 'Low'
+
+        self.Mwf_average = self.Mwf / self.counter_evt  # get average
+        # get average over channels
+        self.Mwf_Mean_overChan = np.mean(self.Mwf_average, axis=0)
 
-
-        self.Mwf_average = self.Mwf/self.counter_evt #get average
-        #get average over channels 
-        self.Mwf_Mean_overChan = np.mean(self.Mwf_average,axis=0)
-        
         if self.counter_ped > 0:
-            self.Mwf_ped_average = self.Mwf_ped/self.counter_ped #get average pedestals
-            self.Mwf_ped_Mean_overChan = np.mean(self.Mwf_ped_average,axis=0)
+            # get average pedestals
+            self.Mwf_ped_average = self.Mwf_ped / self.counter_ped
+            self.Mwf_ped_Mean_overChan = np.mean(self.Mwf_ped_average, axis=0)
 
         return None
 
-
     def GetResults(self):
-
-        #INITIATE DICT
+        # INITIATE DICT
         self.MeanWaveForms_Results_Dict = {}
 
         #ASSIGN RESUTLS TO DICT
         if (self.k==0):
-            self.MeanWaveForms_Results_Dict["WF-PHY-AVERAGE-HIGH-GAIN"]  = self.Mwf_average
+            #self.MeanWaveForms_Results_Dict["WF-PHY-AVERAGE-HIGH-GAIN"]  = self.Mwf_average
             self.MeanWaveForms_Results_Dict["WF-PHY-AVERAGE-CHAN-HIGH-GAIN"]  = self.Mwf_Mean_overChan
             if self.counter_ped > 0:
-                self.MeanWaveForms_Results_Dict["WF-PED-AVERAGE-HIGH-GAIN"] = self.Mwf_ped_average
+                #self.MeanWaveForms_Results_Dict["WF-PED-AVERAGE-HIGH-GAIN"] = self.Mwf_ped_average
                 self.MeanWaveForms_Results_Dict["WF-AVERAGE-PED-CHAN-HIGH-GAIN"]  = self.Mwf_ped_Mean_overChan
 
 
 
         if (self.k ==1):
-            self.MeanWaveForms_Results_Dict["WF-AVERAGE-LOW-GAIN"]  = self.Mwf_average
+            #self.MeanWaveForms_Results_Dict["WF-AVERAGE-LOW-GAIN"]  = self.Mwf_average
             self.MeanWaveForms_Results_Dict["WF-AVERAGE-CHAN-LOW-GAIN"]  = self.Mwf_Mean_overChan
             if self.counter_ped > 0:
-                self.MeanWaveForms_Results_Dict["WF-PHY-PED-AVERAGE-LOW-GAIN"] = self.Mwf_ped_average
+                #self.MeanWaveForms_Results_Dict["WF-PHY-PED-AVERAGE-LOW-GAIN"] = self.Mwf_ped_average
                 self.MeanWaveForms_Results_Dict["WF-PHY-AVERAGE-PED-CHAN-LOW-GAIN"]  = self.Mwf_ped_Mean_overChan
                 
 
 
         return self.MeanWaveForms_Results_Dict
 
-
-    def PlotResults(self,name,FigPath):
+    def PlotResults(self, name, FigPath):
         self.MeanWaveForms_Figures_Dict = {}
         self.MeanWaveForms_Figures_Names_Dict = {}
 
         wf_list = np.array(self.wf_list_plot)
 
         counter_fig = 0
-        colors = ['blue', 'red']
-        colors2 = ['cyan', 'orange']
-        titles = ['Physical', 'Pedestals']
-
-        Mean_plot_array = [self.Mwf_Mean_overChan, self.Mwf_ped_Mean_overChan]
-
-        #Set characters of gain: high or lo
-        if (self.k==0):
-            gain_c = 'High'
-        if (self.k ==1):
-            gain_c = 'Low'
+        colors = ["blue", "red"]
+        # colors2 = ['cyan', 'orange']
+        titles = ["Physical", "Pedestals"]
+
+        # Mean_plot_array = [self.Mwf_Mean_overChan, self.Mwf_ped_Mean_overChan]
+
+        # Set characters of gain: high or lo
+        if self.k == 0:
+            gain_c = "High"
+        if self.k == 1:
+            gain_c = "Low"
 
         full_fig, full_ax = plt.subplots()
         if self.counter_ped > 0:
             array_plot = [self.Mwf_average, self.Mwf_ped_average]
-        else: 
+        else:
             array_plot = [self.Mwf_average]
 
-            
         for x in array_plot:
-
             part_fig, part_ax = plt.subplots()
 
             for ichan in range(self.Chan):
-                full_ax.plot(wf_list ,x[ichan,:], color = colors[counter_fig], alpha = 0.005, linewidth=1)
-                part_ax.plot(wf_list ,x[ichan,:], color = colors[counter_fig], alpha = 0.005, linewidth=1)
-
-            Mean_plot = Mean_plot_array[counter_fig]
-
-            full_ax_return = full_ax.plot(wf_list, Mean_plot, color = colors2[counter_fig], alpha = 1, linewidth=3, label = 'Mean ' + titles[counter_fig])
-            part_ax_return = part_ax.plot(wf_list, Mean_plot, color = colors2[counter_fig], alpha = 1, linewidth=3, label = 'Mean ' + titles[counter_fig])
-            part_ax.set_title('Mean Waveforms %s (%s Gain)' %(titles[counter_fig], gain_c))
-            part_ax.set_xlabel('Samples')
-            part_ax.set_ylabel('Amplitude (DC)')
+                full_ax.plot(
+                    wf_list,
+                    x[ichan, :],
+                    color=colors[counter_fig],
+                    alpha=0.005,
+                    linewidth=1,
+                )
+                part_ax.plot(
+                    wf_list,
+                    x[ichan, :],
+                    color=colors[counter_fig],
+                    alpha=0.005,
+                    linewidth=1,
+                )
+
+            # Mean_plot = Mean_plot_array[counter_fig]
+
+            # full_ax_return = full_ax.plot(wf_list, Mean_plot,
+            #                              color=colors2[counter_fig], alpha=1,
+            #                              linewidth=3,
+            #                              label='Mean ' + titles[counter_fig])
+            # part_ax_return = part_ax.plot(wf_list, Mean_plot,
+            #                              color=colors2[counter_fig], alpha=1,
+            #                              linewidth=3,
+            #                              label='Mean ' + titles[counter_fig])
+            part_ax.set_title(
+                "Mean Waveforms %s (%s Gain)" % (titles[counter_fig], gain_c)
+            )
+            part_ax.set_xlabel("Samples")
+            part_ax.set_ylabel("Amplitude (DC)")
             part_ax.legend()
             part_ax.grid()
 
-            part_name = name + '_MeanWaveforms_%s_%sGain.png' %(titles[counter_fig], gain_c)
+            part_name = name + "_MeanWaveforms_%s_%sGain.png" % (
+                titles[counter_fig],
+                gain_c,
+            )
             PartPath = FigPath + part_name
-            
-            self.MeanWaveForms_Figures_Dict["FIGURE-WF-%s-%s-GAIN" %(titles[counter_fig], gain_c)]= part_fig
-            self.MeanWaveForms_Figures_Names_Dict["FIGURE-WF-%s-%s-GAIN" %(titles[counter_fig], gain_c)]= PartPath
+
+            self.MeanWaveForms_Figures_Dict[
+                "FIGURE-WF-%s-%s-GAIN" % (titles[counter_fig], gain_c)
+            ] = part_fig
+            self.MeanWaveForms_Figures_Names_Dict[
+                "FIGURE-WF-%s-%s-GAIN" % (titles[counter_fig], gain_c)
+            ] = PartPath
 
             plt.close()
 
+            counter_fig += 1
 
-            counter_fig +=1
-        
-        full_ax.set_title('Mean Waveforms Combined Plot (%s Gain)' % gain_c)
-        full_ax.set_xlabel('Samples')
-        full_ax.set_ylabel('Amplitude (DC)')
+        full_ax.set_title("Mean Waveforms Combined Plot (%s Gain)" % gain_c)
+        full_ax.set_xlabel("Samples")
+        full_ax.set_ylabel("Amplitude (DC)")
         full_ax.legend()
         full_ax.grid()
 
-        full_name = name + '_MeanWaveforms_CombinedPlot_%sGain.png' %gain_c
-        FullPath = FigPath +full_name
-        self.MeanWaveForms_Figures_Dict["FIGURE-WF-COMBINED-%s-GAIN" % gain_c] = full_fig
-        self.MeanWaveForms_Figures_Names_Dict["FIGURE-WF-COMBINED-%s-GAIN" % gain_c]= FullPath
+        full_name = name + "_MeanWaveforms_CombinedPlot_%sGain.png" % gain_c
+        FullPath = FigPath + full_name
+        self.MeanWaveForms_Figures_Dict[
+            "FIGURE-WF-COMBINED-%s-GAIN" % gain_c
+        ] = full_fig
+        self.MeanWaveForms_Figures_Names_Dict[
+            "FIGURE-WF-COMBINED-%s-GAIN" % gain_c
+        ] = FullPath
 
         plt.close()
 
-
-        return  self.MeanWaveForms_Figures_Dict, self.MeanWaveForms_Figures_Names_Dict
-
-
-
-
-
+        return self.MeanWaveForms_Figures_Dict, self.MeanWaveForms_Figures_Names_Dict
```

### Comparing `nectarchain-0.1.3/src/nectarchain/dqm/start_calib.py` & `nectarchain-0.1.4/src/nectarchain/dqm/start_calib.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,123 @@
 import os
 import sys
 
 from matplotlib import pyplot as plt
-
+import argparse
 #from multiprocessing import Process
-
 import time
 
 from ctapipe.io import EventSource, EventSeeker
-
+from ctapipe_io_nectarcam.constants import LOW_GAIN, HIGH_GAIN
 
 from mean_waveforms import MeanWaveForms_HighLowGain
 from mean_camera_display import MeanCameraDisplay_HighLowGain
 from charge_integration import ChargeIntegration_HighLowGain
 from trigger_statistics import TriggerStatistics
 from camera_monitoring import CameraMonitoring
 
 
-print(sys.argv)
-path = sys.argv[1] # path of the Run file: ./NectarCAM.Run2720.0000.fits.fz
 
-NectarPath = str(os.environ['NECTARDIR'])
+# Create an ArgumentParser object
+parser = argparse.ArgumentParser(description='NectarCAM Data Quality Monitoring tool')
+parser.add_argument('-p', '--plot',
+                     action='store_true',
+                     help='Enables plots to be generated')
+parser.add_argument('-n', '--noped',
+                     action='store_true',
+                     help='Enables pedestal subtraction in charge integration')
+parser.add_argument('-r', '--runnb',
+                    help='Optional run number, automatically found on DIRAC',
+                    type=int)
+parser.add_argument('-i', '--input-files',
+                    nargs='+',
+                    help='Local input files')
+
+parser.add_argument('input_paths', help='Input paths')
+parser.add_argument('output_paths', help='Output paths')
+
+args, leftovers = parser.parse_known_args()
+
+# Reading arguments, paths and plot-boolean
+NectarPath = args.input_paths  # str(os.environ['NECTARDIR'])
+print("Input file path:", NectarPath)
+
+# Defining and printing the paths of the output files.
+output_path = args.output_paths
+print("Output path:", output_path)
+
+
+# Defining and printing the paths of the input files.
+
+if args.runnb is not None:
+    # Grab runs automatically from DIRAC is the -r option is provided
+    from nectarchain.calibration.container import utils
+    dm = utils.DataManagement()
+    _, filelist = dm.findrun(args.runnb)
+    args.input_files = [s.name for s in filelist]
+elif args.input_files is None:
+    print('Input files should be provided, exiting...')
+    sys.exit(1)
+
+# OTHERWISE READ THE RUNS FROM ARGS
+path1 = args.input_files[0]
+
+#THE PATH OF INPUT FILES
+path = f'{NectarPath}/{path1}'
+print("Input files:")
+print(path)
+for arg in args.input_files[1:]:
+    print(arg)
+
+#Defining and priting the options
+PlotFig = args.plot
+noped = args.noped
+
+print("Plot:", PlotFig)
+print("Noped:", noped)
+
+
+
 
 def GetName(RunFile):
-    name = RunFile.split('/')[-1]
-    name = name.split('.')[0] + '_' + name.split('.')[1]# + '_' +name.split('.')[2]
+    name = RunFile.split("/")[-1]
+    name = name.split(".")[0] + "_" + name.split(".")[1]  # + '_' +name.split('.')[2]
     print(name)
     return name
 
 def CreateFigFolder(name, type):
-    if(type == 0):
-        folder = 'Plots'
+    if type == 0:
+        folder = "Plots"
 
     ParentFolderName = name.split('_')[0] + '_' + name.split('_')[1]
     ChildrenFolderName = './' + ParentFolderName +'/' + name + '_calib'
-    FolderPath = NectarPath + 'output/%s/%s/' %(ChildrenFolderName, folder)
+    FolderPath = f'{output_path}/output/{ChildrenFolderName}/{folder}'
 
     if not os.path.exists(FolderPath):
         os.makedirs(FolderPath)
 
     return ParentFolderName, ChildrenFolderName, FolderPath
 
 
 start = time.time()
 
-#INITIATE
-#######################################################################################################################
+# INITIATE
 path = path
+print(path)
 cmap = 'gnuplot2'
 
-#Read and seek
-reader=EventSource(input_url=path)
+# Read and seek
+reader = EventSource(input_url=path)
 seeker = EventSeeker(reader)
 reader1 = EventSource(input_url=path, max_events=1)
-#print(reader.file_list)
+# print(reader.file_list)
 
 name = GetName(path)
 ParentFolderName, ChildrenFolderName, FigPath = CreateFigFolder(name, 0)
-ResPath = NectarPath + 'output/%s/%s' %(ChildrenFolderName, name)
+ResPath = f'{output_path}/output/{ChildrenFolderName}/{name}'
 #######################################################################################################################
 
 
 
 
                                                   ########################
 
@@ -69,117 +125,109 @@
 
 
 
 
 
 #LIST OF PROCESSES TO RUN
 #######################################################################################################################
-a = TriggerStatistics(0)
-b = MeanWaveForms_HighLowGain(0) #0 is for high gain and 1 is for low gain
-c = MeanWaveForms_HighLowGain(1)
-d = MeanCameraDisplay_HighLowGain(0)
-e = MeanCameraDisplay_HighLowGain(1)
-f = ChargeIntegration_HighLowGain(0)
-g = ChargeIntegration_HighLowGain(1)
-h = CameraMonitoring(0)
+a = TriggerStatistics(HIGH_GAIN)
+b = MeanWaveForms_HighLowGain(HIGH_GAIN) #0 is for high gain and 1 is for low gain
+c = MeanWaveForms_HighLowGain(LOW_GAIN)
+d = MeanCameraDisplay_HighLowGain(HIGH_GAIN)
+e = MeanCameraDisplay_HighLowGain(LOW_GAIN)
+f = ChargeIntegration_HighLowGain(HIGH_GAIN)
+g = ChargeIntegration_HighLowGain(LOW_GAIN)
+h = CameraMonitoring(HIGH_GAIN)
 
 processors = list()
 
 processors.append(a)
 processors.append(b)
 processors.append(c)
 processors.append(d)
 processors.append(e)
 processors.append(f)
 processors.append(g)
 processors.append(h)
-#######################################################################################################################
-
 
 
-
-
-                                                 ########################
-
-
-
-
-#LIST OF DICT RESULTS
-#######################################################################################################################
-Results_MeanWaveForms_HighGain ={}
+# LIST OF DICT RESULTS
+Results_MeanWaveForms_HighGain = {}
 Results_MeanWaveForms_LowGain = {}
 Results_MeanCameraDisplay_HighGain = {}
 Results_MeanCameraDisplay_LowGain = {}
 Results_ChargeIntegration_HighGain = {}
 Results_ChargeIntegration_LowGain = {}
 Results_TriggerStatistics = {}
 Results_CameraMonitoring = {}
 
-NESTED_DICT = {} #The final results dictionary
-NESTED_DICT_KEYS = ["Results_TriggerStatistics", "Results_MeanWaveForms_HighGain", "Results_MeanWaveForms_LowGain", "Results_MeanCameraDisplay_HighGain", "Results_MeanCameraDisplay_LowGain", "Results_ChargeIntegration_HighGain", "Results_ChargeIntegration_LowGain", "Results_CameraMonitoring"]
-#NESTED_DICT_KEYS = ["Results_CameraMonitoring"]
-
-
-#######################################################################################################################
-
-
-
-
-                                                  ########################
-
-
+NESTED_DICT = {}  # The final results dictionary
+NESTED_DICT_KEYS = [
+    "Results_TriggerStatistics",
+    "Results_MeanWaveForms_HighGain",
+    "Results_MeanWaveForms_LowGain",
+    "Results_MeanCameraDisplay_HighGain",
+    "Results_MeanCameraDisplay_LowGain",
+    "Results_ChargeIntegration_HighGain",
+    "Results_ChargeIntegration_LowGain",
+    "Results_CameraMonitoring",
+]
+# NESTED_DICT_KEYS = ["Results_CameraMonitoring"]
 
-#START
-#######################################################################################################################
+# START
 for p in processors:
     Chan, Samp = p.DefineForRun(reader1)
     break
-    
-for p in processors:  
+
+for p in processors:
     p.ConfigureForRun(path, Chan, Samp, reader1)
 
 for i, evt in enumerate(reader):
-	for p in processors:
-		p.ProcessEvent(evt)
+    for p in processors:
+        p.ProcessEvent(evt, noped)
+        
+#for the rest of the event files
+for arg in args.input_files[1:]:
+    path2 = f'{NectarPath}/{arg}'
+    print(path2)
 
-for arg in sys.argv[2:]:
-    reader=EventSource(input_url=arg)
+    reader=EventSource(input_url=path2)
     seeker = EventSeeker(reader)
 
     for i, evt in enumerate(reader):
         for p in processors:
-            p.ProcessEvent(evt)
+            p.ProcessEvent(evt, noped)
 
 for p in processors:
     p.FinishRun()
 
 dict_num = 0
 for p in processors:
-    NESTED_DICT[NESTED_DICT_KEYS[dict_num]] = p.GetResults() #True if want to compute plots, sedond true if want to save results
+    NESTED_DICT[NESTED_DICT_KEYS[dict_num]] = p.GetResults()
     dict_num += 1
 
 
 name = name #in order to allow to change the name easily
-p.WriteAllResults(ResPath, NESTED_DICT) #if we want to write all results in 1 pickle file we do this. 
-
-for p in processors:
-    processor_figure_dict, processor_figure_name_dict  = p.PlotResults(name, FigPath)
+p.WriteAllResults(ResPath, NESTED_DICT) #if we want to write all results in 1 fits file we do this. 
 
-    for fig_plot in processor_figure_dict:
-        fig = processor_figure_dict[fig_plot]
-        SavePath = processor_figure_name_dict[fig_plot]
-        plt.gcf()
-        fig.savefig(SavePath)
-        
-plt.clf()
-plt.cla()
-plt.close()
+#if -plot in args it will construct the figures and save them
+if PlotFig:
+    for p in processors:
+        processor_figure_dict, processor_figure_name_dict  = p.PlotResults(name, FigPath)
+    
+        for fig_plot in processor_figure_dict:
+            fig = processor_figure_dict[fig_plot]
+            SavePath = processor_figure_name_dict[fig_plot]
+            plt.gcf()
+            fig.savefig(SavePath)
+            
+    plt.clf()
+    plt.cla()
+    plt.close()
 
 
 end = time.time()
-print("Processing time:", end-start)
-
-#TODOS
-#######################################################################################################################
-#Reduce code by using loops: for figs and results
-#MONGO: store results 
+print("Processing time:", end - start)
 
+# TODOS
+# Reduce code by using loops: for figs and results
+# MONGO: store results
```

### Comparing `nectarchain-0.1.3/src/nectarchain/dqm/trigger_statistics.py` & `nectarchain-0.1.4/src/nectarchain/dqm/trigger_statistics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,246 @@
-
-from dqm_summary_processor import *
 import math
+from matplotlib import pyplot as plt
+import numpy as np
+from astropy import time as astropytime
+from dqm_summary_processor import dqm_summary
 
-class TriggerStatistics(dqm_summary):
 
+class TriggerStatistics(dqm_summary):
     def __init__(self, gaink):
-
         self.k = gaink
         return None
 
-    def ConfigureForRun(self,path, Chan, Samp, Reader1):
-        #define number of channels and samples
+    def ConfigureForRun(self, path, Chan, Samp, Reader1):
+        # define number of channels and samples
         self.Chan = Chan
-        self.Samp= Samp
-        
+        self.Samp = Samp
+
         self.event_type = []
         self.event_times = []
         self.event_id = []
         self.run_times = []
 
-    def ProcessEvent(self, evt):
+    def ProcessEvent(self, evt, noped):
         trigger_type = evt.trigger.event_type.value
         trigger_time = evt.trigger.time.value
         trigger_id = evt.index.event_id
         trigger_run_time = evt.nectarcam.tel[0].svc.date
 
-
         self.event_type.append(trigger_type)
         self.event_times.append(trigger_time)
         self.event_id.append(trigger_id)
         self.run_times.append(trigger_run_time)
 
-
     def FinishRun(self):
         self.triggers = np.unique(self.event_type)
         pedestal_num = 32
         physical_num = 2
 
         self.event_id = np.array(self.event_id)
         self.run_times = np.array(self.run_times)
         self.event_times = np.array(self.event_times)
         self.event_type = np.array(self.event_type)
 
         self.run_start1 = self.run_times[self.event_id == np.min(self.event_id)]
 
-        #Choose between the following two methods. time for max id can be sometimes 0.
-        #self.run_end = self.event_times[self.event_id == np.max(self.event_id)]
+        # Choose between the following two methods. time for max id can be sometimes 0.
+        # self.run_end = self.event_times[self.event_id == np.max(self.event_id)]
         self.run_start = self.event_times[self.event_id == np.min(self.event_id)]
-        #self.run_start = np.min(self.event_times)
+        # self.run_start = np.min(self.event_times)
         self.run_end = np.max(self.event_times)
 
         self.event_ped_times = self.event_times[self.event_type == pedestal_num]
         self.event_phy_times = self.event_times[self.event_type == physical_num]
-        mask = ((self.event_type != physical_num) & (self.event_type != pedestal_num))
+        mask = (self.event_type != physical_num) & (self.event_type != pedestal_num)
         self.event_other_times = self.event_times[mask]
 
         self.event_ped_id = self.event_id[self.event_type == pedestal_num]
         self.event_phy_id = self.event_id[self.event_type == physical_num]
-        mask = ((self.event_type != physical_num) & (self.event_type != pedestal_num))
+        mask = (self.event_type != physical_num) & (self.event_type != pedestal_num)
         self.event_other_id = self.event_id[mask]
 
-        self.event_ped_times = self.event_ped_times[self.event_ped_times > self.run_start]
-        self.event_phy_times = self.event_phy_times[self.event_phy_times > self.run_start]
-        self.event_other_times = self.event_other_times[self.event_other_times > self.run_start]
+        self.event_ped_times = self.event_ped_times[
+            self.event_ped_times > self.run_start
+        ]
+        self.event_phy_times = self.event_phy_times[
+            self.event_phy_times > self.run_start
+        ]
+        self.event_other_times = self.event_other_times[
+            self.event_other_times > self.run_start
+        ]
         self.event_wrong_times = self.event_times[self.event_times < self.run_start]
         self.event_times = self.event_times[self.event_times > self.run_start]
 
-
-    
     def GetResults(self):
         self.TriggerStat_Results_Dict = {}
         self.TriggerStat_Results_Dict["TRIGGER-TYPES"] = self.triggers
-        self.TriggerStat_Results_Dict["TRIGGER-STATISTICS"] = "All: %s, Physical: %s, Pedestals: %s, Others: %s, Wrong times: %s" %(len(self.event_times), len(self.event_phy_times), len(self.event_ped_times), len(self.event_other_times), len(self.event_wrong_times))
-        self.TriggerStat_Results_Dict["START-TIMES"] = "Run start time: %s, First event: %s, Last event: %s" %(self.run_start1, self.run_start, self.run_end)
+        self.TriggerStat_Results_Dict[
+            "TRIGGER-STATISTICS"
+        ] = "All: %s, Physical: %s, Pedestals: %s, Others: %s, Wrong times: %s" % (
+            len(self.event_times),
+            len(self.event_phy_times),
+            len(self.event_ped_times),
+            len(self.event_other_times),
+            len(self.event_wrong_times),
+        )
+        self.TriggerStat_Results_Dict[
+            "START-TIMES"
+        ] = "Run start time: %s, First event: %s, Last event: %s" % (
+            self.run_start1,
+            self.run_start,
+            self.run_end,
+        )
         return self.TriggerStat_Results_Dict
 
-
-    def PlotResults(self,name,FigPath):
-
+    def PlotResults(self, name, FigPath):
         w = 1
-        n1 = np.array(self.event_times.max() - self.event_times.min(), dtype= object)
-        n = math.ceil(n1/w)
+        n1 = np.array(self.event_times.max() - self.event_times.min(), dtype=object)
+        n = math.ceil(n1 / w)
 
         self.TriggerStat_Figures_Dict = {}
         self.TriggerStat_Figures_Names_Dict = {}
         fig1, ax = plt.subplots()
-        ax.hist(self.event_type, 100, color = 'r', linewidth=1, log = True, alpha = 1, label = 'Trigger types')
+        ax.hist(
+            self.event_type,
+            100,
+            color="r",
+            linewidth=1,
+            log=True,
+            alpha=1,
+            label="Trigger types",
+        )
         for rect in ax.patches:
             height = rect.get_height()
-            ax.annotate(f'{int(height)}', xy=(rect.get_x()+rect.get_width()/2, height), xytext=(0, 5), textcoords='offset points', ha='center', va='bottom') 
+            ax.annotate(
+                f"{int(height)}",
+                xy=(rect.get_x() + rect.get_width() / 2, height),
+                xytext=(0, 5),
+                textcoords="offset points",
+                ha="center",
+                va="bottom",
+            )
         plt.xticks(self.triggers)
         plt.title("Trigger Statistics")
         plt.xlabel("Trigger type")
         plt.grid()
-        full_name = name + '_Trigger_Statistics.png'  
-        FullPath = FigPath +full_name
+        full_name = name + "_Trigger_Statistics.png"
+        FullPath = FigPath + full_name
 
         self.TriggerStat_Figures_Dict["TRIGGER-STATISTICS"] = fig1
         self.TriggerStat_Figures_Names_Dict["TRIGGER-STATISTICS"] = FullPath
         plt.close()
 
         w = 15
         n1 = self.event_times.max() - self.event_times.min()
-        n = math.ceil(n1/w)
-
+        n = math.ceil(n1 / w)
 
         fig2, ax = plt.subplots()
-        ax.hist(self.event_times - self.run_start, n, color = 'grey', linewidth=1, log = True, alpha = 0.5, label = 'All events (%s + %s invisible)' %(len(self.event_times), len(self.event_wrong_times)))
-        ax.hist(self.event_phy_times - self.run_start, n, color = 'cyan', linewidth=1, log = True, alpha = 0.5, label = 'Physical events (%s)' %len(self.event_phy_times))
-        ax.hist(self.event_ped_times - self.run_start, n, color = 'orange', linewidth=1, log = True, alpha = 0.5, label = 'Pedestal events (%s)' %len(self.event_ped_times))
-        ax.hist(self.event_other_times - self.run_start, n, color = 'brown', linewidth=1, log = True, alpha = 0.5, label = 'Other events (%s)' %len(self.event_other_times))
+        ax.hist(
+            self.event_times - self.run_start,
+            n,
+            color="grey",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="All events (%s + %s invisible)"
+            % (len(self.event_times), len(self.event_wrong_times)),
+        )
+        ax.hist(
+            self.event_phy_times - self.run_start,
+            n,
+            color="cyan",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="Physical events (%s)" % len(self.event_phy_times),
+        )
+        ax.hist(
+            self.event_ped_times - self.run_start,
+            n,
+            color="orange",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="Pedestal events (%s)" % len(self.event_ped_times),
+        )
+        ax.hist(
+            self.event_other_times - self.run_start,
+            n,
+            color="brown",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="Other events (%s)" % len(self.event_other_times),
+        )
         plt.legend()
         plt.xlabel("Time")
         plt.grid()
-        plt.title("Trigger rates, run start at %s" %astropytime.Time(self.run_start, format='unix').iso)
-        full_name = name + '_Event_rate.png'  
-        FullPath = FigPath +full_name
+        plt.title(
+            "Trigger rates, run start at %s"
+            % astropytime.Time(self.run_start, format="unix").iso
+        )
+        full_name = name + "_Event_rate.png"
+        FullPath = FigPath + full_name
 
         self.TriggerStat_Figures_Dict["EVENT-TIME"] = fig2
         self.TriggerStat_Figures_Names_Dict["EVENT-TIME"] = FullPath
         plt.close()
 
         fig3, ax = plt.subplots()
-        ax.hist(self.event_id, n, color = 'grey', linewidth=1, log = True, alpha = 0.5, label = 'All events (%s)' %len(self.event_id))
-        ax.hist(self.event_phy_id, n, color = 'orange', linewidth=1, log = True, alpha = 0.5, label = 'Physical events (%s)' %len(self.event_phy_id))
-        ax.hist(self.event_ped_id, n, color = 'cyan', linewidth=1, log = True, alpha = 0.5, label = 'Pedestal events (%s)' %len(self.event_ped_id))
-        ax.hist(self.event_other_id, n, color = 'brown', linewidth=1, log = True, alpha = 0.5, label = 'Other events (%s)' %len(self.event_other_id))
+        ax.hist(
+            self.event_id,
+            n,
+            color="grey",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="All events (%s)" % len(self.event_id),
+        )
+        ax.hist(
+            self.event_phy_id,
+            n,
+            color="orange",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="Physical events (%s)" % len(self.event_phy_id),
+        )
+        ax.hist(
+            self.event_ped_id,
+            n,
+            color="cyan",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="Pedestal events (%s)" % len(self.event_ped_id),
+        )
+        ax.hist(
+            self.event_other_id,
+            n,
+            color="brown",
+            linewidth=1,
+            log=True,
+            alpha=0.5,
+            label="Other events (%s)" % len(self.event_other_id),
+        )
         plt.legend()
         plt.xlabel("ID")
         plt.grid()
-        plt.title("Trigger IDs, run start at %s" %astropytime.Time(self.run_start, format='unix').iso)
-        full_name = name + '_Event_IDs.png'  
-        FullPath = FigPath +full_name
+        plt.title(
+            "Trigger IDs, run start at %s"
+            % astropytime.Time(self.run_start, format="unix").iso
+        )
+        full_name = name + "_Event_IDs.png"
+        FullPath = FigPath + full_name
 
         self.TriggerStat_Figures_Dict["EVENT-ID"] = fig3
         self.TriggerStat_Figures_Names_Dict["EVENT-ID"] = FullPath
         plt.close()
 
-        return  self.TriggerStat_Figures_Dict, self.TriggerStat_Figures_Names_Dict
+        return self.TriggerStat_Figures_Dict, self.TriggerStat_Figures_Names_Dict
 
-#TODO
-#continue GetResults
-#adjust histogram displays
-#Choose between starting since run star time or event start time ?
 
+# TODO
+# continue GetResults
+# adjust histogram displays
+# Choose between starting since run star time or event start time ?
```

### Comparing `nectarchain-0.1.3/src/nectarchain/tools/write_camera_calibration.py` & `nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/tools/write_camera_calibration_param.json` & `nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration_param.json`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/tools/write_pedestals.py` & `nectarchain-0.1.4/src/nectarchain/tools/write_pedestals.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/tools/write_pedestals_param.json` & `nectarchain-0.1.4/src/nectarchain/tools/write_pedestals_param.json`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pathlib import Path
 import sys
 import os
 import argparse
 import json
+import glob
 
 import logging
 logging.getLogger("numba").setLevel(logging.WARNING)
 logging.basicConfig(format='%(asctime)s %(name)s %(levelname)s %(message)s',level=logging.DEBUG,filename = f"{os.environ.get('NECTARCHAIN_LOG')}/{Path(__file__).stem}_{os.getpid()}.log")
 log = logging.getLogger(__name__)
 
-from nectarchain.calibration.container import WaveformsContainer,ChargeContainer
+from nectarchain.calibration.container import WaveformsContainer,WaveformsContainers,ChargeContainer,ChargeContainers
 
 parser = argparse.ArgumentParser(
                     prog = 'load_wfs_compute_charge',
                     description = 'This program load waveforms from fits.fz run files and compute charge')
 
 #run numbers
 parser.add_argument('-s', '--spe_run_number',
@@ -43,15 +44,15 @@
                     #default=[],
                     help='ped max events to be load',
                     type=int)
 parser.add_argument('--ff_max_events',
                     nargs="+",
                     #default=[],
                     help='FF max events to be load',
-                    type=list)
+                    type=int)
 
 #n_events in runs
 parser.add_argument('--spe_nevents',
                     nargs="+",
                     #default=[],
                     help='spe n events to be load',
                     type=int)
@@ -60,31 +61,42 @@
                     #default=[],
                     help='ped n events to be load',
                     type=int)
 parser.add_argument('--ff_nevents',
                     nargs="+",
                     #default=[],
                     help='FF n events to be load',
-                    type=list)
+                    type=int)
 
 #boolean arguments
 parser.add_argument('--reload_wfs',
                     action='store_true',
                     default=False,
                     help='to force re-computation of waveforms from fits.fz files'
                     )
 parser.add_argument('--overwrite',
                     action='store_true',
                     default=False,
                     help='to force overwrite files on disk'
                     )
 
+parser.add_argument('--split',
+                    action='store_true',
+                    default=False,
+                    help='split waveforms extraction with 1 file per fits.fz raw data file'
+                    )
+
 #extractor arguments
 parser.add_argument('--extractorMethod',
-                    choices=["FullWaveformSum","LocalPeakWindowSum"],
+                    choices=["FullWaveformSum",
+                             "FixedWindowSum",
+                             "GlobalPeakWindowSum",
+                             "LocalPeakWindowSum",
+                             "SlidingWindowMaxSum",
+                             "TwoPassWindowSum"],
                     default="LocalPeakWindowSum",
                     help='charge extractor method',
                     type=str
                     )
 parser.add_argument('--extractor_kwargs',
                     default={'window_width' : 16, 'window_shift' : 4},
                     help='charge extractor kwargs',
@@ -110,14 +122,107 @@
         e = Exception(f'{arg}_run_number and {arg}_max_events must have same length')
         log.error(e,exc_info=True)
         raise e
     if not(nevents is None) and len(nevents) != len(run_number) :
         e = Exception(f'{arg}_run_number and {arg}_nevents must have same length')
         log.error(e,exc_info=True)
         raise e
+    
+
+def load_wfs_no_split(i,runs_list,max_events,nevents,overwrite) : 
+    """method to load waveforms without splitting
+
+    Args:
+        i (int): index in the run list
+        runs_list (list): the run number list
+        max_events (list): max_events list
+        nevents (list): nevents list
+        overwrite (bool): to overwrite 
+
+    Returns:
+        WaveformsContainer: the output waveformsContainer
+    """
+    log.info("loading wfs not splitted")
+    wfs = WaveformsContainer(runs_list[i],max_events = max_events[i],nevents = nevents[i])
+    wfs.load_wfs()
+    wfs.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",overwrite = overwrite)
+    return wfs
+
+def load_wfs_charge_split(i,runs_list,max_events,overwrite,charge_childpath,extractor_kwargs) :
+    """_summary_
+
+    Args:
+        i (int): index in the run list
+        runs_list (list): the run number list
+        max_events (list): max_events list
+        nevents (list): nevents list
+        overwrite (bool): to overwrite 
+        charge_childpath (str): the extraction method
+        extractor_kwargs (dict): the charge extractor kwargs
+
+    Returns:
+        WaveformsContainers,ChargeContainers: the output WaveformsContainers and ChargeContainers
+    """
+     
+    log.info("splitting wafevorms extraction with raw data list files")
+    log.debug(f"creation of the WaveformsContainers")
+    wfs = WaveformsContainers(runs_list[i],max_events = max_events[i],init_arrays = False)
+    log.info(f"computation of charge with {charge_childpath}")
+    log.info("splitting charge computation with raw data list files")
+    charge = ChargeContainers()
+    for j in range(wfs.nWaveformsContainer) :
+        log.debug(f"reader events for file {j}")
+        wfs.load_wfs(index = j)
+        wfs.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",index = j, overwrite = overwrite)
+        log.debug(f"computation of charge for file {j}")
+        charge.append(ChargeContainer.from_waveforms(wfs.waveformsContainer[j],
+                                                     method = charge_childpath,
+                                                     **extractor_kwargs))
+        log.debug(f"deleting waveformsContainer at index {j} to free RAM")
+        wfs.waveformsContainer[j] = WaveformsContainer.__new__(WaveformsContainer)
+    
+    
+    log.info("merging charge")
+    charge = charge.merge()
+    return wfs,charge
+
+def load_wfs_charge_split_from_wfsFiles(wfsFiles,charge_childpath,extractor_kwargs) : 
+    """_summary_
+
+    Args:
+        wfsFiles (list): list of the waveformsContainer FITS files
+        charge_childpath (str): the extraction method
+        extractor_kwargs (dict): the charge extractor kwargs
+
+    Returns:
+        None,ChargeContainers: the output ChargeContainers (return tuple with None to keep same structure as load_wfs_charge_split)
+    """
+    charge = ChargeContainers()
+    for j,file in enumerate(wfsFiles):
+        log.debug(f"loading wfs from file {file}")
+        wfs = WaveformsContainer.load(file)
+        log.debug(f"computation of charge for file {file}")
+        charge.append(ChargeContainer.from_waveforms(wfs,
+                                                     method = charge_childpath,
+                                                     **extractor_kwargs))
+        log.debug(f"deleting waveformsContainer from {file} to free RAM")
+        del wfs.wfs_hg
+        del wfs.wfs_lg
+        del wfs.ucts_timestamp
+        del wfs.ucts_busy_counter
+        del wfs.ucts_event_counter
+        del wfs.event_type
+        del wfs.event_id
+        del wfs.trig_pattern_all
+        del wfs
+        #gc.collect()
+    
+    log.info("merging charge")
+    charge = charge.merge()
+    return None,charge
 
 def load_wfs_compute_charge(runs_list : list,
                             reload_wfs : bool = False,
                             overwrite : bool= False,
                             charge_extraction_method : str = "FullWaveformSum",
                             **kwargs) -> None :
     """this method is used to load waveforms from zfits files and compute charge with an user specified method
@@ -140,58 +245,73 @@
     
     
     max_events = kwargs.get("max_events",[None for i in range(len(runs_list))])
     nevents = kwargs.get("nevents",[-1 for i in range(len(runs_list))])
 
     charge_childpath = kwargs.get("charge_childpath",charge_extraction_method)
     extractor_kwargs = kwargs.get("extractor_kwargs",{})
+
+    split =  kwargs.get("split",False)
     
 
     for i in range(len(runs_list)) : 
         log.info(f"treating run {runs_list[i]}")
         log.info("waveform computation")
-        if not(reload_wfs) :
+        if not(reload_wfs):
             log.info(f"trying to load waveforms from {os.environ['NECTARCAMDATA']}/waveforms/")
             try : 
-                wfs = WaveformsContainer.load(f"{os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{runs_list[i]}.fits")
+                if split : 
+                    files = glob.glob(f"{os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{runs_list[i]}_*.fits")
+                    if len(files) ==  0 : 
+                        raise FileNotFoundError(f"no splitted waveforms found")
+                    else :
+                        wfs,charge = load_wfs_charge_split_from_wfsFiles(files,charge_childpath,extractor_kwargs)
+                        
+                else :
+                    wfs = WaveformsContainer.load(f"{os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{runs_list[i]}.fits")
             except FileNotFoundError as e : 
                 log.warning(f"argument said to not reload waveforms from zfits files but computed waveforms not found at {os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{runs_list[i]}.fits")
                 log.warning(f"reloading from zfits files")
-                wfs = WaveformsContainer(runs_list[i],max_events = max_events[i],nevents = nevents[i])
-                wfs.load_wfs()
-                wfs.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",overwrite = overwrite)
+                if split : 
+                    wfs,charge = load_wfs_charge_split(i,runs_list,max_events,overwrite,charge_childpath,extractor_kwargs)
+                else : 
+                    wfs = load_wfs_no_split(i,runs_list,max_events,nevents,overwrite)
             except Exception as e :
                 log.error(e,exc_info = True)
                 raise e
         else : 
-            wfs = WaveformsContainer(runs_list[i],max_events = max_events[i],nevents = nevents[i])
-            wfs.load_wfs()
-            wfs.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",overwrite = overwrite)
-
-        log.info(f"computation of charge with {charge_childpath}")
-        charge = ChargeContainer.from_waveforms(wfs,method = charge_childpath,**extractor_kwargs)
+            if split : 
+                wfs,charge = load_wfs_charge_split(i,runs_list,max_events,overwrite,charge_childpath,extractor_kwargs)
+            else : 
+                wfs = load_wfs_no_split(i,runs_list,max_events,nevents,overwrite)
+
+        
+        if not(split) :   
+            log.info(f"computation of charge with {charge_childpath}")
+            charge = ChargeContainer.from_waveforms(wfs,method = charge_childpath,**extractor_kwargs)
         del wfs
+
         charge.write(f"{os.environ['NECTARCAMDATA']}/charges/{path}/",overwrite = overwrite)
         del charge
     
 
 def main(spe_run_number : list = [],
         ff_run_number : list = [], 
         ped_run_number: list = [],
         **kwargs):
 
     #print(kwargs)
 
     spe_nevents = kwargs.pop('spe_nevents',[-1 for i in range(len(spe_run_number))])
-    ff_nevents = kwargs.pop('spe_nevents',[-1 for i in range(len(ff_run_number))])
-    ped_nevents = kwargs.pop('spe_nevents',[-1 for i in range(len(ped_run_number))])
+    ff_nevents = kwargs.pop('ff_nevents',[-1 for i in range(len(ff_run_number))])
+    ped_nevents = kwargs.pop('ped_nevents',[-1 for i in range(len(ped_run_number))])
 
     spe_max_events = kwargs.pop('spe_max_events',[None for i in range(len(spe_run_number))])
-    ff_max_events = kwargs.pop('spe_max_events',[None for i in range(len(ff_run_number))])
-    ped_max_events = kwargs.pop('spe_max_events',[None for i in range(len(ped_run_number))])
+    ff_max_events = kwargs.pop('ff_max_events',[None for i in range(len(ff_run_number))])
+    ped_max_events = kwargs.pop('ped_max_events',[None for i in range(len(ped_run_number))])
 
     runs_list = spe_run_number + ff_run_number + ped_run_number
     nevents = spe_nevents + ff_nevents + ped_nevents
     max_events = spe_max_events + ff_max_events + ped_max_events
 
     charge_extraction_method = kwargs.get('extractorMethod',"FullWaveformSum")
 
@@ -242,11 +362,18 @@
             key_to_pop.append(key)
 
     for key in key_to_pop : 
         arg.pop(key)
 
     log.info(f"arguments passed to main are : {arg}")
  
-    path= args.extractorMethod+f"_{args.extractor_kwargs['window_shift']}-{args.extractor_kwargs['window_width']-args.extractor_kwargs['window_shift']}"
+    path= args.extractorMethod
+    if args.extractorMethod in ["GlobalPeakWindowSum", "LocalPeakWindowSum"] :
+        path +=f"_{args.extractor_kwargs['window_shift']}-{args.extractor_kwargs['window_width']-args.extractor_kwargs['window_shift']}"
+    elif args.extractorMethod in ["SlidingWindowMaxSum"] :
+        path +=f"_{args.extractor_kwargs['window_width']}"
+    elif args.extractorMethod in ["FixedWindowSum"] :
+        path +=f"_{args.extractor_kwargs['peak_index']}_{args.extractor_kwargs['window_shift']}-{args.extractor_kwargs['window_width']-args.extractor_kwargs['window_shift']}"
+    
     arg['path'] = path
     
     main(**arg)
```

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/ggrolleron/test.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,36 +13,70 @@
 handler.setLevel(logging.INFO)
 formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 handler.setFormatter(formatter)
 log.addHandler(handler)
 
 
 
-from nectarchain.calibration.container import ChargeContainer,WaveformsContainer
+from nectarchain.calibration.container import ChargeContainer,WaveformsContainer,WaveformsContainers,ChargeContainers
 from nectarchain.calibration.container.utils import DataManagement
 
+def test_multicontainers() :
+    run_number = [3731]
+    #waveforms = WaveformsContainers(run_number[0],max_events=20000)
+    #log.info("waveforms created")
+    #waveforms.load_wfs()
+    #log.info("waveforms loaded")
+    #
+    #waveforms.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",overwrite = True)
+    #log.info('waveforms written')
 
+    #waveforms = WaveformsContainers.load(f"{os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{run_number[0]}")
+    #log.info("waveforms loaded")
 
+    #charge = ChargeContainers.from_waveforms(waveforms,method = "LocalPeakWindowSum", window_width = 16, window_shift = 4)
+    #log.info("charge computed")
+    #
+    path = "LocalPeakWindowSum_4-12"
+    #charge.write(f"{os.environ['NECTARCAMDATA']}/charges/{path}/",overwrite = True)
+    #log.info("charge written")
 
-run_number = [2633]
-ped_run_number = [2630]
-FF_run_number = [2609]
+    charge = ChargeContainers.from_file(f"{os.environ['NECTARCAMDATA']}/charges/{path}/",run_number = run_number[0])
+    log.info("charge loaded")
 
-spe_run_1000V = WaveformsContainer(run_number[0],max_events = 1000)
+    charge_merged = charge.merge()
+    log.info('charge merged')
 
-spe_run_1000V.load_wfs()
 
-spe_run_1000V.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",overwrite = True)
 
-spe_run_1000V.load(f"{os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{run_number[0]}.fits")
 
-charge = ChargeContainer.compute_charge(spe_run_1000V,1,method = "gradient_extractor")
 
 
+"""
+def test_simplecontainer() :
+    run_number = [2633]
+    ped_run_number = [2630]
+    FF_run_number = [2609]
 
-charge = ChargeContainer.from_waveform(spe_run_1000V)
+    spe_run_1000V = WaveformsContainer(run_number[0],max_events = 1000)
 
+    spe_run_1000V.load_wfs()
 
-charge.write(f"{os.environ['NECTARCAMDATA']}/charges/std/",overwrite = True)
+    spe_run_1000V.write(f"{os.environ['NECTARCAMDATA']}/waveforms/",overwrite = True)
 
+    spe_run_1000V.load(f"{os.environ['NECTARCAMDATA']}/waveforms/waveforms_run{run_number[0]}.fits")
 
-print("work completed")
+    charge = ChargeContainer.compute_charge(spe_run_1000V,1,method = "gradient_extractor")
+
+
+
+    charge = ChargeContainer.from_waveform(spe_run_1000V)
+
+
+    charge.write(f"{os.environ['NECTARCAMDATA']}/charges/std/",overwrite = True)
+
+"""
+
+if __name__ == "__main__" : 
+    test_multicontainers()
+
+    print("work completed")
```

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md` & `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh` & `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/env bash
 #
-# Time-stamp: "2023-01-30 16:21:22 jlenain"
+# Time-stamp: "2023-05-30 12:05:14 jlenain"
 
 
 function usage ()
 {
     echo "Usage: `basename $0` -r <run number>"
 }
 
@@ -37,56 +37,79 @@
 shift $((OPTIND-1))
 
 if [ -z $runnb ]; then
     usage
     exit 1
 fi
 
-CONTAINER=nectarchain_w_2023_02.sif
+WRAPPER="singularity_wrapper.sh"
+CONTAINER="oras://ghcr.io/cta-observatory/nectarchain:latest"
 OUTDIR=NectarCAM_DQM_Run${runnb}
 DIRAC_OUTDIR=/vo.cta.in2p3.fr/user/j/jlenain/nectarcam/dqm
 
+function exit_script() {
+    return_code=$1
+
+    # Some cleanup before leaving:
+    # [ -d $CONTAINER ] && rm -rf $CONTAINER
+    # [ -f $CONTAINER ] && rm -f $CONTAINER
+    [ -d $OUTDIR ] && rm -rf $OUTDIR
+    [ -f ${OUTDIR}.tar.gz ] && rm -f ${OUTDIR}.tar.gz
+    [ -d ${OUTDIR} ] && rm -rf ${OUTDIR}
+    [ -f $WRAPPER ] && rm -f $WRAPPER
+
+    exit $return_code
+}
+
 # Halim's DQM code needs to use a specific output directory:
 export NECTARDIR=$PWD/$OUTDIR
-[ ! -d $NECTARDIR ] && mkdir -p $NECTARDIR
-mv nectarcam*.sqlite NectarCAM.Run*.fits.fz $NECTARDIR/.
+[ ! -d $NECTARDIR ] && mkdir -p $NECTARDIR || exit_script $?
+# mv nectarcam*.sqlite NectarCAM.Run*.fits.fz $NECTARDIR/.
 
 LISTRUNS=""
-for run in $NECTARDIR/NectarCAM.Run${runnb}.*.fits.fz; do
-    LISTRUNS="$LISTRUNS $run"
+for run in $PWD/NectarCAM.Run${runnb}.*.fits.fz; do
+    LISTRUNS="$LISTRUNS $(basename $run)"
 done
 
 # Create a wrapper BASH script with cleaned environment, see https://redmine.cta-observatory.org/issues/51483
-WRAPPER="sing.sh"
 cat > $WRAPPER <<EOF
 #!/bin/env bash
 echo "Cleaning environment \$CLEANED_ENV" 
 [ -z "\$CLEANED_ENV" ] && exec /bin/env -i CLEANED_ENV="Done" HOME=\${HOME} SHELL=/bin/bash /bin/bash -l "\$0" "\$@" 
 
 
-# Some environment variables related to python, to be passed to container:
+# Some environment variables related to python, to be passed to container, be it for old Singularity version or recent Apptainer ones:
 export SINGULARITYENV_MPLCONFIGDIR=/tmp
 export SINGULARITYENV_NUMBA_CACHE_DIR=/tmp
 export SINGULARITYENV_NECTARDIR=$NECTARDIR
 
+export APPTAINERENV_MPLCONFIGDIR=/tmp
+export APPTAINERENV_NUMBA_CACHE_DIR=/tmp
+export APPTAINERENV_NECTARDIR=$NECTARDIR
+
+# Handle Singularity or Apptainer case:
+if command -v singularity &> /dev/null; then
+    CALLER=singularity
+elif command -v apptainer &> /dev/null; then
+    CALLER=apptainer
+else
+    echo "It seems neither Singularity nor Apptainer are available from here"
+    exit 1
+fi
+
 echo
 echo "Running" 
 # Instantiate the nectarchain Singularity image, run our DQM example run within it:
-cmd="singularity exec --home $PWD $CONTAINER /opt/conda/envs/nectarchain/bin/python /opt/cta/nectarchain/nectarchain/dqm/start_calib.py $LISTRUNS" 
+cmd="\$CALLER exec --home $PWD $CONTAINER /opt/conda/envs/nectarchain/bin/python /opt/cta/nectarchain/src/nectarchain/dqm/start_calib.py $PWD $NECTARDIR -i $LISTRUNS"
 echo \$cmd
 eval \$cmd
 EOF
 
-chmod u+x $WRAPPER
-./${WRAPPER}
+chmod u+x $WRAPPER || exit_script $?
+./${WRAPPER} || exit_script $?
 
 
 # Archive the output directory and push it on DIRAC before leaving the job:
-tar zcf ${OUTDIR}.tar.gz ${OUTDIR}output/
-dirac-dms-add-file ${DIRAC_OUTDIR}/${OUTDIR}.tar.gz ${OUTDIR}.tar.gz LPNHE-USER
+tar zcf ${OUTDIR}.tar.gz ${OUTDIR}/ || exit_script $?
+dirac-dms-add-file ${DIRAC_OUTDIR}/${OUTDIR}.tar.gz ${OUTDIR}.tar.gz LPNHE-USER || exit_script $?
 
-# Some cleanup before leaving:
-[ -d $CONTAINER ] && rm -rf $CONTAINER
-[ -f $CONTAINER ] && rm -f $CONTAINER
-[ -d $OUTDIR ] && rm -rf $OUTDIR
-[ -d ${OUTDIR}output ] && rm -rf ${OUTDIR}output
-[ -f $WRAPPER ] && rm -f $WRAPPER
+exit_script 0
```

### Comparing `nectarchain-0.1.3/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py` & `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Time-stamp: "2023-02-07 21:39:09 jlenain"
+# Time-stamp: "2023-05-30 13:09:04 jlenain"
 
 import argparse
 import sys
 import logging
 from time import sleep
 
 # astropy imports
 from astropy import time
+from astropy import units as u
 
 # DIRAC imports
 from DIRAC.Interfaces.API.Dirac import Dirac
 from DIRAC.Interfaces.API.Job import Job
 from DIRAC.Resources.Catalog.FileCatalogClient import FileCatalogClient
 
 logging.basicConfig(format='[%(levelname)s] %(message)s')
@@ -32,35 +33,38 @@
                     help='only process a specific run (optional)',
                     type=str)
 parser.add_argument('--dry-run',
                     action='store_true',
                     default=False,
                     help='dry run (does not actually submit jobs)')
 parser.add_argument('--log',
-                    default=logging.INFO,
+                    default='info',
                     help='debug output',
                     type=str)
 args = parser.parse_args()
 
-logger.setLevel(args.log)
+logger.setLevel(args.log.upper())
 
 if args.date is None:
     logger.critical('A date should be provided, in a format astropy.time.Time compliant. E.g. "2022-04-01".')
     sys.exit(1)
 
-container="nectarchain_w_2023_02.sif"
 executable_wrapper="dqm_processor.sh"
 
 ## Possible massive job processing via loop on run numbers:
 # for run in ['2720', '3277', '...']:
 
 ## or from DIRAC FileCatalog directory listing:
 processDate = time.Time(args.date)
 dfcDir = f'/vo.cta.in2p3.fr/nectarcam/{processDate.ymdhms[0]}/{processDate.ymdhms[0]}{str(processDate.ymdhms[1]).zfill(2)}{str(processDate.ymdhms[2]).zfill(2)}'
 
+# The relevant DB file may be stored in the directory corresponding to the day after:
+processDateTomorrow = processDate + 1. * u.day
+dfcDirTomorrow = f'/vo.cta.in2p3.fr/nectarcam/{processDateTomorrow.ymdhms[0]}/{processDateTomorrow.ymdhms[0]}{str(processDateTomorrow.ymdhms[1]).zfill(2)}{str(processDateTomorrow.ymdhms[2]).zfill(2)}'
+
 # Sometimes, for unkown reason, the connection to the DFC can fail, try a few times:
 sleep_time = 2
 num_retries = 3
 for x in range(0, num_retries):
     try:
         dfc = FileCatalogClient()
         str_error = None
@@ -72,66 +76,73 @@
     else:
         break
 if not dfc:
     logger.fatal(f'Connection to FileCatalogClient failed, aborting...')
     sys.exit(1)
 
 infos = dfc.listDirectory(dfcDir)
+infosTomorrow = dfc.listDirectory(dfcDirTomorrow)
 if not infos['OK'] or not infos['Value']['Successful']:
     logger.critical(f"Could not properly retrieve the file metadata for {dfcDir} ... Exiting !")
     sys.exit(1)
+if not infosTomorrow['OK'] or not infosTomorrow['Value']['Successful']:
+    logger.warning(f"Could not properly retrieve the file metadata for {dfcDirTomorrow} ... Continuing !")
 meta = infos['Value']['Successful'][dfcDir]
+metaTomorrow = infosTomorrow['Value']['Successful'][dfcDirTomorrow]
 
 runlist = []
 
-sqlfile = None
+sqlfilelist = []
 for f in meta['Files']:
     if f.endswith('.fits.fz'):
         run = f.split('NectarCAM.Run')[1].split('.')[0]
         if run not in runlist and run is not None:
             runlist.append(run)
     if f.endswith('.sqlite'):
-        sqlfile = f
+        sqlfilelist.append(f)
+for f in metaTomorrow['Files']:
+    if f.endswith('.sqlite'):
+        sqlfilelist.append(f)
 if args.run is not None:
     if args.run not in runlist:
         logger.critical(f'Your specified run {args.run} was not found in {dfcDir}, aborting...')
         sys.exit(1)
     runlist = [args.run]
     
 logger.info(f'Found runs {runlist} in {dfcDir}')
 
-if sqlfile is None:
-    logger.critical('Could not find any SQLite file in {dfcDir}, aborting...')
+if len(sqlfilelist) == 0:
+    logger.critical('Could not find any SQLite file in {dfcDir} nor in {dfcDirTomorrow}, aborting...')
     sys.exit(1)
-logger.info(f'Found SQLite file {sqlfile} in {dfcDir}')
+logger.info(f'Found SQLite files {sqlfilelist} in {dfcDir} and {dfcDirTomorrow}')
 
 # Now, submit the DIRAC jobs:
 # for run in ['2721']:
 for run in runlist:
     j = Job()
     # j.setExecutable(f'{executable_wrapper}', '<SOME POSSIBLE ARGUMENTS such as run number>')
     j.setExecutable(f'{executable_wrapper}', f'-r {run}')
     # Force job to be run from a given Computing Element:
     # j.setDestination('LCG.GRIF.fr')
     j.setName(f'NectarCAM DQM run {run}')
     j.setJobGroup('NectarCAM DQM')
-    sandboxlist = [f'{executable_wrapper}',
-                   f'LFN:/vo.cta.in2p3.fr/user/j/jlenain/local/opt/singularity/nectarchain/{container}',
-                   f'LFN:{sqlfile}']
+    sandboxlist = [f'{executable_wrapper}']
     for f in meta['Files']:
         if f.endswith('.fits.fz') and f'NectarCAM.Run{run}' in f:
             sandboxlist.append(f'LFN:{f}')
-    if len(sandboxlist) < 4:
+    for s in sqlfilelist:
+        sandboxlist.append(f'LFN:{s}')
+    if len(sandboxlist) < 2:
         logger.critical(f'''Misformed sandboxlist, actual data .fits.fz files missing:
 {sandboxlist}
 
 Aborting...
 ''')
         sys.exit(1)
     logger.info(f'''Submitting job for run {run}, with the following InputSandbox:
 {sandboxlist}
 ''')
     j.setInputSandbox(sandboxlist)
 
     if not args.dry_run:
-        res = dirac.submitJob(j)  #, mode='local')  # for local execution, simulating a DIRAC job on the local machine, instead of submitting it to a DIRAC Computing Element
+        res = dirac.submitJob(j)  # , mode='local')  # for local execution, simulating a DIRAC job on the local machine, instead of submitting it to a DIRAC Computing Element
         logger.info(f"Submission Result: {res['Value']}")
```

### Comparing `nectarchain-0.1.3/src/nectarchain/version.py` & `nectarchain-0.1.4/src/nectarchain/version.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.3/src/nectarchain.egg-info/SOURCES.txt` & `nectarchain-0.1.4/src/nectarchain.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,24 @@
+LICENSE.md
 MANIFEST.in
 README.md
+Singularity
 environment.yml
 pyproject.toml
-setup.cfg
-setup.py
 examples/waveform_animation_highGain.py
-licenses/LICENSE.rst
-licenses/README.rst
 notebooks/Access NectarCAM data using DIRAC API.ipynb
 notebooks/Read_NectarCAM_events.ipynb
 notebooks/calculate_calibration_coefficients.ipynb
 notebooks/calculate_pedestals.ipynb
-singularity/Singularity
 src/nectarchain/__init__.py
 src/nectarchain/_version.py
 src/nectarchain/version.py
 src/nectarchain.egg-info/PKG-INFO
 src/nectarchain.egg-info/SOURCES.txt
 src/nectarchain.egg-info/dependency_links.txt
-src/nectarchain.egg-info/not-zip-safe
 src/nectarchain.egg-info/requires.txt
 src/nectarchain.egg-info/top_level.txt
 src/nectarchain/calibration/README.md
 src/nectarchain/calibration/__init__.py
 src/nectarchain/calibration/NectarGain/__init__.py
 src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py
 src/nectarchain/calibration/NectarGain/PhotoStat/__init__.py
@@ -41,16 +37,16 @@
 src/nectarchain/calibration/NectarGain/utils/__init__.py
 src/nectarchain/calibration/NectarGain/utils/error.py
 src/nectarchain/calibration/container/__init__.py
 src/nectarchain/calibration/container/charge.py
 src/nectarchain/calibration/container/charge_extractor.py
 src/nectarchain/calibration/container/utils.py
 src/nectarchain/calibration/container/waveforms.py
-src/nectarchain/dqm/README
-src/nectarchain/dqm/ReadPickleFiles.py
+src/nectarchain/dqm/README.md
+src/nectarchain/dqm/__init__.py
 src/nectarchain/dqm/camera_monitoring.py
 src/nectarchain/dqm/charge_integration.py
 src/nectarchain/dqm/dqm_summary_processor.py
 src/nectarchain/dqm/mean_camera_display.py
 src/nectarchain/dqm/mean_waveforms.py
 src/nectarchain/dqm/start_calib.py
 src/nectarchain/dqm/trigger_statistics.py
@@ -70,8 +66,21 @@
 src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py
 src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh
 src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py
 src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.sh
 src/nectarchain/user_scripts/ggrolleron/test.py
 src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md
 src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh
-src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py
+src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py
+src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/GainFitter.sh
+src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/submitGainFitter.py
+src/nectarchain/user_scripts/vmarandon/CalibrationData.py
+src/nectarchain/user_scripts/vmarandon/CalibrationEvoData.py
+src/nectarchain/user_scripts/vmarandon/DBHandler.py
+src/nectarchain/user_scripts/vmarandon/DataUtils.py
+src/nectarchain/user_scripts/vmarandon/ExtractInformation2.py
+src/nectarchain/user_scripts/vmarandon/FileHandler.py
+src/nectarchain/user_scripts/vmarandon/PedestalEstimation.py
+src/nectarchain/user_scripts/vmarandon/ShowDataContent.py
+src/nectarchain/user_scripts/vmarandon/ShowPedestalEvolution.py
+src/nectarchain/user_scripts/vmarandon/Stats.py
+src/nectarchain/user_scripts/vmarandon/Utils.py
```

