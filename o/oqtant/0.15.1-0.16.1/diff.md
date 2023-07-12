# Comparing `tmp/oqtant-0.15.1.tar.gz` & `tmp/oqtant-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-0.15.1.tar", max compression
+gzip compressed data, was "oqtant-0.16.1.tar", max compression
```

## Comparing `oqtant-0.15.1.tar` & `oqtant-0.16.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.15.1/LICENSE
--rw-r--r--   0        0        0     2470 2023-05-31 16:33:52.539128 oqtant-0.15.1/README.md
--rw-r--r--   0        0        0     8005 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/INSTALL.md
--rw-r--r--   0        0        0     4436 2023-06-09 18:32:33.704834 oqtant-0.15.1/documentation/albert_api_docs.md
--rw-r--r--   0        0        0    10904 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/job_analysis_docs.md
--rw-r--r--   0        0        0     4429 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/oqtant_api_docs.md
--rw-r--r--   0        0        0    10273 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/oqtant_client_docs.md
--rw-r--r--   0        0        0    14940 2023-06-12 13:13:09.730118 oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
--rw-r--r--   0        0        0    10097 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md
--rw-r--r--   0        0        0    14392 2023-06-09 18:24:55.746209 oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
--rw-r--r--   0        0        0     9745 2023-05-31 16:33:52.539128 oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
--rw-r--r--   0        0        0    31808 2023-06-01 20:50:58.385110 oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
--rw-r--r--   0        0        0    22140 2023-05-31 16:33:52.543128 oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.md
--rw-r--r--   0        0        0    16253 2023-06-12 13:13:09.730118 oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb
--rw-r--r--   0        0        0    11238 2023-06-09 18:34:38.592484 oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.md
--rw-r--r--   0        0        0    14224 2023-06-12 13:13:09.730118 oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb
--rw-r--r--   0        0        0     9127 2023-06-09 18:35:19.660472 oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.md
--rw-r--r--   0        0        0      452 2023-05-31 16:33:52.543128 oqtant-0.15.1/documentation/walkthroughs/walkthroughs.md
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/__init__.py
--rw-r--r--   0        0        0    21848 2023-05-25 15:03:01.160254 oqtant-0.15.1/oqtant/oqtant_client.py
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0    17813 2023-05-18 18:23:18.769901 oqtant-0.15.1/oqtant/schemas/job.py
--rw-r--r--   0        0        0      994 2023-06-07 21:25:59.477067 oqtant-0.15.1/oqtant/settings.py
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/util/__init__.py
--rw-r--r--   0        0        0     2805 2023-05-18 18:23:18.769901 oqtant-0.15.1/oqtant/util/auth.py
--rw-r--r--   0        0        0     1023 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/util/exceptions.py
--rw-r--r--   0        0        0      474 2023-05-16 16:24:46.335446 oqtant-0.15.1/oqtant/util/server.py
--rw-r--r--   0        0        0     3310 2023-06-09 18:33:02.108747 oqtant-0.15.1/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 oqtant-0.15.1/setup.py
--rw-r--r--   0        0        0     3866 1970-01-01 00:00:00.000000 oqtant-0.15.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.16.1/LICENSE
+-rw-r--r--   0        0        0     2348 2023-07-11 20:26:55.462428 oqtant-0.16.1/README.md
+-rw-r--r--   0        0        0     8565 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/INSTALL.md
+-rw-r--r--   0        0        0    10906 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/job_analysis_docs.md
+-rw-r--r--   0        0        0    10378 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/oqtant_client_docs.md
+-rw-r--r--   0        0        0     4446 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/oraqle_api_docs.md
+-rw-r--r--   0        0        0    16157 2023-07-12 13:56:47.774863 oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
+-rw-r--r--   0        0        0    11171 2023-07-12 13:57:43.766666 oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md
+-rw-r--r--   0        0        0    16533 2023-07-12 14:00:04.078167 oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
+-rw-r--r--   0        0        0    11526 2023-07-12 14:00:21.198106 oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
+-rw-r--r--   0        0        0    32239 2023-07-11 20:26:55.466428 oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
+-rw-r--r--   0        0        0    22278 2023-07-11 20:26:55.466428 oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.md
+-rw-r--r--   0        0        0    16722 2023-07-12 14:00:57.121977 oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb
+-rw-r--r--   0        0        0    11727 2023-07-12 14:01:12.225922 oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.md
+-rw-r--r--   0        0        0    14777 2023-07-12 14:01:44.589805 oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb
+-rw-r--r--   0        0        0     9606 2023-07-12 14:01:58.045757 oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.md
+-rw-r--r--   0        0        0      512 2023-07-11 20:26:55.466428 oqtant-0.16.1/documentation/walkthroughs/walkthroughs.md
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/__init__.py
+-rw-r--r--   0        0        0    21875 2023-07-11 20:26:55.466428 oqtant-0.16.1/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0    17813 2023-05-18 18:23:18.769901 oqtant-0.16.1/oqtant/schemas/job.py
+-rw-r--r--   0        0        0      508 2023-07-11 20:26:55.466428 oqtant-0.16.1/oqtant/settings.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     3323 2023-07-11 20:26:55.470428 oqtant-0.16.1/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1023 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0      474 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/util/server.py
+-rw-r--r--   0        0        0     3310 2023-07-12 14:02:05.017732 oqtant-0.16.1/pyproject.toml
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 oqtant-0.16.1/setup.py
+-rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 oqtant-0.16.1/PKG-INFO
```

### Comparing `oqtant-0.15.1/LICENSE` & `oqtant-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.1/README.md` & `oqtant-0.16.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Oqtant
 
 [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
-[![pypi](https://img.shields.io/pypi/v/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
+[![pypi](https://img.shields.io/pypi/v/oqtant.svg)](https://pypi.python.org/pypi/oqtant)
 [![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)
 
 ## 🚀 Quick Install
 
 ```python
 pip install oqtant
 ```
 
 ## 🧭 Introduction
 
 This API contains tools to:
 
-- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)
+- Access all the functionality of the Oraqle Web App (https://albert-dev.coldquanta.com)
 
   - BARRIER (Barrier Manipulator) jobs
   - BEC (Ultracold Matter) jobs
 
 - Build parameterized (i.e. optimization) experiments using OqtantJobs
 
 - Submit and retrieve OqtantJob results
@@ -47,10 +47,9 @@
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
 - [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)
 - [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)
-- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)
-- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)
+- [Oraqle API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oraqle_api_docs.md)
 - [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)
```

### Comparing `oqtant-0.15.1/documentation/INSTALL.md` & `oqtant-0.16.1/documentation/INSTALL.md`

 * *Files 15% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 - Matplotlib
 - Numpy
 - Scipy
 - Scikit-learn
 
 Below are the steps for installing Oqtant by operating system:
 
+If you are using Anaconda/Miniconda you can follow these [steps](#using-conda)
+
 ### Windows
 
 **Note: You can use either Command Prompt or PowerShell with Oqtant. The steps for each only differ slightly**
 
 1. Create a python virtual environment to install Oqtant into:
 
    ```
@@ -134,17 +136,45 @@
 
 3. Once activated run the following command to install Oqtant and it's dependencies:
 
    ```
    pip install oqtant
    ```
 
+### Using Conda
+
+If you are using Anaconda/Miniconda to manage python environments you can follow the steps below:
+
+1. Create a conda environment to install Oqtant into:
+
+   ```
+   conda create --name oqtant PYTHON=3.10
+   ```
+
+2. Activate your virtual environment:
+
+   ```
+   conda activate oqtant
+   ```
+
+3. Once activated run the following command to install Oqtant and it's dependencies:
+
+   ```
+   pip install oqtant
+   ```
+
+   If your conda environment is missing pip you can install it and run the above again:
+
+   ```
+   conda install pip
+   ```
+
 # Walkthrough Notebooks
 
-Getting started with Oqtant is easy using the walkthrough notebooks (your Oqtant installation already includes the latest version of Jupyter Notebook). These walkthroughs will walk you through the basic functions of using Oqtant to interact with the Oqtant hardware. Feel free to use these as a starting point for your own code: edit, rename, share… they are yours.
+Getting started with Oqtant is easy using the walkthrough notebooks. These walkthroughs will walk you through the basic functions of using Oqtant to interact with the Oqtant hardware. Feel free to use these as a starting point for your own code: edit, rename, share… they are yours.
 
 ## Downloading Walkthrough Notebooks
 
 You can download a copy of our walkthrough notebooks from our GitLab project located here: https://gitlab.com/infleqtion/albert/oqtant/-/tree/main/documentation
 
 ## Running Walkthrough Notebooks
 
@@ -154,22 +184,22 @@
 jupyter notebook
 ```
 
 - This will open a tab in your default web browser with a file explorer type interface.
 - Using this interface navigate to the location of the provided notebooks and select one to open.
 - This will open another tab with the contents of the selected notebook.
 - Each notebook has pre-populated examples you can then execute with instructions for each step
-- For a more detailed explanation of the Oqtant API refer to our [API Docs](oqtant_api_docs.md)
+- For a more detailed explanation of the Oraqle API refer to our [API Docs](oraqle_api_docs.md)
 
 If you run into `ModuleNotFound` errors when running cells within the notebooks it can be a sign that the notebooks are not using the correct version of python. To fix this close the notebook server, run the following, then restart the notebooks:
 
 ```
 python -m ipykernel install --user
 ```
 
 **Note: You may notice that each walkthrough notebook has two files with different extensions (.ipynb and .md). The files you want to be using with Jupyter are the .ipynb files as these are what runs the underlying Oqtant python code. The .md files are static markdown representations of the walkthrough notebooks that can be used as reference if needed. The .md files are safe to delete**
 
 ## Authentication
 
-At the top of each walkthrough notebook you will see a step called `Sign into Oqtant`. This step is required for all notebook and client operations to ensure only authorized parties are accessing Oqtant.
+At the top of each walkthrough notebook you will see a step called `Authenticate with Oraqle`. This step is required for all notebook and client operations to ensure only authorized parties are accessing Oraqle.
 
-This step will require that you already have an account created for Oqtant. If you have not done so yet visit https://albert-dev.coldquanta.com and follow the registration steps to get set up.
+This step will require that you already have an account created for Oraqle. If you have not done so yet visit https://albert-dev.coldquanta.com and follow the registration steps to get set up.
```

### Comparing `oqtant-0.15.1/documentation/albert_api_docs.md` & `oqtant-0.16.1/documentation/oraqle_api_docs.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# Albert REST API
+# Oraqle REST API
 
-The Albert REST API is the RESTful backend to both Oqtant and the Albert Web App. It's API provides endpoints that can be interacted with via Oqtant's Client API to execute and expand upon the same functionality found in the Albert Web App.
+The Oraqle REST API is the RESTful backend to both Oqtant and the Oraqle Web App. It's API provides endpoints that can be interacted with via Oqtant's Client API to execute and expand upon the same functionality found in the Oraqle Web App.
 
-To see a list of available endpoints and try them out you can visit our [OpenAPI documentation](http://albert-dev.coldquanta.com/api/v1/bert/docs)
+To see a list of available endpoints and try them out you can visit our [OpenAPI documentation](http://albert-dev.coldquanta.com/api/docs)
 
-Communication with the Albert REST API will need to be authorized via your Albert Account. To accomplish this you will need to find your authentication token and provide it when using the OpenAPI documentation. To do this you can follow the steps below:
+Communication with the Oraqle REST API will need to be authorized via your Oraqle Account. To accomplish this you will need to find your authentication token and provide it when using the OpenAPI documentation. To do this you can follow the steps below:
 
 ** Both of these methods requires that oqtant be installed on your system and in a place where your python interpreter can access it. Ideally this would be inside of a virtual environment. For more information on how to set that up refer to our [Installation Guide](INSTALL.md) **
 
 ## Authentication Token via Oqtant Notebooks
 
-When installing Oqtant for the first time you will have received a set of tutorial Jupyter notebooks. Within each of these notebooks you will find that the beginning of each one starts with a step called `Authenticate with Albert`. At the end of this step is a line that contains the following:
+When installing Oqtant for the first time you will have received a set of walkthrough Jupyter notebooks. Within each of these notebooks you will find that the beginning of each one starts with a step called `Authenticate with Oraqle`. At the end of this step is a line that contains the following:
 
 ```python
 token = get_user_token()
 ```
 
-This line is what handles the authorization process for you to begin using Oqtant and as a result the Albert REST API. To be able to use the endpoints available in our OpenAPI documentation you will need to perform the following using the aforementioned step:
+This line is what handles the authorization process for you to begin using Oqtant and as a result the Oraqle REST API. To be able to use the endpoints available in our OpenAPI documentation you will need to perform the following using the aforementioned step:
 
 1. Start up Jupyter
 
    ```shell
    jupyter notebook
    ```
 
-2. Open up one of the tutorial notebooks. Depending on the location you started Jupyter from you may need to navigate the file explorer interface of Jupyter to find them.
+2. Open up one of the walkthrough notebooks. Depending on the location you started Jupyter from you may need to navigate the file explorer interface of Jupyter to find them.
 
 3. In the code cell that contains the import statements and the `get_user_token()` method call, add a new line at the bottom that contains:
 
    ```python
    print(token)
    ```
 
-4. Run the cell in the Jupyter notebook. It will open up a new tab in your default browser where you will be prompted to log in with your Albert Account. Once logged in successfully you can close that tab and return to the Jupyter notebook.
+4. Run the cell in the Jupyter notebook. It will open up a new tab in your default browser where you will be prompted to log in with your Oraqle Account. Once logged in successfully you can close that tab and return to the Jupyter notebook.
 
 5. Now that you are authenticated you can see in the output of the code cell the printed authentication token. Select it all and copy it to your clipboard. This is your token.
 
 ## Authentication Token via Pure Python
 
-While Oqtant comes with a set of tutorial Jupyter notebooks, at its core it is a python library and can be used on its own. To be able to use the endpoint available in our OpenAPI documentation you will need to perform the following inside of a python interpreter:
+While a set of walkthrough Jupyter notebooks is provided to be used with Oqtant, at its core it is a python library and can be used on its own. To be able to use the endpoint available in our OpenAPI documentation you will need to perform the following inside of a python interpreter:
 
 1. Inside of a terminal with `oqtant` available open a python interpreter by running `python`
 
 2. Import the `get_user_token`method
 
    ```python
    from oqtant.util.auth import get_user_token
@@ -50,30 +50,30 @@
 
 3. Call the imported method and assign the result to a variable
 
    ```python
    token = get_user_token()
    ```
 
-4. A new tab in your default browser will open where you will be prompted to log in with your Albert Account. Once logged in successfully you can close that tab and return to your python interpreter.
+4. A new tab in your default browser will open where you will be prompted to log in with your Oraqle Account. Once logged in successfully you can close that tab and return to your python interpreter.
 
 5. Print the contents of the variable
 
    ```python
    print(token)
    ```
 
 6. Select all of the output from the printed variable and copy it to your clipboard. This is your token.
 
 ## Authorizing OpenAPI Documentation
 
-Now that you have your authentication token from one of the previous methods you can authorize the OpenAPI documentation to allow for interaction with the Albert REST API endpoints. To do this follow the below steps:
+Now that you have your authentication token from one of the previous methods you can authorize the OpenAPI documentation to allow for interaction with the Oraqle REST API endpoints. To do this follow the below steps:
 
-1. Navigate to our [OpenAPI documentation](https://albert-dev.coldquanta.com/api/v1/bert/docs)
+1. Navigate to our [OpenAPI documentation](https://albert-dev.coldquanta.com/api/docs)
 
-2. Once loaded you will see a list of the endpoints provided by the Albert REST API. Most of these will show a lock icon next to them on the right-hand side. Endpoints with a lock will require the authentication token we retrieved from the above methods.
+2. Once loaded you will see a list of the endpoints provided by the Oraqle REST API. Most of these will show a lock icon next to them on the right-hand side. Endpoints with a lock will require the authentication token we retrieved from the above methods.
 
 3. Near the top right-hand side of the page you will see a green button with the text `Authorize`. Clicking on this will open a pop-up with a form to input `HTTPBearer`inside.
 
 4. Paste the token from our clipboard into this field and click `Authorize`.
 
 5. You should now see a message that says `Authorized`. You can close the pop-up and begin using the endpoints that require an authentication token.
```

### Comparing `oqtant-0.15.1/documentation/job_analysis_docs.md` & `oqtant-0.16.1/documentation/job_analysis_docs.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 ## Capabilities
 
 - Contains job inputs and outputs (if they exist) as well as information about the user, hardware, and submission time.
 - Analysis functions for TOF images and some convenient output/plotting utilities
 
 ## How the BEC Job Analysis Library works
 
-1. A OqtantJob is a container object for inputs and results generated by the Oqtant system.
+1. A OqtantJob is a container object for inputs and results generated by the Oraqle system.
    The OqtantJob object has a variety of common utility functions for processing results.
 
 2. Within a Oqtant session, OqtantJob objects are created and stored in active_jobs.
    These jobs are available until the python session ends. All jobs are tracked by their id,
    which is issued at the time of job submit.
 
 3. To handle job results from a previous session, load them into active_jobs with
    load_job_from_id() or load_job_from_file(). This will create the OqtantJob object(s).
 
-4. Each OqtantJob object has a status assigned by the Oqtant hardware:
+4. Each OqtantJob object has a status assigned by the Oraqle hardware:
    - Pending - This job has not run yet. No results available
    - Running - This job is being evaluated. Run time is 1 minute.
    - Complete - This job has run successfully and results are available.
    - Failed - This job has failed. This can occur due to inappropriate input parameters or
      hardware outages. Contact **albert@infleqtion.com** for support
 
 ## Helper functions
@@ -118,15 +118,15 @@
     :type yc: float - Cloud center along the y-direction
 
     :param os:
     :type os: float - Constant offset
 
     returns array sampled OD, sum of 2d gaussian distribution and TF distribution. flattened to 1D
 
-## BEC_job class
+## OqtantJob class
 
 This is a container class for an Oqtant job in any state
 
 A OqtantJob object contains job parameters and results (if they have been generated).
 The OqtantJob class contains analysis functions to apply to TOF images.
 
 ### init
```

### Comparing `oqtant-0.15.1/documentation/oqtant_client_docs.md` & `oqtant-0.16.1/documentation/oqtant_client_docs.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Oqtant Client
 
 ## Capabilities
 
-- Access all the functionality of the Oqtant Web App (https://albert-dev.coldquanta.com)
+- Access all the functionality of the Oraqle Web App (https://albert-dev.coldquanta.com)
 
   - BARRIER (Barrier Manipulator) jobs
   - BEC (Ultracold Matter) jobs
 
 - Build parameterized (i.e. optimization) experiments using OqtantJobs
 
 - Submit and retrieve OqtantJob results
@@ -30,59 +30,61 @@
 
   - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()
 
 - To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.
 
 ## Considerations
 
-- Oqtant cannot interact with jobs that have been deleted via the Oqtant Web App
+- Oqtant cannot interact with jobs that have been deleted via the Oraqle Web App
 
-- Job results and limits are restricted to the account used to authenticate the Oqtant client
+- Job results and limits are restricted to the Oraqle account used to authenticate the Oqtant client
 
 - All jobs that have been submitted will be processed even if the Oqtant client session is ended before they complete
 
 ## Oqtant API
 
-The Oqtant API provides everything you need to get started working with OqtantJobs and the Oqtant REST API. For more information regarding the Oqtant REST API refer to our [Oqtant REST API Docs](albert_api_docs.md)
+The Oqtant API provides everything you need to get started working with OqtantJobs and the Oraqle REST API. For more information regarding the Oraqle REST API refer to our [Oraqle REST API Docs](oraqle_api_docs.md)
 
 ### get_user_token
 
-A utility function required for getting Oqtant authenticated with your Oqtant account. Starts up a server to handle the Auth0 authentication process and acquire a token. This helper function is located in `oqtant.util.auth`
+A utility function required for getting Oqtant authenticated with your Oraqle account. Starts up a server to handle the Auth0 authentication process and acquire a token. This helper function is located in `oqtant.util.auth`
 
 ```
+Args:
+    auth_server_port (int): optional port to run the authentication server on
 Returns:
     str: Auth0 user token
 ```
 
 ### get_oqtant_client
 
 A utility function to create a new OqtantClient instance. This helper method requires the token returned from `oqtant.util.auth.get_user_token` and is located in `oqtant.oqtant_client`
 
 ```
 Args:
-    token (str): the auth0 token required for interacting with the REST API
+    token (str): the auth0 token required for interacting with the Oraqle REST API
 Returns:
     OqtantClient: authenticated instance of OqtantClient
 ```
 
 ### get_job
 
-Gets an OqtantJob from the Oqtant REST API. This will always be a targeted query for a specific run. If the run is omitted then this will always return the first run of the job. Will return results for any job regardless of it's status. This function is a member of `OqtantClient`
+Gets an OqtantJob from the Oraqle REST API. This will always be a targeted query for a specific run. If the run is omitted then this will always return the first run of the job. Will return results for any job regardless of it's status. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id (str): this is the external_id of the job to fetch
     run (int): the run to target, this defaults to the first run if omitted
 Returns:
     OqtantJob: an OqtantJob instance with the values of the job queried
 ```
 
 ### get_job_inputs_without_output
 
-Gets an OqtantJob from the Oqtant REST API. This can return all runs within a job or a single run based on whether a run value is provided. The OqtantJobs returned will be converted to dictionaries and will not have any output data, even if they are complete. This is useful for taking an existing job and creating a new one based on it's input data. This function is a member of `OqtantClient`
+Gets an OqtantJob from the Oraqle REST API. This can return all runs within a job or a single run based on whether a run value is provided. The OqtantJobs returned will be converted to dictionaries and will not have any output data, even if they are complete. This is useful for taking an existing job and creating a new one based on it's input data. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id (str): this is the external_id of the job to fetch
     run (Union[int, None]): optional argument if caller wishes to only has a single run returned
     include_notes (bool): optional argument if caller wishes to include any notes associated with OqtantJob inputs. Defaults to False is not provided
 Returns:
@@ -98,94 +100,94 @@
     job (Dict): dictionary containing job details and input
 Returns:
     OqtantJob: an OqtantJob instance containing the details and input from the provided dictionary
 ```
 
 ### submit_job
 
-Submits a single OqtantJob to the Oqtant REST API. Upon successful submission this function will return a dictionary containing the external_id of the job and it's position in the queue. This function is a member of `OqtantClient`
+Submits a single OqtantJob to the Oraqle REST API. Upon successful submission this function will return a dictionary containing the external_id of the job and it's position in the queue. This function is a member of `OqtantClient`
 
 ```
 Args:
     job (OqtantJob): the OqtantJob instance to submit for processing
 Returns:
     Dict: dictionary containing the external_id of the job and it's queue position
 ```
 
 ### run_jobs
 
-Submits a list of OqtantJobs to the Oqtant REST API. This function provides some optional functionality to alter how it behaves. Providing it with an argument of track_status=True will make it wait and poll the Oqtant REST API until all jobs in the list have completed. The track_status functionality outputs each jobs current status as it is polling and opens up the ability to use the other optional arguments write and filename. The write and filename arguments enable the ability to have the results of each completed job written to a file. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If running more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
+Submits a list of OqtantJobs to the Oraqle REST API. This function provides some optional functionality to alter how it behaves. Providing it with an argument of track_status=True will make it wait and poll the Oraqle REST API until all jobs in the list have completed. The track_status functionality outputs each jobs current status as it is polling and opens up the ability to use the other optional arguments write and filename. The write and filename arguments enable the ability to have the results of each completed job written to a file. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If running more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_list (List[OqtantJob]): the list of OqtantJob instances to submit for processing
     track_status (bool): optional argument to tell this function to either return immediately or wait and poll until all jobs have completed
     write (bool): optional argument to tell this function to write the results of each job to file when complete
     filename (Union[str, List[str]]): optional argument to be used in conjunction with the write argument. allows the caller to customize the name(s) of the files being created
 Returns:
     List[str]: list of the external_id(s) returned for each submitted job in job_list
 ```
 
 ### search_jobs
 
-Submits a query to the REST API to search for jobs that match the provided criteria. The search results will be limited to jobs that meet your Oqtant account access. This function is a member of `OqtantClient`
+Submits a query to the Oraqle REST API to search for jobs that match the provided criteria. The search results will be limited to jobs that meet your Oraqle account access. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_type (JobSchema.JobType): the type of the jobs to search for
     name (JobSchema.JobName): the name of the job to search for
     submit_start (str): the earliest submit date of the jobs to search for
     submit_start (str): the latest submit date of the jobs to search for
     notes (str): the notes of the jobs to search for
 Returns:
     List[Dict]: a list of jobs matching the provided search criteria
 ```
 
 ### track_jobs
 
-Polls the Oqtant REST API with a list of job external_ids and waits until all of them have completed. Will output each job's status while it is polling and will output a message when all jobs have completed. This function provides some optional functionality to alter how it behaves. Providing it with an argument of write will have it write the results of each completed job to a file. There is an additional argument that can be used with write called filename. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If tracking more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
+Polls the Oraqle REST API with a list of job external_ids and waits until all of them have completed. Will output each job's status while it is polling and will output a message when all jobs have completed. This function provides some optional functionality to alter how it behaves. Providing it with an argument of write will have it write the results of each completed job to a file. There is an additional argument that can be used with write called filename. The value of filename is optional and if not provided will cause the files to be created using the external_id of each job. If tracking more than one job and using the filename argument it is required that the number of jobs in job_list match the number of values in filename. This function is a member of `OqtantClient`
 
 ```
 Args:
     pending_jobs (List[str]): list of job external_ids to track
     write (bool): optional argument to tell this function to write the results of each job to file when complete
     filename (Union[str, List[str]]): optional argument to be used in conjunction with the write argument. allows the caller to customize the name(s) of the files being created
 ```
 
 ### load_job_from_id_list
 
-Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list of job external_ids. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
+Loads OqtantJobs from the Oraqle REST API into the current active_jobs list using a list of job external_ids. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id_list (List[str]): list of job external_ids to load
 ```
 
 ### load_job_from_id
 
-Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a job external_id. The results of the jobs loaded by this function can be targeted to a specific run if there are multiple. This function is a member of `OqtantClient`
+Loads an OqtantJob from the Oraqle REST API into the current active_jobs list using a job external_id. The results of the jobs loaded by this function can be targeted to a specific run if there are multiple. This function is a member of `OqtantClient`
 
 ```
 Args:
     job_id (str): the external_id of the job to load
     run (int): optional argument to target a specific job run
 ```
 
 ### load_job_from_file_list
 
-Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list of filenames containing OqtantJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
+Loads OqtantJobs from the Oraqle REST API into the current active_jobs list using a list of filenames containing OqtantJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
 
 ```
 Args:
     file_list (List[str]): list of filenames containing OqtantJob information
 ```
 
 ### load_job_from_file
 
-Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a file containing OqtantJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
+Loads an OqtantJob from the Oraqle REST API into the current active_jobs list using a file containing OqtantJob info. The results of the jobs loaded by this function are limited to their first run. This function is a member of `OqtantClient`
 
 ```
 Args:
     file_list (List[str]): list of filenames containing OqtantJob information
 ```
 
 ### see_active_jobs
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9381060557140853%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 2: Barrier Manipulator #\\n'), (2, "*

 * *            "'### This walkthrough covers authorizing an Oraqle session using the OqtantClient, "*

 * *            'generating, running and viewing the results of a Barrier Manipulator OqtantJob. '*

 * *            "###\\n'), (6, '*Batch job functionality is available for users with a subscription "*

 * *            "tier of EXPLORER or INNOVATOR.*\\n'), (7, '\\n'), (8, '`get_user_token` creates a "*

 * *            'temporary  […]*

```diff
@@ -1,29 +1,31 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Walkthrough 1: Getting Started #\n",
+                "# Oqtant Walkthrough 2: Barrier Manipulator #\n",
                 "\n",
-                "### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
+                "### This walkthrough covers authorizing an Oraqle session using the OqtantClient, generating, running and viewing the results of a Barrier Manipulator OqtantJob. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
                 "\n",
-                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
+                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*\n",
+                "\n",
+                "`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Authenticate with Oqtant\n",
+                "# Authenticate with Oraqle\n",
                 "\n",
-                "## Before you can view and submit jobs you must first authenticate with your Oqtant account\n",
+                "## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account\n",
                 "\n",
                 "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -40,26 +42,26 @@
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
                 "\n",
-                "token = get_user_token()"
+                "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Creating a Oqtant Client Instance ##\n",
+                "## Creating a OqtantClient Instance ##\n",
                 "\n",
-                "### After successful login, create an authorized session with the Oqtant Client ###\n",
-                "- the oqtant_client interacts with the albert server to perform remote lab functions.\n",
-                "- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session"
+                "### After successfully logging in, create an authorized session with the OqtantClient ###\n",
+                "- The OqtantClient interacts with the Oraqle server to perform remote lab functions. \n",
+                "- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -67,144 +69,166 @@
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Generate parameters to create a job ##\n",
-                "Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:"
+                "## Generate parameters to create an OqtantJob ##\n",
+                "Every OqtantJob is specified by a name, job_type, and a dictionary of input parameters. Below is an example with default parameters for a Barrier Manipulator OqtantJob:\n",
+                "\n",
+                "*Ultracold Matter and Barrier Manipulator jobs are represented as OqtantJob objects with different `job_type` fields*\n",
+                "\n",
+                " - Ultracold Matter: `BEC`\n",
+                " - Barrier Manipulator: `BARRIER`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "default_bec_job = {\n",
-                "    \"name\": \"Example Ultracold Matter Generator Job\",\n",
-                "    \"job_type\": \"BEC\",\n",
+                "barrier_manipulator_job = {\n",
+                "    \"name\": \"Example Barrier Manipulator Job\",\n",
+                "    \"job_type\": \"BARRIER\",\n",
                 "    \"inputs\": [\n",
                 "        {\n",
                 "            \"values\": {\n",
-                "                \"time_of_flight_ms\": 8.0,\n",
-                "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
-                "                \"end_time_ms\": 0.0,\n",
+                "                \"time_of_flight_ms\": 7.0,\n",
+                "                \"image_type\": \"IN_TRAP\",\n",
+                "                \"end_time_ms\": 20.0,\n",
                 "                \"rf_evaporation\": {\n",
-                "                    \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.045],\n",
                 "                    \"powers_mw\": [500.0, 500.0, 475.0, 360.0, 220.0],\n",
+                "                    \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.1],\n",
                 "                    \"interpolation\": \"LINEAR\",\n",
                 "                    \"times_ms\": [-1600, -1200, -800, -400, 0],\n",
                 "                },\n",
-                "                \"optical_barriers\": None,\n",
+                "                \"optical_barriers\": [\n",
+                "                    {\n",
+                "                        \"heights_khz\": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 25.0, 25.0, 25.0, 25.0, 25.0],\n",
+                "                        \"positions_um\": [-10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0],\n",
+                "                        \"interpolation\": \"OFF\",\n",
+                "                        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
+                "                        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
+                "                        \"shape\": \"GAUSSIAN\",\n",
+                "                    },\n",
+                "                    {\n",
+                "                        \"heights_khz\": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 40.0, 40.0],\n",
+                "                        \"positions_um\": [10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0],\n",
+                "                        \"interpolation\": \"OFF\",\n",
+                "                        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
+                "                        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
+                "                        \"shape\": \"GAUSSIAN\",\n",
+                "                    },\n",
+                "                ],\n",
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
-                "            },\n",
-                "        }\n",
+                "            }\n",
+                "        },\n",
                 "    ],\n",
                 "}\n",
                 "\n",
-                "example_bec_job = oqtant_client.generate_oqtant_job(job=default_bec_job)\n",
-                "print(example_bec_job)"
+                "barrier_manipulator_job = oqtant_client.generate_oqtant_job(job=barrier_manipulator_job)\n",
+                "print(barrier_manipulator_job)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Add notes to your job input (Optional) ##\n",
-                "Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
+                "## Add notes to your OqtantJob input (Optional) ##\n",
+                "Every OqtantJob input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# In this example we are only working with a single input\n",
                 "# so we will add the note to the first and only input in the array\n",
-                "example_bec_job.inputs[0].notes = \"This is an example BEC job created from Oqtant walkthrough #1\""
+                "barrier_manipulator_job.inputs[0].notes = \"This is an Ultracold Matter job created from Oqtant walkthrough #1\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Submit the job to run on the Oqtant hardware ##\n",
+                "## Submit the OqtantJob to run on the Oraqle hardware ##\n",
                 "\n",
-                "**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.\n",
+                "`OqtantClient.run_jobs()` takes a list of OqtantJob objects, `job_list=[*OqtantJob]` and submits them to the online queue. For each OqtantJob added to the queue a unique UUID is generated and associated to it.\n",
                 "\n",
-                "The output of **run_jobs()** is a list of the unique UUIDs generated during submission. \n",
+                "The output of `OqtantClient.run_jobs()` is a list of the unique UUIDs generated during submission. \n",
                 "\n",
-                "If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.\n",
+                "If you are submitting a list of OqtantJobs and wish to wait for the results to return, use the flag `track_status=True`.\n",
                 "\n",
                 "If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:\n",
                 "\n",
-                "- **track_status=True**\n",
-                "- **filename=\"name_of_file\"**\n",
-                "- **write=True**\n",
+                "- `track_status=True`\n",
+                "- `filename=\"name_of_file\"`\n",
+                "- `write=True`\n",
                 "\n",
                 "When writing to a file be sure to <span style=\"color:red\">not overwrite it</span>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "[example_bec_job_uuid] = oqtant_client.run_jobs(job_list=[example_bec_job], track_status=True)"
+                "[barrier_manipulator_job_uuid] = oqtant_client.run_jobs(job_list=[barrier_manipulator_job], track_status=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Best practices for referencing ##"
+                "## Best practices for referencing ##\n",
+                "\n",
+                "To easily reference OqtantJobs from the current or previous sessions it is useful to write their ids to a file named after the job. This file can be used later to access the OqtantJob.\n",
+                "\n",
+                "In this case we are saving this OqtantJob's id under a file named after this walkthrough."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with open('example_bec_job-walkthrough0.txt', 'w') as f:\n",
-                "    f.write(example_bec_job_uuid)"
+                "with open('walkthrough_2_barrier_manipulator.txt', 'w') as f:\n",
+                "    f.write(barrier_manipulator_job_uuid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Check the status of this session's active jobs ##\n",
-                "\n",
-                "The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. \n",
-                "\n",
-                "**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. \n",
+                "## Check the status of this session's active OqtantJobs ##\n",
                 "\n",
-                "<span style=\"color:red\"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>\n",
+                "The OqtantClient object contains a dictionary (indexed by job_id) of all the active OqtantJobs from the current session. To keep inputs and results organized, all jobs are handled as objects of the OqtantJob class.\n",
                 "\n",
-                "To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. \n",
-                "\n",
-                "<span style=\"color:red\"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>\n",
+                "`OqtantClient.active jobs` contains OqtantJobs that have been submitted with `OqtantClient.run_jobs()` or loaded with either `OqtantClient.load_job_from_id()` or `OqtantClient.load_job_from_file()`. \n",
+                " \n",
+                " <span style=\"color:red\"> Note: `OqtantClient.active_jobs` does not automatically include OqtantJobs which were submitted on the Oraqle web application or in a different python session, even if those jobs are currently in the queue to run. </span>\n",
                 "\n",
                 "### To access information about a OqtantJob object ###\n",
                 "\n",
                 "**EXAMPLEJOB.DESIRED_INFO**\n",
                 "\n",
                 "OqtantJob objects have the following relevant fields:\n",
                 "\n",
-                " - name\n",
-                " - job_type\n",
-                " - status\n",
-                " - time_submit (datetime object)\n",
-                " - inputs list (see walkthrough 2 for specifics)\n",
+                " - name (str)\n",
+                " - job_type (str)\n",
+                " - status (str)\n",
+                " - time_submit (datetime)\n",
+                " - inputs (list) (see walkthrough 2 for specifics)\n",
                 "\n",
                 "To see all the job information, you can print the object. \n",
                 "\n",
                 "Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python. "
             ]
         },
         {
@@ -216,180 +240,154 @@
                 "oqtant_client.see_active_jobs()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Wait for job results ##\n",
+                "## Wait for OqtantJob results ##\n",
                 "\n",
-                "If your job is in the PENDING or RUNNING state, wait for 1 minute and update/see active jobs again. When the job \"Example Ultracold Matter Generator Job\" shows status COMPLETE, proceed to the next code block\n",
+                "If your OqtantJob is in the PENDING or RUNNING status, wait for 1 minute and run `OqtantClient.see_active_jobs()` again. When the OqtantJob \"Example Ultracold Matter Generator Job\" shows with status COMPLETE, proceed to the next code block\n",
                 "\n",
                 "\n",
-                "## Loading job results ##\n",
+                "## Loading OqtantJob results ##\n",
                 "\n",
                 "### From this session ###\n",
                 "\n",
-                "When a job is COMPLETE and the active jobs dictionary is updated, the OqtantJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary."
+                "When an OqtantJob is COMPLETE and `OqtantClient.active_jobs` is updated, the OqtantJob object is automatically populated with the job results. Define a variable to assign it to, or access it by it's id directly from the `OqtantJobs.active_jobs` dictionary."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]\n",
-                "print(example_bec_job)"
+                "barrier_manipulator_job = oqtant_client.active_jobs[barrier_manipulator_job_uuid]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Loading job results from a previous session ###\n",
+                "### Loading OqtantJob results from a previous session ###\n",
                 "\n",
-                "When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
+                "When Oraqle is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's `OqtantClient.active_jobs`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run\n",
-                "oqtant_client.load_job_from_id(example_bec_job_uuid)\n",
+                "oqtant_client.load_job_from_id(barrier_manipulator_job_uuid)\n",
                 "# access job from active_jobs\n",
-                "example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]"
+                "barrier_manipulator_job = oqtant_client.active_jobs[barrier_manipulator_job_uuid]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Accessing job results - TOF images ##\n",
+                "## Accessing OqtantJob results - IT images ##\n",
                 "\n",
-                "Job results for jobs run with TOF imaging contain the following fields:"
+                "Results for OqtantJobs run with IT imaging contain the following fields:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for key in example_bec_job.inputs[0].output.values.dict().keys():\n",
+                "for key in barrier_manipulator_job.inputs[0].output.values.dict().keys():\n",
                 "    print(key)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Viewing TOF images and slice plots ##\n",
-                "\n",
-                "The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms. \n",
+                "## Viewing IT images ##\n",
                 "\n",
-                "To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself."
+                "To view the TOF results in 2D or 1D, use the built in functions of the OqtantJob class to plot or access the results directly and plot them yourself."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "example_bec_job.atoms_2dplot(figsize=(6,6))\n",
-                "\n",
-                "example_bec_job.atoms_sliceplot()\n",
-                "\n",
-                "TOF_data = example_bec_job.get_TOF()\n",
+                "IT_OD = barrier_manipulator_job.get_IT()\n",
+                "pix_cal = barrier_manipulator_job.pix_cal\n",
                 "\n",
-                "plt.figure(figsize=(6,6))\n",
-                "plt.title(\"This is a customized plot of the same results\")\n",
-                "TOF_plot = plt.imshow(TOF_data,origin=\"lower\",\n",
-                "            cmap=\"nipy_spectral\")\n",
+                "plt.figure(figsize=(12,4))\n",
+                "plt.title(\"In-Trap Optical Depth\")\n",
+                "IT_plot = plt.imshow(IT_OD,origin=\"lower\",\n",
+                "            cmap=\"nipy_spectral\", extent=[-256, 256, -74, 74])\n",
+                "plt.xlabel(\"X position (um)\")\n",
+                "plt.ylabel(\"Y position (um)\")\n",
                 "plt.grid(visible=True)\n",
-                "plt.colorbar(TOF_plot, shrink=0.8)\n",
+                "plt.colorbar(IT_plot)\n",
                 "\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Viewing atom cloud statistics ##\n",
+                "## Creating OqtantJobs based off previous ones ##\n",
                 "\n",
-                "The Oqtant system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "output = example_bec_job.inputs[0].output.values\n",
-                "print(\"temperature (nK):\"+ str(output.temperature_uk))\n",
-                "print(\"total atoms :\"+ str(output.tof_atom_number))\n",
-                "print(\"condensed atoms :\"+ str(output.condensed_atom_number))\n",
-                "print(\"thermal atoms :\"+ str(output.thermal_atom_number))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Creating jobs based off previous ones ##\n",
-                "\n",
-                "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
+                "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the OqtantClient class provides a method that retrieves an entire OqtantJob's input structure to allow for editing and submission. The steps to do this can be found below."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# identify the job you wish to copy, this can be any job id you want to use.\n",
                 "# the status of the job does not matter\n",
-                "already_submitted_job_id = example_bec_job.external_id\n",
+                "already_submitted_job_id = barrier_manipulator_job.external_id\n",
                 "\n",
                 "# for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.\n",
                 "# without a targeted input run oqtant will default to the first run\n",
-                "new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)\n",
+                "new_barrier_manipulator_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)\n",
                 "\n",
                 "# at this point 'new_job_stub' is a python dict with the following keys\n",
-                "print(\"new job stub keys:\")\n",
-                "print(new_job_stub.keys())\n",
+                "print(\"new barrier manipulator job stub keys:\")\n",
+                "print(new_barrier_manipulator_job_stub.keys())\n",
                 "print(\"\\n\")\n",
                 "\n",
                 "# if you wish to include any job notes associated with the existing job input you can run the\n",
                 "# same command above but with the `include_notes` flag set to True\n",
                 "# new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)\n",
                 "\n",
                 "# from here you can update any of the inputs and the name of the job to your liking\n",
-                "new_job_stub[\"name\"] = \"this is a stub of another job\"\n",
+                "new_barrier_manipulator_job_stub[\"name\"] = \"this is a stub of another job\"\n",
                 "\n",
-                "# at this point 'new_job_stub' can be provided to the 'generate_oqtant_job' function and then submitted with\n",
+                "# at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with\n",
                 "# the 'run_jobs' function as demonstrated in previous steps\n",
-                "new_example_bec_job = oqtant_client.generate_oqtant_job(job=new_job_stub)\n",
-                "print(\"new job object:\")\n",
-                "print(new_example_bec_job)"
+                "new_barrier_manipulator_job = oqtant_client.generate_oqtant_job(job=new_barrier_manipulator_job_stub)\n",
+                "print(\"new barrier manipulator job object:\")\n",
+                "print(new_barrier_manipulator_job)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## View your current job limits\n",
                 "\n",
-                "Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `oqtant_client.get_limits()` method:"
+                "Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `OqtantClient.get_limits()` method:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -418,13 +416,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.11.4"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "9d324fb170b849c0db1b04a4eaa5a753613b2d729749991e51e49ca6f200afbc"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Oqtant Walkthrough 1: Getting Started
+# Oqtant Walkthrough 1: Ultracold Matter
 
-### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###
+### This walkthrough covers authorizing an Oraqle session using the OqtantClient, generating, running and viewing the results of a Ultracold Matter OqtantJob.
 
 For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
 
-*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
+_Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR._
 
-# Authenticate with Oqtant
+# Authenticate with Oraqle
 
-## Before you can view and submit jobs you must first authenticate with your Oqtant account
+## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account
 
 Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
+`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085.
 
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 from oqtant.oqtant_client import get_oqtant_client
@@ -24,34 +25,39 @@
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 
-token = get_user_token()
+token = get_user_token(auth_server_port=8080)
 ```
 
-## Creating a Oqtant Client Instance ##
+## Creating a OqtantClient Instance
 
-### After successful login, create an authorized session with the Oqtant Client ###
-- the oqtant_client interacts with the albert server to perform remote lab functions.
-- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
+### After successfully logging in, create an authorized session with the OqtantClient
 
+- The OqtantClient class interacts with the Oraqle server to perform remote lab functions.
+- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Generate parameters to create a job ##
-Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BEC job:
+## Generate parameters to create an OqtantJob
 
+Every OqtantJob is specified by a name, job_type, and a dictionary of input parameters. Below is an example with default parameters for a Ultracold Matter OqtantJob:
+
+_Ultracold Matter and Barrier Manipulator jobs are represented as OqtantJob objects with different `job_type` fields_
+
+- Ultracold Matter: `BEC`
+- Barrier Manipulator: `BARRIER`
 
 ```python
-default_bec_job = {
+ultracold_matter_job = {
     "name": "Example Ultracold Matter Generator Job",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
@@ -66,203 +72,192 @@
                 "optical_landscape": None,
                 "lasers": None,
             },
         }
     ],
 }
 
-example_bec_job = oqtant_client.generate_oqtant_job(job=default_bec_job)
-print(example_bec_job)
+ultracold_matter_job = oqtant_client.generate_oqtant_job(job=ultracold_matter_job)
+print(ultracold_matter_job)
 ```
 
-## Add notes to your job input (Optional) ##
-Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
+## Add notes to your OqtantJob input (Optional)
 
+Every OqtantJob input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
-example_bec_job.inputs[0].notes = "This is an example BEC job created from Oqtant walkthrough #1"
+ultracold_matter_job.inputs[0].notes = "This is an Ultracold Matter job created from Oqtant walkthrough #1"
 ```
 
-## Submit the job to run on the Oqtant hardware ##
+## Submit the OqtantJob to run on the Oraqle hardware
 
-**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.
+`OqtantClient.run_jobs()` takes a list of OqtantJob objects, `job_list=[*OqtantJob]` and submits them to the online queue. For each OqtantJob added to the queue a unique UUID is generated and associated to it.
 
-The output of **run_jobs()** is a list of the unique UUIDs generated during submission. 
+The output of `OqtantClient.run_jobs()` is a list of the unique UUIDs generated during submission.
 
-If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.
+If you are submitting a list of OqtantJobs and wish to wait for the results to return, use the flag `track_status=True`.
 
 If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:
 
-- **track_status=True**
-- **filename="name_of_file"**
-- **write=True**
+- `track_status=True`
+- `filename="name_of_file"`
+- `write=True`
 
 When writing to a file be sure to <span style="color:red">not overwrite it</span>
 
-
 ```python
-[example_bec_job_uuid] = oqtant_client.run_jobs(job_list=[example_bec_job], track_status=True)
+[ultracold_matter_job_uuid] = oqtant_client.run_jobs(job_list=[ultracold_matter_job], track_status=True)
 ```
 
-## Best practices for referencing ##
+## Best practices for referencing
+
+To easily reference OqtantJobs from the current or previous sessions it is useful to write their ids to a file named after the job. This file can be used later to access the OqtantJob.
 
+In this case we are saving this OqtantJob's id under a file named after this walkthrough.
 
 ```python
-with open('example_bec_job-walkthrough0.txt', 'w') as f:
-    f.write(example_bec_job_uuid)
+with open('walkthrough_1_ultracold_matter.txt', 'w') as f:
+    f.write(ultracold_matter_job_uuid)
 ```
 
-## Check the status of this session's active jobs ##
+## Check the status of this session's active OqtantJobs
 
-The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. 
+The OqtantClient object contains a dictionary (indexed by job_id) of all the active OqtantJobs from the current session. To keep inputs and results organized, all jobs are handled as objects of the OqtantJob class.
 
-**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. 
+`OqtantClient.active jobs` contains OqtantJobs that have been submitted with `OqtantClient.run_jobs()` or loaded with either `OqtantClient.load_job_from_id()` or `OqtantClient.load_job_from_file()`.
 
-<span style="color:red"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>
+<span style="color:red"> Note: `OqtantClient.active_jobs` does not automatically include OqtantJobs which were submitted on the Oraqle web application or in a different python session, even if those jobs are currently in the queue to run. </span>
 
-To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. 
-
-<span style="color:red"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>
-
-### To access information about a OqtantJob object ###
+### To access information about a OqtantJob object
 
 **EXAMPLEJOB.DESIRED_INFO**
 
 OqtantJob objects have the following relevant fields:
 
- - name
- - job_type
- - status
- - time_submit (datetime object)
- - inputs list (see walkthrough 2 for specifics)
+- name (str)
+- job_type (str)
+- status (str)
+- time_submit (datetime)
+- inputs (list) (see walkthrough 2 for specifics)
 
-To see all the job information, you can print the object. 
-
-Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python. 
+To see all the job information, you can print the object.
 
+Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python.
 
 ```python
 oqtant_client.see_active_jobs()
 ```
 
-## Wait for job results ##
-
-If your job is in the PENDING or RUNNING state, wait for 1 minute and update/see active jobs again. When the job "Example Ultracold Matter Generator Job" shows status COMPLETE, proceed to the next code block
+## Wait for OqtantJob results
 
+If your OqtantJob is in the PENDING or RUNNING status, wait for 1 minute and run `OqtantClient.see_active_jobs()` again. When the OqtantJob "Example Ultracold Matter Generator Job" shows with status COMPLETE, proceed to the next code block
 
-## Loading job results ##
+## Loading OqtantJob results
 
-### From this session ###
-
-When a job is COMPLETE and the active jobs dictionary is updated, the OqtantJob object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary.
+### From this session
 
+When an OqtantJob is COMPLETE and `OqtantClient.active_jobs` is updated, the OqtantJob object is automatically populated with the job results. Define a variable to assign it to, or access it by it's id directly from the `OqtantJobs.active_jobs` dictionary.
 
 ```python
-example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]
-print(example_bec_job)
+ultracold_matter_job = oqtant_client.active_jobs[ultracold_matter_job_uuid]
+print(ultracold_matter_job)
 ```
 
-### Loading job results from a previous session ###
-
-When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
+### Loading OqtantJob results from a previous session
 
+When Oraqle is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's `OqtantClient.active_jobs`.
 
 ```python
 # for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run
-oqtant_client.load_job_from_id(example_bec_job_uuid)
+oqtant_client.load_job_from_id(ultracold_matter_job_uuid)
 # access job from active_jobs
-example_bec_job = oqtant_client.active_jobs[example_bec_job_uuid]
+ultracold_matter_job = oqtant_client.active_jobs[ultracold_matter_job_uuid]
 ```
 
-## Accessing job results - TOF images ##
-
-Job results for jobs run with TOF imaging contain the following fields:
+## Accessing OqtantJob results - TOF images
 
+Results for OqtantJobs run with TOF imaging contain the following fields:
 
 ```python
-for key in example_bec_job.inputs[0].output.values.dict().keys():
+for key in ultracold_matter_job.inputs[0].output.values.dict().keys():
     print(key)
 ```
 
-## Viewing TOF images and slice plots ##
+## Viewing TOF images and slice plots
 
-The Oqtant system automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms. 
+The OqtantJob class automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms.
 
 To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself.
 
-
 ```python
-example_bec_job.atoms_2dplot(figsize=(6,6))
+ultracold_matter_job.atoms_2dplot(figsize=(6,6))
 
-example_bec_job.atoms_sliceplot()
+ultracold_matter_job.atoms_sliceplot()
 
-TOF_data = example_bec_job.get_TOF()
+TOF_data = ultracold_matter_job.get_TOF()
 
 plt.figure(figsize=(6,6))
 plt.title("This is a customized plot of the same results")
 TOF_plot = plt.imshow(TOF_data,origin="lower",
             cmap="nipy_spectral")
 plt.grid(visible=True)
 plt.colorbar(TOF_plot, shrink=0.8)
 
 plt.show()
 ```
 
-## Viewing atom cloud statistics ##
-
-The Oqtant system performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:
+## Viewing atom cloud statistics
 
+The Oraqle service performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:
 
 ```python
-output = example_bec_job.inputs[0].output.values
+output = ultracold_matter_job.inputs[0].output.values
 print("temperature (nK):"+ str(output.temperature_uk))
 print("total atoms :"+ str(output.tof_atom_number))
 print("condensed atoms :"+ str(output.condensed_atom_number))
 print("thermal atoms :"+ str(output.thermal_atom_number))
 ```
 
-## Creating jobs based off previous ones ##
-
-There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
+## Creating OqtantJobs based off previous ones
 
+There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the OqtantClient class provides a method that retrieves an entire OqtantJob's input structure to allow for editing and submission. The steps to do this can be found below.
 
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
-already_submitted_job_id = example_bec_job.external_id
+already_submitted_job_id = ultracold_matter_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
 # without a targeted input run oqtant will default to the first run
-new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)
+new_ultracold_matter_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)
 
 # at this point 'new_job_stub' is a python dict with the following keys
-print("new job stub keys:")
-print(new_job_stub.keys())
+print("new ultracold matter job stub keys:")
+print(new_ultracold_matter_job_stub.keys())
 print("\n")
 
 # if you wish to include any job notes associated with the existing job input you can run the
 # same command above but with the `include_notes` flag set to True
 # new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)
 
 # from here you can update any of the inputs and the name of the job to your liking
-new_job_stub["name"] = "this is a stub of another job"
+new_ultracold_matter_job_stub["name"] = "this is a stub of another job"
 
 # at this point 'new_job_stub' can be provided to the 'generate_oqtant_job' function and then submitted with
 # the 'run_jobs' function as demonstrated in previous steps
-new_example_bec_job = oqtant_client.generate_oqtant_job(job=new_job_stub)
-print("new job object:")
-print(new_example_bec_job)
+new_ultracold_matter_job = oqtant_client.generate_oqtant_job(job=new_ultracold_matter_job_stub)
+print("new ultracold matter job object:")
+print(new_ultracold_matter_job)
 ```
 
 ## View your current job limits
 
-Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `oqtant_client.get_limits()` method:
-
+Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `OqtantClient.get_limits()` method:
 
 ```python
 limits = oqtant_client.get_job_limits()
 print(limits)
 ```
 
 If you are running batch jobs, each run is counted as a job against your limit (i.e., a batch job with 10 runs counts as 10 against your limits).
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9297581601029876%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 5: Ultracold Matter Optimization "*

 * *            "#\\n'), (2, '### This walkthrough covers optimization of Ultracold Matter OqtantJobs. "*

 * *            "###\\n'), (6, '*Batch job functionality is available for users with a subscription "*

 * *            "tier of EXPLORER or INNOVATOR.*\\n'), (7, '\\n'), (8, '`get_user_token` creates a "*

 * *            'temporary web server on your machine to handle authenticating with Oraqle. By default '*

 * *            'thi […]*

```diff
@@ -1,65 +1,75 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Walkthrough 2: Barrier Manipulator #\n",
+                "# Oqtant Walkthrough 5: Ultracold Matter Optimization #\n",
                 "\n",
-                "### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###\n",
+                "### This walkthrough covers optimization of Ultracold Matter OqtantJobs. ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
                 "\n",
-                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
+                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*\n",
+                "\n",
+                "`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Authenticate with Oqtant\n",
+                "# Authenticate with Oraqle\n",
                 "\n",
-                "## Before you can view and submit jobs you must first authenticate with your Oqtant account\n",
+                "## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account\n",
                 "\n",
                 "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from sklearn.gaussian_process import GaussianProcessRegressor as GPR\n",
                 "from matplotlib import pyplot as plt\n",
+                "from scipy.optimize import minimize\n",
+                "from warnings import catch_warnings\n",
+                "from warnings import simplefilter\n",
+                "from scipy.stats import norm\n",
                 "from lmfit import Model\n",
                 "import numpy as np\n",
                 "import inspect\n",
+                "import copy\n",
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
+                "from bert_schemas import job as JobSchema\n",
                 "from oqtant.schemas.job import (\n",
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
+                "import csv\n",
                 "\n",
-                "token = get_user_token()"
+                "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Creating a Oqtant Client Instance ##\n",
+                "## Creating a OqtantClient Instance ##\n",
                 "\n",
-                "### After successful login, create an authorized session with the Oqtant Client ###\n",
-                "- the oqtant_client interacts with the albert server to perform remote lab functions. \n",
-                "- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session"
+                "### After successfully logging in, create an authorized session with the OqtantClient ###\n",
+                "- The OqtantClient class interacts with the Oraqle server to perform remote lab functions.\n",
+                "- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -67,307 +77,357 @@
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Generate parameters to create a job ##\n",
-                "Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:"
+                "## Define a cost function for optimization ## \n",
+                "\n",
+                "A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script \n",
+                "\n",
+                "Larger value = Good:  Condensed and total atom number, condensate fraction \n",
+                "Smaller value = Good: Thermal atom number, temperature \n",
+                "\n",
+                "Ad hoc Cost function: **C = (Nth*T)/Nc**\n",
+                "\n",
+                "### cost_func_5D ### \n",
+                "This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "default_barrier_job = {\n",
-                "    \"name\": \"Example Barrier Manipulator Job\",\n",
-                "    \"job_type\": \"BARRIER\",\n",
+                "costs_5D = []\n",
+                "\n",
+                "base_ultracold_matter_job = {\n",
+                "    \"name\": \"Example Ultracold Matter Generator Job\",\n",
+                "    \"job_type\": \"BEC\",\n",
                 "    \"inputs\": [\n",
                 "        {\n",
                 "            \"values\": {\n",
-                "                \"time_of_flight_ms\": 7.0,\n",
-                "                \"image_type\": \"IN_TRAP\",\n",
-                "                \"end_time_ms\": 20.0,\n",
+                "                \"time_of_flight_ms\": 8.0,\n",
+                "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
+                "                \"end_time_ms\": 0.0,\n",
                 "                \"rf_evaporation\": {\n",
+                "                    \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.045],\n",
                 "                    \"powers_mw\": [500.0, 500.0, 475.0, 360.0, 220.0],\n",
-                "                    \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.1],\n",
                 "                    \"interpolation\": \"LINEAR\",\n",
                 "                    \"times_ms\": [-1600, -1200, -800, -400, 0],\n",
                 "                },\n",
-                "                \"optical_barriers\": [\n",
-                "                    {\n",
-                "                        \"heights_khz\": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 25.0, 25.0, 25.0, 25.0, 25.0],\n",
-                "                        \"positions_um\": [-10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0],\n",
-                "                        \"interpolation\": \"OFF\",\n",
-                "                        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
-                "                        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
-                "                        \"shape\": \"GAUSSIAN\",\n",
-                "                    },\n",
-                "                    {\n",
-                "                        \"heights_khz\": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 40.0, 40.0],\n",
-                "                        \"positions_um\": [10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0],\n",
-                "                        \"interpolation\": \"OFF\",\n",
-                "                        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
-                "                        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
-                "                        \"shape\": \"GAUSSIAN\",\n",
-                "                    },\n",
-                "                ],\n",
+                "                \"optical_barriers\": None,\n",
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
-                "            }\n",
-                "        },\n",
+                "            },\n",
+                "        }\n",
                 "    ],\n",
                 "}\n",
                 "\n",
-                "example_barrier_job = oqtant_client.generate_oqtant_job(job=default_barrier_job)\n",
-                "print(example_barrier_job)"
+                "def cost_func_5D(RF_freqs = [17.0, 8.0, 4.0, 1.2, 0.045]): # added 5th power to default\n",
+                "    base_ultracold_matter_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = list(RF_freqs)\n",
+                "    print(base_ultracold_matter_job)\n",
+                "    job = oqtant_client.generate_oqtant_job(job=base_ultracold_matter_job)\n",
+                "    [job_id] = oqtant_client.run_jobs(job_list=[job], track_status=True)\n",
+                "    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values\n",
+                "    Nth = job_output.thermal_atom_number\n",
+                "    T = job_output.temperature_uk\n",
+                "    Nc = job_output.condensed_atom_number\n",
+                "    C = (Nth*T)/Nc\n",
+                "    costs_5D.append(C)\n",
+                "    return C"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Add notes to your job input (Optional) ##\n",
-                "Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:"
+                "## Set bounds for optimization ## \n",
+                "\n",
+                "Bounds will prevent invalid jobs parameters from being submitted to the Oraqle."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# In this example we are only working with a single input\n",
-                "# so we will add the note to the first and only input in the array\n",
-                "example_barrier_job.inputs[0].notes = \"This is an example BARRIER job created from Oqtant walkthrough #1\""
+                "bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Submit the job to run on the Oqtant hardware ##\n",
-                "\n",
-                "**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.\n",
-                "\n",
-                "The output of **run_jobs()** is a list of the unique UUIDs generated during submission. \n",
+                "## Choose an optimization algorithm ##\n",
                 "\n",
-                "If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.\n",
+                "Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:  \n",
                 "\n",
-                "If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:\n",
-                "\n",
-                "- **track_status=True**\n",
-                "- **filename=\"name_of_file\"**\n",
-                "- **write=True**\n",
-                "\n",
-                "When writing to a file be sure to <span style=\"color:red\">not overwrite it</span>"
+                " - L-BFGS-B \n",
+                " - TNC\n",
+                " - COBYLA\n",
+                " - SLSQP\n",
+                " \n",
+                " \n",
+                " ## Provide initial conditions and max iterations ##\n",
+                " \n",
+                " I chose the Oraqle web application's default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "[example_barrier_job_uuid] = oqtant_client.run_jobs(job_list=[example_barrier_job], track_status=True)"
+                "res_5d = minimize(cost_func_5D, method=\"TNC\", bounds=bnds_5d, x0 = [17,8,4,1.2,0.05], options={'maxiter':10})\n",
+                "\n",
+                "print(\"optimization results freq tuning:\")\n",
+                "print(res_5d)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Best practices for referencing"
+                "## Bayesian Optimization with a Gaussian Process model ##\n"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Extract and shape the training data: ##\n",
+                "\n",
+                "x_train : array-like of shape (n_samples, n_features) or list of object\n",
+                "Feature vectors or other representations of training data (also required for prediction).\n",
+                "\n",
+                "y_train : array-like of shape (n_samples,) or (n_samples, n_targets)\n",
+                "Target values in training data (also required for prediction)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Define a new target cost function ##"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with open('example_barrier_job-walkthrough1.txt', 'w') as f:\n",
-                "    f.write(example_barrier_job_uuid)"
+                "def cost(Nc, Nth, T):\n",
+                "    C = (Nth*T)/Nc\n",
+                "    return C"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Check the status of this session's active jobs ##\n",
-                "\n",
-                "The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. \n",
-                "\n",
-                "**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. \n",
-                "\n",
-                "<span style=\"color:red\"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>\n",
-                "\n",
-                "To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. \n",
-                "\n",
-                "<span style=\"color:red\"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>\n",
-                "\n",
-                "### To access information about a OqtantJob object ###\n",
-                "\n",
-                "**EXAMPLEJOB.DESIRED_INFO**\n",
-                "\n",
-                "OqtantJob objects have the following relevant fields:\n",
-                "\n",
-                " - name\n",
-                " - job_type\n",
-                " - status\n",
-                " - time_submit (datetime object)\n",
-                " - inputs list (see walkthrough 2 for specifics)\n",
-                "\n",
-                "To see all the job information, you can print the object. \n",
-                "\n",
-                "Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python. "
+                "The optimization jobs run above will now be included in your list of currently active OqtantJobs:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client.see_active_jobs()"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "\n",
-                "## Loading job results ##\n",
-                "\n",
-                "### From this session ###\n",
-                "\n",
-                "When a job is COMPLETE and the active jobs dictionary is updated, the BEC_job object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary."
+                "x_train = []\n",
+                "y_train = []\n",
+                "for job_id in oqtant_client.active_jobs:\n",
+                "    job = oqtant_client.active_jobs[job_id]\n",
+                "    output = job.inputs[0].output.values\n",
+                "    condensed_atom_number = output.condensed_atom_number\n",
+                "    thermal_atom_number = output.thermal_atom_number\n",
+                "    temperature_uk = output.temperature_uk\n",
+                "    input = job.inputs[0].values\n",
+                "    x_train.append(input.rf_evaporation.frequencies_mhz)\n",
+                "    y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk)) \n",
+                "    "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]"
+                "# surrogate or approximation for the objective function\n",
+                "def surrogate(model, X):\n",
+                "    # catch any warning generated when making a prediction\n",
+                "    with catch_warnings():\n",
+                "        # ignore generated warnings\n",
+                "        simplefilter(\"ignore\")\n",
+                "        return model.predict(X, return_std=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Loading job results from a previous session ###\n",
+                "## Define an acquisition function ## \n",
+                "\n",
+                "This is a score assigned to each candidate sample on the domain. \n",
+                "\n",
+                "The surrogate function can be used as an acquisition (minimizing the surrogate is the goal after all)\n",
+                "\n",
+                "OR\n",
+                "\n",
+                "An acquisition function can be used. 3 common options:\n",
+                "- Probability of Improvement (PI).\n",
+                "- Expected Improvement (EI).\n",
+                "- Lower Confidence Bound (LCB).\n",
+                "\n",
+                "Here I chose probability of improvement \n",
+                "\n",
+                "**PI = cdf((mu \u2013 best_mu) / stdev)**\n",
                 "\n",
-                "When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs."
+                "Where PI is the probability of improvement, cdf() is the normal cumulative distribution function, mu is the mean of the surrogate function for a given sample x, stdev is the standard deviation of the surrogate function for a given sample x, and best_mu is the mean of the surrogate function for the best sample found so far."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run\n",
-                "oqtant_client.load_job_from_id(example_barrier_job_uuid)\n",
-                "# access job from active_jobs\n",
-                "example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]"
+                "def acquisition(X, Xsamples, model):\n",
+                "    # calculate the best surrogate score found so far\n",
+                "    yhat, _ = surrogate(model, X)\n",
+                "    best = max(yhat)\n",
+                "    # calculate mean and stdev via surrogate function\n",
+                "    mu, std = surrogate(model, Xsamples)\n",
+                "    #mu = mu[:, 0]\n",
+                "    # calculate the probability of improvement\n",
+                "    probs = norm.cdf((mu - best) / (std+1E-9))\n",
+                "    return probs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Accessing job results - IT images ##\n",
+                "## Define a domain ##\n",
                 "\n",
-                "Job results for jobs run with IT imaging contain the following fields:"
+                "This is the domain of the samples. This one point where we inject prior knowledge of the system from previous experience"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "for key in example_barrier_job.inputs[0].output.values.dict().keys():\n",
-                "    print(key)"
+                "domain = [(20.,15.),(12.,5.),(5.,2.),(1.9,0.2),(0.2,0.01),\n",
+                "          (500.,470.),(470.,460.),(459.,420.),(420.,350.)]\n",
+                "\n",
+                "def rand_domain_sample(domain):\n",
+                "    scale = domain[0]-domain[1]\n",
+                "    random_number = np.random.uniform()+(1E-9)\n",
+                "    sample = scale*random_number+domain[1]\n",
+                "    return sample"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Viewing IT images ##\n",
+                "## Define an optimizer on the acquisition function ##\n",
                 "\n",
-                "To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself."
+                "Here I have chosen a random search over the domain, but other search algorithms can be used. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "IT_OD = example_barrier_job.get_IT()\n",
-                "pix_cal = example_barrier_job.pix_cal\n",
-                "\n",
-                "plt.figure(figsize=(12,4))\n",
-                "plt.title(\"In-Trap Optical Depth\")\n",
-                "IT_plot = plt.imshow(IT_OD,origin=\"lower\",\n",
-                "            cmap=\"nipy_spectral\", extent=[-256, 256, -74, 74])\n",
-                "plt.xlabel(\"X position (um)\")\n",
-                "plt.ylabel(\"Y position (um)\")\n",
-                "plt.grid(visible=True)\n",
-                "plt.colorbar(IT_plot)\n",
-                "\n",
-                "plt.show()"
+                "def optimize_acquisition(X, y, model, sample_population):\n",
+                "    # random search, generate random samples\n",
+                "    Xsamples = np.asarray([[rand_domain_sample(domain[i]) for i in range(len(X[0]))] for j in range(sample_population)])\n",
+                "    Xsamples = Xsamples.reshape(len(Xsamples), len(X[0]))\n",
+                "    # calculate the acquisition function for each sample\n",
+                "    scores = acquisition(X, Xsamples, model)\n",
+                "    # locate the index of the largest scores\n",
+                "    ix = np.argmax(scores)\n",
+                "    return Xsamples[ix]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Creating jobs based off previous ones ##\n",
-                "\n",
-                "There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below."
+                "## Perform the optimization ##"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# identify the job you wish to copy, this can be any job id you want to use.\n",
-                "# the status of the job does not matter\n",
-                "already_submitted_job_id = example_barrier_job.external_id\n",
+                "X = x_train\n",
+                "Y = y_train\n",
+                "Oqtant_model = GPR()\n",
+                "Oqtant_model.fit(x_train, y_train)\n",
                 "\n",
-                "# for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.\n",
-                "# without a targeted input run oqtant will default to the first run\n",
-                "new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)\n",
+                "cost = []\n",
                 "\n",
-                "# at this point 'new_job_stub' is a python dict with the following keys\n",
-                "print(\"new job stub keys:\")\n",
-                "print(new_job_stub.keys())\n",
-                "print(\"\\n\")\n",
-                "\n",
-                "# if you wish to include any job notes associated with the existing job input you can run the\n",
-                "# same command above but with the `include_notes` flag set to True\n",
-                "# new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)\n",
-                "\n",
-                "# from here you can update any of the inputs and the name of the job to your liking\n",
-                "new_job_stub[\"name\"] = \"this is a stub of another job\"\n",
-                "\n",
-                "# at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with\n",
-                "# the 'run_jobs' function as demonstrated in previous steps\n",
-                "new_example_barrier_job = oqtant_client.generate_oqtant_job(job=new_job_stub)\n",
-                "print(\"new job object:\")\n",
-                "print(new_example_barrier_job)"
+                "for i in range(10):\n",
+                "    # select the next point to sample\n",
+                "    x = optimize_acquisition(X, Y, Oqtant_model, 500)\n",
+                "    print('x', x)\n",
+                "    # sample the point\n",
+                "    actual = cost_func_5D(x)\n",
+                "    cost.append(actual)\n",
+                "    # summarize the finding\n",
+                "    est, _ = surrogate(Oqtant_model, [x])\n",
+                "    print(x, est, actual)\n",
+                "    # add the data to the dataset\n",
+                "    X = np.vstack((X, [x]))\n",
+                "    Y.append(actual)\n",
+                "    # update the model\n",
+                "    Oqtant_model.fit(X, Y)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# plot all samples and the final surrogate function\n",
+                "plt.plot(cost[5:])\n",
+                "#plt.yscale(\"log\")\n",
+                "plt.xlabel(\"function evaluations\")\n",
+                "plt.ylabel(\"Cost\")\n",
+                "plt.title(\"20 evaluations, 500 surrogate samples, 335pm 5_5_21\")\n",
+                "plt.savefig(\"335pm 5_5_21.png\")\n",
+                "plt.show()\n",
+                "# best result\n",
+                "ix = np.argmax(Y)\n",
+                "print('Best Result:'+str([X[ix], Y[ix]]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -386,18 +446,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "9d324fb170b849c0db1b04a4eaa5a753613b2d729749991e51e49ca6f200afbc"
-            }
+            "version": "3.11.4"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Oqtant Walkthrough 2: Barrier Manipulator
 
-### This walkthrough covers authorizing an Oqtant session using the Oqtant client, generating, running and viewing the results of a job. ###
+### This walkthrough covers authorizing an Oraqle session using the OqtantClient, generating, running and viewing the results of a Barrier Manipulator OqtantJob.
 
 For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
 
-*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
+_Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR._
 
-# Authenticate with Oqtant
+`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085.
 
-## Before you can view and submit jobs you must first authenticate with your Oqtant account
+# Authenticate with Oraqle
 
-Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
+## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account
 
+Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from matplotlib import pyplot as plt
 from lmfit import Model
 import numpy as np
 import inspect
 from oqtant.oqtant_client import get_oqtant_client
@@ -24,34 +25,39 @@
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 
-token = get_user_token()
+token = get_user_token(auth_server_port=8080)
 ```
 
-## Creating a Oqtant Client Instance ##
+## Creating a OqtantClient Instance
 
-### After successful login, create an authorized session with the Oqtant Client ###
-- the oqtant_client interacts with the albert server to perform remote lab functions. 
-- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
+### After successfully logging in, create an authorized session with the OqtantClient
 
+- The OqtantClient interacts with the Oraqle server to perform remote lab functions.
+- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Generate parameters to create a job ##
-Every Oqtant job is specified by a **name**, **job_type**, and a dictionary of input parameters. Below is an example with default parameters for a BARRIER job:
+## Generate parameters to create an OqtantJob
+
+Every OqtantJob is specified by a name, job_type, and a dictionary of input parameters. Below is an example with default parameters for a Barrier Manipulator OqtantJob:
 
+_Ultracold Matter and Barrier Manipulator jobs are represented as OqtantJob objects with different `job_type` fields_
+
+- Ultracold Matter: `BEC`
+- Barrier Manipulator: `BARRIER`
 
 ```python
-default_barrier_job = {
+barrier_manipulator_job = {
     "name": "Example Barrier Manipulator Job",
     "job_type": "BARRIER",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 7.0,
                 "image_type": "IN_TRAP",
@@ -83,170 +89,176 @@
                 "optical_landscape": None,
                 "lasers": None,
             }
         },
     ],
 }
 
-example_barrier_job = oqtant_client.generate_oqtant_job(job=default_barrier_job)
-print(example_barrier_job)
+barrier_manipulator_job = oqtant_client.generate_oqtant_job(job=barrier_manipulator_job)
+print(barrier_manipulator_job)
 ```
 
-## Add notes to your job input (Optional) ##
-Every Oqtant job input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
+## Add notes to your OqtantJob input (Optional)
 
+Every OqtantJob input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
-example_barrier_job.inputs[0].notes = "This is an example BARRIER job created from Oqtant walkthrough #1"
+barrier_manipulator_job.inputs[0].notes = "This is an Ultracold Matter job created from Oqtant walkthrough #1"
 ```
 
-## Submit the job to run on the Oqtant hardware ##
+## Submit the OqtantJob to run on the Oraqle hardware
 
-**run_jobs(job_list=jobs)** takes a list of OqtantJob objects and submits them to the online queue for Oqtant Jobs. For each OqtantJob added to the queue a unique UUID is generated and associated to the job.
+`OqtantClient.run_jobs()` takes a list of OqtantJob objects, `job_list=[*OqtantJob]` and submits them to the online queue. For each OqtantJob added to the queue a unique UUID is generated and associated to it.
 
-The output of **run_jobs()** is a list of the unique UUIDs generated during submission. 
+The output of `OqtantClient.run_jobs()` is a list of the unique UUIDs generated during submission.
 
-If you are submitting a list of jobs and wish to wait for the results to return, use the flag **track_status=True**.
+If you are submitting a list of OqtantJobs and wish to wait for the results to return, use the flag `track_status=True`.
 
 If you would like the resulting unique UUIDs to be written to a file for later reference you can do so by providing the following flags:
 
-- **track_status=True**
-- **filename="name_of_file"**
-- **write=True**
+- `track_status=True`
+- `filename="name_of_file"`
+- `write=True`
 
 When writing to a file be sure to <span style="color:red">not overwrite it</span>
 
-
 ```python
-[example_barrier_job_uuid] = oqtant_client.run_jobs(job_list=[example_barrier_job], track_status=True)
+[barrier_manipulator_job_uuid] = oqtant_client.run_jobs(job_list=[barrier_manipulator_job], track_status=True)
 ```
 
 ## Best practices for referencing
 
+To easily reference OqtantJobs from the current or previous sessions it is useful to write their ids to a file named after the job. This file can be used later to access the OqtantJob.
+
+In this case we are saving this OqtantJob's id under a file named after this walkthrough.
 
 ```python
-with open('example_barrier_job-walkthrough1.txt', 'w') as f:
-    f.write(example_barrier_job_uuid)
+with open('walkthrough_2_barrier_manipulator.txt', 'w') as f:
+    f.write(barrier_manipulator_job_uuid)
 ```
 
-## Check the status of this session's active jobs ##
-
-The **oqtant_client** object contains a dictionary (indexed by job_id) of all the active jobs from the current session. 
-
-**oqtant_client.active jobs** contains jobs that have been submitted with **run_jobs()**, loaded with **load_job_from_id()** or **load_job_from_file()**. 
+## Check the status of this session's active OqtantJobs
 
-<span style="color:red"> Note: oqtant_client.active_jobs does not automatically include jobs which were submitted on the web app or in a different python session, even if those jobs are currently in the queue to run. </span>
+The OqtantClient object contains a dictionary (indexed by job_id) of all the active OqtantJobs from the current session. To keep inputs and results organized, all jobs are handled as objects of the OqtantJob class.
 
-To keep inputs and results organized, all jobs are handled as objects of the **OqtantJob** class. 
+`OqtantClient.active jobs` contains OqtantJobs that have been submitted with `OqtantClient.run_jobs()` or loaded with either `OqtantClient.load_job_from_id()` or `OqtantClient.load_job_from_file()`.
 
-<span style="color:red"> Note: both BEC and BARRIER job types are represented as OqtantJob objects with different job_type fields </span>
+<span style="color:red"> Note: `OqtantClient.active_jobs` does not automatically include OqtantJobs which were submitted on the Oraqle web application or in a different python session, even if those jobs are currently in the queue to run. </span>
 
-### To access information about a OqtantJob object ###
+### To access information about a OqtantJob object
 
 **EXAMPLEJOB.DESIRED_INFO**
 
 OqtantJob objects have the following relevant fields:
 
- - name
- - job_type
- - status
- - time_submit (datetime object)
- - inputs list (see walkthrough 2 for specifics)
+- name (str)
+- job_type (str)
+- status (str)
+- time_submit (datetime)
+- inputs (list) (see walkthrough 2 for specifics)
 
-To see all the job information, you can print the object. 
-
-Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python. 
+To see all the job information, you can print the object.
 
+Click [here](https://www.learnpython.org/en/Classes_and_Objects) for an example-based intro to objects and classes in python.
 
 ```python
 oqtant_client.see_active_jobs()
 ```
 
+## Wait for OqtantJob results
 
-## Loading job results ##
+If your OqtantJob is in the PENDING or RUNNING status, wait for 1 minute and run `OqtantClient.see_active_jobs()` again. When the OqtantJob "Example Ultracold Matter Generator Job" shows with status COMPLETE, proceed to the next code block
 
-### From this session ###
+## Loading OqtantJob results
 
-When a job is COMPLETE and the active jobs dictionary is updated, the BEC_job object is automatically populated with the job results. Define a variable to access to job object, or access it by job id directly from the active jobs dictionary.
+### From this session
 
+When an OqtantJob is COMPLETE and `OqtantClient.active_jobs` is updated, the OqtantJob object is automatically populated with the job results. Define a variable to assign it to, or access it by it's id directly from the `OqtantJobs.active_jobs` dictionary.
 
 ```python
-example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]
+barrier_manipulator_job = oqtant_client.active_jobs[barrier_manipulator_job_uuid]
 ```
 
-### Loading job results from a previous session ###
-
-When Oqtant is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's active_jobs.
+### Loading OqtantJob results from a previous session
 
+When Oraqle is offline or you wish to analyze jobs from a previous run, use the job id to access it from the database and save it to the session's `OqtantClient.active_jobs`.
 
 ```python
 # for jobs with multiple runs add `run=<int>` where <int> equals the input you wish to view. defaults to the first run
-oqtant_client.load_job_from_id(example_barrier_job_uuid)
+oqtant_client.load_job_from_id(barrier_manipulator_job_uuid)
 # access job from active_jobs
-example_barrier_job = oqtant_client.active_jobs[example_barrier_job_uuid]
+barrier_manipulator_job = oqtant_client.active_jobs[barrier_manipulator_job_uuid]
 ```
 
-## Accessing job results - IT images ##
-
-Job results for jobs run with IT imaging contain the following fields:
+## Accessing OqtantJob results - IT images
 
+Results for OqtantJobs run with IT imaging contain the following fields:
 
 ```python
-for key in example_barrier_job.inputs[0].output.values.dict().keys():
+for key in barrier_manipulator_job.inputs[0].output.values.dict().keys():
     print(key)
 ```
 
-## Viewing IT images ##
-
-To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself.
+## Viewing IT images
 
+To view the TOF results in 2D or 1D, use the built in functions of the OqtantJob class to plot or access the results directly and plot them yourself.
 
 ```python
-IT_OD = example_barrier_job.get_IT()
-pix_cal = example_barrier_job.pix_cal
+IT_OD = barrier_manipulator_job.get_IT()
+pix_cal = barrier_manipulator_job.pix_cal
 
 plt.figure(figsize=(12,4))
 plt.title("In-Trap Optical Depth")
 IT_plot = plt.imshow(IT_OD,origin="lower",
             cmap="nipy_spectral", extent=[-256, 256, -74, 74])
 plt.xlabel("X position (um)")
 plt.ylabel("Y position (um)")
 plt.grid(visible=True)
 plt.colorbar(IT_plot)
 
 plt.show()
 ```
 
-## Creating jobs based off previous ones ##
-
-There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the `oqtant_client` provides a method that retrieves an entire job's input structure to allow for editing and submission. The steps to do this can be found below.
+## Creating OqtantJobs based off previous ones
 
+There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the OqtantClient class provides a method that retrieves an entire OqtantJob's input structure to allow for editing and submission. The steps to do this can be found below.
 
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
-already_submitted_job_id = example_barrier_job.external_id
+already_submitted_job_id = barrier_manipulator_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
 # without a targeted input run oqtant will default to the first run
-new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)
+new_barrier_manipulator_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)
 
 # at this point 'new_job_stub' is a python dict with the following keys
-print("new job stub keys:")
-print(new_job_stub.keys())
+print("new barrier manipulator job stub keys:")
+print(new_barrier_manipulator_job_stub.keys())
 print("\n")
 
 # if you wish to include any job notes associated with the existing job input you can run the
 # same command above but with the `include_notes` flag set to True
 # new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)
 
 # from here you can update any of the inputs and the name of the job to your liking
-new_job_stub["name"] = "this is a stub of another job"
+new_barrier_manipulator_job_stub["name"] = "this is a stub of another job"
 
 # at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with
 # the 'run_jobs' function as demonstrated in previous steps
-new_example_barrier_job = oqtant_client.generate_oqtant_job(job=new_job_stub)
-print("new job object:")
-print(new_example_barrier_job)
+new_barrier_manipulator_job = oqtant_client.generate_oqtant_job(job=new_barrier_manipulator_job_stub)
+print("new barrier manipulator job object:")
+print(new_barrier_manipulator_job)
 ```
+
+## View your current job limits
+
+Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `OqtantClient.get_limits()` method:
+
+```python
+limits = oqtant_client.get_job_limits()
+print(limits)
+```
+
+If you are running batch jobs, each run is counted as a job against your limit (i.e., a batch job with 10 runs counts as 10 against your limits).
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937056182121972%*

 * *Differences: {"'cells'": "{1: {'source': ['## Import Packages']}, 3: {'source': ['## OqtantJobs and their "*

 * *            "constituent primitives']}, 4: {'source': ['In this walkthrough, we will explore the "*

 * *            'structure of OqtantJobs that you submit to Oraqle.  In an earlier walkthrough, we saw '*

 * *            'that a basic Ultracold Matter OqtantJob could be defined by with dictionary structure '*

 * *            "like the following:']}, 5: {'source': {insert: [(0, 'ultracold_matter_job_data = "*

 * *            '{\\n\') […]*

```diff
@@ -1,15 +1,23 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "f66e25b8",
+            "metadata": {},
+            "source": [
+                "# Oqtant Walkthrough 3: Abstractions #"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "d11e3a03",
             "metadata": {},
             "source": [
-                "## Imports"
+                "## Import Packages"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e6164db6",
             "metadata": {},
@@ -20,34 +28,34 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "38b61ffc",
             "metadata": {},
             "source": [
-                "## Oqtant jobs and their constituent primitives"
+                "## OqtantJobs and their constituent primitives"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4942af2d",
             "metadata": {},
             "source": [
-                "In this walkthrough, we will explore the structure of jobs that you submit to Oqtant.  In an earlier walkthrough, we saw that a basic BEC job could be defined by a dictionary structure like"
+                "In this walkthrough, we will explore the structure of OqtantJobs that you submit to Oraqle.  In an earlier walkthrough, we saw that a basic Ultracold Matter OqtantJob could be defined by with dictionary structure like the following:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c08f5594",
             "metadata": {},
             "outputs": [],
             "source": [
-                "default_bec_job_data = {\n",
-                "    \"name\": \"Example BEC Job\",\n",
+                "ultracold_matter_job_data = {\n",
+                "    \"name\": \"Example Ultracold Matter Job\",\n",
                 "    \"job_type\": \"BEC\",\n",
                 "    \"inputs\": [\n",
                 "        {\n",
                 "            \"values\": {\n",
                 "                \"time_of_flight_ms\": 8.0,\n",
                 "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
                 "                \"end_time_ms\": 0.0,\n",
@@ -67,25 +75,25 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "61960d47",
             "metadata": {},
             "source": [
-                "We could then feed the above data structure to the API's *generate_Oqtant_job()* function to create the job object.  Here, we would like to explore the contents of the underlying job data structure more in depth.  The fields that control the behavior of the quantum matter machine are contained as *values* in the *inputs* list ([]).  For now, we will only discuss cases where the *inputs* list contains a single element.  When this list's length is greater than one, it signifies a so-called *batch* job, which will be discussed in a later walkthrough.  \n",
+                "We could then feed the above data structure to the API's *generate_oqtant_job()* function to create the job object.  Here, we would like to explore the contents of the underlying job data structure more in depth.  The fields that control the behavior of the quantum matter machine are contained as *values* in the *inputs* list ([]).  For now, we will only discuss cases where the *inputs* list contains a single element.  When this list's length is greater than one, it signifies a so-called *batch* job, which will be discussed in a later walkthrough.  \n",
                 "\n",
                 "The contents of *values* includes directives on the type of imaging to perform (*image_type* etc.) and how long to run the experiment (*end_time_ms*) after evaporation to BEC is complete.  Also included are various job primitives that can be created and edited as programmable objects in their own right.  These primitives include *rf_evaporation*, *optical_barriers*, *optical_landscape*, and *lasers*.  Much like an *OqtantJob* itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object.  Although not shown explicitly in our simple job data structure above, both *optical_barriers* and *lasers* are lists containing *Barrier* and *Laser* objects, respectively.  These objects will be explored below.  You are likely already familiar with the structure of the *rf_evaporation* data and how defining that data controls the evaporation to BEC in the experiment.  The *optical_landscape* data is a bit more complicated and will be explored in more detail below in a dedicated section.       \n",
                 "\n",
-                "Not all job types support every one of these data structures.  For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers.  BEC jobs, for instance, only support the rf_evaporation primitive.  After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate.  At the next level of complexity, BARRIER jobs support both *rf_evaporation* and *optical_barriers* but not \"optical_landscape\" or \"lasers\".  What data structures are supported by different job types will become clear as those job types are created/used/submitted.  As a preview, please refer to the following table.\n",
+                "Not all job types support every one of these data structures.  For the basic Ultracold Matter job above, we did not have data entries for barriers, the landscape, or lasers.  Ultracold Matter jobs, for instance, only support the rf_evaporation primitive.  After all, the purpose of a Ultracold Matter job is to keep things simple and just focus on the ability to tune the creation of the condensate.  At the next level of complexity, Barrier Manipulator jobs support both *rf_evaporation* and *optical_barriers* but not \"optical_landscape\" or \"lasers\".  What data structures are supported by different job types will become clear as those job types are created/used/submitted.  As a preview, please refer to the following table.\n",
                 "\n",
                 "| Job type   | Supports       |                  |                   |        |\n",
                 "|------------|----------------|------------------|-------------------|--------|\n",
                 "|            | rf_evaporation | optical_barriers | optical_landscape | lasers |\n",
-                "| BEC        |                |                  |                   |        |\n",
-                "| BARRIER    | X              | X                |                   |        |\n",
+                "| Ultracold Matter (BEC)        |                |                  |                   |        |\n",
+                "| Barrier Manipulator (BARRIER)    | X              | X                |                   |        |\n",
                 "| TRANSISTOR | X              | X                | X                 | X      |\n",
                 "| PAINT_1D   | X              | X                | X                 | X      |\n",
                 "\n",
                 "Please note that not all these job types are yet available at the time of this writing."
             ]
         },
         {
@@ -115,15 +123,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d2a8885a",
             "metadata": {},
             "source": [
-                "Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Oqtant job.  We can create this object by either calling the constructor directly with the required data fields:"
+                "Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific OqtantJob.  We can create this object by either calling the constructor directly with the required data fields:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8eecbfcf",
             "metadata": {},
@@ -217,15 +225,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0cfc0e41",
             "metadata": {},
             "source": [
-                "This behavior is generic to most objects in oqtant -- any temporal or spatial extrapolation requests yield 0.0.  \n",
+                "This behavior is generic to most objects in Oqtant -- any temporal or spatial extrapolation requests yield 0.0.  \n",
                 "\n",
                 "There are also functions that extract the time-dependent parameters for a list of input times:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -540,15 +548,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "23affffd",
             "metadata": {},
             "source": [
-                "Another Oqtant job primitive is the (singular) 'OpticalLandscape' object.  This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment.  However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.    \n",
+                "Another OqtantJob primitive is the (singular) 'OpticalLandscape' object.  This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment.  However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.    \n",
                 "\n",
                 "The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together *in time* (if there exists more than one underlying landscape).  Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.   "
             ]
         },
         {
             "cell_type": "markdown",
             "id": "758cae38",
@@ -745,14 +753,22 @@
             "execution_count": null,
             "id": "663ea847",
             "metadata": {},
             "outputs": [],
             "source": [
                 "laser.plot_intensity()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2241e7f9",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -763,15 +779,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.10.11"
         },
         "vscode": {
             "interpreter": {
                 "hash": "13fb51af87d45e56afa36501f99325526ec135b669e4eea3c0d0150b11fb593e"
             }
         }
     },
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_3_abstractions.md` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-## Imports
+# Oqtant Walkthrough 3: Abstractions
 
+## Import Packages
 
 ```python
 %matplotlib inline
 from bert_schemas import job as JobSchema
 ```
 
-## Oqtant jobs and their constituent primitives
+## OqtantJobs and their constituent primitives
 
-In this walkthrough, we will explore the structure of jobs that you submit to Oqtant. In an earlier walkthrough, we saw that a basic BEC job could be defined by a dictionary structure like
+In this walkthrough, we will explore the structure of OqtantJobs that you submit to Oraqle. In an earlier walkthrough, we saw that a basic Ultracold Matter OqtantJob could be defined by with dictionary structure like the following:
 
 ```python
-default_bec_job_data = {
-    "name": "Example BEC Job",
+ultracold_matter_job_data = {
+    "name": "Example Ultracold Matter Job",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
                 "end_time_ms": 0.0,
@@ -33,238 +34,224 @@
         }
     ]
 }
 ```
 
 We could then feed the above data structure to the API's _generate_oqtant_job()_ function to create the job object. Here, we would like to explore the contents of the underlying job data structure more in depth. The fields that control the behavior of the quantum matter machine are contained as _values_ in the _inputs_ list ([]). For now, we will only discuss cases where the _inputs_ list contains a single element. When this list's length is greater than one, it signifies a so-called _batch_ job, which will be discussed in a later walkthrough.
 
-The contents of *values* includes directives on the type of imaging to perform (*image_type* etc.) and how long to run the experiment (*end_time_ms*) after evaporation to BEC is complete.  Also included are various job primitives that can be created and edited as programmable objects in their own right.  These primitives include *rf_evaporation*, *optical_barriers*, *optical_landscape*, and *lasers*.  Much like an *OqtantJob* itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object.  Although not shown explicitly in our simple job data structure above, both *optical_barriers* and *lasers* are lists containing *Barrier* and *Laser* objects, respectively.  These objects will be explored below.  You are likely already familiar with the structure of the *rf_evaporation* data and how defining that data controls the evaporation to BEC in the experiment.  The *optical_landscape* data is a bit more complicated and will be explored in more detail below in a dedicated section.       
+The contents of _values_ includes directives on the type of imaging to perform (_image_type_ etc.) and how long to run the experiment (_end_time_ms_) after evaporation to BEC is complete. Also included are various job primitives that can be created and edited as programmable objects in their own right. These primitives include _rf_evaporation_, _optical_barriers_, _optical_landscape_, and _lasers_. Much like an _OqtantJob_ itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object. Although not shown explicitly in our simple job data structure above, both _optical_barriers_ and _lasers_ are lists containing _Barrier_ and _Laser_ objects, respectively. These objects will be explored below. You are likely already familiar with the structure of the _rf_evaporation_ data and how defining that data controls the evaporation to BEC in the experiment. The _optical_landscape_ data is a bit more complicated and will be explored in more detail below in a dedicated section.
 
-Not all job types support every one of these data structures.  For the basic BEC-type job above, we did not have data entries for barriers, the landscape, or lasers.  BEC jobs, for instance, only support the rf_evaporation primitive.  After all, the purpose of a BEC job is to keep things simple and just focus on the ability to tune the creation of the condensate.  At the next level of complexity, BARRIER jobs support both *rf_evaporation* and *optical_barriers* but not "optical_landscape" or "lasers".  What data structures are supported by different job types will become clear as those job types are created/used/submitted.  As a preview, please refer to the following table.
+Not all job types support every one of these data structures. For the basic Ultracold Matter job above, we did not have data entries for barriers, the landscape, or lasers. Ultracold Matter jobs, for instance, only support the rf_evaporation primitive. After all, the purpose of a Ultracold Matter job is to keep things simple and just focus on the ability to tune the creation of the condensate. At the next level of complexity, Barrier Manipulator jobs support both _rf_evaporation_ and _optical_barriers_ but not "optical_landscape" or "lasers". What data structures are supported by different job types will become clear as those job types are created/used/submitted. As a preview, please refer to the following table.
 
-| Job type   | Supports       |                  |                   |        |
-|------------|----------------|------------------|-------------------|--------|
-|            | rf_evaporation | optical_barriers | optical_landscape | lasers |
-| BEC        |                |                  |                   |        |
-| BARRIER    | X              | X                |                   |        |
-| TRANSISTOR | X              | X                | X                 | X      |
-| PAINT_1D   | X              | X                | X                 | X      |
+| Job type                      | Supports       |                  |                   |        |
+| ----------------------------- | -------------- | ---------------- | ----------------- | ------ |
+|                               | rf_evaporation | optical_barriers | optical_landscape | lasers |
+| Ultracold Matter (BEC)        |                |                  |                   |        |
+| Barrier Manipulator (BARRIER) | X              | X                |                   |        |
+| TRANSISTOR                    | X              | X                | X                 | X      |
+| PAINT_1D                      | X              | X                | X                 | X      |
 
 Please note that not all these job types are yet available at the time of this writing.
 
 ## The RfEvaporation Object
 
-Every job input has exactly one constituent RfEvaporation object defined by the "rf_evaporation" data shown above.  The behavior of this object controls the RF knife evaporation from an ultracold gas to Bose-Einstein condensate (BEC), as well as providing flexibility for applying RF fields during the experiment phase after the initial evaporation is complete.  The evaporation stage results in a tradeoff between final atom number and temperature -- evaporating more deeply, signified by RF detuning values closer to 0, produces less atoms but at colder temperature (and correspondingly higher condensate fraction).  Applying RF radiation during the experiment phase allows for hot atoms above some temperature, produced for example by rapid manipulation of optical barries or landscape potentials (explored below), to be removed the experiment -- a so-called "RF shield". 
+Every job input has exactly one constituent RfEvaporation object defined by the "rf_evaporation" data shown above. The behavior of this object controls the RF knife evaporation from an ultracold gas to Bose-Einstein condensate (BEC), as well as providing flexibility for applying RF fields during the experiment phase after the initial evaporation is complete. The evaporation stage results in a tradeoff between final atom number and temperature -- evaporating more deeply, signified by RF detuning values closer to 0, produces less atoms but at colder temperature (and correspondingly higher condensate fraction). Applying RF radiation during the experiment phase allows for hot atoms above some temperature, produced for example by rapid manipulation of optical barries or landscape potentials (explored below), to be removed the experiment -- a so-called "RF shield".
 
-It is important to note here that we adopt the convention that time = 0 refers to the *end* of the evaporation period.  As such, the initial evaporation to BEC, as defined by the object under current inspection, will involve negative (relative) times.  In our trap, the entire evaporation cycle takes on the order of a second, and times are specified in ms, so we should see negative times as large as a few thousand ms.   
+It is important to note here that we adopt the convention that time = 0 refers to the _end_ of the evaporation period. As such, the initial evaporation to BEC, as defined by the object under current inspection, will involve negative (relative) times. In our trap, the entire evaporation cycle takes on the order of a second, and times are specified in ms, so we should see negative times as large as a few thousand ms.
 
 ### Construction
 
-Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific Oqtant job.  We can create this object by either calling the constructor directly with the required data fields:
-
+Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific OqtantJob. We can create this object by either calling the constructor directly with the required data fields:
 
 ```python
 evap = JobSchema.RfEvaporation(
         times_ms = [-1600, -1200, -800, -400, 0],
         frequencies_mhz = [17.0, 8.0, 4.0, 1.2, 0.045],
         powers_mw = [500.0, 500.0, 475.0, 360.0, 220.0],
         interpolation = "LINEAR"
 )
 ```
 
 or by placing the underlying data in a dictionary and unpacking that dictionary in order to pass it to the constructor:
 
-
 ```python
 evap = JobSchema.RfEvaporation(**{
         "times_ms": [-1600, -1200, -800, -400, 0],
         "frequencies_mhz": [17.0, 8.0, 4.0, 1.2, 0.045],
         "powers_mw": [500.0, 490.0, 475.0, 360.0, 220.0],
         "interpolation": "LINEAR"
 })
 ```
 
-Inherent to the RfEvaporation object are three lists, *times_ms*, *frequencies_mhz*, and *powers_mw*.  The key prefix corresponds to the parameter being controlled, while the suffix refers to the associated units.  In this case, we specify a list of times in milliseconds (ms), frequencies in MHz (mhz), and powers in milliwatts (mw).  Note that all units are lower case, which can cause confusion if taken out of context.  All three lists must share the same length as each time element is paired with the corresponding element of the frequencies/powers list(s).  The specified behavior of the RF evaporation stage defind by the above data is as follows: At -1.6 seconds the RF power is set at 500 mW and the frequency (detuning) at 17 MHz.  By the end of the evaporation period, defined by t=0, the frequency/detuning has decreased to 0.045 MHz = 45 kHz and the power has been reduced to 220 mW.  Intermediate values of frequency and power are adopted between those two points in time, with the full time dependence being a result of the given data and chosen interpolation type, which controls how the RF fields behave between the given data points.      
+Inherent to the RfEvaporation object are three lists, _times_ms_, _frequencies_mhz_, and _powers_mw_. The key prefix corresponds to the parameter being controlled, while the suffix refers to the associated units. In this case, we specify a list of times in milliseconds (ms), frequencies in MHz (mhz), and powers in milliwatts (mw). Note that all units are lower case, which can cause confusion if taken out of context. All three lists must share the same length as each time element is paired with the corresponding element of the frequencies/powers list(s). The specified behavior of the RF evaporation stage defind by the above data is as follows: At -1.6 seconds the RF power is set at 500 mW and the frequency (detuning) at 17 MHz. By the end of the evaporation period, defined by t=0, the frequency/detuning has decreased to 0.045 MHz = 45 kHz and the power has been reduced to 220 mW. Intermediate values of frequency and power are adopted between those two points in time, with the full time dependence being a result of the given data and chosen interpolation type, which controls how the RF fields behave between the given data points.
 
-Frequencies are given as a detuning with respect to the energetic trap bottom, so RF fields at a frequency/detuning of 0 would eliminate all atoms from the trap.  Achieving final BEC temperatures on the order of 100 nK usually corresponds to final RF frequencies of a few tens of kHz.  Powers refer to the amount of power delivered to an antenna that bathes the ultracold atoms with RF radiation.  The actual local RF field experienced by the atoms depends on system losses and the exact geometry of the antenna.      
+Frequencies are given as a detuning with respect to the energetic trap bottom, so RF fields at a frequency/detuning of 0 would eliminate all atoms from the trap. Achieving final BEC temperatures on the order of 100 nK usually corresponds to final RF frequencies of a few tens of kHz. Powers refer to the amount of power delivered to an antenna that bathes the ultracold atoms with RF radiation. The actual local RF field experienced by the atoms depends on system losses and the exact geometry of the antenna.
 
 ### Time-dependent evaporation parameters
 
-We can explore the time-dependence of the RFEvaporation object frequency and power, as defined by the data structure above, using some useful functions included with oqtant.  For example, we can query the object for the instantaneous power or frequency at any point in time.  Recall that the units of power are mW and the units of frequency are MHz.
-
+We can explore the time-dependence of the RFEvaporation object frequency and power, as defined by the data structure above, using some useful functions included with oqtant. For example, we can query the object for the instantaneous power or frequency at any point in time. Recall that the units of power are mW and the units of frequency are MHz.
 
 ```python
 print(evap.get_power(time = -100))
 print(evap.get_frequency(time = -750))
 ```
 
 If we request the power or frequency for a time value outside the range of the underlying data, which would require extrapolation, we get 0.0:
 
-
 ```python
 print(evap.get_power(time = 100))           # request after last defined object time of 0 ms -> 0.0
 print(evap.get_frequency(time = -1800))     # request before first defined object time of -1600 ms -> 0.0
 ```
 
-This behavior is generic to most objects in oqtant -- any temporal or spatial extrapolation requests yield 0.0.  
+This behavior is generic to most objects in Oqtant -- any temporal or spatial extrapolation requests yield 0.0.
 
 There are also functions that extract the time-dependent parameters for a list of input times:
 
-
 ```python
 print(evap.get_powers(times = [-1600, -1000, -500, 0]))
 print(evap.get_frequencies(times = [-1600, -1000, -600, 0]))
 ```
 
 There are even useful plotting functions for visualizing these parameters over time.
 
-
 ```python
 evap.plot_power()
 evap.plot_frequency()
 ```
 
 ## Barrier Objects
 
-  
-
 ### Construction
 
-First, let us demonstrate the construction of a Barrier object, which represents a one-dimensional optical potential barrier to the BEC.  A barrier is characterized by a shape, a time-dependent position, height, and width, and information on how to interpolate over the underlying data in time.  For example, let us construct a Barrier object named *barr* for which the center scans from 1-11 microns in the first 10 ms of an experiment.  Over this same time period, the barrier height will increase from 1 kHz to 11 kHz.  The width will remain constant at 1 micron throughout, as will the (fixed) Gaussian shape.  In this case, the width parameter corresponds to the Gaussian width of the barrier.
-
+First, let us demonstrate the construction of a Barrier object, which represents a one-dimensional optical potential barrier to the BEC. A barrier is characterized by a shape, a time-dependent position, height, and width, and information on how to interpolate over the underlying data in time. For example, let us construct a Barrier object named _barr_ for which the center scans from 1-11 microns in the first 10 ms of an experiment. Over this same time period, the barrier height will increase from 1 kHz to 11 kHz. The width will remain constant at 1 micron throughout, as will the (fixed) Gaussian shape. In this case, the width parameter corresponds to the Gaussian width of the barrier.
 
 ```python
 barr = JobSchema.Barrier(
-    times_ms = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 
+    times_ms = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
     positions_um = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
     heights_khz = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
     widths_um = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
     interpolation = 'LINEAR',
     shape = 'GAUSSIAN'
 )
 ```
 
-Alternatively, as above, we can create the same object by generating the underlying data in a dictionary and then unpacking that dictionary (using the ** prefix) when we pass it to the Barrier class constructor:
-
+Alternatively, as above, we can create the same object by generating the underlying data in a dictionary and then unpacking that dictionary (using the \*\* prefix) when we pass it to the Barrier class constructor:
 
 ```python
 barr = JobSchema.Barrier(**{
-    "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], 
-    "positions_um": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], 
-    "heights_khz": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], 
-    "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], 
-    "interpolation": "LINEAR", 
+    "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+    "positions_um": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+    "heights_khz": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+    "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+    "interpolation": "LINEAR",
     "shape": "GAUSSIAN"
 })
 ```
 
-The lists of time-dependent quantities (position, height, and width) used to define *barr* must have the same length as the corresponding list of times.  In this case, the ordered pairs consisting of a list of, e.g., [times, positions], will be linearly interpolated in time.  
+The lists of time-dependent quantities (position, height, and width) used to define _barr_ must have the same length as the corresponding list of times. In this case, the ordered pairs consisting of a list of, e.g., [times, positions], will be linearly interpolated in time.
 
 ### Time-dependent barrier parameters
 
-We can explore the time-dependence of the barrier parameters using some in-built functions in pyubert.  For example, we can retrieve and/or plot the barriers positions over time:
-
+We can explore the time-dependence of the barrier parameters using some in-built functions in pyubert. For example, we can retrieve and/or plot the barriers positions over time:
 
 ```python
 print(barr.get_position(time = 2))
 print(barr.get_positions(times = [1,2,3]))
 ```
 
-Similarly, there are native functions for extracting a Barrier objects height and width at specified time(s).  In our case, the width evolution is trivial (constant).
-
+Similarly, there are native functions for extracting a Barrier objects height and width at specified time(s). In our case, the width evolution is trivial (constant).
 
 ```python
 print(barr.get_height(1.5))
 print(barr.get_heights([1.5, 2.5, 3.5]))
 
 print(barr.get_width(1.5))
 print(barr.get_widths([1.5, 2.5, 3.5]))
 ```
 
-As well as methods for extracting the time-dependent parameters of the barrier, we can also use some in-built plotting functions.  In the examples below, you can see the underlying data points (that we used to define the Barrier object) as points, with the full dynamics of the barrier parameters over time determined by the interpolation style and indicated by a solid line. In an actual experiment, the barrier positions are updated every 100 microseconds, so the time-dependent barrier parameters will only approximately follow the idealized interpolated line.   
-
+As well as methods for extracting the time-dependent parameters of the barrier, we can also use some in-built plotting functions. In the examples below, you can see the underlying data points (that we used to define the Barrier object) as points, with the full dynamics of the barrier parameters over time determined by the interpolation style and indicated by a solid line. In an actual experiment, the barrier positions are updated every 100 microseconds, so the time-dependent barrier parameters will only approximately follow the idealized interpolated line.
 
 ```python
 barr.plot_position()
 barr.plot_height()
 barr.plot_width()
 ```
 
-### Plotting the potential energy for a barrier  
-
-There are also methods native to oqtant for plotting Barrier object potential energies at different times of the experiment.  Here, we will explicitly specify the positional range of the plot (x-axis domain) in order to better be able to see the barrier displacement. 
+### Plotting the potential energy for a barrier
 
+There are also methods native to oqtant for plotting Barrier object potential energies at different times of the experiment. Here, we will explicitly specify the positional range of the plot (x-axis domain) in order to better be able to see the barrier displacement.
 
 ```python
 xlim = [-5, 15]
 ylim = [0, 12.5]
 barr.plot_potential(time = 1, x_limits = xlim, y_limits = ylim)
 barr.plot_potential(time = 5, x_limits = xlim, y_limits = ylim)
 barr.plot_potential(time = 9, x_limits = xlim, y_limits = ylim)
 ```
 
 ### Exploring Barrier shape options
 
-Supported Barrier shape options include GAUSSIAN, SQUARE, and LORENTZIAN.  In all three cases, the "width_um" parameter list means something slightly different.  For the GAUSSIAN case, the functional form of the barrier potential $U(x)$ follows the standard Gaussian formula
+Supported Barrier shape options include GAUSSIAN, SQUARE, and LORENTZIAN. In all three cases, the "width_um" parameter list means something slightly different. For the GAUSSIAN case, the functional form of the barrier potential $U(x)$ follows the standard Gaussian formula
+
 $$
 U(x) = H e^{-\frac{(x - x_0)^2}{2 w^2}} \quad \textrm{(GAUSSIAN)}
 $$
-where $H=H(t)$, $x_{0} = x_{0}(t)$, and $w = w(t)$ represent the time-dependent barrier height, center position, and width, respectively.  In this case, our width parameter corresponds to the traditional definition of the Gaussian width, often denoted as $\sigma$.    
+
+where $H=H(t)$, $x_{0} = x_{0}(t)$, and $w = w(t)$ represent the time-dependent barrier height, center position, and width, respectively. In this case, our width parameter corresponds to the traditional definition of the Gaussian width, often denoted as $\sigma$.
 
 For the LORENTZIAN case, the potential follows
+
 $$
 U(x) = \frac{H}{1 + (x - x_0)^{2} / w^{2}} \quad \textrm{(LORENTZIAN)},
 $$
-i.e. our width parameter w(t) corresponds to the half-width half-max of the Lorentzian.
 
-For the SQUARE case, the potential is simple a flat-topped potential-energy hill of height H(t) and *full* width w(t).  
+i.e. our width parameter w(t) corresponds to the half-width half-max of the Lorentzian.
 
+For the SQUARE case, the potential is simple a flat-topped potential-energy hill of height H(t) and _full_ width w(t).
 
 ```python
 barr.shape = JobSchema.ShapeType.SQUARE
 barr.plot_potential(time = 5, x_limits = [-25,25])
 
 barr.shape = JobSchema.ShapeType.LORENTZIAN
 barr.plot_potential(time = 5, x_limits = [-25,25])
 ```
 
-Note that the resolution of the projected light optical system is on the order of 2 microns.  Thus, *Barrier* objects with small widths will all appear similar in reality (the experiment) even if they have different *shape* settings.
+Note that the resolution of the projected light optical system is on the order of 2 microns. Thus, _Barrier_ objects with small widths will all appear similar in reality (the experiment) even if they have different _shape_ settings.
 
 ### Exploring Barrier interpolation options
 
-A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times_ms' list class member. At this time, the interpolation choice is *shared* for all three time-dependent barrier parameters.  Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.  
-
+A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times_ms' list class member. At this time, the interpolation choice is _shared_ for all three time-dependent barrier parameters. Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.
 
 ```python
 barr.positions_um = [2, 4, 6, 8, 10, 2, 4, 6, 8, 6, 4]
 
 barr.interpolation = JobSchema.InterpolationType.STEP
 barr.plot_position()
 
 barr.interpolation = JobSchema.InterpolationType.CUBIC
 barr.plot_position()
 ```
 
-As you can see above, 'STEP' style interpolation gives a "jumpy" barrier that changes position at discrete times.  Other interpolation options, like 'SMOOTH' (which is functionally equivalent to 'CUBIC'), give rise to a continually varying barrier position (and height/width).  The full list of interpolation options is as follows:
-
+As you can see above, 'STEP' style interpolation gives a "jumpy" barrier that changes position at discrete times. Other interpolation options, like 'SMOOTH' (which is functionally equivalent to 'CUBIC'), give rise to a continually varying barrier position (and height/width). The full list of interpolation options is as follows:
 
 ```python
 print([e.value for e in JobSchema.InterpolationType])
 ```
 
 ## The Optical Landscape Object
 
-Another Oqtant job primitive is the (singular) 'OpticalLandscape' object.  This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment.  However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.    
+Another OqtantJob primitive is the (singular) 'OpticalLandscape' object. This construct is similar to the optical barriers list in the sense that it instructs the experiment to apply 1D optical potentials, in the form of painted blue-detuned light, to the condensate over the course of the experiment. However, now the user (you!) is free to specify a list of positions and corresponding potential energies at specified times, instead of being limited to the concept of a singular barrier or combination of multiple barriers.
 
-The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together *in time* (if there exists more than one underlying landscape).  Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.   
+The OpticalLandscape object consists of a list of individual potential-energy landscapes and an interpolation option on how those landscapes connect together _in time_ (if there exists more than one underlying landscape). Let us begin by constructing a couple Landscape objects, from which we will compose the OpticalLandscape container object.
 
 ### Construction
 
-We can directly compose an *OpticalLandscape* object, as above with the *Barrier* object(s), or we can compose the constituent Landscape objects and then compose the full *OpticalLandscape* object accordingly:
-
+We can directly compose an _OpticalLandscape_ object, as above with the _Barrier_ object(s), or we can compose the constituent Landscape objects and then compose the full _OpticalLandscape_ object accordingly:
 
 ```python
 landscape_1 = JobSchema.Landscape(
     time_ms = 1.0,
     positions_um = [-50, -25, 0, 25, 50],
     potentials_khz = [100, 50, 0, 50, 100],
     spatial_interpolation = 'LINEAR'
@@ -281,57 +268,53 @@
     interpolation = 'LINEAR',
     landscapes = [landscape_1, landscape_2]
 )
 ```
 
 ### Inspecting consituent 'Landscape' objects
 
-
 ```python
 print(landscape_1.get_potential_at_position(10))
 print(landscape_2.get_potential_at_positions([-75, -50, -25, 0, 25, 50, 75]))
 ```
 
-
 ```python
 landscape_1.plot_potential()
 landscape_2.plot_potential(y_limits = [-1, 101])
 ```
 
-In the plots above, you can see the potential energy profile specified by our two Landscape objects.  The underlying data shows up as points, with the overall profile determined by the values of these points and the chosen value for *spatial_interpolation*.  The same values are available here as were for (temporal) interpolation options for Barrier objects.  
+In the plots above, you can see the potential energy profile specified by our two Landscape objects. The underlying data shows up as points, with the overall profile determined by the values of these points and the chosen value for _spatial_interpolation_. The same values are available here as were for (temporal) interpolation options for Barrier objects.
 
 ### Understanding the time dependence of the composed OpticalLandscape object
 
-The time-dependence of the overall optical potential-energy landscape, as derived from the individual *landscapes[]* list, is somewhat complicated.  As for *Barrier* and other similar objects, any temporal extrapolation (behavior for data outside the defined time period, i.e. before the first or after the last elements of the *landscapes[]* list) results in zero potential  (in the absence of any other sources, such as Barriers).  Therefore, the only way to get a non-zero painted potential optical landscape is to define at least two landscapes that can be interpolated between.  To hold a static (unchanging) potential during a period of the experiment, one would define two elements of the *landscapes[]* list with identical potential energy profiles but differing times, with the potential being applied between those two times.  If one desires the potential to change dynamically, then adjacent elements of the *landscapes[]* list (elements with the nearest *time_ms* values) should define the snapshots of the desired potential at the temporal endpoints.  In between these endpoints the potential landscape is interpolated point-by-point (in position) according to the user-specified value for *interpolation*.  This process continues so that, at the specified times of the elements of *landscapes[]*, the overall optical potential energy landscape instantaneously equal to those individual landscapes.  
-
-In our example above, with linear interpolation, this means that there will be a period of no optical potential between 0 and 1 ms, our *landscape_1* potential will start being applied at 1 ms, this potential will smoothly (linearly, in this case) morph into the *landscape_2* potential between 1 and 10 ms, and then this potential landscape will be held until the end of the experiment.  Let us use oqtant's visualization functions to inspect this behavior to make it clear.       
+The time-dependence of the overall optical potential-energy landscape, as derived from the individual _landscapes[]_ list, is somewhat complicated. As for _Barrier_ and other similar objects, any temporal extrapolation (behavior for data outside the defined time period, i.e. before the first or after the last elements of the _landscapes[]_ list) results in zero potential (in the absence of any other sources, such as Barriers). Therefore, the only way to get a non-zero painted potential optical landscape is to define at least two landscapes that can be interpolated between. To hold a static (unchanging) potential during a period of the experiment, one would define two elements of the _landscapes[]_ list with identical potential energy profiles but differing times, with the potential being applied between those two times. If one desires the potential to change dynamically, then adjacent elements of the _landscapes[]_ list (elements with the nearest _time_ms_ values) should define the snapshots of the desired potential at the temporal endpoints. In between these endpoints the potential landscape is interpolated point-by-point (in position) according to the user-specified value for _interpolation_. This process continues so that, at the specified times of the elements of _landscapes[]_, the overall optical potential energy landscape instantaneously equal to those individual landscapes.
 
+In our example above, with linear interpolation, this means that there will be a period of no optical potential between 0 and 1 ms, our _landscape_1_ potential will start being applied at 1 ms, this potential will smoothly (linearly, in this case) morph into the _landscape_2_ potential between 1 and 10 ms, and then this potential landscape will be held until the end of the experiment. Let us use oqtant's visualization functions to inspect this behavior to make it clear.
 
 ```python
 optical_landscape.plot_potential(time = 0.9)
 optical_landscape.plot_potential(time = 1)
 optical_landscape.plot_potential(time = 3)
 optical_landscape.plot_potential(time = 5)
 optical_landscape.plot_potential(time = 7)
 optical_landscape.plot_potential(time = 9)
 optical_landscape.plot_potential(time = 11)
 ```
 
-As descibed above, we can see zero overall potential both before the first and after the last times of the individual Landscape objects.  At 1 ms, the first Landscape is assumed.  The potential landscape then morphs into our second Landscape object at t = 10 ms.  
+As descibed above, we can see zero overall potential both before the first and after the last times of the individual Landscape objects. At 1 ms, the first Landscape is assumed. The potential landscape then morphs into our second Landscape object at t = 10 ms.
 
-## Laser Objects 
+## Laser Objects
 
-The last data structure to explore here is the *lasers[]* list in the job data.  This is a list of *Laser* objects.  Currently, the user is limited to a single element/laser.  
+The last data structure to explore here is the _lasers[]_ list in the job data. This is a list of _Laser_ objects. Currently, the user is limited to a single element/laser.
 
 ### Construction
 
-Let us begin by constructing a *Laser* object, which gives the user control over near-resonant laser light applied to the atoms over the course of the experiment.  This differs from the painted potential laser, which is far off-resonance in order to apply potential energy landscapes and barriers to the trapped condensate.  Resonant or near-resonant light, on the other hand, results in scattering of photons from the light field by the atoms.  This is useful, for example, in TRANSISTOR jobs where we want to remove atoms from some spatial region of the trap using a so-called TERMINATOR laser.  
-
-A *Laser* object gives the user control of the time-dependence of laser light applied to the atomic ensemble, including the time-dependent intensity and detuning given by a series of *pulse* objects specified by a *pulses[]* list.  We can construct such an object as follows:
+Let us begin by constructing a _Laser_ object, which gives the user control over near-resonant laser light applied to the atoms over the course of the experiment. This differs from the painted potential laser, which is far off-resonance in order to apply potential energy landscapes and barriers to the trapped condensate. Resonant or near-resonant light, on the other hand, results in scattering of photons from the light field by the atoms. This is useful, for example, in TRANSISTOR jobs where we want to remove atoms from some spatial region of the trap using a so-called TERMINATOR laser.
 
+A _Laser_ object gives the user control of the time-dependence of laser light applied to the atomic ensemble, including the time-dependent intensity and detuning given by a series of _pulse_ objects specified by a _pulses[]_ list. We can construct such an object as follows:
 
 ```python
 pulse_1 = JobSchema.Pulse(
     times_ms = [1, 1.5, 2, 3],
     intensities_mw_per_cm2 = [0, 10, 2, 0],
     detuning_mhz = 5,
     interpolation = 'SMOOTH'
@@ -353,11 +336,14 @@
 
 laser = JobSchema.Laser(
     type = 'TERMINATOR',
     pulses = [pulse_1, pulse_2, pulse_3]
 )
 ```
 
-
 ```python
 laser.plot_intensity()
 ```
+
+```python
+
+```
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9845001714429511%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Oqtant Walkthrough 4: RF Sweep Experimentation "*

 * *            "#\\n'), (2, '### This walkthrough covers creating and executings an RF Sweep "*

 * *            "Experiement using Ultracold Matter OqtantJobs ###\\n'), (6, '*Batch job functionality "*

 * *            "is available for users with a subscription tier of EXPLORER or INNOVATOR.*\\n'), (7, "*

 * *            "'\\n'), (8, '`get_user_token` creates a temporary web server on your machine to "*

 * *            'handle authentica […]*

```diff
@@ -1,32 +1,33 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Oqtant Walkthrough 4: BEC Experimentation #\n",
+                "# Oqtant Walkthrough 4: RF Sweep Experimentation #\n",
                 "\n",
-                "### This walkthrough covers best practices for conducting experiments on the Oqtant system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis. ###\n",
+                "### This walkthrough covers creating and executings an RF Sweep Experiement using Ultracold Matter OqtantJobs ###\n",
                 "\n",
                 "For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md\n",
                 "\n",
-                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*"
+                "*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*\n",
+                "\n",
+                "`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Sign into Oqtant\n",
+                "# Authenticate with Oraqle\n",
                 "\n",
-                "## Before you can view and submit jobs you must first sign into your Oqtant account\n",
+                "## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account\n",
                 "\n",
-                "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out of that tab and return to this notebook."
+                "Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -40,39 +41,38 @@
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
                 "    round_sig\n",
                 ")\n",
                 "\n",
-                "token = get_user_token()"
+                "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Creating a Oqtant Client Instance ##\n",
+                "## Creating a OqtantClient Instance ##\n",
                 "\n",
-                "### After successfully logged in, create an authorized session with the Oqtant Client ###\n",
-                "- the oqtant_client interacts with the Oqtant server to perform remote lab functions. \n",
-                "- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session"
+                "### After successfully logging in, create an authorized session with the OqtantClient ###\n",
+                "- The OqtantClient class interacts with the Oraqle server to perform remote lab functions.\n",
+                "- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "oqtant_client = get_oqtant_client(token)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Design a simple experiment ##\n",
                 "\n",
                 "For this example, we will investigate the effect of altering the final frequency of the RF knife on the evolution of the condensate and its temperature. \n",
                 "\n",
@@ -82,15 +82,14 @@
                 "### Observables ###\n",
                 " - TOF images\n",
                 " - Temperature (calculated from TOF images)\n",
                 " - Atom number and condensate fraction (calculated from TOF images)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let us explore the interplay between the final RF evaporation frequency and the resulting cloud temperature in a one-parameter scan \"experiment\".  "
             ]
         },
         {
@@ -99,38 +98,37 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "final_rf_freqs_mhz = [0.07, 0.03, 0.05]"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Performing the experiment ## \n",
                 "\n",
                 "Depending on your subscription tier there are two different options for performing this experiment\n",
                 "\n",
-                "- Users in the GROUND tier can create 3 separate jobs with each job's input representing a step in the experiment\n",
+                "- Users in the GROUND tier can create 3 separate OqtantJobs with each job's input representing a step in the experiment\n",
                 "\n",
-                "- Users in the EXPLORER and INNOVATOR tiers can create a single job that contains three inputs for all of the steps in the experiment\n",
+                "- Users in the EXPLORER and INNOVATOR tiers can create a single OqtantJob that contains three inputs for all of the steps in the experiment\n",
                 "\n",
                 "The rest of this walkthrough will showcase how to perform and analyze the experiment using both options.\n",
                 "\n",
                 "Both submission options / subscription tiers will make use of a 'base' job definition:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "base_bec_job = {\n",
+                "base_ultracold_matter_job = {\n",
                 "    \"name\": \"RF Sweep Experiment\",\n",
                 "    \"job_type\": \"BEC\",\n",
                 "    \"inputs\": [\n",
                 "        {\n",
                 "            \"values\": {\n",
                 "                \"time_of_flight_ms\": 8.0,\n",
                 "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
@@ -147,112 +145,112 @@
                 "            },\n",
                 "        }\n",
                 "    ],\n",
                 "}"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Generating parameter scan jobs as GROUND ## \n",
+                "## Generating parameter scan OqtantJobs as GROUND ## \n",
                 "\n",
-                "This experiment will consist of 3 jobs and no repeated trials. Below we will create a BEC job with default parameters and copy it three times. Once we have three instances of the same job we can update the inputs for each one to match the steps in the experiment.\n",
+                "This experiment will consist of 3 OqtantJobs and no repeated trials. Below we will take the dictionary with deafult Ultracold Matter job parameters and copy it three times. Once we have three instances of the same dictionary we can update the inputs for each one to match the steps in the experiment.\n",
                 "\n",
-                "Print out the jobs once updated to review the input parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
+                "Print out the OqtantJobs once updated to review the input parameters before submitting to run on the Oraqle hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "njobs = len(final_rf_freqs_mhz)\n",
                 "jobs = []\n",
                 "for step in range(njobs):\n",
-                "    job = copy.deepcopy(base_bec_job)\n",
+                "    job = copy.deepcopy(base_ultracold_matter_job)\n",
                 "    job[\"name\"] = \"RF sweep experiment step \" + str(step+1)\n",
                 "    job[\"notes\"] = \"RF sweep experiment step \" + str(step+1) + \" of \" + str(njobs)\n",
                 "    job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][-1] = final_rf_freqs_mhz[step]\n",
                 "    jobs.append(job)\n",
                 "\n",
                 "jobs = [oqtant_client.generate_oqtant_job(job=job) for job in jobs]\n",
                 "    \n",
                 "for job in jobs:\n",
                 "    print(\n",
                 "        job.name,\n",
                 "        \"\\n\",\n",
                 "        job.inputs[0].values,\n",
                 "        \"\\n\"\n",
-                "    )"
+                "    )\n",
+                "    \n",
+                "batch_job = oqtant_client.generate_oqtant_job(job=batch_job)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Generating job parameters as EXPLORER / INNOVATOR ## \n",
+                "## Generating OqtantJob parameters as EXPLORER / INNOVATOR ## \n",
                 "\n",
-                "This experiment will consist of a single job with 3 inputs and no repeated trials. Below we will create an input object with default BEC parameters. Next we will copy this input three times and make updates to match the steps in the experiment.\n",
+                "This experiment will consist of a single OqtantJob with 3 inputs and no repeated trials. Below we will create an input object with default Ultracold Matter parameters. Next we will copy this input three times and make updates to match the steps in the experiment.\n",
                 "\n",
-                "Print out the job inputs once updated to review the parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
+                "Print out the job inputs once updated to review the parameters before submitting to run on the Oraqle hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "batch_job = copy.deepcopy(base_bec_job)\n",
+                "batch_job = copy.deepcopy(base_ultracold_matter_job)\n",
                 "batch_job[\"inputs\"] = []\n",
                 "batch_job[\"name\"] = \"RF sweep experiment\"\n",
                 "batch_job[\"notes\"] = \"RF sweep experiment as sequential runs\"\n",
                 "\n",
                 "for step in range(njobs):\n",
-                "    input = copy.deepcopy(base_bec_job[\"inputs\"][0])\n",
+                "    input = copy.deepcopy(base_ultracold_matter_job[\"inputs\"][0])\n",
                 "    input[\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][-1] = final_rf_freqs_mhz[step]\n",
                 "    batch_job[\"inputs\"].append(input)\n",
                 "\n",
                 "print(batch_job[\"name\"])\n",
                 "for input in batch_job[\"inputs\"]:\n",
                 "    print(\n",
                 "        input,\n",
                 "        \"\\n\"\n",
                 "    )\n",
                 "    \n",
                 "batch_job = oqtant_client.generate_oqtant_job(job=batch_job)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "\n",
                 "## Accessing the fields of an OqtantJob ##\n",
                 "\n",
-                "The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) its output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.\n",
+                "The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) it's output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.\n",
                 "\n",
                 "To get the input parameters for this experiment you would do the following:\n",
                 "\n",
-                "**JOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**\n",
+                "`OqtantJob.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST`\n",
                 "\n",
                 "All OqtantJobs contain the same high-level input parameters, with some being empty depending on the type of job.\n",
                 "\n",
-                "For BEC jobs the following parameters are used and required:\n",
+                "For Ultracold Matter (BEC) jobs the following parameters are used and required:\n",
                 "\n",
                 "- end_time_ms\n",
                 "- image_type\n",
                 "- time_of_flight_ms\n",
                 "- rf_evaporation\n",
                 "\n",
-                "For BARRIER jobs the following parameters are used and required:\n",
+                "For Barrier Manipulator (BARRIER) jobs the following parameters are used and required:\n",
                 "\n",
                 "- end_time_ms\n",
                 "- image_type\n",
                 "- time_of_flight_ms\n",
                 "- rf_evaporation\n",
                 "- optical_barriers\n",
                 "\n",
@@ -285,25 +283,25 @@
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Submiting jobs and storing the job IDs as GROUND ##\n",
+                "## Submiting OqtantJobs and storing the their IDs as GROUND ##\n",
                 "\n",
-                "Once you are ready to submit the experiment jobs you will have two options. One will be to track the status of them as they are processed and the other will be to not track their status. When you choose to track the status of your submitted jobs the function will not return immediately and will instead continuously ping the Albert service until all of the jobs have finished.\n",
+                "Once you are ready to submit the experiment jobs you will have two options. One will be to track the status of them as they are processed and the other will be to not track their status. When you choose to track the status of your submitted jobs the function will not return immediately and will instead continuously ping the Oraqle service until all of the jobs have finished.\n",
                 "\n",
-                "Track status: **track_status=True**\n",
+                "Track status: `track_status=True`\n",
                 "\n",
-                "Dont track status: **track_status=False**\n",
+                "Dont track status: `track_status=False`\n",
                 "\n",
                 "Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.\n",
                 "\n",
-                "Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing."
+                "Option to run the jobs and wait for results (`track_status=True`) OR submit the jobs and return later to retrieve the results (`track_status=False`). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -319,25 +317,25 @@
                 "        filewriter.write(experiment_step_job_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Submiting jobs and storing the job IDs as EXPLORER / INNOVATOR ##\n",
+                "## Submiting OqtantJobs and storing their IDs as EXPLORER / INNOVATOR ##\n",
                 "\n",
-                "Once you are ready to submit the experiment job you will have two options. One will be to track the status of it as it is being processed and the other will be to not track it's status. When you choose to track the status of your submitted job the function will not return immediately and will instead continuously ping the Albert service until the job has finished.\n",
+                "Once you are ready to submit the experiment job you will have two options. One will be to track the status of it as it is being processed and the other will be to not track it's status. When you choose to track the status of your submitted job the function will not return immediately and will instead continuously ping the Oraqle service until the job has finished.\n",
                 "\n",
-                "Track status: **track_status=True**\n",
+                "Track status: `track_status=True`\n",
                 "\n",
-                "Dont track status: **track_status=False**\n",
+                "Dont track status: `track_status=False`\n",
                 "\n",
                 "Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.\n",
                 "\n",
-                "Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing."
+                "Option to run the jobs and wait for results (`track_status=True`) OR submit the jobs and return later to retrieve the results (`track_status=False`). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -352,17 +350,17 @@
                 "    filewriter.write(rf_sweep_experiment_job_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Load results from completed jobs ##\n",
+                "## Load results from completed OqtantJobs ##\n",
                 "\n",
-                "Use **load_jobs_from_id** to retrieve jobs in any state from a previous run. "
+                "Use `OqtantClient.load_jobs_from_id()` to retrieve jobs in any state from a previous run. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -376,17 +374,17 @@
                 "    print(\"id: \", job_id, job.job_type, job.status)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Plot completed jobs ##\n",
+                "## Plot completed OqtantJobs ##\n",
                 "\n",
-                "When job status is COMPLETE above, plot the results"
+                "Once your OqtantJob(s) status is COMPLETE, plot the results"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -424,15 +422,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.11.4"
         },
         "vscode": {
             "interpreter": {
                 "hash": "9d324fb170b849c0db1b04a4eaa5a753613b2d729749991e51e49ca6f200afbc"
             }
         }
     },
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_4_experiment.md` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Oqtant Walkthrough 3: BEC Experimentation #
+# Oqtant Walkthrough 4: RF Sweep Experimentation
 
-### This walkthrough covers best practices for conducting experiments on the Oqtant system, including submitting batches of jobs, tracking experiment progress, and handling output data for later analysis. ###
+### This walkthrough covers creating and executings an RF Sweep Experiement using Ultracold Matter OqtantJobs
 
 For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
 
-*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
+_Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR._
 
-# Sign into Oqtant
+`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085.
 
-## Before you can view and submit jobs you must first sign into your Oqtant account
+# Authenticate with Oraqle
 
-Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out of that tab and return to this notebook.
+## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account
 
+Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from matplotlib import pyplot as plt
 import copy
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from bert_schemas import job as JobSchema
@@ -23,62 +24,62 @@
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 
-token = get_user_token()
+token = get_user_token(auth_server_port=8080)
 ```
 
-## Creating a Oqtant Client Instance ##
+## Creating a OqtantClient Instance
 
-### After successfully logged in, create an authorized session with the Oqtant Client ###
-- the oqtant_client interacts with the Oqtant server to perform remote lab functions.
-- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
+### After successfully logging in, create an authorized session with the OqtantClient
 
+- The OqtantClient class interacts with the Oraqle server to perform remote lab functions.
+- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Design a simple experiment ##
+## Design a simple experiment
 
 For this example, we will investigate the effect of altering the final frequency of the RF knife on the evolution of the condensate and its temperature.
 
-### Variables ###
+### Variables
+
 1. The final frequency of the rf knife
 
-### Observables ###
- - TOF images
- - Temperature (calculated from TOF images)
- - Atom number and condensate fraction (calculated from TOF images)
+### Observables
 
-Let us explore the interplay between the final RF evaporation frequency and the resulting cloud temperature in a one-parameter scan "experiment".
+- TOF images
+- Temperature (calculated from TOF images)
+- Atom number and condensate fraction (calculated from TOF images)
 
+Let us explore the interplay between the final RF evaporation frequency and the resulting cloud temperature in a one-parameter scan "experiment".
 
 ```python
 final_rf_freqs_mhz = [0.07, 0.03, 0.05]
 ```
 
-## Performing the experiment ##
+## Performing the experiment
 
 Depending on your subscription tier there are two different options for performing this experiment
 
-- Users in the GROUND tier can create 3 separate jobs with each job's input representing a step in the experiment
+- Users in the GROUND tier can create 3 separate OqtantJobs with each job's input representing a step in the experiment
 
-- Users in the EXPLORER and INNOVATOR tiers can create a single job that contains three inputs for all of the steps in the experiment
+- Users in the EXPLORER and INNOVATOR tiers can create a single OqtantJob that contains three inputs for all of the steps in the experiment
 
 The rest of this walkthrough will showcase how to perform and analyze the experiment using both options.
 
 Both submission options / subscription tiers will make use of a 'base' job definition:
 
-
 ```python
-base_bec_job = {
+base_ultracold_matter_job = {
     "name": "RF Sweep Experiment",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
@@ -94,99 +95,97 @@
                 "lasers": None,
             },
         }
     ],
 }
 ```
 
-## Generating parameter scan jobs as GROUND ##
-
-This experiment will consist of 3 jobs and no repeated trials. Below we will create a BEC job with default parameters and copy it three times. Once we have three instances of the same job we can update the inputs for each one to match the steps in the experiment.
+## Generating parameter scan OqtantJobs as GROUND
 
-Print out the jobs once updated to review the input parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
+This experiment will consist of 3 OqtantJobs and no repeated trials. Below we will take the dictionary with deafult Ultracold Matter job parameters and copy it three times. Once we have three instances of the same dictionary we can update the inputs for each one to match the steps in the experiment.
 
+Print out the OqtantJobs once updated to review the input parameters before submitting to run on the Oraqle hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
 
 ```python
 njobs = len(final_rf_freqs_mhz)
 jobs = []
 for step in range(njobs):
-    job = copy.deepcopy(base_bec_job)
+    job = copy.deepcopy(base_ultracold_matter_job)
     job["name"] = "RF sweep experiment step " + str(step+1)
     job["notes"] = "RF sweep experiment step " + str(step+1) + " of " + str(njobs)
     job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"][-1] = final_rf_freqs_mhz[step]
     jobs.append(job)
 
 jobs = [oqtant_client.generate_oqtant_job(job=job) for job in jobs]
 
 for job in jobs:
     print(
         job.name,
         "\n",
         job.inputs[0].values,
         "\n"
     )
-```
 
-## Generating job parameters as EXPLORER / INNOVATOR ##
+batch_job = oqtant_client.generate_oqtant_job(job=batch_job)
+```
 
-This experiment will consist of a single job with 3 inputs and no repeated trials. Below we will create an input object with default BEC parameters. Next we will copy this input three times and make updates to match the steps in the experiment.
+## Generating OqtantJob parameters as EXPLORER / INNOVATOR
 
-Print out the job inputs once updated to review the parameters before submitting to run on the Oqtant hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
+This experiment will consist of a single OqtantJob with 3 inputs and no repeated trials. Below we will create an input object with default Ultracold Matter parameters. Next we will copy this input three times and make updates to match the steps in the experiment.
 
+Print out the job inputs once updated to review the parameters before submitting to run on the Oraqle hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
 
 ```python
-batch_job = copy.deepcopy(base_bec_job)
+batch_job = copy.deepcopy(base_ultracold_matter_job)
 batch_job["inputs"] = []
 batch_job["name"] = "RF sweep experiment"
 batch_job["notes"] = "RF sweep experiment as sequential runs"
 
 for step in range(njobs):
-    input = copy.deepcopy(base_bec_job["inputs"][0])
+    input = copy.deepcopy(base_ultracold_matter_job["inputs"][0])
     input["values"]["rf_evaporation"]["frequencies_mhz"][-1] = final_rf_freqs_mhz[step]
     batch_job["inputs"].append(input)
 
 print(batch_job["name"])
 for input in batch_job["inputs"]:
     print(
         input,
         "\n"
     )
 
 batch_job = oqtant_client.generate_oqtant_job(job=batch_job)
 ```
 
+## Accessing the fields of an OqtantJob
 
-## Accessing the fields of an OqtantJob ##
-
-The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) its output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.
+The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) it's output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.
 
 To get the input parameters for this experiment you would do the following:
 
-**JOB.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST**
+`OqtantJob.inputs[desired-input-index].values.FIELD_FROM_BELOW_LIST`
 
 All OqtantJobs contain the same high-level input parameters, with some being empty depending on the type of job.
 
-For BEC jobs the following parameters are used and required:
+For Ultracold Matter (BEC) jobs the following parameters are used and required:
 
 - end_time_ms
 - image_type
 - time_of_flight_ms
 - rf_evaporation
 
-For BARRIER jobs the following parameters are used and required:
+For Barrier Manipulator (BARRIER) jobs the following parameters are used and required:
 
 - end_time_ms
 - image_type
 - time_of_flight_ms
 - rf_evaporation
 - optical_barriers
 
 All of these inputs have constraints on them which are validated when given values. To view these constraints you can refer to 'Schemas' section of our OpenAPI Documentation: https://albert-dev.coldquanta.com/api/docs
 
-
 ```python
 # if using the GROUND option
 for job in jobs:
     print(
         job.name,
         job.inputs[0].values.rf_evaporation.frequencies_mhz[-1],
         job.inputs[0].values.time_of_flight_ms
@@ -200,98 +199,92 @@
         batch_job.name,
         f"input run #{i + 1}",
         input.values.rf_evaporation.frequencies_mhz[-1],
         input.values.time_of_flight_ms
     )
 ```
 
-## Submiting jobs and storing the job IDs as GROUND ##
+## Submiting OqtantJobs and storing the their IDs as GROUND
 
-Once you are ready to submit the experiment jobs you will have two options. One will be to track the status of them as they are processed and the other will be to not track their status. When you choose to track the status of your submitted jobs the function will not return immediately and will instead continuously ping the Albert service until all of the jobs have finished.
+Once you are ready to submit the experiment jobs you will have two options. One will be to track the status of them as they are processed and the other will be to not track their status. When you choose to track the status of your submitted jobs the function will not return immediately and will instead continuously ping the Oraqle service until all of the jobs have finished.
 
-Track status: **track_status=True**
+Track status: `track_status=True`
 
-Dont track status: **track_status=False**
+Dont track status: `track_status=False`
 
 Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.
 
-Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
-
+Option to run the jobs and wait for results (`track_status=True`) OR submit the jobs and return later to retrieve the results (`track_status=False`). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
 
 ```python
 # track the status
 rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=jobs, track_status=True)
 
 # dont track the status
 # rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=False)
 
 with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:
     for experiment_step_job_id in rf_sweep_experiment_job_ids:
         filewriter.write(experiment_step_job_id)
 ```
 
-## Submiting jobs and storing the job IDs as EXPLORER / INNOVATOR ##
+## Submiting OqtantJobs and storing their IDs as EXPLORER / INNOVATOR
 
-Once you are ready to submit the experiment job you will have two options. One will be to track the status of it as it is being processed and the other will be to not track it's status. When you choose to track the status of your submitted job the function will not return immediately and will instead continuously ping the Albert service until the job has finished.
+Once you are ready to submit the experiment job you will have two options. One will be to track the status of it as it is being processed and the other will be to not track it's status. When you choose to track the status of your submitted job the function will not return immediately and will instead continuously ping the Oraqle service until the job has finished.
 
-Track status: **track_status=True**
+Track status: `track_status=True`
 
-Dont track status: **track_status=False**
+Dont track status: `track_status=False`
 
 Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.
 
-Option to run the jobs and wait for results (**track_status=True**) OR submit the jobs and return later to retrieve the results (**track_status=False**). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
-
+Option to run the jobs and wait for results (`track_status=True`) OR submit the jobs and return later to retrieve the results (`track_status=False`). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
 
 ```python
 # track the status
 rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[batch_job], track_status=True)[0]
 
 # dont track the status
 # rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=False)[0]
 
 with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:
     filewriter.write(rf_sweep_experiment_job_id)
 ```
 
-## Load results from completed jobs ##
-
-Use **load_jobs_from_id** to retrieve jobs in any state from a previous run.
+## Load results from completed OqtantJobs
 
+Use `OqtantClient.load_jobs_from_id()` to retrieve jobs in any state from a previous run.
 
 ```python
 with open('bec_rf_sweep_experiment.txt', 'r') as filereader:
     for line in filereader:
         # remove linebreak which is the last character of the string
         oqtant_client.load_job_from_id(line)
+
 for job_id, job in oqtant_client.active_jobs.items():
     print("id: ", job_id, job.job_type, job.status)
 ```
 
-## Plot completed jobs ##
-
-When job status is COMPLETE above, plot the results
+## Plot completed OqtantJobs
 
+Once your OqtantJob(s) status is COMPLETE, plot the results
 
 ```python
 for a, job in oqtant_client.active_jobs.items():
     if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:
         job.atoms_2dplot()
         job.atoms_sliceplot()
+
 # by default jobs that are loaded will only contain the first input/output entry
 # if you have more than one input for a job you can view its details by specifying the 'run' like below
 desired_input_run = 2 # here we are asking for the second input/output entry
 with open('bec_rf_sweep_experiment.txt', 'r') as filereader:
     for line in filereader:
         # remove linebreak which is the last character of the string
         oqtant_client.load_job_from_id(line, run=desired_input_run)
+
 # now we can display the second input/output entry results
 for a, job in oqtant_client.active_jobs.items():
     if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:
         job.atoms_2dplot()
         job.atoms_sliceplot()
 ```
-
-
-```python
-
-```
```

### Comparing `oqtant-0.15.1/documentation/walkthroughs/walkthrough_5_optimization.md` & `oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Oqtant Walkthrough 5: BEC Optimization #
+# Oqtant Walkthrough 5: Ultracold Matter Optimization
 
-### This walkthrough reviews authorizing an Oqtant session and an example of optimization for BEC. ###
+### This walkthrough covers optimization of Ultracold Matter OqtantJobs.
 
 For more information about Oqtant refer to our documentation: https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/README.md
 
-*Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR.*
+_Batch job functionality is available for users with a subscription tier of EXPLORER or INNOVATOR._
 
-# Sign into Oqtant
+`get_user_token` creates a temporary web server on your machine to handle authenticating with Oraqle. By default this server will run on port 8080, if that port is unavailable you can edit the `get_user_token` default port `token = get_user_token(auth_server_port=8080)` with one of the following: 8081, 8082, 8083, 8084, 8085.
 
-## Before you can view and submit jobs you must first sign into your Oqtant account
+# Authenticate with Oraqle
 
-Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
+## Before you can view and submit OqtantJobs you must first authenticate with your Oraqle account
 
+Run the below cell to be re-directed to our login page and provide your account credentials. Once authenticated you can safely close out that tab and return to this notebook.
 
 ```python
 from sklearn.gaussian_process import GaussianProcessRegressor as GPR
 from matplotlib import pyplot as plt
 from scipy.optimize import minimize
 from warnings import catch_warnings
 from warnings import simplefilter
@@ -32,46 +33,45 @@
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
     round_sig
 )
 import csv
 
-token = get_user_token()
+token = get_user_token(auth_server_port=8080)
 ```
 
-## Creating a Oqtant Client Instance ##
+## Creating a OqtantClient Instance
 
-### After successful login, create an authorized session with the Oqtant Client ###
-- the oqtant_client interacts with the Oraqle server to perform remote lab functions.
-- the oqtant_client object also contains all the jobs which have been submitted, run, or loaded (from database or file) during this python session
+### After successfully logging in, create an authorized session with the OqtantClient
 
+- The OqtantClient class interacts with the Oraqle server to perform remote lab functions.
+- The OqtantClient object also contains all the OqtantJobs which have been submitted, run, or loaded (from database or file) during this python session
 
 ```python
 oqtant_client = get_oqtant_client(token)
 ```
 
-## Define a cost function for optimization ##
+## Define a cost function for optimization
 
-A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script 
+A cost function is a metric calculated for the system of interest which is lowered over time via some optimization script
 
-Larger value = Good:  Condensed and total atom number, condensate fraction
+Larger value = Good: Condensed and total atom number, condensate fraction
 Smaller value = Good: Thermal atom number, temperature
 
-Ad hoc Cost function: **C = (Nth*T)/Nc**
-
-### cost_func_5D ###
-This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies.
+Ad hoc Cost function: **C = (Nth\*T)/Nc**
 
+### cost_func_5D
 
+This cost function is for a 5-dimensional optimization space, where the 5 dimensions are the RF corner frequencies.
 
 ```python
 costs_5D = []
 
-base_bec_job = {
+base_ultracold_matter_job = {
     "name": "Example Ultracold Matter Generator Job",
     "job_type": "BEC",
     "inputs": [
         {
             "values": {
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
@@ -87,86 +87,79 @@
                 "lasers": None,
             },
         }
     ],
 }
 
 def cost_func_5D(RF_freqs = [17.0, 8.0, 4.0, 1.2, 0.045]): # added 5th power to default
-    base_bec_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = list(RF_freqs)
-    print(base_bec_job)
-    job = oqtant_client.generate_oqtant_job(job=base_bec_job)
+    base_ultracold_matter_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = list(RF_freqs)
+    print(base_ultracold_matter_job)
+    job = oqtant_client.generate_oqtant_job(job=base_ultracold_matter_job)
     [job_id] = oqtant_client.run_jobs(job_list=[job], track_status=True)
     job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values
     Nth = job_output.thermal_atom_number
     T = job_output.temperature_uk
     Nc = job_output.condensed_atom_number
     C = (Nth*T)/Nc
     costs_5D.append(C)
     return C
 ```
 
-## Set bounds for optimization ##
-
-Bounds will prevent invalid jobs parameters from being submitted to the job runner.
+## Set bounds for optimization
 
+Bounds will prevent invalid jobs parameters from being submitted to the Oraqle.
 
 ```python
 bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))
 ```
 
-## Choose an optimization algorithm ##
+## Choose an optimization algorithm
 
-Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:  
+Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:
 
- - L-BFGS-B
- - TNC
- - COBYLA
- - SLSQP
+- L-BFGS-B
+- TNC
+- COBYLA
+- SLSQP
 
+## Provide initial conditions and max iterations
 
- ## Provide initial conditions and max iterations ##
-
- I chose the web app default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period.
-
+I chose the Oraqle web application's default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period.
 
 ```python
 res_5d = minimize(cost_func_5D, method="TNC", bounds=bnds_5d, x0 = [17,8,4,1.2,0.05], options={'maxiter':10})
 
 print("optimization results freq tuning:")
 print(res_5d)
 ```
 
-## Bayesian Optimization with a Gaussian Process model ##
-
+## Bayesian Optimization with a Gaussian Process model
 
-## Extract and shape the training data: ##
+## Extract and shape the training data:
 
 x_train : array-like of shape (n_samples, n_features) or list of object
 Feature vectors or other representations of training data (also required for prediction).
 
 y_train : array-like of shape (n_samples,) or (n_samples, n_targets)
 Target values in training data (also required for prediction)
 
-## Define a new target cost function ##
-
+## Define a new target cost function
 
 ```python
 def cost(Nc, Nth, T):
     C = (Nth*T)/Nc
     return C
 ```
 
-The optimization jobs run above will now be included in your list of currently active jobs:
-
+The optimization jobs run above will now be included in your list of currently active OqtantJobs:
 
 ```python
 oqtant_client.see_active_jobs()
 ```
 
-
 ```python
 x_train = []
 y_train = []
 for job_id in oqtant_client.active_jobs:
     job = oqtant_client.active_jobs[job_id]
     output = job.inputs[0].output.values
     condensed_atom_number = output.condensed_atom_number
@@ -174,92 +167,89 @@
     temperature_uk = output.temperature_uk
     input = job.inputs[0].values
     x_train.append(input.rf_evaporation.frequencies_mhz)
     y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))
 
 ```
 
-
 ```python
 # surrogate or approximation for the objective function
 def surrogate(model, X):
     # catch any warning generated when making a prediction
     with catch_warnings():
         # ignore generated warnings
         simplefilter("ignore")
         return model.predict(X, return_std=True)
 ```
 
-## Define an acquisition function ##
+## Define an acquisition function
 
-This is a score assigned to each candidate sample on the domain. 
+This is a score assigned to each candidate sample on the domain.
 
 The surrogate function can be used as an acquisition (minimizing the surrogate is the goal after all)
 
 OR
 
 An acquisition function can be used. 3 common options:
+
 - Probability of Improvement (PI).
 - Expected Improvement (EI).
 - Lower Confidence Bound (LCB).
 
-Here I chose probability of improvement 
+Here I chose probability of improvement
 
 **PI = cdf((mu – best_mu) / stdev)**
 
 Where PI is the probability of improvement, cdf() is the normal cumulative distribution function, mu is the mean of the surrogate function for a given sample x, stdev is the standard deviation of the surrogate function for a given sample x, and best_mu is the mean of the surrogate function for the best sample found so far.
 
-
 ```python
 def acquisition(X, Xsamples, model):
     # calculate the best surrogate score found so far
     yhat, _ = surrogate(model, X)
     best = max(yhat)
     # calculate mean and stdev via surrogate function
     mu, std = surrogate(model, Xsamples)
     #mu = mu[:, 0]
     # calculate the probability of improvement
     probs = norm.cdf((mu - best) / (std+1E-9))
     return probs
 ```
 
-## Define a domain ##
+## Define a domain
 
 This is the domain of the samples. This one point where we inject prior knowledge of the system from previous experience
 
-
 ```python
 domain = [(20.,15.),(12.,5.),(5.,2.),(1.9,0.2),(0.2,0.01),
           (500.,470.),(470.,460.),(459.,420.),(420.,350.)]
 
 def rand_domain_sample(domain):
     scale = domain[0]-domain[1]
     random_number = np.random.uniform()+(1E-9)
     sample = scale*random_number+domain[1]
     return sample
 ```
 
-## Define an optimizer on the acquisition function ##
-
+## Define an optimizer on the acquisition function
 
+Here I have chosen a random search over the domain, but other search algorithms can be used.
 
 ```python
 def optimize_acquisition(X, y, model, sample_population):
     # random search, generate random samples
     Xsamples = np.asarray([[rand_domain_sample(domain[i]) for i in range(len(X[0]))] for j in range(sample_population)])
     Xsamples = Xsamples.reshape(len(Xsamples), len(X[0]))
     # calculate the acquisition function for each sample
     scores = acquisition(X, Xsamples, model)
     # locate the index of the largest scores
     ix = np.argmax(scores)
     return Xsamples[ix]
 ```
 
-## Perform the optimization ##
-
+## Perform the optimization
 
 ```python
 X = x_train
 Y = y_train
 Oqtant_model = GPR()
 Oqtant_model.fit(x_train, y_train)
 
@@ -278,21 +268,24 @@
     # add the data to the dataset
     X = np.vstack((X, [x]))
     Y.append(actual)
     # update the model
     Oqtant_model.fit(X, Y)
 ```
 
-
 ```python
 # plot all samples and the final surrogate function
 plt.plot(cost[5:])
 #plt.yscale("log")
 plt.xlabel("function evaluations")
 plt.ylabel("Cost")
 plt.title("20 evaluations, 500 surrogate samples, 335pm 5_5_21")
 plt.savefig("335pm 5_5_21.png")
 plt.show()
 # best result
 ix = np.argmax(Y)
 print('Best Result:'+str([X[ix], Y[ix]]))
 ```
+
+```python
+
+```
```

### Comparing `oqtant-0.15.1/oqtant/oqtant_client.py` & `oqtant-0.16.1/oqtant/oqtant_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 from oqtant.settings import Settings
 from oqtant.util import exceptions as api_exceptions
 
 settings = Settings()
 
 
 class OqtantClient:
-    """Python class for interacting with Oqtant
+    """Python class for interacting with Oraqle
     This class contains tools for:
-        - Accessing all of the functionality of the Oqtant Web App (https://albert-dev.coldquanta.com)
+        - Accessing all of the functionality of the Oraqle Web App (https://albert-dev.coldquanta.com)
             - BARRIER (Barrier Manipulator) jobs
             - BEC (Ultracold Matter) jobs
         - Building parameterized (i.e. optimization) experiments using OqtantJobs
         - Submitting and retrieving OqtantJob results
     How Oqtant works:
         1.) Construct a single or list of OqtantJobs using 'generate_oqtant_job()'
-        2.) Run the single or list of OqtantJobs on the Oqtant hardware using 'run_jobs()'
+        2.) Run the single or list of OqtantJobs on the Oraqle hardware using 'run_jobs()'
             - There is a limit of 30 OqtantJobs per use of 'run_jobs()'
         3.) As OqtantJobs are running, the results are automatically stored in 'active_jobs'
             - The OqtantJobs stored in 'active_jobs' are available until the python session ends
         4.) If you choose to not track the status of OqtantJobs with 'run_jobs()' you can see the status
             of your session's active OqtantJobs with 'see_active_jobs()'
         5.) To operate on jobs submitted in a previous session you can load them into your 'active_jobs'
             by using either 'load_job_from_id()' or 'load_job_from_file()'
@@ -60,15 +60,15 @@
         """
         return {
             "Authorization": f"Bearer {self.token}",
             "X-Client-Version": version("oqtant"),
         }
 
     def get_job(self, job_id: str, run: int = 1) -> OqtantJob:
-        """Gets an OqtantJob from the Oqtant REST API. This will always be a targeted query
+        """Gets an OqtantJob from the Oraqle REST API. This will always be a targeted query
            for a specific run. If the run is omitted then this will always return the first
            run of the job. Will return results for any job regardless of it's status.
         Args:
             job_id (str): this is the external_id of the job to fetch
             run (int): the run to target, this defaults to the first run if omitted
         Returns:
             OqtantJob: an OqtantJob instance with the values of the job queried
@@ -90,15 +90,15 @@
         except (KeyError, ValidationError) as err:
             raise api_exceptions.ValidationError(f"Failed to get job {job_id}: {err}")
         return job
 
     def get_job_inputs_without_output(
         self, job_id: str, run: int | None = None, include_notes: bool = False
     ) -> dict:
-        """Gets an OqtantJob from the Oqtant REST API. This can return all runs within a job
+        """Gets an OqtantJob from the Oraqle REST API. This can return all runs within a job
            or a single run based on whether a run value is provided. The OqtantJobs returned
            will be converted to dictionaries and will not have any output data, even if
            they are complete. This is useful for taking an existing job and creating a new one
            based on it's input data.
         Args:
            job_id (str): this is the external_id of the job to fetch
            run (Union[int, None]): optional argument if caller wishes to only has a single run returned
@@ -144,15 +144,15 @@
         try:
             oqtant_job = OqtantJob(**job)
         except ValidationError as err:
             raise api_exceptions.ValidationError(f"Failed to generate OqtantJob: {err}")
         return oqtant_job
 
     def submit_job(self, *, job: OqtantJob) -> dict:
-        """Submits a single OqtantJob to the Oqtant REST API. Upon successful submission this
+        """Submits a single OqtantJob to the Oraqle REST API. Upon successful submission this
            function will return a dictionary containing the external_id of the job and it's
            position in the queue.
         Args:
            job (OqtantJob): the OqtantJob instance to submit for processing
         Returns:
            dict: dictionary containing the external_id of the job and it's queue position
         """
@@ -182,17 +182,17 @@
     def run_jobs(
         self,
         job_list: list[OqtantJob],
         track_status: bool = False,
         write: bool = False,
         filename: str | list[str] = "",
     ) -> list[str]:
-        """Submits a list of OqtantJobs to the Oqtant REST API. This function provides some
+        """Submits a list of OqtantJobs to the Oraqle REST API. This function provides some
            optional functionality to alter how it behaves. Providing it with an argument of
-           track_status=True will make it wait and poll the Oqtant REST API until all jobs
+           track_status=True will make it wait and poll the Oraqle REST API until all jobs
            in the list have completed. The track_status functionality outputs each jobs
            current status as it is polling and opens up the ability to use the other optional
            arguments write and filename. The write and filename arguments enable the ability
            to have the results of each completed job written to a file. The value of filename
            is optional and if not provided will cause the files to be created using the
            external_id of each job. If running more than one job and using the filename
            argument it is required that the number of jobs in job_list match the number of
@@ -239,16 +239,16 @@
         *,
         job_type: job_schema.JobType | None = None,
         name: job_schema.JobName | None = None,
         submit_start: str | None = None,
         submit_end: str | None = None,
         notes: str | None = None,
     ) -> list[dict]:
-        """Submits a query to the REST API to search for jobs that match the provided criteria.
-           The search results will be limited to jobs that meet your Oqtant account access.
+        """Submits a query to the Oraqle REST API to search for jobs that match the provided criteria.
+           The search results will be limited to jobs that meet your Oraqle account access.
         Args:
            job_type (job_schema.JobType): the type of the jobs to search for
            name (job_schema.JobName): the name of the job to search for
            submit_start (str): the earliest submit date of the jobs to search for
            submit_start (str): the latest submit date of the jobs to search for
            notes (str): the notes of the jobs to search for
         Returns:
@@ -275,15 +275,15 @@
     def track_jobs(
         self,
         *,
         pending_jobs: list[str],
         filename: str | list = "",
         write: bool = False,
     ) -> None:
-        """Polls the Oqtant REST API with a list of job external_ids and waits until all of them have
+        """Polls the Oraqle REST API with a list of job external_ids and waits until all of them have
            completed. Will output each job's status while it is polling and will output a message when
            all jobs have completed. This function provides some optional functionality to alter how it
            behaves. Providing it with an argument of write will have it write the results of each
            completed job to a file. There is an additional argument that can be used with write called
            filename. The value of filename is optional and if not provided will cause the files to be
            created using the external_id of each job. If tracking more than one job and using the
            filename argument it is required that the number of jobs in job_list match the number of
@@ -329,25 +329,25 @@
                     pending_jobs.remove(pending_job)
                     if write:
                         job_filenames.pop(0)
                 time.sleep(2)
         print("all jobs complete")
 
     def load_job_from_id_list(self, job_id_list: list[str]) -> None:
-        """Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list
+        """Loads OqtantJobs from the Oraqle REST API into the current active_jobs list using a list
            of job external_ids. The results of the jobs loaded by this function are limited to their
            first run.
         Args:
            job_id_list (list[str]): list of job external_ids to load
         """
         for job_id in job_id_list:
             self.load_job_from_id(job_id)
 
     def load_job_from_id(self, job_id: str, run: int = 1) -> None:
-        """Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a job
+        """Loads an OqtantJob from the Oraqle REST API into the current active_jobs list using a job
            external_id. The results of the jobs loaded by this function can be targeted to a specific
            run if there are multiple.
         Args:
            job_id (str): the external_id of the job to load
            run (int): optional argument to target a specific job run
         """
         try:
@@ -356,25 +356,25 @@
             print(f"Loaded job: {job.name} {job_id}")
         except Exception as err:
             raise api_exceptions.ValidationError(
                 f"Failed to fetch job {job_id}: {err}. Please contact ColdQuanta if error persists"
             )
 
     def load_job_from_file_list(self, file_list: list[str]) -> None:
-        """Loads OqtantJobs from the Oqtant REST API into the current active_jobs list using a list
+        """Loads OqtantJobs from the Oraqle REST API into the current active_jobs list using a list
            of filenames containing OqtantJob info. The results of the jobs loaded by this function are
            limited to their first run.
         Args:
            file_list (list[str]): list of filenames containing OqtantJob information
         """
         for f in file_list:
             self.load_job_from_file(f)
 
     def load_job_from_file(self, file: str) -> None:
-        """Loads an OqtantJob from the Oqtant REST API into the current active_jobs list using a file
+        """Loads an OqtantJob from the Oraqle REST API into the current active_jobs list using a file
            containing OqtantJob info. The results of the jobs loaded by this function are limited to
            their first run.
         Args:
            file_list (list[str]): list of filenames containing OqtantJob information
         """
         try:
             with open(file) as json_file:
@@ -425,15 +425,15 @@
             with open(filepath, "w") as f:
                 f.write(str(job.json()))
             print(f"Wrote job {job.external_id} to file {filepath}")
         except (FileNotFoundError, Exception) as err:
             print(f"Failed to write job {job.external_id} to {filepath}: {err}")
 
     def get_job_limits(self) -> dict:
-        """Utility method to get job limits from the REST API
+        """Utility method to get job limits from the Oraqle REST API
         Returns:
             dict: dictionary of job limits
         """
         try:
             token_data = jwt.decode(
                 self.token, key=None, options={"verify_signature": False}
             )
@@ -453,16 +453,16 @@
             raise api_exceptions.AuthorizationError("Unauthorized")
         response.raise_for_status()
         job_limits = response.json()
         return job_limits
 
 
 def version_check(client_version: str) -> None:
-    """Compares the given current Oqtant version with the version currently on pypi, and raises a warning if it is older.
-
+    """Compares the given current Oqtant version with the version currently on pypi,
+       and raises a warning if it is older.
     Args:
         client_version (str): the client semver version number
     """
     resp = requests.get("https://pypi.org/pypi/oqtant/json", timeout=5)
     if resp.status_code == 200:
         current_version = resp.json()["info"]["version"]
         if semver.compare(client_version, current_version) < 0:
@@ -470,15 +470,15 @@
                 f"Please upgrade to Oqtant version {current_version}. You are currently using version {client_version}."
             )
 
 
 def get_oqtant_client(token: str) -> OqtantClient:
     """A utility function to create a new OqtantClient instance.
     Args:
-        token (str): the auth0 token required for interacting with the REST API
+        token (str): the auth0 token required for interacting with the Oraqle REST API
     Returns:
         OqtantClient: authenticated instance of OqtantClient
     """
 
     client = OqtantClient(settings=settings, token=token)
     version_check(client.version)
     return client
```

### Comparing `oqtant-0.15.1/oqtant/schemas/job.py` & `oqtant-0.16.1/oqtant/schemas/job.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.1/oqtant/util/auth.py` & `oqtant-0.16.1/oqtant/util/auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import hashlib
 import os
 import webbrowser
 from multiprocessing import Queue
 
 import requests
 import uvicorn
-from fastapi import APIRouter, FastAPI
+from fastapi import APIRouter, FastAPI, Request
 from fastapi.responses import RedirectResponse
 
 from oqtant.settings import Settings
 from oqtant.util.server import ThreadServer
 
 settings = Settings()
 
@@ -26,73 +26,80 @@
 
 
 def generate_challenge(verifier: str) -> str:
     hashed = hashlib.sha256(verifier.encode("utf-8")).digest()
     return base64.urlsafe_b64encode(hashed).decode("utf-8").replace("=", "")
 
 
-def get_authentication_url():
+def get_authentication_url(auth_server_port: int):
     code_challenge = generate_challenge(verifier)
     auth_url = "".join(
         [
             f"{settings.auth0_base_url}/authorize",
             "?response_type=code",
             f"&scope={settings.auth0_scope}",
             f"&audience={settings.auth0_audience}",
             f"&code_challenge={code_challenge}",
             "&code_challenge_method=S256",
             f"&client_id={settings.auth0_client_id}",
-            "&redirect_uri=http://localhost:8080",
+            f"&redirect_uri=http://localhost:{auth_server_port}",
         ]
     )
     return auth_url
 
 
 queue = Queue()
 
 
 @app.get("/")
-async def main(code):
-    resp = await get_token(verifier, code)
+async def main(request: Request, code):
+    resp = await get_token(verifier, code, request.url.port)
     token = resp["access_token"]
     queue.put({"token": token})
     if token:
         return "Successfully authenticated, you may close this tab now"
     else:
         return "Failed to authenticate, please close this tab and try again"
 
 
 @app.get("/login")
-def login():
-    return RedirectResponse(url=get_authentication_url())
+def login(request: Request):
+    return RedirectResponse(
+        url=get_authentication_url(auth_server_port=request.url.port)
+    )
 
 
-async def get_token(verifier: str, code: str):
+async def get_token(verifier: str, code: str, auth_server_port: int):
     url = f"{settings.auth0_base_url}/oauth/token"
     headers = {"content-type": "application/x-www-form-urlencoded"}
     data = {
         "grant_type": "authorization_code",
         "client_id": settings.auth0_client_id,
         "code_verifier": verifier,
         "code": code,
-        "redirect_uri": "http://localhost:8080",
+        "redirect_uri": f"http://localhost:{auth_server_port}",
     }
     resp = requests.post(
         url, headers=headers, data=data, allow_redirects=False, timeout=(5, 30)
     )
     return resp.json()
 
 
-def get_user_token() -> str:
+def get_user_token(auth_server_port: int = 8080) -> str:
     """A utility function required for getting Oqtant authenticated with your Oqtant account.
        Starts up a server to handle the Auth0 authentication process and acquire a token.
+    Args:
+        auth_server_port (int): optional port to run the authentication server on
     Returns:
         str: Auth0 user token
     """
+    allowed_ports = [8080, 8081, 8082, 8083, 8084, 8085]
+    if auth_server_port not in allowed_ports:
+        raise ValueError(f"{auth_server_port} not in allowed ports: {allowed_ports}")
     server_config = uvicorn.Config(
-        app=app, host="localhost", port=8080, log_level="error"
+        app=app, host="localhost", port=auth_server_port, log_level="error"
     )
     server = ThreadServer(config=server_config)
     with server.run_in_thread():
-        webbrowser.open("http://localhost:8080/login")
+        webbrowser.open(f"http://localhost:{auth_server_port}/login")
         token = queue.get(block=True)
     return token["token"]
```

### Comparing `oqtant-0.15.1/oqtant/util/exceptions.py` & `oqtant-0.16.1/oqtant/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.15.1/pyproject.toml` & `oqtant-0.16.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "0.15.1"
+version = "0.16.1"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
@@ -36,15 +36,15 @@
 urllib3 = "^1.26.12"
 notebook = "^6.4.12"
 lmfit = "^1.0.3"
 fastapi = "^0.92.0"
 uvicorn = { extras = ["standard"], version = "^0.20.0" }
 scikit-learn = "^1.2.0"
 python-dotenv = "^0.21.1"
-bert-schemas = "^1.18.2"
+bert-schemas = "^1.18.3"
 pyjwt = { extras = ["crypto"], version = "^2.6.0" }
 semver = "^3.0.0"
 ipykernel = "^6.23.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 pytest-xdist = "^3.2.0"
```

### Comparing `oqtant-0.15.1/setup.py` & `oqtant-0.16.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 packages = \
 ['oqtant', 'oqtant.schemas', 'oqtant.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bert-schemas>=1.18.2,<2.0.0',
+['bert-schemas>=1.18.3,<2.0.0',
  'fastapi>=0.92.0,<0.93.0',
  'ipykernel>=6.23.1,<7.0.0',
  'lmfit>=1.0.3,<2.0.0',
  'matplotlib>=3.6.2,<3.7.0',
  'notebook>=6.4.12,<7.0.0',
  'numpy>=1.23.2,<2.0.0',
  'pydantic>=1.10.1,<2.0.0',
@@ -28,17 +28,17 @@
 
 entry_points = \
 {'console_scripts': ['authorize = '
                      'oqtant.tests.integration.authorize:authorize']}
 
 setup_kwargs = {
     'name': 'oqtant',
-    'version': '0.15.1',
+    'version': '0.16.1',
     'description': 'Oqtant Desktop Suite',
-    'long_description': "# Oqtant\n\n[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)\n[![pypi](https://img.shields.io/pypi/v/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)\n[![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)\n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)\n\n## 🚀 Quick Install\n\n```python\npip install oqtant\n```\n\n## 🧭 Introduction\n\nThis API contains tools to:\n\n- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)\n\n  - BARRIER (Barrier Manipulator) jobs\n  - BEC (Ultracold Matter) jobs\n\n- Build parameterized (i.e. optimization) experiments using OqtantJobs\n\n- Submit and retrieve OqtantJob results\n\n## 🤖 How Oqtant Works\n\n- Construct a single or list of jobs using the OqtantJob class\n\n  - 1D parameter sweeps are supported\n\n- Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.\n\n  - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs\n\n- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.\n\n  - View these jobs with see_active_jobs()\n  - These jobs are available until the python session ends.\n\n- To operate on jobs from a current or previous session, load them into active_jobs with\n\n  - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()\n\n- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.\n\nNeed help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!\n\n## 📓 Documentation\n\n- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)\n- [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)\n- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)\n- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)\n- [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)\n",
+    'long_description': "# Oqtant\n\n[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)\n[![pypi](https://img.shields.io/pypi/v/oqtant.svg)](https://pypi.python.org/pypi/oqtant)\n[![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)\n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)\n\n## 🚀 Quick Install\n\n```python\npip install oqtant\n```\n\n## 🧭 Introduction\n\nThis API contains tools to:\n\n- Access all the functionality of the Oraqle Web App (https://albert-dev.coldquanta.com)\n\n  - BARRIER (Barrier Manipulator) jobs\n  - BEC (Ultracold Matter) jobs\n\n- Build parameterized (i.e. optimization) experiments using OqtantJobs\n\n- Submit and retrieve OqtantJob results\n\n## 🤖 How Oqtant Works\n\n- Construct a single or list of jobs using the OqtantJob class\n\n  - 1D parameter sweeps are supported\n\n- Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.\n\n  - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs\n\n- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.\n\n  - View these jobs with see_active_jobs()\n  - These jobs are available until the python session ends.\n\n- To operate on jobs from a current or previous session, load them into active_jobs with\n\n  - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()\n\n- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.\n\nNeed help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!\n\n## 📓 Documentation\n\n- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)\n- [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)\n- [Oraqle API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oraqle_api_docs.md)\n- [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)\n",
     'author': 'Larry Buza',
     'author_email': 'lawrence.buza@coldquanta.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://albert-dev.coldquanta.com/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `oqtant-0.15.1/PKG-INFO` & `oqtant-0.16.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 0.15.1
+Version: 0.16.1
 Summary: Oqtant Desktop Suite
 Home-page: https://albert-dev.coldquanta.com/
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: bert-schemas (>=1.18.2,<2.0.0)
+Requires-Dist: bert-schemas (>=1.18.3,<2.0.0)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: ipykernel (>=6.23.1,<7.0.0)
 Requires-Dist: lmfit (>=1.0.3,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<3.7.0)
 Requires-Dist: notebook (>=6.4.12,<7.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.1,<2.0.0)
@@ -32,29 +32,29 @@
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
 Project-URL: Repository, https://gitlab.com/infleqtion/albert/oqtant
 Description-Content-Type: text/markdown
 
 # Oqtant
 
 [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
-[![pypi](https://img.shields.io/pypi/v/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
+[![pypi](https://img.shields.io/pypi/v/oqtant.svg)](https://pypi.python.org/pypi/oqtant)
 [![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)
 
 ## 🚀 Quick Install
 
 ```python
 pip install oqtant
 ```
 
 ## 🧭 Introduction
 
 This API contains tools to:
 
-- Access all the functionality of the Albert Web App (https://albert-dev.coldquanta.com)
+- Access all the functionality of the Oraqle Web App (https://albert-dev.coldquanta.com)
 
   - BARRIER (Barrier Manipulator) jobs
   - BEC (Ultracold Matter) jobs
 
 - Build parameterized (i.e. optimization) experiments using OqtantJobs
 
 - Submit and retrieve OqtantJob results
@@ -82,11 +82,10 @@
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
 - [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)
 - [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)
-- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oqtant_api_docs.md)
-- [Oqtant API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/albert_api_docs.md)
+- [Oraqle API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oraqle_api_docs.md)
 - [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)
```

