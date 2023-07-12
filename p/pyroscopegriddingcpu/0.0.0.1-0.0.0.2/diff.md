# Comparing `tmp/pyroscopegriddingcpu-0.0.0.1.tar.gz` & `tmp/pyroscopegriddingcpu-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegriddingcpu-0.0.0.1.tar", last modified: Wed Jul 12 18:37:33 2023, max compression
+gzip compressed data, was "pyroscopegriddingcpu-0.0.0.2.tar", last modified: Wed Jul 12 18:57:53 2023, max compression
```

## Comparing `pyroscopegriddingcpu-0.0.0.1.tar` & `pyroscopegriddingcpu-0.0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-07-12 18:37:33.744192 pyroscopegriddingcpu-0.0.0.1/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.1/LICENSE.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10868 2023-07-12 18:37:33.738194 pyroscopegriddingcpu-0.0.0.1/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.1/README.md
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-07-12 18:37:33.442355 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/__init__.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/fileparser.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/filter_data.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/grid_ncf.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     6323 2023-07-12 18:27:40.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/gridding.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    26374 2023-07-12 16:34:02.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/gtools.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/naming_conventions.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/sat_data_input.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/solar_zenith.py
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     5191 2023-07-12 16:34:13.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/time_conv.py
-drwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        0 2023-07-12 18:37:33.697008 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)    10868 2023-07-12 18:37:32.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/PKG-INFO
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)      650 2023-07-12 18:37:32.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/SOURCES.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)        1 2023-07-12 18:37:32.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/dependency_links.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       74 2023-07-12 18:37:32.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/entry_points.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       50 2023-07-12 18:37:32.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/requires.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       21 2023-07-12 18:37:32.000000 pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/top_level.txt
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)       38 2023-07-12 18:37:33.746193 pyroscopegriddingcpu-0.0.0.1/setup.cfg
--rwxrwxrwx   0 szhao007  (1000) szhao007  (1000)     1860 2023-07-12 16:12:33.000000 pyroscopegriddingcpu-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:53.775836 pyroscopegriddingcpu-0.0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    11069 2023-07-12 18:57:53.775836 pyroscopegriddingcpu-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:53.729003 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/
+-rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/__init__.py
+-rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/fileparser.py
+-rw-rw-rw-   0        0        0    10415 2023-07-12 16:27:48.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/filter_data.py
+-rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/grid_ncf.py
+-rw-rw-rw-   0        0        0     6323 2023-07-12 18:27:40.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gridding.py
+-rw-rw-rw-   0        0        0    26374 2023-07-12 16:34:02.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gtools.py
+-rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/naming_conventions.py
+-rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/sat_data_input.py
+-rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/solar_zenith.py
+-rw-rw-rw-   0        0        0     5191 2023-07-12 16:34:13.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/time_conv.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:57:53.760213 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 18:57:53.000000 pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 18:57:53.775836 pyroscopegriddingcpu-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1908 2023-07-12 18:42:08.000000 pyroscopegriddingcpu-0.0.0.2/setup.py
```

### Comparing `pyroscopegriddingcpu-0.0.0.1/LICENSE.txt` & `pyroscopegriddingcpu-0.0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: pyroscopegriddingcpu
-Version: 0.0.0.1
-Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
-Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
-Author: Sally Zhao, Neil Gutkin
-Author-email: zhaosally0@gmail.com
-License: MIT
-Keywords: data fusion,satellite,L2,L3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # README
 
 Author: Sally Zhao, Neil Gutkin
 
 ## Introduction and Overview
 
 It is important to monitor Earth system data for both research and scientific reasons — analysis of such data furthers understanding of the planet and better informs political, economic, and policy decisions. Thus, in an effort to aid the Making Earth System Data Records for Use in Research Environments (MEaSUREs) Program, this project developed Python code for fusing six satellite Level 2 aerosol data (three are from geostationary satellites (GEO), and other three are from low earth orbital satellites (LEO)) from Dark Target Aerosol Retrieval Algorithm. This work emulated existing IDL workflow, which was originally created with IDL (interactive data language) by the science team. Quality checking was done by comparison to Panoply results and netCDF output matching through Python. Fused datasets generated by the program allow for visualization and analysis of the global aerosol data record over specific time periods. It also aids in research and analysis as users can better manipulate and work with satellite and sensor data. By making such code, and the accompanying functionality, open source and scalable, the scientific community is granted easier access to aerosol data processing resources.
```

### Comparing `pyroscopegriddingcpu-0.0.0.1/README.md` & `pyroscopegriddingcpu-0.0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,174 +1,196 @@
-# README
-
-Author: Sally Zhao, Neil Gutkin
-
-## Introduction and Overview
-
-It is important to monitor Earth system data for both research and scientific reasons — analysis of such data furthers understanding of the planet and better informs political, economic, and policy decisions. Thus, in an effort to aid the Making Earth System Data Records for Use in Research Environments (MEaSUREs) Program, this project developed Python code for fusing six satellite Level 2 aerosol data (three are from geostationary satellites (GEO), and other three are from low earth orbital satellites (LEO)) from Dark Target Aerosol Retrieval Algorithm. This work emulated existing IDL workflow, which was originally created with IDL (interactive data language) by the science team. Quality checking was done by comparison to Panoply results and netCDF output matching through Python. Fused datasets generated by the program allow for visualization and analysis of the global aerosol data record over specific time periods. It also aids in research and analysis as users can better manipulate and work with satellite and sensor data. By making such code, and the accompanying functionality, open source and scalable, the scientific community is granted easier access to aerosol data processing resources. 
-
-## Installation
-
-Required libraries:
-1. numpy (statistics and calculations)
-2. pyhdf (process HDF files)
-3. netCDF4 (process netCDF files)
-4. pyyaml (YAML user config)
-
-
-## Inputs
-
-Supported input formats include netCDF4 and HDF file formats.
-
-## Outputs
-
-Depending on export selection, the package can create netCDF4 or geoTIFF files.
-
-## User Configuration
-
-### Command Line Input
-
-Users can manually call functions from the command line. User specifications are demarked by flags.
-
-#### Flags
-
--fn (filename): Single filename to read in.
-
--fl (filelist): Location of file that contains a list of files (and their locations) to read in.
-
--gl (geolocation variables): Geolocation variables for parsing and calculations. Default would be latitude, longitude.
-
--gp (geophysical variables): Geophysical variables for parsing and calculations (e.g. aerosol optical depth land and ocean, solar azumith, etc).
-
--gs (gridding size): Gridding size and pixel resolution level.
-
--o (output): Output location 
-
--on (output name): Output name. If there are multiple files created, output name will be the prefix and appended to time interval associated with the calculations.
-
--l (limit): Boundary box for latitude longitude (-90 90 180 180 would encompass the full Earth)
-
-
-#### Possible Commands
-
--r (read): Reads in raw data from L2 file.
-
--f (filter): Reads in raw data from L2 file and filters based on metadata.
-
--g (grid): Reads, filters, and grids single L2 file.
-
--ns (netCDF single): Reads, filters, grids single L2 file and saves output as netCDF file.
-
--nm (netCDF multiple): Reads, filters, grids single L2 file and saves output as single netCDF file regardless of time interval.
-
--nmt (netCDF multiple time): Reads, filters, grids single L2 file and saves output as single netCDF file with time interval separation as a layer dimension.
-
--ss (sensor statistics): Reads sensors and reports statistics and individual gridded data.
-
--sss (sensor statistic split): Reads sensors and reports statistics and gridded data based on satellite categorization.
-
--ssi (sensor statistic split id): Reads sensors and reports statistics and gridded data based on satellite categorization.
-
--cfg (config): Reads in YAML file and executes commands.
-
-### YAML configuration
-
-Command line input to call YAML file: 
-
-python3 gtools.py -cfg -fn "C:\LOCATION\CONFIG_FILE_NAME.yml"
-
-The command line also has the ability to use YAML file while specifying the time start and end in the command line. This way there is no need to edit the YAML file every time when run (or create a new Docker image).
-
-Command line input to call the YAML file with time start and end: 
-
-python3 gtools.py -cfgtime -fn "C:\LOCATION\CONFIG_FILE_NAME.yml" -ts 2020/01/01/00/00 -te 2020/01/01/00/30
-
-#### User specifications
-
-The YAML file also has inputs for user specifications. This includes:
-
-##### grid_settings: 
-- gridsize (pixel resolution size)
-- limit (rectangular boundaries for gridding - default: [-89.875, 89.875, -179.875, 179.875])
-- fill_value (fill value for areas with no calculations or data)
-- time_start (start of gridding time)
-- time_end (end of gridding time)
-
-##### variables: (variables to take from input files)
-- geo_var (i.e. latitude, longitude)
-- phy_var (geophysical variables)
-- phy_var_nc (naming for geophysical variables in netCDF files (e.g. ABI_G16, ABI_G17, etc))
-- phy_var_hdf (naming for geophysical variables in HDF files (e.g. MODIS))
-- aod_range (user settings for aod. Is overwritten)
-- pixel_range (user settings for pixel range for single gridded point)
-
-##### file_io: (file inputs and outputs)
-- file_directory_folder (Path to directory. Reads all files in subdirectories as well. Takes precedence over file_location_folder and file_location_file. )
-- file_location_folder (Path to directory folder. Only reads files in the current directory. Takes precedence over  file_location_file.)
-- file_location_file (Path to file that contains paths to individual file paths. Only reads files with paths contained in this file.)
-- output_location (Path to folder for outputs)
-- output_name (User input name. Default is overwritten. Optional "NA")
-- static_file (Path to static file where certain geophysical variable values are copied from)
-
-When reading a directory with subdirectories (e.g. LAADS archive), input path to the top directory in file_directory_folder. This would then read all files contained in subdirectories. 
-
-When creating a text file with paths to files, input path to this text file in file_directory_file. 
-Paths should be included: 
-C:\LOCATION\SATELLITE1.nc
-C:\LOCATION\SATELLITE2.hdf
-
-#### YAML file format
-
-![image.png](attachment:04ae5dab-4462-4faf-9a80-a1a1879bda71.png)
-
-## Docker
-
-The repository includes a Dockerfile, which was used to a build a Docker image for the package, which is available here: https://hub.docker.com/repository/docker/neilgutkin/aerosol-data-fusion/general.
-
-A Docker image is essentially a blueprint for the creation of a Docker container. A container run from the image is a host-isolated environment that can be used to execute the data fusion package with provided user inputs.
-
-Configuration of a YAML file is required for the package to be run with Docker. Through this configuration, the user specifies the various parameters for the package run. The template for this YAML file is available in the source directory of this repository, under the name "example_config.yml". The input, output, and static file location fields in the YAML should be set to the paths of the input and output as they appear in the container - the "file_io" section of the example config is already set up for the provided Docker image, so there is no need to change it. 
-
-The next step is setting up the file system on the host. The input file directory, output file directory, config.yml file, and static file must all be grouped into one directory on the host machine, referred to as the "ioFiles" directory in the example below. 
-
-Finally, it's time to run a container from the Docker image. This step requires the user to specify the location of the ioFiles directory that the package should use. This data will be shared between the container environment and the host, meaning that changes made in the container (e.g. by the package) will be reflected on the host. To run the container, a user can execute the following command:
-
-docker run [flags] -v "/your/host/path/to/ioFilesDirectory:/app/src/ioFiles" [image_name]:[version] python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
-
-Below is an example - note especially the appearance of the windows source path (/c/ instead of C:/):
-
-docker run -it --gpus all -v "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" aerosol-df:v0 python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
-
-If running on s4psci or a similar server environment, permissions might require that you add the :z flag to the command when linking directories. In the above example, you would replace "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" with "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles:z". After execution, the package will run and the output files directory on the host machine will be populated with the newly fused outputs. 
-
-## Example Inputs / Outputs
-
-Navigate to the gridtools folder to run commands:
-
--$ python3 gtools.py [commands] [flags] 
-
-One example of this (run the yaml config file):
-
--$ python3 gtools.py -cfg -fn "PATH/config.yml"
-
-where "-cfg" is the "config yaml" command and "-fn" is the filename flag for the proceeding path.
-
-#### Inputs
-
-Inputs can be of the form of netCDF4 or HDf4 files. Sample files can be found in the respective folder in the "SampleInputs 0000-0059 01-01-2020" folder. These files can be found on NASA LAADS DAAC:
-https://ladsweb.modaps.eosdis.nasa.gov/archive/allData/
-
-One can also request files at the NASA website (look under Atmosphere-Aerosol):
-https://ladsweb.modaps.eosdis.nasa.gov/search/
-
-#### Outputs
-
-Outputs are in the form of netCDF4 file. Sample output files can be found in the respective folder in the "SampleOutputs 0000-0059 01-01-2020" folder.
-
-Each output file is the fused statistics and grid for the input files for that time interval. If input files range between 00:00-23:59 for a single day and the time interval is 30 minutes, there will be 48 files produced (each of which is for that 30 minute time interval). These times can be changed by user preference.
-
-The output files here use the sample input files provided and grid/fuse/provide statistics for Optical_Depth_Land_And_Ocean and Solar_Azumith between the times of 00:00 - 01:00, Jan 1 2020.
-
-
-```python
-
-```
+Metadata-Version: 2.1
+Name: pyroscopegriddingcpu
+Version: 0.0.0.2
+Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
+Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
+Author: Sally Zhao, Neil Gutkin
+Author-email: zhaosally0@gmail.com
+License: MIT
+Keywords: data fusion,satellite,L2,L3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# README
+
+Author: Sally Zhao, Neil Gutkin
+
+## Introduction and Overview
+
+It is important to monitor Earth system data for both research and scientific reasons â€” analysis of such data furthers understanding of the planet and better informs political, economic, and policy decisions. Thus, in an effort to aid the Making Earth System Data Records for Use in Research Environments (MEaSUREs) Program, this project developed Python code for fusing six satellite Level 2 aerosol data (three are from geostationary satellites (GEO), and other three are from low earth orbital satellites (LEO)) from Dark Target Aerosol Retrieval Algorithm. This work emulated existing IDL workflow, which was originally created with IDL (interactive data language) by the science team. Quality checking was done by comparison to Panoply results and netCDF output matching through Python. Fused datasets generated by the program allow for visualization and analysis of the global aerosol data record over specific time periods. It also aids in research and analysis as users can better manipulate and work with satellite and sensor data. By making such code, and the accompanying functionality, open source and scalable, the scientific community is granted easier access to aerosol data processing resources. 
+
+## Installation
+
+Required libraries:
+1. numpy (statistics and calculations)
+2. pyhdf (process HDF files)
+3. netCDF4 (process netCDF files)
+4. pyyaml (YAML user config)
+
+
+## Inputs
+
+Supported input formats include netCDF4 and HDF file formats.
+
+## Outputs
+
+Depending on export selection, the package can create netCDF4 or geoTIFF files.
+
+## User Configuration
+
+### Command Line Input
+
+Users can manually call functions from the command line. User specifications are demarked by flags.
+
+#### Flags
+
+-fn (filename): Single filename to read in.
+
+-fl (filelist): Location of file that contains a list of files (and their locations) to read in.
+
+-gl (geolocation variables): Geolocation variables for parsing and calculations. Default would be latitude, longitude.
+
+-gp (geophysical variables): Geophysical variables for parsing and calculations (e.g. aerosol optical depth land and ocean, solar azumith, etc).
+
+-gs (gridding size): Gridding size and pixel resolution level.
+
+-o (output): Output location 
+
+-on (output name): Output name. If there are multiple files created, output name will be the prefix and appended to time interval associated with the calculations.
+
+-l (limit): Boundary box for latitude longitude (-90 90 180 180 would encompass the full Earth)
+
+
+#### Possible Commands
+
+-r (read): Reads in raw data from L2 file.
+
+-f (filter): Reads in raw data from L2 file and filters based on metadata.
+
+-g (grid): Reads, filters, and grids single L2 file.
+
+-ns (netCDF single): Reads, filters, grids single L2 file and saves output as netCDF file.
+
+-nm (netCDF multiple): Reads, filters, grids single L2 file and saves output as single netCDF file regardless of time interval.
+
+-nmt (netCDF multiple time): Reads, filters, grids single L2 file and saves output as single netCDF file with time interval separation as a layer dimension.
+
+-ss (sensor statistics): Reads sensors and reports statistics and individual gridded data.
+
+-sss (sensor statistic split): Reads sensors and reports statistics and gridded data based on satellite categorization.
+
+-ssi (sensor statistic split id): Reads sensors and reports statistics and gridded data based on satellite categorization.
+
+-cfg (config): Reads in YAML file and executes commands.
+
+### YAML configuration
+
+Command line input to call YAML file: 
+
+python3 gtools.py -cfg -fn "C:\LOCATION\CONFIG_FILE_NAME.yml"
+
+The command line also has the ability to use YAML file while specifying the time start and end in the command line. This way there is no need to edit the YAML file every time when run (or create a new Docker image).
+
+Command line input to call the YAML file with time start and end: 
+
+python3 gtools.py -cfgtime -fn "C:\LOCATION\CONFIG_FILE_NAME.yml" -ts 2020/01/01/00/00 -te 2020/01/01/00/30
+
+#### User specifications
+
+The YAML file also has inputs for user specifications. This includes:
+
+##### grid_settings: 
+- gridsize (pixel resolution size)
+- limit (rectangular boundaries for gridding - default: [-89.875, 89.875, -179.875, 179.875])
+- fill_value (fill value for areas with no calculations or data)
+- time_start (start of gridding time)
+- time_end (end of gridding time)
+
+##### variables: (variables to take from input files)
+- geo_var (i.e. latitude, longitude)
+- phy_var (geophysical variables)
+- phy_var_nc (naming for geophysical variables in netCDF files (e.g. ABI_G16, ABI_G17, etc))
+- phy_var_hdf (naming for geophysical variables in HDF files (e.g. MODIS))
+- aod_range (user settings for aod. Is overwritten)
+- pixel_range (user settings for pixel range for single gridded point)
+
+##### file_io: (file inputs and outputs)
+- file_directory_folder (Path to directory. Reads all files in subdirectories as well. Takes precedence over file_location_folder and file_location_file. )
+- file_location_folder (Path to directory folder. Only reads files in the current directory. Takes precedence over  file_location_file.)
+- file_location_file (Path to file that contains paths to individual file paths. Only reads files with paths contained in this file.)
+- output_location (Path to folder for outputs)
+- output_name (User input name. Default is overwritten. Optional "NA")
+- static_file (Path to static file where certain geophysical variable values are copied from)
+
+When reading a directory with subdirectories (e.g. LAADS archive), input path to the top directory in file_directory_folder. This would then read all files contained in subdirectories. 
+
+When creating a text file with paths to files, input path to this text file in file_directory_file. 
+Paths should be included: 
+C:\LOCATION\SATELLITE1.nc
+C:\LOCATION\SATELLITE2.hdf
+
+#### YAML file format
+
+![image.png](attachment:04ae5dab-4462-4faf-9a80-a1a1879bda71.png)
+
+## Docker
+
+The repository includes a Dockerfile, which was used to a build a Docker image for the package, which is available here: https://hub.docker.com/repository/docker/neilgutkin/aerosol-data-fusion/general.
+
+A Docker image is essentially a blueprint for the creation of a Docker container. A container run from the image is a host-isolated environment that can be used to execute the data fusion package with provided user inputs.
+
+Configuration of a YAML file is required for the package to be run with Docker. Through this configuration, the user specifies the various parameters for the package run. The template for this YAML file is available in the source directory of this repository, under the name "example_config.yml". The input, output, and static file location fields in the YAML should be set to the paths of the input and output as they appear in the container - the "file_io" section of the example config is already set up for the provided Docker image, so there is no need to change it. 
+
+The next step is setting up the file system on the host. The input file directory, output file directory, config.yml file, and static file must all be grouped into one directory on the host machine, referred to as the "ioFiles" directory in the example below. 
+
+Finally, it's time to run a container from the Docker image. This step requires the user to specify the location of the ioFiles directory that the package should use. This data will be shared between the container environment and the host, meaning that changes made in the container (e.g. by the package) will be reflected on the host. To run the container, a user can execute the following command:
+
+docker run [flags] -v "/your/host/path/to/ioFilesDirectory:/app/src/ioFiles" [image_name]:[version] python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
+
+Below is an example - note especially the appearance of the windows source path (/c/ instead of C:/):
+
+docker run -it --gpus all -v "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" aerosol-df:v0 python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
+
+If running on s4psci or a similar server environment, permissions might require that you add the :z flag to the command when linking directories. In the above example, you would replace "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" with "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles:z". After execution, the package will run and the output files directory on the host machine will be populated with the newly fused outputs. 
+
+## Example Inputs / Outputs
+
+Navigate to the gridtools folder to run commands:
+
+-$ python3 gtools.py [commands] [flags] 
+
+One example of this (run the yaml config file):
+
+-$ python3 gtools.py -cfg -fn "PATH/config.yml"
+
+where "-cfg" is the "config yaml" command and "-fn" is the filename flag for the proceeding path.
+
+#### Inputs
+
+Inputs can be of the form of netCDF4 or HDf4 files. Sample files can be found in the respective folder in the "SampleInputs 0000-0059 01-01-2020" folder. These files can be found on NASA LAADS DAAC:
+https://ladsweb.modaps.eosdis.nasa.gov/archive/allData/
+
+One can also request files at the NASA website (look under Atmosphere-Aerosol):
+https://ladsweb.modaps.eosdis.nasa.gov/search/
+
+#### Outputs
+
+Outputs are in the form of netCDF4 file. Sample output files can be found in the respective folder in the "SampleOutputs 0000-0059 01-01-2020" folder.
+
+Each output file is the fused statistics and grid for the input files for that time interval. If input files range between 00:00-23:59 for a single day and the time interval is 30 minutes, there will be 48 files produced (each of which is for that 30 minute time interval). These times can be changed by user preference.
+
+The output files here use the sample input files provided and grid/fuse/provide statistics for Optical_Depth_Land_And_Ocean and Solar_Azumith between the times of 00:00 - 01:00, Jan 1 2020.
+
+
+```python
+
+```
```

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/fileparser.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/filter_data.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/filter_data.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/grid_ncf.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/grid_ncf.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/gridding.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/gtools.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/naming_conventions.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/sat_data_input.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/solar_zenith.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu/time_conv.py` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-Metadata-Version: 2.1
-Name: pyroscopegriddingcpu
-Version: 0.0.0.1
-Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
-Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
-Author: Sally Zhao, Neil Gutkin
-Author-email: zhaosally0@gmail.com
-License: MIT
-Keywords: data fusion,satellite,L2,L3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# README
-
-Author: Sally Zhao, Neil Gutkin
-
-## Introduction and Overview
-
-It is important to monitor Earth system data for both research and scientific reasons — analysis of such data furthers understanding of the planet and better informs political, economic, and policy decisions. Thus, in an effort to aid the Making Earth System Data Records for Use in Research Environments (MEaSUREs) Program, this project developed Python code for fusing six satellite Level 2 aerosol data (three are from geostationary satellites (GEO), and other three are from low earth orbital satellites (LEO)) from Dark Target Aerosol Retrieval Algorithm. This work emulated existing IDL workflow, which was originally created with IDL (interactive data language) by the science team. Quality checking was done by comparison to Panoply results and netCDF output matching through Python. Fused datasets generated by the program allow for visualization and analysis of the global aerosol data record over specific time periods. It also aids in research and analysis as users can better manipulate and work with satellite and sensor data. By making such code, and the accompanying functionality, open source and scalable, the scientific community is granted easier access to aerosol data processing resources. 
-
-## Installation
-
-Required libraries:
-1. numpy (statistics and calculations)
-2. pyhdf (process HDF files)
-3. netCDF4 (process netCDF files)
-4. pyyaml (YAML user config)
-
-
-## Inputs
-
-Supported input formats include netCDF4 and HDF file formats.
-
-## Outputs
-
-Depending on export selection, the package can create netCDF4 or geoTIFF files.
-
-## User Configuration
-
-### Command Line Input
-
-Users can manually call functions from the command line. User specifications are demarked by flags.
-
-#### Flags
-
--fn (filename): Single filename to read in.
-
--fl (filelist): Location of file that contains a list of files (and their locations) to read in.
-
--gl (geolocation variables): Geolocation variables for parsing and calculations. Default would be latitude, longitude.
-
--gp (geophysical variables): Geophysical variables for parsing and calculations (e.g. aerosol optical depth land and ocean, solar azumith, etc).
-
--gs (gridding size): Gridding size and pixel resolution level.
-
--o (output): Output location 
-
--on (output name): Output name. If there are multiple files created, output name will be the prefix and appended to time interval associated with the calculations.
-
--l (limit): Boundary box for latitude longitude (-90 90 180 180 would encompass the full Earth)
-
-
-#### Possible Commands
-
--r (read): Reads in raw data from L2 file.
-
--f (filter): Reads in raw data from L2 file and filters based on metadata.
-
--g (grid): Reads, filters, and grids single L2 file.
-
--ns (netCDF single): Reads, filters, grids single L2 file and saves output as netCDF file.
-
--nm (netCDF multiple): Reads, filters, grids single L2 file and saves output as single netCDF file regardless of time interval.
-
--nmt (netCDF multiple time): Reads, filters, grids single L2 file and saves output as single netCDF file with time interval separation as a layer dimension.
-
--ss (sensor statistics): Reads sensors and reports statistics and individual gridded data.
-
--sss (sensor statistic split): Reads sensors and reports statistics and gridded data based on satellite categorization.
-
--ssi (sensor statistic split id): Reads sensors and reports statistics and gridded data based on satellite categorization.
-
--cfg (config): Reads in YAML file and executes commands.
-
-### YAML configuration
-
-Command line input to call YAML file: 
-
-python3 gtools.py -cfg -fn "C:\LOCATION\CONFIG_FILE_NAME.yml"
-
-The command line also has the ability to use YAML file while specifying the time start and end in the command line. This way there is no need to edit the YAML file every time when run (or create a new Docker image).
-
-Command line input to call the YAML file with time start and end: 
-
-python3 gtools.py -cfgtime -fn "C:\LOCATION\CONFIG_FILE_NAME.yml" -ts 2020/01/01/00/00 -te 2020/01/01/00/30
-
-#### User specifications
-
-The YAML file also has inputs for user specifications. This includes:
-
-##### grid_settings: 
-- gridsize (pixel resolution size)
-- limit (rectangular boundaries for gridding - default: [-89.875, 89.875, -179.875, 179.875])
-- fill_value (fill value for areas with no calculations or data)
-- time_start (start of gridding time)
-- time_end (end of gridding time)
-
-##### variables: (variables to take from input files)
-- geo_var (i.e. latitude, longitude)
-- phy_var (geophysical variables)
-- phy_var_nc (naming for geophysical variables in netCDF files (e.g. ABI_G16, ABI_G17, etc))
-- phy_var_hdf (naming for geophysical variables in HDF files (e.g. MODIS))
-- aod_range (user settings for aod. Is overwritten)
-- pixel_range (user settings for pixel range for single gridded point)
-
-##### file_io: (file inputs and outputs)
-- file_directory_folder (Path to directory. Reads all files in subdirectories as well. Takes precedence over file_location_folder and file_location_file. )
-- file_location_folder (Path to directory folder. Only reads files in the current directory. Takes precedence over  file_location_file.)
-- file_location_file (Path to file that contains paths to individual file paths. Only reads files with paths contained in this file.)
-- output_location (Path to folder for outputs)
-- output_name (User input name. Default is overwritten. Optional "NA")
-- static_file (Path to static file where certain geophysical variable values are copied from)
-
-When reading a directory with subdirectories (e.g. LAADS archive), input path to the top directory in file_directory_folder. This would then read all files contained in subdirectories. 
-
-When creating a text file with paths to files, input path to this text file in file_directory_file. 
-Paths should be included: 
-C:\LOCATION\SATELLITE1.nc
-C:\LOCATION\SATELLITE2.hdf
-
-#### YAML file format
-
-![image.png](attachment:04ae5dab-4462-4faf-9a80-a1a1879bda71.png)
-
-## Docker
-
-The repository includes a Dockerfile, which was used to a build a Docker image for the package, which is available here: https://hub.docker.com/repository/docker/neilgutkin/aerosol-data-fusion/general.
-
-A Docker image is essentially a blueprint for the creation of a Docker container. A container run from the image is a host-isolated environment that can be used to execute the data fusion package with provided user inputs.
-
-Configuration of a YAML file is required for the package to be run with Docker. Through this configuration, the user specifies the various parameters for the package run. The template for this YAML file is available in the source directory of this repository, under the name "example_config.yml". The input, output, and static file location fields in the YAML should be set to the paths of the input and output as they appear in the container - the "file_io" section of the example config is already set up for the provided Docker image, so there is no need to change it. 
-
-The next step is setting up the file system on the host. The input file directory, output file directory, config.yml file, and static file must all be grouped into one directory on the host machine, referred to as the "ioFiles" directory in the example below. 
-
-Finally, it's time to run a container from the Docker image. This step requires the user to specify the location of the ioFiles directory that the package should use. This data will be shared between the container environment and the host, meaning that changes made in the container (e.g. by the package) will be reflected on the host. To run the container, a user can execute the following command:
-
-docker run [flags] -v "/your/host/path/to/ioFilesDirectory:/app/src/ioFiles" [image_name]:[version] python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
-
-Below is an example - note especially the appearance of the windows source path (/c/ instead of C:/):
-
-docker run -it --gpus all -v "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" aerosol-df:v0 python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
-
-If running on s4psci or a similar server environment, permissions might require that you add the :z flag to the command when linking directories. In the above example, you would replace "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" with "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles:z". After execution, the package will run and the output files directory on the host machine will be populated with the newly fused outputs. 
-
-## Example Inputs / Outputs
-
-Navigate to the gridtools folder to run commands:
-
--$ python3 gtools.py [commands] [flags] 
-
-One example of this (run the yaml config file):
-
--$ python3 gtools.py -cfg -fn "PATH/config.yml"
-
-where "-cfg" is the "config yaml" command and "-fn" is the filename flag for the proceeding path.
-
-#### Inputs
-
-Inputs can be of the form of netCDF4 or HDf4 files. Sample files can be found in the respective folder in the "SampleInputs 0000-0059 01-01-2020" folder. These files can be found on NASA LAADS DAAC:
-https://ladsweb.modaps.eosdis.nasa.gov/archive/allData/
-
-One can also request files at the NASA website (look under Atmosphere-Aerosol):
-https://ladsweb.modaps.eosdis.nasa.gov/search/
-
-#### Outputs
-
-Outputs are in the form of netCDF4 file. Sample output files can be found in the respective folder in the "SampleOutputs 0000-0059 01-01-2020" folder.
-
-Each output file is the fused statistics and grid for the input files for that time interval. If input files range between 00:00-23:59 for a single day and the time interval is 30 minutes, there will be 48 files produced (each of which is for that 30 minute time interval). These times can be changed by user preference.
-
-The output files here use the sample input files provided and grid/fuse/provide statistics for Optical_Depth_Land_And_Ocean and Solar_Azumith between the times of 00:00 - 01:00, Jan 1 2020.
-
-
-```python
-
-```
+Metadata-Version: 2.1
+Name: pyroscopegriddingcpu
+Version: 0.0.0.2
+Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
+Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
+Author: Sally Zhao, Neil Gutkin
+Author-email: zhaosally0@gmail.com
+License: MIT
+Keywords: data fusion,satellite,L2,L3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# README
+
+Author: Sally Zhao, Neil Gutkin
+
+## Introduction and Overview
+
+It is important to monitor Earth system data for both research and scientific reasons â€” analysis of such data furthers understanding of the planet and better informs political, economic, and policy decisions. Thus, in an effort to aid the Making Earth System Data Records for Use in Research Environments (MEaSUREs) Program, this project developed Python code for fusing six satellite Level 2 aerosol data (three are from geostationary satellites (GEO), and other three are from low earth orbital satellites (LEO)) from Dark Target Aerosol Retrieval Algorithm. This work emulated existing IDL workflow, which was originally created with IDL (interactive data language) by the science team. Quality checking was done by comparison to Panoply results and netCDF output matching through Python. Fused datasets generated by the program allow for visualization and analysis of the global aerosol data record over specific time periods. It also aids in research and analysis as users can better manipulate and work with satellite and sensor data. By making such code, and the accompanying functionality, open source and scalable, the scientific community is granted easier access to aerosol data processing resources. 
+
+## Installation
+
+Required libraries:
+1. numpy (statistics and calculations)
+2. pyhdf (process HDF files)
+3. netCDF4 (process netCDF files)
+4. pyyaml (YAML user config)
+
+
+## Inputs
+
+Supported input formats include netCDF4 and HDF file formats.
+
+## Outputs
+
+Depending on export selection, the package can create netCDF4 or geoTIFF files.
+
+## User Configuration
+
+### Command Line Input
+
+Users can manually call functions from the command line. User specifications are demarked by flags.
+
+#### Flags
+
+-fn (filename): Single filename to read in.
+
+-fl (filelist): Location of file that contains a list of files (and their locations) to read in.
+
+-gl (geolocation variables): Geolocation variables for parsing and calculations. Default would be latitude, longitude.
+
+-gp (geophysical variables): Geophysical variables for parsing and calculations (e.g. aerosol optical depth land and ocean, solar azumith, etc).
+
+-gs (gridding size): Gridding size and pixel resolution level.
+
+-o (output): Output location 
+
+-on (output name): Output name. If there are multiple files created, output name will be the prefix and appended to time interval associated with the calculations.
+
+-l (limit): Boundary box for latitude longitude (-90 90 180 180 would encompass the full Earth)
+
+
+#### Possible Commands
+
+-r (read): Reads in raw data from L2 file.
+
+-f (filter): Reads in raw data from L2 file and filters based on metadata.
+
+-g (grid): Reads, filters, and grids single L2 file.
+
+-ns (netCDF single): Reads, filters, grids single L2 file and saves output as netCDF file.
+
+-nm (netCDF multiple): Reads, filters, grids single L2 file and saves output as single netCDF file regardless of time interval.
+
+-nmt (netCDF multiple time): Reads, filters, grids single L2 file and saves output as single netCDF file with time interval separation as a layer dimension.
+
+-ss (sensor statistics): Reads sensors and reports statistics and individual gridded data.
+
+-sss (sensor statistic split): Reads sensors and reports statistics and gridded data based on satellite categorization.
+
+-ssi (sensor statistic split id): Reads sensors and reports statistics and gridded data based on satellite categorization.
+
+-cfg (config): Reads in YAML file and executes commands.
+
+### YAML configuration
+
+Command line input to call YAML file: 
+
+python3 gtools.py -cfg -fn "C:\LOCATION\CONFIG_FILE_NAME.yml"
+
+The command line also has the ability to use YAML file while specifying the time start and end in the command line. This way there is no need to edit the YAML file every time when run (or create a new Docker image).
+
+Command line input to call the YAML file with time start and end: 
+
+python3 gtools.py -cfgtime -fn "C:\LOCATION\CONFIG_FILE_NAME.yml" -ts 2020/01/01/00/00 -te 2020/01/01/00/30
+
+#### User specifications
+
+The YAML file also has inputs for user specifications. This includes:
+
+##### grid_settings: 
+- gridsize (pixel resolution size)
+- limit (rectangular boundaries for gridding - default: [-89.875, 89.875, -179.875, 179.875])
+- fill_value (fill value for areas with no calculations or data)
+- time_start (start of gridding time)
+- time_end (end of gridding time)
+
+##### variables: (variables to take from input files)
+- geo_var (i.e. latitude, longitude)
+- phy_var (geophysical variables)
+- phy_var_nc (naming for geophysical variables in netCDF files (e.g. ABI_G16, ABI_G17, etc))
+- phy_var_hdf (naming for geophysical variables in HDF files (e.g. MODIS))
+- aod_range (user settings for aod. Is overwritten)
+- pixel_range (user settings for pixel range for single gridded point)
+
+##### file_io: (file inputs and outputs)
+- file_directory_folder (Path to directory. Reads all files in subdirectories as well. Takes precedence over file_location_folder and file_location_file. )
+- file_location_folder (Path to directory folder. Only reads files in the current directory. Takes precedence over  file_location_file.)
+- file_location_file (Path to file that contains paths to individual file paths. Only reads files with paths contained in this file.)
+- output_location (Path to folder for outputs)
+- output_name (User input name. Default is overwritten. Optional "NA")
+- static_file (Path to static file where certain geophysical variable values are copied from)
+
+When reading a directory with subdirectories (e.g. LAADS archive), input path to the top directory in file_directory_folder. This would then read all files contained in subdirectories. 
+
+When creating a text file with paths to files, input path to this text file in file_directory_file. 
+Paths should be included: 
+C:\LOCATION\SATELLITE1.nc
+C:\LOCATION\SATELLITE2.hdf
+
+#### YAML file format
+
+![image.png](attachment:04ae5dab-4462-4faf-9a80-a1a1879bda71.png)
+
+## Docker
+
+The repository includes a Dockerfile, which was used to a build a Docker image for the package, which is available here: https://hub.docker.com/repository/docker/neilgutkin/aerosol-data-fusion/general.
+
+A Docker image is essentially a blueprint for the creation of a Docker container. A container run from the image is a host-isolated environment that can be used to execute the data fusion package with provided user inputs.
+
+Configuration of a YAML file is required for the package to be run with Docker. Through this configuration, the user specifies the various parameters for the package run. The template for this YAML file is available in the source directory of this repository, under the name "example_config.yml". The input, output, and static file location fields in the YAML should be set to the paths of the input and output as they appear in the container - the "file_io" section of the example config is already set up for the provided Docker image, so there is no need to change it. 
+
+The next step is setting up the file system on the host. The input file directory, output file directory, config.yml file, and static file must all be grouped into one directory on the host machine, referred to as the "ioFiles" directory in the example below. 
+
+Finally, it's time to run a container from the Docker image. This step requires the user to specify the location of the ioFiles directory that the package should use. This data will be shared between the container environment and the host, meaning that changes made in the container (e.g. by the package) will be reflected on the host. To run the container, a user can execute the following command:
+
+docker run [flags] -v "/your/host/path/to/ioFilesDirectory:/app/src/ioFiles" [image_name]:[version] python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
+
+Below is an example - note especially the appearance of the windows source path (/c/ instead of C:/):
+
+docker run -it --gpus all -v "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" aerosol-df:v0 python ./gridtools/gtools.py -cfg -fn /app/src/ioFiles/config.yml
+
+If running on s4psci or a similar server environment, permissions might require that you add the :z flag to the command when linking directories. In the above example, you would replace "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles" with "/c/Users/Neil/Desktop/Work/s23/ioFiles:/app/src/ioFiles:z". After execution, the package will run and the output files directory on the host machine will be populated with the newly fused outputs. 
+
+## Example Inputs / Outputs
+
+Navigate to the gridtools folder to run commands:
+
+-$ python3 gtools.py [commands] [flags] 
+
+One example of this (run the yaml config file):
+
+-$ python3 gtools.py -cfg -fn "PATH/config.yml"
+
+where "-cfg" is the "config yaml" command and "-fn" is the filename flag for the proceeding path.
+
+#### Inputs
+
+Inputs can be of the form of netCDF4 or HDf4 files. Sample files can be found in the respective folder in the "SampleInputs 0000-0059 01-01-2020" folder. These files can be found on NASA LAADS DAAC:
+https://ladsweb.modaps.eosdis.nasa.gov/archive/allData/
+
+One can also request files at the NASA website (look under Atmosphere-Aerosol):
+https://ladsweb.modaps.eosdis.nasa.gov/search/
+
+#### Outputs
+
+Outputs are in the form of netCDF4 file. Sample output files can be found in the respective folder in the "SampleOutputs 0000-0059 01-01-2020" folder.
+
+Each output file is the fused statistics and grid for the input files for that time interval. If input files range between 00:00-23:59 for a single day and the time interval is 30 minutes, there will be 48 files produced (each of which is for that 30 minute time interval). These times can be changed by user preference.
+
+The output files here use the sample input files provided and grid/fuse/provide statistics for Optical_Depth_Land_And_Ocean and Solar_Azumith between the times of 00:00 - 01:00, Jan 1 2020.
+
+
+```python
+
+```
```

### Comparing `pyroscopegriddingcpu-0.0.0.1/pyroscopegriddingcpu.egg-info/SOURCES.txt` & `pyroscopegriddingcpu-0.0.0.2/pyroscopegriddingcpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.1/setup.py` & `pyroscopegriddingcpu-0.0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegriddingcpu',         # Package name
     packages = ['pyroscopegriddingcpu'],   
-    version = '0.0.0.1',      # Initial version
+    version = '0.0.0.2',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository  
@@ -21,21 +21,21 @@
     #packages = find_packages(),
     entry_points ={
         'console_scripts': [
             'pyroscopegriddingcpu = pyroscopegriddingcpu.gtools:main',
         ],
     },
     install_requires=[            
-            'numpy',
-            'joblib',
-            'netCDF4',
-            'pyhdf',
-            'pyyaml',
+            'numpy ==1.23.5',
+            'joblib ==1.2.0',
+            'netCDF4 ==1.6.3',
+            'pyhdf ==0.10.5',
+            'pyyaml ==6.0',
             'argparse',
-            'pandas'
+            'pandas ==2.0.0'
         ],
     classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Developers',     
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',      #supported versions
```

