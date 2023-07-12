# Comparing `tmp/nectarchain-0.1.4.tar.gz` & `tmp/nectarchain-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nectarchain-0.1.4.tar", last modified: Wed Jul 12 15:49:38 2023, max compression
+gzip compressed data, was "nectarchain-0.1.5.tar", last modified: Wed Jul 12 20:39:52 2023, max compression
```

## Comparing `nectarchain-0.1.4.tar` & `nectarchain-0.1.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.426652 nectarchain-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 15:49:28.000000 nectarchain-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 15:49:28.000000 nectarchain-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-12 15:49:38.426652 nectarchain-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-12 15:49:28.000000 nectarchain-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-12 15:49:28.000000 nectarchain-0.1.4/Singularity
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 15:49:28.000000 nectarchain-0.1.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.410652 nectarchain-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-12 15:49:28.000000 nectarchain-0.1.4/examples/waveform_animation_highGain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   208363 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/Access NectarCAM data using DIRAC API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/Read_NectarCAM_events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   832042 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/calculate_calibration_coefficients.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1718551 2023-07-12 15:49:28.000000 nectarchain-0.1.4/notebooks/calculate_pedestals.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-12 15:49:28.000000 nectarchain-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:49:38.426652 nectarchain-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.410652 nectarchain-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/calibration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py
--rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_ped.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signalStd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_fromHHVFit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/calibration/container/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26120 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/charge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/calibration/container/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.418652 nectarchain-0.1.4/src/nectarchain/dqm/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/camera_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/charge_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/dqm_summary_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/mean_camera_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/mean_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/start_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/dqm/trigger_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration_param.json
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_pedestals.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/tools/write_pedestals_param.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.410652 nectarchain-0.1.4/src/nectarchain/user_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/fbradascio/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/fbradascio/fbradascio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/fbrun_scripts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3154 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.422652 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3833 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/GainFitter.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/submitGainFitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.426652 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/
--rw-r--r--   0 runner    (1001) docker     (123)    26016 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/CalibrationData.py
--rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/CalibrationEvoData.py
--rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/DBHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/DataUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ExtractInformation2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/PedestalEstimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ShowDataContent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ShowPedestalEvolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/Stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 15:49:28.000000 nectarchain-0.1.4/src/nectarchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:38.414652 nectarchain-0.1.4/src/nectarchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 15:49:38.000000 nectarchain-0.1.4/src/nectarchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.113765 nectarchain-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-12 20:39:40.000000 nectarchain-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-12 20:39:40.000000 nectarchain-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-12 20:39:52.113765 nectarchain-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-12 20:39:40.000000 nectarchain-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-12 20:39:40.000000 nectarchain-0.1.5/Singularity
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 20:39:40.000000 nectarchain-0.1.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.085765 nectarchain-0.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-12 20:39:40.000000 nectarchain-0.1.5/examples/waveform_animation_highGain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.089765 nectarchain-0.1.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   208363 2023-07-12 20:39:40.000000 nectarchain-0.1.5/notebooks/Access NectarCAM data using DIRAC API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-12 20:39:40.000000 nectarchain-0.1.5/notebooks/Read_NectarCAM_events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   832042 2023-07-12 20:39:40.000000 nectarchain-0.1.5/notebooks/calculate_calibration_coefficients.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1718551 2023-07-12 20:39:40.000000 nectarchain-0.1.5/notebooks/calculate_pedestals.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-12 20:39:40.000000 nectarchain-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:39:52.113765 nectarchain-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.077765 nectarchain-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.089765 nectarchain-0.1.5/src/nectarchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 20:39:51.000000 nectarchain-0.1.5/src/nectarchain/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.093765 nectarchain-0.1.5/src/nectarchain/calibration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.093765 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.093765 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/PhotoStat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/PhotoStat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.097765 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48612 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters_ped.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signalStd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_fromHHVFit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.097765 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.101765 nectarchain-0.1.5/src/nectarchain/calibration/container/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26120 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/container/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/container/charge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/container/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/calibration/container/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.101765 nectarchain-0.1.5/src/nectarchain/dqm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/camera_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/charge_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/dqm_summary_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/mean_camera_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/mean_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/start_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/dqm/trigger_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.101765 nectarchain-0.1.5/src/nectarchain/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.105765 nectarchain-0.1.5/src/nectarchain/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/tools/write_camera_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/tools/write_camera_calibration_param.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/tools/write_pedestals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/tools/write_pedestals_param.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.081765 nectarchain-0.1.5/src/nectarchain/user_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.105765 nectarchain-0.1.5/src/nectarchain/user_scripts/fbradascio/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/fbradascio/fbradascio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.105765 nectarchain-0.1.5/src/nectarchain/user_scripts/fbrun/
+-rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/fbrun/fbrun_scripts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.109765 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.109765 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.109765 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3154 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.109765 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3833 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/GainFitter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/submitGainFitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.113765 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/
+-rw-r--r--   0 runner    (1001) docker     (123)    26016 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/CalibrationData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18746 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/CalibrationEvoData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/DBHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/DataUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/ExtractInformation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/PedestalEstimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/ShowDataContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/ShowPedestalEvolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/Stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 20:39:40.000000 nectarchain-0.1.5/src/nectarchain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:39:52.093765 nectarchain-0.1.5/src/nectarchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-12 20:39:52.000000 nectarchain-0.1.5/src/nectarchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-12 20:39:52.000000 nectarchain-0.1.5/src/nectarchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:39:52.000000 nectarchain-0.1.5/src/nectarchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-12 20:39:52.000000 nectarchain-0.1.5/src/nectarchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 20:39:52.000000 nectarchain-0.1.5/src/nectarchain.egg-info/top_level.txt
```

### Comparing `nectarchain-0.1.4/LICENSE.md` & `nectarchain-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/PKG-INFO` & `nectarchain-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nectarchain
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analysis chain for the CTA MSTN NectarCAM prototype
 Author: NectarCAM collaboration
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/cta-observatory/nectarchain/issues
 Project-URL: Source Code, https://github.com/cta-observatory/nectarchain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nectarchain-0.1.4/README.md` & `nectarchain-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/Singularity` & `nectarchain-0.1.5/Singularity`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/examples/waveform_animation_highGain.py` & `nectarchain-0.1.5/examples/waveform_animation_highGain.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/notebooks/Access NectarCAM data using DIRAC API.ipynb` & `nectarchain-0.1.5/notebooks/Access NectarCAM data using DIRAC API.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/notebooks/Read_NectarCAM_events.ipynb` & `nectarchain-0.1.5/notebooks/Read_NectarCAM_events.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/notebooks/calculate_calibration_coefficients.ipynb` & `nectarchain-0.1.5/notebooks/calculate_calibration_coefficients.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/notebooks/calculate_pedestals.ipynb` & `nectarchain-0.1.5/notebooks/calculate_pedestals.ipynb`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/pyproject.toml` & `nectarchain-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "browser_cookie3",
     "ctapipe~=0.19",
     "ctapipe-io-nectarcam",
-    "mechanize",
     "pandas",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown; charset=UTF-8"
```

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/PhotoStat/PhotoStat.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGAIN_old.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_combined.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/NectarGainSPE_singlerun.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/parameters_signal_combined.yaml`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/NectarGain/SPEfit/utils.py` & `nectarchain-0.1.5/src/nectarchain/calibration/NectarGain/SPEfit/utils.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/container/charge.py` & `nectarchain-0.1.5/src/nectarchain/calibration/container/charge.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/container/charge_extractor.py` & `nectarchain-0.1.5/src/nectarchain/calibration/container/charge_extractor.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/container/utils.py` & `nectarchain-0.1.5/src/nectarchain/calibration/container/utils.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/calibration/container/waveforms.py` & `nectarchain-0.1.5/src/nectarchain/calibration/container/waveforms.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/README.md` & `nectarchain-0.1.5/src/nectarchain/dqm/README.md`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/camera_monitoring.py` & `nectarchain-0.1.5/src/nectarchain/dqm/camera_monitoring.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/charge_integration.py` & `nectarchain-0.1.5/src/nectarchain/dqm/charge_integration.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/dqm_summary_processor.py` & `nectarchain-0.1.5/src/nectarchain/dqm/dqm_summary_processor.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/mean_camera_display.py` & `nectarchain-0.1.5/src/nectarchain/dqm/mean_camera_display.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/mean_waveforms.py` & `nectarchain-0.1.5/src/nectarchain/dqm/mean_waveforms.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/start_calib.py` & `nectarchain-0.1.5/src/nectarchain/dqm/start_calib.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/dqm/trigger_statistics.py` & `nectarchain-0.1.5/src/nectarchain/dqm/trigger_statistics.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration.py` & `nectarchain-0.1.5/src/nectarchain/tools/write_camera_calibration.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/tools/write_camera_calibration_param.json` & `nectarchain-0.1.5/src/nectarchain/tools/write_camera_calibration_param.json`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/tools/write_pedestals.py` & `nectarchain-0.1.5/src/nectarchain/tools/write_pedestals.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/tools/write_pedestals_param.json` & `nectarchain-0.1.5/src/nectarchain/tools/write_pedestals_param.json`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/fbrun/ComputeCalibCoefs.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_PhotoStat_computation.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_combined_computation.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/gain_SPEfit_computation.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/load_wfs_compute_charge.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/ggrolleron/test.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/ggrolleron/test.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md` & `nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/Dark room temperature analysis.md`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh` & `nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/dqm_processor.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/dqm_job_submitter/submit_dqm_processor.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/GainFitter.sh` & `nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/GainFitter.sh`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/submitGainFitter.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/jlenain/submitGainFitDIRAC/submitGainFitter.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/CalibrationData.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/CalibrationData.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/CalibrationEvoData.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/CalibrationEvoData.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/DBHandler.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/DBHandler.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/DataUtils.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/DataUtils.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ExtractInformation2.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/ExtractInformation2.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/FileHandler.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/FileHandler.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/PedestalEstimation.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/PedestalEstimation.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ShowDataContent.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/ShowDataContent.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/ShowPedestalEvolution.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/ShowPedestalEvolution.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/Stats.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/Stats.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/user_scripts/vmarandon/Utils.py` & `nectarchain-0.1.5/src/nectarchain/user_scripts/vmarandon/Utils.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain/version.py` & `nectarchain-0.1.5/src/nectarchain/version.py`

 * *Files identical despite different names*

### Comparing `nectarchain-0.1.4/src/nectarchain.egg-info/PKG-INFO` & `nectarchain-0.1.5/src/nectarchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nectarchain
-Version: 0.1.4
+Version: 0.1.5
 Summary: Analysis chain for the CTA MSTN NectarCAM prototype
 Author: NectarCAM collaboration
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/cta-observatory/nectarchain/issues
 Project-URL: Source Code, https://github.com/cta-observatory/nectarchain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nectarchain-0.1.4/src/nectarchain.egg-info/SOURCES.txt` & `nectarchain-0.1.5/src/nectarchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

