# Comparing `tmp/pcdsdevices-7.4.2.tar.gz` & `tmp/pcdsdevices-7.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdsdevices-7.4.2.tar", last modified: Fri Jul  7 18:43:41 2023, max compression
+gzip compressed data, was "pcdsdevices-7.4.3.tar", last modified: Tue Jul 11 23:11:29 2023, max compression
```

## Comparing `pcdsdevices-7.4.2.tar` & `pcdsdevices-7.4.3.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.721532 pcdsdevices-7.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.693532 pcdsdevices-7.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.693532 pcdsdevices-7.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-07-07 18:43:41.721532 pcdsdevices-7.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.693532 pcdsdevices-7.4.2/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.693532 pcdsdevices-7.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      739 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.693532 pcdsdevices-7.4.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/README.inc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.689532 pcdsdevices-7.4.2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.697532 pcdsdevices-7.4.2/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2695 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/base_classes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8755 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      925 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/mv.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/presets.rst
--rw-r--r--   0 runner    (1001) docker     (122)    77561 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/signals.rst
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/sim_types.rst
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/tab.rst
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/ui.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.697532 pcdsdevices-7.4.2/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/source/upcoming_release_notes/template-short.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/update_api_list.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs/view-build.sh
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/docs-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      168 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/make_ophyd_device
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.705532 pcdsdevices-7.4.2/pcdsdevices/
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/_html.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/analog_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.705532 pcdsdevices-7.4.2/pcdsdevices/areadetector/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/areadetector/cam.py
--rw-r--r--   0 runner    (1001) docker     (122)    19375 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/areadetector/detectors.py
--rw-r--r--   0 runner    (1001) docker     (122)     6459 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/areadetector/plugins.py
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/atm.py
--rw-r--r--   0 runner    (1001) docker     (122)    60210 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/attenuator.py
--rw-r--r--   0 runner    (1001) docker     (122)    12442 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/beam_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    39229 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ccm.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/crix_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/cvmi_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/dc_devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/delay_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    17619 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/device_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    30560 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/digitizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/doc_stubs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)    51429 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/epics_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/evr.py
--rw-r--r--   0 runner    (1001) docker     (122)    14511 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/fms.py
--rw-r--r--   0 runner    (1001) docker     (122)    16504 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/gauge.py
--rw-r--r--   0 runner    (1001) docker     (122)    22654 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/gon.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.705532 pcdsdevices-7.4.2/pcdsdevices/happi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/happi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29150 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/happi/containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     9121 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/inout.py
--rw-r--r--   0 runner    (1001) docker     (122)    64152 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/interface.py
--rw-r--r--   0 runner    (1001) docker     (122)    19459 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ipm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/jet.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lamp_motion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.709532 pcdsdevices-7.4.2/pcdsdevices/lasers/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19804 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/btms_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    22910 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/btps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/counters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/dicon.py
--rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/ek9000.py
--rw-r--r--   0 runner    (1001) docker     (122)     5767 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/elliptec.py
--rw-r--r--   0 runner    (1001) docker     (122)     4669 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/qmini.py
--rw-r--r--   0 runner    (1001) docker     (122)    15417 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/rfof.py
--rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/thorlabsWFS.py
--rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/tuttifrutti.py
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lasers/zoomtelescope.py
--rw-r--r--   0 runner    (1001) docker     (122)    21112 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lens.py
--rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lic.py
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/light_control.py
--rw-r--r--   0 runner    (1001) docker     (122)    74029 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lodcm.py
--rw-r--r--   0 runner    (1001) docker     (122)    16653 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/lxe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/make_ophyd_device.py
--rw-r--r--   0 runner    (1001) docker     (122)    49040 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/mirror.py
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/movablestand.py
--rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/mpod.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8327 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/mpod_apalis.py
--rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/mps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/mrco_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/mv_interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/piezo.py
--rw-r--r--   0 runner    (1001) docker     (122)    20301 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pim.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pmps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (122)     7358 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/positioner.py
--rw-r--r--   0 runner    (1001) docker     (122)    39960 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pseudopos.py
--rw-r--r--   0 runner    (1001) docker     (122)     6901 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pulsepicker.py
--rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pump.py
--rw-r--r--   0 runner    (1001) docker     (122)     5607 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/pv_positioner.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/radiation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ref.py
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/rs_powersupply.py
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/rtds_ebd.py
--rw-r--r--   0 runner    (1001) docker     (122)    11767 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/sample_delivery.py
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11909 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (122)    58121 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/signal.py
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/sim.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/slits.py
--rw-r--r--   0 runner    (1001) docker     (122)    15582 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (122)    29013 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     6245 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/stopper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/sxr_test_absorber.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tags.py
--rw-r--r--   0 runner    (1001) docker     (122)    48269 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.713532 pcdsdevices-7.4.2/pcdsdevices/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_analog_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_atm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_attenuator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_beam_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    14520 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_btms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10004 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_ccm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_crix_motion.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_dc_devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     6658 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_device_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_disconnected.py
--rw-r--r--   0 runner    (1001) docker     (122)      868 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_epics_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_evr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_gauge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8654 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_gon.py
--rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_inout.py
--rw-r--r--   0 runner    (1001) docker     (122)     9847 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_ipm.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_jet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lens.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.713532 pcdsdevices-7.4.2/pcdsdevices/tests/test_lens_sets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lens_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lens_sets/original.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lens_sets/test
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lens_sets/test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lic.py
--rw-r--r--   0 runner    (1001) docker     (122)    19101 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lodcm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_lxe.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_movablestand.py
--rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_mpod.py
--rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_mpod_apalis.py
--rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_mps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_pim.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_pneumatic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_positioner.py
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_pseudopos.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_pulsepicker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_pump.py
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (122)     5738 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_sample_delivery.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (122)    16240 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_slits.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10914 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)    17153 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_timetool.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_valve.py
--rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_variety.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/test_wfs.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/tests/xcslt8717_wpcalib_opa
--rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/timetool.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/type_hints.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.721532 pcdsdevices-7.4.2/pcdsdevices/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AT1K2.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AT1K2.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AT2L0.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AT2L0.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6586 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    25452 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5729 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    18911 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4876 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    22407 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
--rw-r--r--   0 runner    (1001) docker     (122)    17847 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
--rw-r--r--   0 runner    (1001) docker     (122)    15571 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5918 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_filter.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffAxis.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffAxis.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    41696 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    25557 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffSlits.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/BtpsState.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/BtpsState.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    60307 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/JJSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/LCP.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/Leviton1.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/LightControl.ui
--rw-r--r--   0 runner    (1001) docker     (122)    51167 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/PowerSlits.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    34999 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/PowerSlits.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    27032 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/QminiSpectrometer.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    10488 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/Setra5000.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)    10138 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/StatePositioner.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/StatePositioner.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)    10236 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/at2l0_filters.json
--rw-r--r--   0 runner    (1001) docker     (122)    15242 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-camera-summary.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12171 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-config.ui
--rw-r--r--   0 runner    (1001) docker     (122)    33295 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-overview.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12410 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-range-config.ui
--rw-r--r--   0 runner    (1001) docker     (122)     9784 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-range-summary.ui
--rw-r--r--   0 runner    (1001) docker     (122)    46416 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-dest.ui
--rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-tabs-config.ui
--rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-tabs.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-valves.ui
--rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/btps.ui
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/ui/detailed_tree.ui
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/usb_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    27787 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    23272 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/valve.py
--rw-r--r--   0 runner    (1001) docker     (122)     9015 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/variety.py
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pcdsdevices/wfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:43:41.705532 pcdsdevices-7.4.2/pcdsdevices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8262 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-07 18:43:41.000000 pcdsdevices-7.4.2/pcdsdevices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-07-07 18:43:25.000000 pcdsdevices-7.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 18:43:41.721532 pcdsdevices-7.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.279142 pcdsdevices-7.4.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.239140 pcdsdevices-7.4.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.239140 pcdsdevices-7.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-07-11 23:11:29.279142 pcdsdevices-7.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.243141 pcdsdevices-7.4.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.243141 pcdsdevices-7.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.243141 pcdsdevices-7.4.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/README.inc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.239140 pcdsdevices-7.4.3/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.243141 pcdsdevices-7.4.3/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2695 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/base_classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8755 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/mv.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/presets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    77995 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/sim_types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/tab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/ui.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.243141 pcdsdevices-7.4.3/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/source/upcoming_release_notes/template-short.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/update_api_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs/view-build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/docs-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      168 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/make_ophyd_device
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.255141 pcdsdevices-7.4.3/pcdsdevices/
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/analog_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.259141 pcdsdevices-7.4.3/pcdsdevices/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/areadetector/cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19375 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/areadetector/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6459 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/areadetector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/atm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60210 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12442 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39229 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ccm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/cvmi_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/delay_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17619 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30560 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/doc_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51429 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/evr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14511 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/fms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16504 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22654 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/gon.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.259141 pcdsdevices-7.4.3/pcdsdevices/happi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29150 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9121 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/inout.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64152 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19459 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ipm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/jet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lamp_motion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.259141 pcdsdevices-7.4.3/pcdsdevices/lasers/
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19804 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/btms_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22910 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/btps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/counters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/dicon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/ek9000.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5767 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/elliptec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4669 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/qmini.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15417 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/rfof.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/thorlabsWFS.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/tuttifrutti.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lasers/zoomtelescope.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21112 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/light_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74029 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16653 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/lxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/make_ophyd_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49040 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/mpod.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8327 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/mrco_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/mv_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/piezo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20300 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pmps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7358 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39960 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6901 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5607 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/pv_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/radiation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/rs_powersupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/rtds_ebd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11767 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11909 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58121 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/sim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/slits.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15582 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29013 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6245 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/stopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/sxr_test_absorber.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48269 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.267141 pcdsdevices-7.4.3/pcdsdevices/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_analog_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_atm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14520 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_btms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10004 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_ccm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6658 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_disconnected.py
+-rw-r--r--   0 runner    (1001) docker     (122)      868 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_evr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8654 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_gon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_inout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9847 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_ipm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_jet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lens.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.267141 pcdsdevices-7.4.3/pcdsdevices/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lens_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lens_sets/original.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lens_sets/test
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lens_sets/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19101 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_lxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_mpod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_pim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5738 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16240 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_slits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10914 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17153 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_timetool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_valve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_variety.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/test_wfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/tests/xcslt8717_wpcalib_opa
+-rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/timetool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.279142 pcdsdevices-7.4.3/pcdsdevices/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AT1K2.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AT1K2.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AT2L0.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6586 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    25452 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5729 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    18911 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4876 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    22407 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    17847 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    15571 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5918 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_filter.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffAxis.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffAxis.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    41696 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    25557 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/BtpsState.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/BtpsState.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    60307 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/JJSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/LCP.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/Leviton1.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/LightControl.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    51167 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/PowerSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    34999 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/PowerSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    27032 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/QminiSpectrometer.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10488 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/Setra5000.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10138 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/StatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/StatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10236 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/at2l0_filters.json
+-rw-r--r--   0 runner    (1001) docker     (122)    15242 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-camera-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12171 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    33295 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12410 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-range-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     9784 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-range-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    46416 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-dest.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-tabs-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-tabs.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-valves.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/btps.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/ui/detailed_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/usb_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27787 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23272 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9015 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/variety.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pcdsdevices/wfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 23:11:29.259141 pcdsdevices-7.4.3/pcdsdevices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8262 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-11 23:11:29.000000 pcdsdevices-7.4.3/pcdsdevices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-11 23:11:07.000000 pcdsdevices-7.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 23:11:29.279142 pcdsdevices-7.4.3/setup.cfg
```

### Comparing `pcdsdevices-7.4.2/.github/ISSUE_TEMPLATE.md` & `pcdsdevices-7.4.3/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/.github/PULL_REQUEST_TEMPLATE.md` & `pcdsdevices-7.4.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/.github/workflows/standard.yml` & `pcdsdevices-7.4.3/.github/workflows/standard.yml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/.pre-commit-config.yaml` & `pcdsdevices-7.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/CONTRIBUTING.rst` & `pcdsdevices-7.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/LICENSE.md` & `pcdsdevices-7.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/PKG-INFO` & `pcdsdevices-7.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdevices
-Version: 7.4.2
+Version: 7.4.3
 Summary: Ophyd Device definitions for LCLS Beamline components
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.2 Summary: Ophyd Device
+Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.3 Summary: Ophyd Device
 definitions for LCLS Beamline components Author: SLAC National Accelerator
 Laboratory License: Copyright (c) 2023, The Board of Trustees of the Leland
 Stanford Junior University, through SLAC National Accelerator Laboratory
 (subject to receipt of any required approvals from the U.S. Dept. of Energy).
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: (1) Redistributions of source code must retain the above copyright notice,
```

### Comparing `pcdsdevices-7.4.2/README.md` & `pcdsdevices-7.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/conda-recipe/meta.yaml` & `pcdsdevices-7.4.3/conda-recipe/meta.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,17 @@
     - pytmc >=2.7.0
     - pyyaml
     - schema
     - scipy
   run_constrained:
     - pmgr >=2.0.2
     - typhos >=2.4.0
-    # Note: these should be removed once a newer xraylib is available on conda-forge
-    # or moved to pcdscalc after testing
-    - sqlalchemy <2.0.0
-    - xraydb <4.5.0
 
 test:
-  requirements:
+  requires:
     - pytest
     - pytest-timeout
     - matplotlib
     - typhos
   imports:
     - {{ import_name }}
```

### Comparing `pcdsdevices-7.4.2/docs/Makefile` & `pcdsdevices-7.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/pre-release-notes.sh` & `pcdsdevices-7.4.3/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/release_notes.py` & `pcdsdevices-7.4.3/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/README.inc` & `pcdsdevices-7.4.3/docs/source/README.inc`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/_templates/autosummary/class.rst` & `pcdsdevices-7.4.3/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/_templates/autosummary/module.rst` & `pcdsdevices-7.4.3/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/api.rst` & `pcdsdevices-7.4.3/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/base_classes.rst` & `pcdsdevices-7.4.3/docs/source/base_classes.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/conf.py` & `pcdsdevices-7.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/mv.rst` & `pcdsdevices-7.4.3/docs/source/mv.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/presets.rst` & `pcdsdevices-7.4.3/docs/source/presets.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/releases.rst` & `pcdsdevices-7.4.3/docs/source/releases.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 Release History
 ###############
 
 
+v7.4.3 (2023-07-11)
+===================
+
+Bugfixes
+--------
+- Fix typo in zoom motor prefix for PIM devices.
+
+Maintenance
+-----------
+- Fix conda recipe test-requires.
+- Remove sqlalchemy and xraydb pins from requirements.txt.
+  These were pinned because the most recent versions of these packages
+  were previously incompatible with each other. This has since been resolved.
+
+Contributors
+------------
+- tangkong
+- vespos
+- zllentz
+
+
 v7.4.2 (2023-07-07)
 ===================
 
 Device Updates
 --------------
 - ``.screen()`` and ``.post_elog_status()`` methods were added to the
   BaseInterface whitelist for tab completion.
```

### Comparing `pcdsdevices-7.4.2/docs/source/signals.rst` & `pcdsdevices-7.4.3/docs/source/signals.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/tab.rst` & `pcdsdevices-7.4.3/docs/source/tab.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/source/upcoming_release_notes/template-full.rst` & `pcdsdevices-7.4.3/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/docs/update_api_list.py` & `pcdsdevices-7.4.3/docs/update_api_list.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/__init__.py` & `pcdsdevices-7.4.3/pcdsdevices/__init__.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/_html.py` & `pcdsdevices-7.4.3/pcdsdevices/_html.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/analog_signals.py` & `pcdsdevices-7.4.3/pcdsdevices/analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/areadetector/cam.py` & `pcdsdevices-7.4.3/pcdsdevices/areadetector/cam.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/areadetector/detectors.py` & `pcdsdevices-7.4.3/pcdsdevices/areadetector/detectors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/areadetector/plugins.py` & `pcdsdevices-7.4.3/pcdsdevices/areadetector/plugins.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/atm.py` & `pcdsdevices-7.4.3/pcdsdevices/atm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/attenuator.py` & `pcdsdevices-7.4.3/pcdsdevices/attenuator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/beam_stats.py` & `pcdsdevices-7.4.3/pcdsdevices/beam_stats.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ccm.py` & `pcdsdevices-7.4.3/pcdsdevices/ccm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/crix_motion.py` & `pcdsdevices-7.4.3/pcdsdevices/crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/cvmi_motion.py` & `pcdsdevices-7.4.3/pcdsdevices/cvmi_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/dc_devices.py` & `pcdsdevices-7.4.3/pcdsdevices/dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/delay_generator.py` & `pcdsdevices-7.4.3/pcdsdevices/delay_generator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/device.py` & `pcdsdevices-7.4.3/pcdsdevices/device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/device_types.py` & `pcdsdevices-7.4.3/pcdsdevices/device_types.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/digitizers.py` & `pcdsdevices-7.4.3/pcdsdevices/digitizers.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/doc_stubs.py` & `pcdsdevices-7.4.3/pcdsdevices/doc_stubs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/energy_monitor.py` & `pcdsdevices-7.4.3/pcdsdevices/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/epics_motor.py` & `pcdsdevices-7.4.3/pcdsdevices/epics_motor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/evr.py` & `pcdsdevices-7.4.3/pcdsdevices/evr.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/fms.py` & `pcdsdevices-7.4.3/pcdsdevices/fms.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/gauge.py` & `pcdsdevices-7.4.3/pcdsdevices/gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/gon.py` & `pcdsdevices-7.4.3/pcdsdevices/gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/happi/containers.py` & `pcdsdevices-7.4.3/pcdsdevices/happi/containers.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/inout.py` & `pcdsdevices-7.4.3/pcdsdevices/inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/interface.py` & `pcdsdevices-7.4.3/pcdsdevices/interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ipm.py` & `pcdsdevices-7.4.3/pcdsdevices/ipm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/jet.py` & `pcdsdevices-7.4.3/pcdsdevices/jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lamp_motion.py` & `pcdsdevices-7.4.3/pcdsdevices/lamp_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/btms_config.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/btms_config.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/btps.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/btps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/counters.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/counters.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/dicon.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/dicon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/ek9000.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/ek9000.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/elliptec.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/elliptec.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/qmini.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/qmini.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/rfof.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/rfof.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/thorlabsWFS.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/thorlabsWFS.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/tuttifrutti.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/tuttifrutti.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lasers/zoomtelescope.py` & `pcdsdevices-7.4.3/pcdsdevices/lasers/zoomtelescope.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lens.py` & `pcdsdevices-7.4.3/pcdsdevices/lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lic.py` & `pcdsdevices-7.4.3/pcdsdevices/lic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/light_control.py` & `pcdsdevices-7.4.3/pcdsdevices/light_control.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lodcm.py` & `pcdsdevices-7.4.3/pcdsdevices/lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/lxe.py` & `pcdsdevices-7.4.3/pcdsdevices/lxe.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/make_ophyd_device.py` & `pcdsdevices-7.4.3/pcdsdevices/make_ophyd_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/mirror.py` & `pcdsdevices-7.4.3/pcdsdevices/mirror.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/movablestand.py` & `pcdsdevices-7.4.3/pcdsdevices/movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/mpod.py` & `pcdsdevices-7.4.3/pcdsdevices/mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/mpod_apalis.py` & `pcdsdevices-7.4.3/pcdsdevices/mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/mps.py` & `pcdsdevices-7.4.3/pcdsdevices/mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/mrco_motion.py` & `pcdsdevices-7.4.3/pcdsdevices/mrco_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/piezo.py` & `pcdsdevices-7.4.3/pcdsdevices/piezo.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pim.py` & `pcdsdevices-7.4.3/pcdsdevices/pim.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         else:
             self._prefix_det = self.prefix_start+'CVV:01:'
 
         # Infer the zoom motor PV from the base prefix
         if prefix_zoom:
             self._prefix_zoom = prefix_zoom
         else:
-            self._prefix_zoom = self.prefix_start+'CLZ:01:'
+            self._prefix_zoom = self.prefix_start+'CLZ:01'
 
         super().__init__(prefix, name=name, **kwargs)
         self.y = self.state.motor
 
 
 class PIMWithFocus(PIM):
     """
```

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pmps.py` & `pcdsdevices-7.4.3/pcdsdevices/pmps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pneumatic.py` & `pcdsdevices-7.4.3/pcdsdevices/pneumatic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/positioner.py` & `pcdsdevices-7.4.3/pcdsdevices/positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pseudopos.py` & `pcdsdevices-7.4.3/pcdsdevices/pseudopos.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pulsepicker.py` & `pcdsdevices-7.4.3/pcdsdevices/pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pump.py` & `pcdsdevices-7.4.3/pcdsdevices/pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/pv_positioner.py` & `pcdsdevices-7.4.3/pcdsdevices/pv_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/radiation.py` & `pcdsdevices-7.4.3/pcdsdevices/radiation.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ref.py` & `pcdsdevices-7.4.3/pcdsdevices/ref.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/rs_powersupply.py` & `pcdsdevices-7.4.3/pcdsdevices/rs_powersupply.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/rtds_ebd.py` & `pcdsdevices-7.4.3/pcdsdevices/rtds_ebd.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/sample_delivery.py` & `pcdsdevices-7.4.3/pcdsdevices/sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/sensors.py` & `pcdsdevices-7.4.3/pcdsdevices/sensors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/sequencer.py` & `pcdsdevices-7.4.3/pcdsdevices/sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/signal.py` & `pcdsdevices-7.4.3/pcdsdevices/signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/sim.py` & `pcdsdevices-7.4.3/pcdsdevices/sim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/slits.py` & `pcdsdevices-7.4.3/pcdsdevices/slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/spectrometer.py` & `pcdsdevices-7.4.3/pcdsdevices/spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/state.py` & `pcdsdevices-7.4.3/pcdsdevices/state.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/stopper.py` & `pcdsdevices-7.4.3/pcdsdevices/stopper.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/sxr_test_absorber.py` & `pcdsdevices-7.4.3/pcdsdevices/sxr_test_absorber.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/targets.py` & `pcdsdevices-7.4.3/pcdsdevices/targets.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/conftest.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_analog_signals.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_attenuator.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_attenuator.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_beam_stats.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_beam_stats.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_btms.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_btms.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_ccm.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_ccm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_crix_motion.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_dc_devices.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_device.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_disconnected.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_disconnected.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_entrypoints.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_epics_motor.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_epics_motor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_gauge.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_gon.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_inout.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_interface.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_ipm.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_ipm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_jet.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_lens.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_lodcm.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_lxe.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_lxe.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_mirror.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_movablestand.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_mpod.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_mpod_apalis.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_mps.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_pim.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_pim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_pneumatic.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_pneumatic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_positioner.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_pseudopos.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_pseudopos.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_pulsepicker.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_pump.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_sample_delivery.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_sequencer.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_signal.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_slits.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_spectrometer.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_state.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_targets.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_timetool.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_utils.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_valve.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/test_variety.py` & `pcdsdevices-7.4.3/pcdsdevices/tests/test_variety.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/tests/xcslt8717_wpcalib_opa` & `pcdsdevices-7.4.3/pcdsdevices/tests/xcslt8717_wpcalib_opa`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/timetool.py` & `pcdsdevices-7.4.3/pcdsdevices/timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/type_hints.py` & `pcdsdevices-7.4.3/pcdsdevices/type_hints.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AT1K2.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AT1K2.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AT1K2.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AT1K2.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AT2L0.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AT2L0.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AT2L0.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorCalculator_filter.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorCalculator_filter.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffAxis.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffAxis.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffAxis.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffAxis.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffSlits.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/BeckhoffSlits.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/BeckhoffSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/BtpsState.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/BtpsState.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/BtpsState.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/BtpsState.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/JJSlits.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/JJSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/LCP.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/LCP.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/Leviton1.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/Leviton1.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/LightControl.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/LightControl.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/PowerSlits.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/PowerSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/PowerSlits.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/PowerSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/QminiSpectrometer.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/QminiSpectrometer.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/Setra5000.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/Setra5000.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/StatePositioner.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/StatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/StatePositioner.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/StatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-camera-summary.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-camera-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-config.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-overview.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-range-config.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-range-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-range-summary.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-range-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-dest.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-dest.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-tabs-config.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-tabs-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-tabs.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-tabs.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps-source-valves.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps-source-valves.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/btps.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/btps.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/ui/detailed_tree.ui` & `pcdsdevices-7.4.3/pcdsdevices/ui/detailed_tree.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/usb_encoder.py` & `pcdsdevices-7.4.3/pcdsdevices/usb_encoder.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/utils.py` & `pcdsdevices-7.4.3/pcdsdevices/utils.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/valve.py` & `pcdsdevices-7.4.3/pcdsdevices/valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/variety.py` & `pcdsdevices-7.4.3/pcdsdevices/variety.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/version.py` & `pcdsdevices-7.4.3/pcdsdevices/version.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices/wfs.py` & `pcdsdevices-7.4.3/pcdsdevices/wfs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pcdsdevices.egg-info/PKG-INFO` & `pcdsdevices-7.4.3/pcdsdevices.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdsdevices
-Version: 7.4.2
+Version: 7.4.3
 Summary: Ophyd Device definitions for LCLS Beamline components
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.2 Summary: Ophyd Device
+Metadata-Version: 2.1 Name: pcdsdevices Version: 7.4.3 Summary: Ophyd Device
 definitions for LCLS Beamline components Author: SLAC National Accelerator
 Laboratory License: Copyright (c) 2023, The Board of Trustees of the Leland
 Stanford Junior University, through SLAC National Accelerator Laboratory
 (subject to receipt of any required approvals from the U.S. Dept. of Energy).
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: (1) Redistributions of source code must retain the above copyright notice,
```

### Comparing `pcdsdevices-7.4.2/pcdsdevices.egg-info/SOURCES.txt` & `pcdsdevices-7.4.3/pcdsdevices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.4.2/pyproject.toml` & `pcdsdevices-7.4.3/pyproject.toml`

 * *Files identical despite different names*

