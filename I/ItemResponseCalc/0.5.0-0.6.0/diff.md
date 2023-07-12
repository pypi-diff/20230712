# Comparing `tmp/ItemResponseCalc-0.5.0.tar.gz` & `tmp/ItemResponseCalc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ItemResponseCalc-0.5.0.tar", last modified: Tue Jun  9 02:25:37 2020, max compression
+gzip compressed data, was "ItemResponseCalc-0.6.0.tar", last modified: Wed Jul 12 12:25:19 2023, max compression
```

## Comparing `ItemResponseCalc-0.5.0.tar` & `ItemResponseCalc-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/
--rw-r--r--   0 arne       (503) staff       (20)     8472 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/PKG-INFO
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/
--rw-r--r--   0 arne       (503) staff       (20)     8472 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/PKG-INFO
--rw-r--r--   0 arne       (503) staff       (20)      954 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (503) staff       (20)       45 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/requires.txt
--rw-r--r--   0 arne       (503) staff       (20)       17 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/top_level.txt
--rw-r--r--   0 arne       (503) staff       (20)        1 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (503) staff       (20)     6742 2020-06-08 09:53:51.000000 ItemResponseCalc-0.5.0/README.md
--rw-r--r--   0 arne       (503) staff       (20)     1031 2020-05-28 02:36:36.000000 ItemResponseCalc-0.5.0/setup.py
--rw-r--r--   0 arne       (503) staff       (20)       38 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/setup.cfg
-drwxr-xr-x   0 arne       (503) staff       (20)        0 2020-06-09 02:25:37.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/
--rw-r--r--   0 arne       (503) staff       (20)     5473 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/table_reader_csv.py
--rw-r--r--   0 arne       (503) staff       (20)    13275 2020-06-06 09:00:02.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/item_scale_gamma.py
--rw-r--r--   0 arne       (503) staff       (20)     5520 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/table_reader_sql.py
--rw-r--r--   0 arne       (503) staff       (20)    13257 2020-06-08 09:46:54.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/trait_precision.py
--rw-r--r--   0 arne       (503) staff       (20)     4597 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/table_reader_sqlite.py
--rw-r--r--   0 arne       (503) staff       (20)    29126 2020-06-08 03:41:32.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/item_response_model.py
--rw-r--r--   0 arne       (503) staff       (20)    28499 2020-06-08 04:44:50.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/item_scale.py
--rw-r--r--   0 arne       (503) staff       (20)     4597 2020-06-08 07:55:55.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/item_trait_selector.py
--rw-r--r--   0 arne       (503) staff       (20)     4077 2020-06-08 03:41:33.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/__init__.py
--rw-r--r--   0 arne       (503) staff       (20)    21113 2020-06-08 03:41:33.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/ir_display_format.py
--rw-r--r--   0 arne       (503) staff       (20)     1280 2020-02-05 01:54:21.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/ir_logging.py
--rw-r--r--   0 arne       (503) staff       (20)    15291 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/run_irt.py
--rw-r--r--   0 arne       (503) staff       (20)    18817 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/item_response_data.py
--rw-r--r--   0 arne       (503) staff       (20)     7428 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/table_reader_xlsx.py
--rw-r--r--   0 arne       (503) staff       (20)     3631 2019-04-28 15:14:08.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/safe_logistic.py
--rw-r--r--   0 arne       (503) staff       (20)    43482 2020-06-08 08:52:14.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/item_respondents.py
--rw-r--r--   0 arne       (503) staff       (20)     3146 2020-06-08 03:41:33.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/ir_predictive.py
--rw-r--r--   0 arne       (503) staff       (20)     6275 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/table_reader_spss.py
--rw-r--r--   0 arne       (503) staff       (20)     4576 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/show_irt.py
--rw-r--r--   0 arne       (503) staff       (20)     7157 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/table_reader.py
--rw-r--r--   0 arne       (503) staff       (20)    19886 2020-06-08 08:35:12.000000 ItemResponseCalc-0.5.0/ItemResponseCalc/ir_display.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-07-12 12:25:19.981657 ItemResponseCalc-0.6.0/
+-rw-r--r--   0 arne       (503) staff       (20)     1083 2020-04-29 09:07:53.000000 ItemResponseCalc-0.6.0/LICENSE.txt
+-rw-r--r--   0 arne       (503) staff       (20)     7108 2023-07-12 12:25:19.981711 ItemResponseCalc-0.6.0/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)     6398 2023-07-09 10:48:54.000000 ItemResponseCalc-0.6.0/README.md
+-rw-r--r--   0 arne       (503) staff       (20)      105 2023-06-24 14:38:35.000000 ItemResponseCalc-0.6.0/pyproject.toml
+-rw-r--r--   0 arne       (503) staff       (20)      957 2023-07-12 12:25:19.981967 ItemResponseCalc-0.6.0/setup.cfg
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-07-12 12:25:19.968692 ItemResponseCalc-0.6.0/src/
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-07-12 12:25:19.975481 ItemResponseCalc-0.6.0/src/ItemResponseCalc/
+-rw-r--r--   0 arne       (503) staff       (20)     4430 2023-07-12 06:27:23.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/__init__.py
+-rw-r--r--   0 arne       (503) staff       (20)    25005 2023-07-12 07:07:06.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_display.py
+-rw-r--r--   0 arne       (503) staff       (20)    22017 2023-07-08 10:09:38.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_display_format.py
+-rw-r--r--   0 arne       (503) staff       (20)    16221 2023-06-13 07:03:40.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_graded_response_prob.py
+-rw-r--r--   0 arne       (503) staff       (20)     1280 2020-02-05 01:54:21.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_logging.py
+-rw-r--r--   0 arne       (503) staff       (20)     3146 2020-06-08 03:41:33.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_predictive.py
+-rw-r--r--   0 arne       (503) staff       (20)    21970 2023-07-11 10:01:43.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_source.py
+-rw-r--r--   0 arne       (503) staff       (20)    31504 2023-06-13 07:53:22.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_graded_response.py
+-rw-r--r--   0 arne       (503) staff       (20)    35397 2023-07-12 07:50:37.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_respondents.py
+-rw-r--r--   0 arne       (503) staff       (20)    21417 2023-07-11 10:01:43.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_response_data.py
+-rw-r--r--   0 arne       (503) staff       (20)    31005 2023-07-12 07:52:16.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_response_model.py
+-rw-r--r--   0 arne       (503) staff       (20)    13277 2020-06-13 03:32:07.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_scale_gamma.py
+-rw-r--r--   0 arne       (503) staff       (20)     4599 2020-06-13 03:32:07.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_trait_selector.py
+-rw-r--r--   0 arne       (503) staff       (20)    14403 2023-07-12 08:55:40.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/run_irt.py
+-rw-r--r--   0 arne       (503) staff       (20)     3631 2019-04-28 15:14:08.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/safe_logistic.py
+-rw-r--r--   0 arne       (503) staff       (20)    13257 2020-06-08 09:46:54.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc/trait_precision.py
+drwxr-xr-x   0 arne       (503) staff       (20)        0 2023-07-12 12:25:19.981538 ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/
+-rw-r--r--   0 arne       (503) staff       (20)     7108 2023-07-12 12:25:19.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/PKG-INFO
+-rw-r--r--   0 arne       (503) staff       (20)      898 2023-07-12 12:25:19.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/SOURCES.txt
+-rw-r--r--   0 arne       (503) staff       (20)        1 2023-07-12 12:25:19.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/dependency_links.txt
+-rw-r--r--   0 arne       (503) staff       (20)       74 2023-07-12 12:25:19.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/requires.txt
+-rw-r--r--   0 arne       (503) staff       (20)       17 2023-07-12 12:25:19.000000 ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ItemResponseCalc-0.5.0/PKG-INFO` & `ItemResponseCalc-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,142 @@
 Metadata-Version: 2.1
 Name: ItemResponseCalc
-Version: 0.5.0
+Version: 0.6.0
 Summary: Statistical Analysis of Questionnaire Response Data
-Home-page: UNKNOWN
 Author: Arne Leijon
 Author-email: leijon@kth.se
-License: MIT
-Description: Package **ItemResponseCalc** implements probabilistic Bayesian analysis
-        of responses from a questionnaire designed to measure individual `traits', 
-        i.e., preferences, judgments, or capabilities.
-        
-        The analysis is based on *Item Response Theory (IRT)*.
-        This is a family of probabilistic models designed to handle responses to test instruments for any purpose in social, psychological, or educational research.
-        The analysis model estimates individual parameters numerically on an objective *interval scale*,
-        although the raw input data are *subjective*
-        and indicate only an *ordinal* judgment for each item in the questionnaire.
-        
-        This implementation uses the *Graded Response Model* (Samejima, 1997; Fox, 2010), 
-        applied with a logistic distribution for the latent random variable assumed to determine each response.
-        This model treats subjects' responses
-        as determined by the outcome of a latent individual trait variable,
-        i.e., somewhat similar to the latent internal "sensation"
-        variable assumed to determine responses in psycho-physical experiments.
-        
-        Another model for similar data might be the Partial Credits Model (Masters, 1982; Fox, 2010),
-        which belongs to the Rasch family.
-        
-        ## Data Collection
-        The present package version can only handle discrete *ordinal* response data.
-        The response alternatives must represent a natural order, e.g., 
-        `strongly disagree`, `disagree`, `no opinion`, `agree`, `strongly agree`.
-        
-        This package *does not include* functions to administer the data collection;
-        it can only use existing recorded data.
-        The present version *does not include* functions to validate the statistical properties of the questionnaire itself,
-        and thus cannot help in the design of a questionnaire.
-        It can only analyze recorded response data sets obtained from an existing test instrument.
-        
-        The package can analyze response data with the following features:
-        
-        1. The questionnaire may include several items.
-        
-        1. The items may be designed to measure either 
-        	a single individual trait, or several traits.
-        	The analysis will automatically determine how many traits are needed
-        	to effectively model the complete set of response data.
-            	The analysis results will show estimated values for each trait.
-           	 
-         1. Separate model parameters are estimated for the traits of individual respondents, 
-         	and for the response scale of each item.
-        	The analysis results will show which items are associated with each individual trait.
-        	The results also show how the trait scale corresponds to the ordinal responses for each item.
-         
-        1. The number of response alternatives may differ among questionnaire items.
-        	Each item must have at least two response alternatives,
-        	even if one alternative is not explicitly shown in the questionnaire. 
-        	(For example, if an item requires a Yes/No answer, 
-        	only the Yes alternative might be shown as a tick box, 
-        	and the absence of a tick mark is interpreted as a No answer.) 
-        	
-        1. Data for one or more distinct **Participant Groups** may be included.
-        	The analysis will show predicted differences between the populations
-        	from which the groups are recruited.
-        	The statistical credibility is calculated *jointly* for all population differences,
-        	accounting for the effects of multiple comparisons.	
-            
-        1. The analysis model can use input data stored in various file formats. 
-        	The user can specify different recoding functions for each input source, 
-        	e.g., to handle different codes for missing responses, 
-        	or different wordings for the response alternatives. 
-        	Responses are recoded into an ordinal integer index 1, 2, etc., for each item.
-        
-        1. The analysis can handle missing responses in the input data sets. 	
-        
-        1. The user may specify arbitrary inclusion criteria for respondent records,
-        	separately for each input file.
-        
-        1. The present version does not distinguish *repeated* responses from a single subject. 
-        	All input records are treated as independent, 
-        	assumed to be given by different respondents.
-        
-        The Bayesian model is hierarchical.
-        The package can estimate predictive distributions of results for
-        * a random individual in each population represented by a group of respondents,
-        * the mean in each population represented by a group of respondents,
-        * a random individual in the total population for which all respondent groups are representative.
-        All results are saved in files with figures and tables, with user-selectable formats. 
-        
-        ## Package Documentation
-        General information and version history is given in the package doc-string that may be accessed by command
-        `help(ItemResponseCalc)`.
-        
-        Specific information about the organization and accepted formats of input data files
-        is presented in the doc-string of module item_response_data, accessible via `help(ItemResponseCalc.item_response_data)`.
-        The most flexible file format is an Excel (xlsx) work-sheet, where each row
-        contains all responses from one subject, with one column for each item.
-        
-        After running an analysis, the logging output file briefly explains
-        the analysis results presented in figures and tables.
-        
-        ## Usage
-        1. Install the most recent package version:
-            `python3 -m pip install --upgrade ItemResponseCalc`
-        
-        1. Copy the template script `run_irt.py`, rename it, and
-            edit the copy as suggested in the template, to specify
-            - your questionnaire and response alternatives,
-            - the respondent groups and corresponding input data files,
-            - a directory where all output result files will be stored.
-        
-        1. Run your edited script: `python3 run_my_irt.py`.
-        
-        ## Requirements
-        This package requires Python 3.6 or newer, with Numpy 1.17 or newer, Scipy, and Matplotlib,
-        as well as a support package samppy, and openpyxl for reading xlsx files.
-        The pip installer will check and install these required packages if needed.
-        
-        If the user needs to access data in a MySQL database, 
-        a connection package must be installed manually, e.g., as
-         `python3 -m pip install  mysql-connector-python`
-        
-        If the user needs to analyze SPSS (.sav) data files, 
-        it is recommended to first use SPSS to convert the data to xlsx or csv file format.
-        
-        ## References
-        A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist (2020).
-        Analysis of Data from the International Outcome Inventory for Hearing Aids (IOI-HA) using Bayesian Item Response Theory.
-        *Manuscript in preparation*. Contact the package author for more information.
-        
-        J.-P. Fox (2010). *Bayesian Item Response Modeling: Theory and Applications*. Statistics for Social and Behavioral Sciences. Springer.
-        
-        G. N. Masters (1982). A Rasch model for partial credit scoring. *Psychometrika*, 47(2):149–174.
-        
-        F. Samejima (1997). Graded response model. In W. J. v. D. Linden and R. K. Hambleton, eds., *Handbook of Modern Item Response Theory*, p. 85–100. Springer, New York.
-        
-        
-Keywords: questionnaire item-response-theory Bayesian
-Platform: UNKNOWN
+License: MIT License
+Keywords: Questionnaire,Item Response Theory,IRT,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+Package **ItemResponseCalc** implements probabilistic Bayesian analysis
+of responses from a questionnaire designed to measure individual `traits', 
+i.e., preferences, judgments, or capabilities.
+
+The analysis is based on *Item Response Theory (IRT)*.
+This is a family of probabilistic models designed to handle responses to test instruments for any purpose in social, psychological, or educational research.
+The analysis model estimates individual parameters numerically on an objective *interval scale*,
+although the raw input data are *subjective*
+and indicate only an *ordinal* judgment for each item in the questionnaire.
+
+This implementation uses the *Graded Response Model* (Samejima, 1997; Fox, 2010), 
+applied with a logistic distribution for the latent random variable assumed to determine each response.
+This model treats subjects' responses
+as determined by the outcome of a latent individual trait variable,
+i.e., somewhat similar to the latent internal "sensation"
+variable assumed to determine responses in psycho-physical experiments.
+
+Another model for similar data might be the Partial Credits Model (Masters, 1982; Fox, 2010),
+which belongs to the Rasch family.
+
+## Data Collection
+The present package version can only handle discrete *ordinal* response data.
+The response alternatives must represent a natural order, e.g., 
+`strongly disagree`, `disagree`, `no opinion`, `agree`, `strongly agree`.
+
+This package *does not include* functions to administer the data collection;
+it can only use existing recorded data.
+The present version *does not include* functions to validate the statistical properties of the questionnaire itself,
+and thus cannot help in the design of a questionnaire.
+It can only analyze recorded response data sets obtained from an existing test instrument.
+
+The package can analyze response data with the following features:
+
+1. The questionnaire may include several items.
+
+1. The items may be designed to measure either 
+	a single trait, or several traits.
+	The analysis will automatically determine how many traits are needed
+	to effectively model the complete set of response data.
+    	The analysis results will show estimated values for each trait.
+   	 
+ 1. Separate model parameters are estimated for the traits of individual respondents, 
+ 	and for the response scale of each item.
+	The analysis results will show which items are associated with each individual trait.
+	The results also show how the trait scale corresponds to the ordinal responses for each item.
+ 
+1. The number of response alternatives may differ among questionnaire items.
+	Each item must have at least two response alternatives,
+	even if one alternative is not explicitly shown in the questionnaire. 
+	(For example, if an item requires a Yes/No answer, 
+	only the Yes alternative might be shown as a tick box, 
+	and the absence of a tick mark is interpreted as a No answer.) 
+	
+1. Data for one or more distinct *Participant Groups* may be included.
+	The analysis will show predicted differences between the populations
+	from which the groups are recruited.
+	The statistical credibility is calculated *jointly* for all population differences,
+	automatically accounting for the effects of multiple comparisons.	
+    
+1. The analysis model can use input data stored in various file formats. 
+    Package Pandas is used to access the data. 
+	The response alternatives for each item may be encoded in different ways 
+	in each input source.
+
+1. The user may specify arbitrary inclusion criteria for respondent records,
+	separately for each input file.
+
+1. If an input data file includes unique respondent labels, only the last record from each respondent will be used. Otherwise, all input records are treated as independent, 
+	assumed to be given by different respondents.
+
+The Bayesian model is hierarchical.
+The package can estimate predictive distributions of results for
+* a random individual in each population represented by a group of respondents,
+* the mean in each population represented by a group of respondents,
+* a random individual in the total population for which all respondent groups are representative.
+All results are saved in files with figures and tables, with user-selectable formats. 
+
+## Package Documentation
+General information and version history is given in the package doc-string that may be accessed by command
+`help(ItemResponseCalc)`.
+
+Specific information about the organization and accepted formats of input data files
+is presented in the doc-string of module item_response_data, accessible 
+via `help(ItemResponseCalc.item_response_data)`.
+
+After running an analysis, the logging output file briefly explains
+the analysis results presented in figures and tables.
+
+## Usage
+1. Install the most recent package version:
+    `python3 -m pip install --upgrade ItemResponseCalc`
+
+1. Copy the template script `run_irt.py`, rename it, and
+    edit the copy as suggested in the template, to specify
+    - your questionnaire and response alternatives,
+    - the respondent groups and corresponding input data sources,
+    - a directory where all output result files will be stored.
+
+1. Run your edited script: `python3 run_my_irt.py`.
+
+## Requirements
+This package requires Python 3.9 or newer, with recent versions of 
+Numpy, Scipy, Pandas, and Matplotlib, 
+as well as a support package samppy, and openpyxl for reading xlsx files.
+The pip installer will check and install these required packages if needed.
+
+Input data can be accessed from sources in any format 
+that package Pandas can handle.
+Some file formats may require additional help packages to be installed manually.
+
+Pandas can also extract data from an SQL database, 
+but then the SQLAlchemy package might need to be installed manually.
+
+
+## References
+A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist (2020). Analysis of data from the international outcome inventory for hearing aids (IOI-HA) using Bayesian item response theory. *Int J Audiol* 60(2):81–88.
+
+J.-P. Fox (2010). *Bayesian Item Response Modeling: Theory and Applications*. Statistics for Social and Behavioral Sciences. Springer.
+
+G. N. Masters (1982). A Rasch model for partial credit scoring. *Psychometrika*, 47(2):149–174.
+
+F. Samejima (1997). Graded response model. In W. J. v. D. Linden and R. K. Hambleton, eds., *Handbook of Modern Item Response Theory*, p. 85–100. Springer, New York.
+
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc.egg-info/PKG-INFO` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,142 @@
 Metadata-Version: 2.1
 Name: ItemResponseCalc
-Version: 0.5.0
+Version: 0.6.0
 Summary: Statistical Analysis of Questionnaire Response Data
-Home-page: UNKNOWN
 Author: Arne Leijon
 Author-email: leijon@kth.se
-License: MIT
-Description: Package **ItemResponseCalc** implements probabilistic Bayesian analysis
-        of responses from a questionnaire designed to measure individual `traits', 
-        i.e., preferences, judgments, or capabilities.
-        
-        The analysis is based on *Item Response Theory (IRT)*.
-        This is a family of probabilistic models designed to handle responses to test instruments for any purpose in social, psychological, or educational research.
-        The analysis model estimates individual parameters numerically on an objective *interval scale*,
-        although the raw input data are *subjective*
-        and indicate only an *ordinal* judgment for each item in the questionnaire.
-        
-        This implementation uses the *Graded Response Model* (Samejima, 1997; Fox, 2010), 
-        applied with a logistic distribution for the latent random variable assumed to determine each response.
-        This model treats subjects' responses
-        as determined by the outcome of a latent individual trait variable,
-        i.e., somewhat similar to the latent internal "sensation"
-        variable assumed to determine responses in psycho-physical experiments.
-        
-        Another model for similar data might be the Partial Credits Model (Masters, 1982; Fox, 2010),
-        which belongs to the Rasch family.
-        
-        ## Data Collection
-        The present package version can only handle discrete *ordinal* response data.
-        The response alternatives must represent a natural order, e.g., 
-        `strongly disagree`, `disagree`, `no opinion`, `agree`, `strongly agree`.
-        
-        This package *does not include* functions to administer the data collection;
-        it can only use existing recorded data.
-        The present version *does not include* functions to validate the statistical properties of the questionnaire itself,
-        and thus cannot help in the design of a questionnaire.
-        It can only analyze recorded response data sets obtained from an existing test instrument.
-        
-        The package can analyze response data with the following features:
-        
-        1. The questionnaire may include several items.
-        
-        1. The items may be designed to measure either 
-        	a single individual trait, or several traits.
-        	The analysis will automatically determine how many traits are needed
-        	to effectively model the complete set of response data.
-            	The analysis results will show estimated values for each trait.
-           	 
-         1. Separate model parameters are estimated for the traits of individual respondents, 
-         	and for the response scale of each item.
-        	The analysis results will show which items are associated with each individual trait.
-        	The results also show how the trait scale corresponds to the ordinal responses for each item.
-         
-        1. The number of response alternatives may differ among questionnaire items.
-        	Each item must have at least two response alternatives,
-        	even if one alternative is not explicitly shown in the questionnaire. 
-        	(For example, if an item requires a Yes/No answer, 
-        	only the Yes alternative might be shown as a tick box, 
-        	and the absence of a tick mark is interpreted as a No answer.) 
-        	
-        1. Data for one or more distinct **Participant Groups** may be included.
-        	The analysis will show predicted differences between the populations
-        	from which the groups are recruited.
-        	The statistical credibility is calculated *jointly* for all population differences,
-        	accounting for the effects of multiple comparisons.	
-            
-        1. The analysis model can use input data stored in various file formats. 
-        	The user can specify different recoding functions for each input source, 
-        	e.g., to handle different codes for missing responses, 
-        	or different wordings for the response alternatives. 
-        	Responses are recoded into an ordinal integer index 1, 2, etc., for each item.
-        
-        1. The analysis can handle missing responses in the input data sets. 	
-        
-        1. The user may specify arbitrary inclusion criteria for respondent records,
-        	separately for each input file.
-        
-        1. The present version does not distinguish *repeated* responses from a single subject. 
-        	All input records are treated as independent, 
-        	assumed to be given by different respondents.
-        
-        The Bayesian model is hierarchical.
-        The package can estimate predictive distributions of results for
-        * a random individual in each population represented by a group of respondents,
-        * the mean in each population represented by a group of respondents,
-        * a random individual in the total population for which all respondent groups are representative.
-        All results are saved in files with figures and tables, with user-selectable formats. 
-        
-        ## Package Documentation
-        General information and version history is given in the package doc-string that may be accessed by command
-        `help(ItemResponseCalc)`.
-        
-        Specific information about the organization and accepted formats of input data files
-        is presented in the doc-string of module item_response_data, accessible via `help(ItemResponseCalc.item_response_data)`.
-        The most flexible file format is an Excel (xlsx) work-sheet, where each row
-        contains all responses from one subject, with one column for each item.
-        
-        After running an analysis, the logging output file briefly explains
-        the analysis results presented in figures and tables.
-        
-        ## Usage
-        1. Install the most recent package version:
-            `python3 -m pip install --upgrade ItemResponseCalc`
-        
-        1. Copy the template script `run_irt.py`, rename it, and
-            edit the copy as suggested in the template, to specify
-            - your questionnaire and response alternatives,
-            - the respondent groups and corresponding input data files,
-            - a directory where all output result files will be stored.
-        
-        1. Run your edited script: `python3 run_my_irt.py`.
-        
-        ## Requirements
-        This package requires Python 3.6 or newer, with Numpy 1.17 or newer, Scipy, and Matplotlib,
-        as well as a support package samppy, and openpyxl for reading xlsx files.
-        The pip installer will check and install these required packages if needed.
-        
-        If the user needs to access data in a MySQL database, 
-        a connection package must be installed manually, e.g., as
-         `python3 -m pip install  mysql-connector-python`
-        
-        If the user needs to analyze SPSS (.sav) data files, 
-        it is recommended to first use SPSS to convert the data to xlsx or csv file format.
-        
-        ## References
-        A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist (2020).
-        Analysis of Data from the International Outcome Inventory for Hearing Aids (IOI-HA) using Bayesian Item Response Theory.
-        *Manuscript in preparation*. Contact the package author for more information.
-        
-        J.-P. Fox (2010). *Bayesian Item Response Modeling: Theory and Applications*. Statistics for Social and Behavioral Sciences. Springer.
-        
-        G. N. Masters (1982). A Rasch model for partial credit scoring. *Psychometrika*, 47(2):149–174.
-        
-        F. Samejima (1997). Graded response model. In W. J. v. D. Linden and R. K. Hambleton, eds., *Handbook of Modern Item Response Theory*, p. 85–100. Springer, New York.
-        
-        
-Keywords: questionnaire item-response-theory Bayesian
-Platform: UNKNOWN
+License: MIT License
+Keywords: Questionnaire,Item Response Theory,IRT,Ordinal Ratings,Bayesian
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+Package **ItemResponseCalc** implements probabilistic Bayesian analysis
+of responses from a questionnaire designed to measure individual `traits', 
+i.e., preferences, judgments, or capabilities.
+
+The analysis is based on *Item Response Theory (IRT)*.
+This is a family of probabilistic models designed to handle responses to test instruments for any purpose in social, psychological, or educational research.
+The analysis model estimates individual parameters numerically on an objective *interval scale*,
+although the raw input data are *subjective*
+and indicate only an *ordinal* judgment for each item in the questionnaire.
+
+This implementation uses the *Graded Response Model* (Samejima, 1997; Fox, 2010), 
+applied with a logistic distribution for the latent random variable assumed to determine each response.
+This model treats subjects' responses
+as determined by the outcome of a latent individual trait variable,
+i.e., somewhat similar to the latent internal "sensation"
+variable assumed to determine responses in psycho-physical experiments.
+
+Another model for similar data might be the Partial Credits Model (Masters, 1982; Fox, 2010),
+which belongs to the Rasch family.
+
+## Data Collection
+The present package version can only handle discrete *ordinal* response data.
+The response alternatives must represent a natural order, e.g., 
+`strongly disagree`, `disagree`, `no opinion`, `agree`, `strongly agree`.
+
+This package *does not include* functions to administer the data collection;
+it can only use existing recorded data.
+The present version *does not include* functions to validate the statistical properties of the questionnaire itself,
+and thus cannot help in the design of a questionnaire.
+It can only analyze recorded response data sets obtained from an existing test instrument.
+
+The package can analyze response data with the following features:
+
+1. The questionnaire may include several items.
+
+1. The items may be designed to measure either 
+	a single trait, or several traits.
+	The analysis will automatically determine how many traits are needed
+	to effectively model the complete set of response data.
+    	The analysis results will show estimated values for each trait.
+   	 
+ 1. Separate model parameters are estimated for the traits of individual respondents, 
+ 	and for the response scale of each item.
+	The analysis results will show which items are associated with each individual trait.
+	The results also show how the trait scale corresponds to the ordinal responses for each item.
+ 
+1. The number of response alternatives may differ among questionnaire items.
+	Each item must have at least two response alternatives,
+	even if one alternative is not explicitly shown in the questionnaire. 
+	(For example, if an item requires a Yes/No answer, 
+	only the Yes alternative might be shown as a tick box, 
+	and the absence of a tick mark is interpreted as a No answer.) 
+	
+1. Data for one or more distinct *Participant Groups* may be included.
+	The analysis will show predicted differences between the populations
+	from which the groups are recruited.
+	The statistical credibility is calculated *jointly* for all population differences,
+	automatically accounting for the effects of multiple comparisons.	
+    
+1. The analysis model can use input data stored in various file formats. 
+    Package Pandas is used to access the data. 
+	The response alternatives for each item may be encoded in different ways 
+	in each input source.
+
+1. The user may specify arbitrary inclusion criteria for respondent records,
+	separately for each input file.
+
+1. If an input data file includes unique respondent labels, only the last record from each respondent will be used. Otherwise, all input records are treated as independent, 
+	assumed to be given by different respondents.
+
+The Bayesian model is hierarchical.
+The package can estimate predictive distributions of results for
+* a random individual in each population represented by a group of respondents,
+* the mean in each population represented by a group of respondents,
+* a random individual in the total population for which all respondent groups are representative.
+All results are saved in files with figures and tables, with user-selectable formats. 
+
+## Package Documentation
+General information and version history is given in the package doc-string that may be accessed by command
+`help(ItemResponseCalc)`.
+
+Specific information about the organization and accepted formats of input data files
+is presented in the doc-string of module item_response_data, accessible 
+via `help(ItemResponseCalc.item_response_data)`.
+
+After running an analysis, the logging output file briefly explains
+the analysis results presented in figures and tables.
+
+## Usage
+1. Install the most recent package version:
+    `python3 -m pip install --upgrade ItemResponseCalc`
+
+1. Copy the template script `run_irt.py`, rename it, and
+    edit the copy as suggested in the template, to specify
+    - your questionnaire and response alternatives,
+    - the respondent groups and corresponding input data sources,
+    - a directory where all output result files will be stored.
+
+1. Run your edited script: `python3 run_my_irt.py`.
+
+## Requirements
+This package requires Python 3.9 or newer, with recent versions of 
+Numpy, Scipy, Pandas, and Matplotlib, 
+as well as a support package samppy, and openpyxl for reading xlsx files.
+The pip installer will check and install these required packages if needed.
+
+Input data can be accessed from sources in any format 
+that package Pandas can handle.
+Some file formats may require additional help packages to be installed manually.
+
+Pandas can also extract data from an SQL database, 
+but then the SQLAlchemy package might need to be installed manually.
+
+
+## References
+A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist (2020). Analysis of data from the international outcome inventory for hearing aids (IOI-HA) using Bayesian item response theory. *Int J Audiol* 60(2):81–88.
+
+J.-P. Fox (2010). *Bayesian Item Response Modeling: Theory and Applications*. Statistics for Social and Behavioral Sciences. Springer.
+
+G. N. Masters (1982). A Rasch model for partial credit scoring. *Psychometrika*, 47(2):149–174.
+
+F. Samejima (1997). Graded response model. In W. J. v. D. Linden and R. K. Hambleton, eds., *Handbook of Modern Item Response Theory*, p. 85–100. Springer, New York.
+
```

### Comparing `ItemResponseCalc-0.5.0/README.md` & `ItemResponseCalc-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 It can only analyze recorded response data sets obtained from an existing test instrument.
 
 The package can analyze response data with the following features:
 
 1. The questionnaire may include several items.
 
 1. The items may be designed to measure either 
-	a single individual trait, or several traits.
+	a single trait, or several traits.
 	The analysis will automatically determine how many traits are needed
 	to effectively model the complete set of response data.
     	The analysis results will show estimated values for each trait.
    	 
  1. Separate model parameters are estimated for the traits of individual respondents, 
  	and for the response scale of each item.
 	The analysis results will show which items are associated with each individual trait.
@@ -47,82 +47,77 @@
 1. The number of response alternatives may differ among questionnaire items.
 	Each item must have at least two response alternatives,
 	even if one alternative is not explicitly shown in the questionnaire. 
 	(For example, if an item requires a Yes/No answer, 
 	only the Yes alternative might be shown as a tick box, 
 	and the absence of a tick mark is interpreted as a No answer.) 
 	
-1. Data for one or more distinct **Participant Groups** may be included.
+1. Data for one or more distinct *Participant Groups* may be included.
 	The analysis will show predicted differences between the populations
 	from which the groups are recruited.
 	The statistical credibility is calculated *jointly* for all population differences,
-	accounting for the effects of multiple comparisons.	
+	automatically accounting for the effects of multiple comparisons.	
     
 1. The analysis model can use input data stored in various file formats. 
-	The user can specify different recoding functions for each input source, 
-	e.g., to handle different codes for missing responses, 
-	or different wordings for the response alternatives. 
-	Responses are recoded into an ordinal integer index 1, 2, etc., for each item.
-
-1. The analysis can handle missing responses in the input data sets. 	
+    Package Pandas is used to access the data. 
+	The response alternatives for each item may be encoded in different ways 
+	in each input source.
 
 1. The user may specify arbitrary inclusion criteria for respondent records,
 	separately for each input file.
 
-1. The present version does not distinguish *repeated* responses from a single subject. 
-	All input records are treated as independent, 
+1. If an input data file includes unique respondent labels, only the last record from each respondent will be used. Otherwise, all input records are treated as independent, 
 	assumed to be given by different respondents.
 
 The Bayesian model is hierarchical.
 The package can estimate predictive distributions of results for
 * a random individual in each population represented by a group of respondents,
 * the mean in each population represented by a group of respondents,
 * a random individual in the total population for which all respondent groups are representative.
 All results are saved in files with figures and tables, with user-selectable formats. 
 
 ## Package Documentation
 General information and version history is given in the package doc-string that may be accessed by command
 `help(ItemResponseCalc)`.
 
 Specific information about the organization and accepted formats of input data files
-is presented in the doc-string of module item_response_data, accessible via `help(ItemResponseCalc.item_response_data)`.
-The most flexible file format is an Excel (xlsx) work-sheet, where each row
-contains all responses from one subject, with one column for each item.
+is presented in the doc-string of module item_response_data, accessible 
+via `help(ItemResponseCalc.item_response_data)`.
 
 After running an analysis, the logging output file briefly explains
 the analysis results presented in figures and tables.
 
 ## Usage
 1. Install the most recent package version:
     `python3 -m pip install --upgrade ItemResponseCalc`
 
 1. Copy the template script `run_irt.py`, rename it, and
     edit the copy as suggested in the template, to specify
     - your questionnaire and response alternatives,
-    - the respondent groups and corresponding input data files,
+    - the respondent groups and corresponding input data sources,
     - a directory where all output result files will be stored.
 
 1. Run your edited script: `python3 run_my_irt.py`.
 
 ## Requirements
-This package requires Python 3.6 or newer, with Numpy 1.17 or newer, Scipy, and Matplotlib,
+This package requires Python 3.9 or newer, with recent versions of 
+Numpy, Scipy, Pandas, and Matplotlib, 
 as well as a support package samppy, and openpyxl for reading xlsx files.
 The pip installer will check and install these required packages if needed.
 
-If the user needs to access data in a MySQL database, 
-a connection package must be installed manually, e.g., as
- `python3 -m pip install  mysql-connector-python`
+Input data can be accessed from sources in any format 
+that package Pandas can handle.
+Some file formats may require additional help packages to be installed manually.
+
+Pandas can also extract data from an SQL database, 
+but then the SQLAlchemy package might need to be installed manually.
 
-If the user needs to analyze SPSS (.sav) data files, 
-it is recommended to first use SPSS to convert the data to xlsx or csv file format.
 
 ## References
-A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist (2020).
-Analysis of Data from the International Outcome Inventory for Hearing Aids (IOI-HA) using Bayesian Item Response Theory.
-*Manuscript in preparation*. Contact the package author for more information.
+A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist (2020). Analysis of data from the international outcome inventory for hearing aids (IOI-HA) using Bayesian item response theory. *Int J Audiol* 60(2):81–88.
 
 J.-P. Fox (2010). *Bayesian Item Response Modeling: Theory and Applications*. Statistics for Social and Behavioral Sciences. Springer.
 
 G. N. Masters (1982). A Rasch model for partial credit scoring. *Psychometrika*, 47(2):149–174.
 
 F. Samejima (1997). Graded response model. In W. J. v. D. Linden and R. K. Hambleton, eds., *Handbook of Modern Item Response Theory*, p. 85–100. Springer, New York.
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/item_scale_gamma.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_scale_gamma.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ **** NOT USED ****
 Module defining probability distribution of rating-interval thresholds for
 response categories in an OrdinalItemResponseModel.
 
 *** Main Class:
-OrdinalItemScale --- defining response intervals for one item
+GradedResponseItem --- defining response intervals for one item
 
 Method:
 In this version, response thresholds are indirectly determined by vector
 w = non-normalized width parameters in the logistic-mapped domain.
 The prior distribution of w is gamma,
 and the posterior is approximated by a set of equally probable sample vectors.
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/trait_precision.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/trait_precision.py`

 * *Files identical despite different names*

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/item_response_model.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_response_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,70 @@
 """This module implements a Bayesian model of subjects' responses
-to items in a questionnaire, using the Graded Response Model of Item Response Theory.
+to items in a questionnaire, using Item Response Theory (IRT).
+
+The present version allows two classes of IRT models for ordinal data:
+ir_graded_response_prob.GradedResponse, (using logistic distribution) or
+ir_partial_credits.PartialCredits  ****** not yet *********************
 
 *** Main Classes:
 
 OrdinalItemResponseModel, defining a complete Bayesian model with all parameters
     adapted to a data set with individual responses to each item in a questionnaire.
     obtained from subjects in one or more different groups.
 
 *** Usage Example: see template script run_irt.py
 
-
 *** Reference:
 Leijon, Kramer et al.:
 Analysis of Data from the International Outcome Inventory for Hearing Aids (IOI-HA)
-using Bayesian Item Response Theory. 2019, Manuscript in preparation.
+using Bayesian Item Response Theory. 2020, Int J Audiol.
+doi: 10.1080/14992027.2020.1813338
 
-Arne Leijon, 2019-07-08, first functional version
+** Version history:
+* Version 0.6.0:
+2023-07-12, predictive_individual_cov uses only precision_within if only one group
+            (because precision_among is then undefined = NaN).
+
+* Version 0.5.0:
+2020-06-13, change internal names scales -> items for clarity
+2020-06-15, internal changes to allow choice of prob_class models
+
+2019-07-08, first functional version
 2019-07-23, set Initial Trait Scale only here,
     for use by both item_scale and item_respondent initialization
 2019-08-15, trying new initialization method, no boolean item_trait_map input
 2019-08-16, max_hours limit for learn
-2019-08-21, using Pool multi-processing for learn
+2019-08-21, using Pool multiprocessing for learn
+
 """
 # **** allow string item_id ? *********************
 # **** allow string trait_id ? *********************
 
 import numpy as np
 import datetime as dt
 
 from collections import Counter
 
 from .item_respondents import ResponseGroup
 from .item_trait_selector import TraitProb
-from .item_scale import make_scales
 from .trait_precision import prior_precision_within, prior_precision_among
 from .ir_predictive import GaussianGivenParam
+from .ir_graded_response_prob import GradedResponse
 
 from multiprocessing.pool import Pool
 import os
 
 import logging
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.INFO)
 # logger.setLevel(logging.DEBUG)  # test
 
 # ----------------------------------------------
-__version__ = '2020-06-06'
+__version__ = '2020-06-14'
 
 INITIAL_TRAIT_SCALE = 3.  # larger? ***********
 # = crude assumed initial scale of model trait values
 # ----------------------------------------------
 
 
 usePool = True
@@ -76,184 +90,199 @@
     The i-th item has L_i ordinal integer response values.
 
     NOTE: In most modules of this package,
     the math notation assumes that R[s, i] is an integer in range(L_i),
     i.e., it can have integer values 0, 1,..., L_i-1.
 
     However, in the input data files,
-    the recorded responses are usually coded as values 1, 2,..., L_i,
+    the recorded responses may be coded as values 1, 2,..., L_i,
     with missing values encoded as zero.
-    This response notation is used in module item_response_data.
 
     All model parameters are treated as random variables.
     The main parameter distributions are represented by equally probable samples.
 
     This package uses the Graded Response Model (Samejima, 1969, 1997):
-    Each rating R_si is assumed to be determined by ONE latent random Trait variable
+    Each rating R_si is determined by ONE latent random Trait variable
     Y_st = a real-valued random variable in the range (-inf, inf).
     There may be one or more separate trait variables,
     each determining the responses to one or more items.
 
     IF the i-th item is associated with the t-th trait,
     the latent variable Y_st is assumed to determine the response R_si as
-    a_{i, l} < Y_st <= a_{i, l+1} => R_si = l,
+    tau_{i, l} < Y_st <= tau_{i, l+1} => R_si = l,
     where the response thresholds are defined in
-    an array (a_k0, ..., a_kL) with strictly increasing elements, and
-    a_k0 = -inf; a_kL = +inf
+    an array (tau_k0, ..., tau_kL) with strictly increasing elements, and
+    tau_k0 = -inf; tau_kL = +inf
 
     The latent random variable Y_st has a logistic distribution
     with location theta_st = a subject-specific TRAIT variable,
     for the t-th trait of the s-th subject.
 
     The trait (location) parameters represent
     the individual performance measures to be estimated.
 
     The response thresholds are represented by
-    an item_scale.OrdinalItemScale object for each item,
+    an item_scale.GradedResponseItem object for each item,
     adapted to the distribution of responses from all subjects.
 
     Each item response is modelled as determined by ONE trait variable,
     identified by an item_trait_selector.TraitSelector object
     connected as a property of each item scale object.
     The association between traits and items is automatically
     estimated by the learning procedure.
 
     The scale of model parameters is arbitrary, assigned as follows:
-    The scale of the latent variable is unity during model estimation.
+    The scale of the latent-variable distribution is unity during model estimation.
     However, after learning, all model parameters may be re-scaled jointly,
-    such that the predicted global variance is unity for all traits.
+    such that the inter-individual variance is unity for all traits.
 
     The model is implemented by main properties
+    prob_class = a class defining core response probabilities,
+        given item-specific and subject-specific sets of parameters.
+        The present version allows two alternatives:
+        ir_graded_response_prob.GradedResponse, (using logistic distribution) or
+        ir_partial_credits.PartialCredits  ****** not yet *********************
     groups = a list with one item_respondents.RespondentGroup instance for each group of subjects.
-        Each group model includes all responses for each subject.
-    scales = a list of item_scale.OrdinalItemScale objects,
+        Each group model includes all responses for all subjects in the group.
+    items = a list of prob_class.item_class objects,
         each defining rating intervals for the mapping
         from latent interval-scale values to ordinal ratings.
         Each scale object has its own item_trait_selector.TraitSelector object,
         defining the association between traits and the item.
     trait_prob = an item_trait_selector.TraitProb object,
         representing the overall probability for each trait to be used for each item.
     precision_within = a trait_precision.TraitPrecisionWithinGroup object, representing
-        a Wishart distribution of the intra-group precision of trait vectors theta.
+        a Wishart distribution of the within-group precision of trait vectors theta.
     precision_among = a trait_precision.TraitPrecisionAmongGroups object, representing
         a gamma distribution for the precision of mean trait vectors between groups.
     """
     @classmethod
     def initialize(cls, data_source,
+                   prob_class=GradedResponse,  # default, only possibility so far
                    n_traits=None,
                    n_scale_samples=1,
                    n_subject_samples=50,
                    trait_scale=INITIAL_TRAIT_SCALE):
         """Initialize a model crudely from given item response data.
         :param data_source: a single ItemResponseDataSet instance,
             including response data from one or more groups of subjects.
+        :param prob_class: (optional) class of response-probability model,
+            either GradedResponse, or PartialCredits
         :param n_traits: (optional) scalar integer max number of effective latent traits
         :param n_scale_samples: (optional) number of samples of scale parameters tau for each item
         :param n_subject_samples: (optional) number of samples of trait parameter theta for each subject
         :param trait_scale: (optional) scalar initially assumed scale of model trait values
         :return: a cls instance, crudely initialized for given data_source
             to be refined later, by method learn
 
         Method:
-        1: Use item response counts to crudely initialize all item scales
-        2.1: Initialize groups with individual response data for all items, using scales
+        1: Use item response counts to crudely initialize all items
+        2.1: Initialize groups with individual response data for all items
         2.2: Use PCA or Factor Analysis (with varimax?) on these item-specific trait variables
         2.3: Transform all item-specific traits to a space with n_traits dimensions.
         3: Initialize precision_within, using data from these groups
         4: Initialize groups with only summary data
         5: Initialize precision_among using data from all groups
         """
         assert len(data_source.groups) > 0, 'Must have at least one group'
 
-        item_response_count = data_source.item_response_count
+        item_response_count = data_source.item_response_count()
         # item_response_count[i] = 1D array of response counts for i-th item
         n_items = len(item_response_count)
         if n_traits is None:
             n_traits = n_items
 
-        # ----------------------------------------- initialize scales
+        # ----------------------------------------- initialize items
         trait_prob = TraitProb.initialize(n_traits)
         logger.debug(f'Prior TraitProb.alpha = {np.array2string(trait_prob.alpha, precision=4)}')
-        scales = make_scales(item_response_count,
-                             trait_prob,
-                             n_scale_samples,
-                             trait_scale)
+        items = [prob_class.item_class.initialize(count_i,
+                                                  n_samples=n_scale_samples,
+                                                  trait_scale=trait_scale,
+                                                  trait_prob=trait_prob,
+                                                  item_index=i,
+                                                  prob_class=prob_class)
+                 for (i, count_i) in enumerate(item_response_count)]
         logger.debug('\n' +
-                     '\n'.join(f'Init scales[{i}] mean tau: '
+                     '\n'.join(f'Init items[{i}] mean tau: '
                                + np.array2string(np.mean(sc.tau, axis=0), precision=3)
                                + '; trait_sel.mean= '
                                + np.array2string(sc.trait_sel.mean, precision=2)
-                               for (i, sc) in enumerate(scales)))  # ******** do this in scales ********
+                               for (i, sc) in enumerate(items)))  # ******** do this in items ********
 
         # ----------------------------------------- initialize groups with subjects
         groups = [ResponseGroup.initialize_by_item(subject_responses=g_responses,
-                                                   scales=scales,
+                                                   items=items,
                                                    trait_scale=trait_scale,
                                                    n_samples=n_subject_samples,
                                                    name=g_name)
                   for (g_name, g_responses) in data_source.groups.items()]
         # = groups with individual response data for each item
-        # g_responses = iterable yielding subject responses, coded as a 1D list with
-        # g_responses[s][i] = integer index of response to i-th item
+        # g_responses = iterable yielding subject_responses, coded as a 1D list with
+        # subject_responses[i] = integer index of response to i-th item
         trait_cov = np.sum(g.cov_all()
                            for g in groups)
         transform_matrix = _trait_rotation(trait_cov, n_traits)
         for g in groups:
             g.transform_traits(transform_matrix)
 
         # ----------------------------------------- initialize precision_within
         precision_within = prior_precision_within(n_traits)
         precision_within.adapt((g.mean_cov_theta for g in groups))
 
         # ----------------------------------------- initialize precision_among
         precision_among = prior_precision_among(n_traits)
         logger.debug(f'prior_precision_among.b= {np.mean(precision_among.b)}')
 
-        return cls(data_source.questionnaire,
-                   groups, scales, trait_prob,
+        return cls(prob_class,
+                   data_source.questionnaire,
+                   groups, items, trait_prob,
                    precision_within, precision_among)
 
     # --------------------------------------------------------------------
-    def __init__(self, questionnaire,
-                 groups, scales, trait_prob,
+    def __init__(self, prob_class,
+                 questionnaire,
+                 groups, items, trait_prob,
                  precision_within, precision_among):
         """
+        :param prob_class: class of response-probability model
         :param questionnaire: Questionnaire object with info about the items
         :param groups: list with ResponseGroup elements
-        :param scales: list of OrdinalItemScale instances, one for each item
+        :param items: list of ResponseItem instances, one for each item
         :param trait_prob: single TraitProb object, prior for all scale.trait_sel objects
         :param precision_within: Wishart distribution object
-            representing inter-individual precision matrix
+            representing inter-individual precision matrix within each group
             for subject trait vectors, assumed valid for all subject groups
         :param precision_among: gamma distribution object
             representing inter-group precision (inverse variance)
             for mean trait vectors across groups.
         """
         self.version = __version__
+        self.prob_class = prob_class
         self.questionnaire = questionnaire
         self.groups = groups
-        self.scales = scales
+        self.items = items
         self.trait_prob = trait_prob
         # self.trait_item_map = trait_item_map
         self.precision_within = precision_within
         self.precision_among = precision_among
         # self.latent_scale = 1.  # scale parameter of logistic latent variable
         # may be changed after learning, by method standardize
         self.log_prob = []
 
-    def __repr__(self):  # **********************************
-        return (self.__class__.__name__ + '('
+    def __repr__(self):
+        return (self.__class__.__name__
+                + '(prob_class= ' + self.prob_class.__name__ + ','
                 + f'\n\t questionnaire= {self.questionnaire.__class__.__name__} '
                 + f'object with {self.questionnaire.n_items} items,'
                 + '\n\t groups= [\n\t\t'
-                + ',\n\t\t'.join(f'{g.__class__.__name__}(name={repr(g.name)}, with {g.n_subjects} subjects)'
+                + ',\n\t\t'.join(f'{g.__class__.__name__}(name={repr(g.name)}, with {g.n_subjects} respondents)'
                                  for g in self.groups) + '],'
-                + f'\n\t scales= [{len(self.scales)} item-scale objects],'
+                + f'\n\t items= [{len(self.items)} item-scale objects],'
                 + f'\n\t trait_prob = {self.trait_prob.__class__.__name__} object, '
-                + f'mapping items to {self.n_traits} latent traits, '
+                + f'mapping {len(self.items)} items to {self.n_traits} latent traits, '
                 + f'\n\t precision_within= {self.precision_within.__class__.__name__} object,'
                 + f'\n\t precision_among= {self.precision_among.__class__.__name__} object,'
                 + f'\n\t version= {self.version}'
                 + ')')
 
     @property
     def n_groups(self):
@@ -261,15 +290,15 @@
 
     @property
     def n_subjects(self):
         return sum(g.n_subjects for g in self.groups)
 
     @property
     def n_items(self):
-        return len(self.scales)
+        return len(self.items)
 
     @property
     def n_traits(self):
         return len(self.trait_prob.mean)
 
     # ------------------------------------------ General VI learn algorithm:
     def learn(self,
@@ -316,68 +345,70 @@
         """One adaptation step for all parameters
         using all response data stored in self.groups.
         :return: ll = scalar lower bound to data log-likelihood,
             incl. negative contributions for KLdiv re priors
         """
         ll = 0.
         ll += self._adapt_prec()
-        ll += self._adapt_scales()
+        ll += self._adapt_items()
         ll += self._adapt_groups()
         # *** should be done in this order,
-        # because prec are used in scales update
-        # and prec and scales are used in groups update.
+        # because prec are used in items update
+        # and prec and items are used in groups update.
         # All KLdiv calculations must use SAME distributions
         # i.e., the current value AFTER adaptations  *********************** CHECK !!!
         return ll
 
-    def _adapt_scales(self):
-        """One adaptation step for all parameters
+    def _adapt_items(self):
+        """One adaptation step for all item parameters
         using all response data stored in self.groups.
         :return: ll = scalar lower bound to data log-likelihood
         """
-        _adapt_args = (self.groups, self.trait_prob)
+        _adapt_args = (self.groups, self.trait_prob, self.prob_class)
         if usePool:
-            n_pool = _pool_size(len(self.scales))
+            n_pool = _pool_size(len(self.items))
             ch_size = 1  # *** probably slightly faster than ch_size=2
-            logger.debug(f'_adapt_scales Pool: n_pool= {n_pool}, ch_size= {ch_size}')
+            logger.debug(f'_adapt_items Pool: n_pool= {n_pool}, ch_size= {ch_size}')
             with Pool(n_pool) as p:
-                self.scales = list(p.imap(_adapt, ((sc, _adapt_args)
-                                                   for sc in self.scales),
-                                          chunksize=ch_size))
+                self.items = list(p.imap(_adapt, ((item, _adapt_args)
+                                                  for item in self.items),
+                                         chunksize=ch_size))
         else:
-            self.scales = list(map(_adapt, ((sc, _adapt_args)
-                                            for sc in self.scales)))
+            self.items = list(map(_adapt, ((item, _adapt_args)
+                                           for item in self.items)))
 
-        for (i, sc) in enumerate(self.scales):
-            logger.debug(f'scales[{i}] mean tau: '
-                         + np.array2string(np.mean(sc.tau, axis=0),
+        for (i, item) in enumerate(self.items):
+            logger.debug(f'items[{i}] mean tau: '
+                         + np.array2string(np.mean(item.tau, axis=0),
                                            precision=2, suppress_small=True)
                          + ' trait_sel.mean= '
-                         + np.array2string(sc.trait_sel.mean,
+                         + np.array2string(item.trait_sel.mean,
                                            precision=4, suppress_small=True))
         sum_r = sum(sc.trait_sel.mean
-                    for sc in self.scales)
+                    for sc in self.items)
         logger.debug('TraitProb sum responsibility = '
                      + np.array2string(sum_r, precision=2, suppress_small=True))
         ll = self.trait_prob.adapt(sum_r)
         logger.debug(f'TraitProb.adapted: mean='
                      + np.array2string(self.trait_prob.mean, precision=3, suppress_small=True)
                      + f'; ll= -KLdiv = {ll}')
         # NOTE: scale.trait_sel kl_div must be calculated AFTER TraitProb update
-        for sc in self.scales:
-            ll -= sc.relative_entropy_re_prior(self.trait_prob)  # incl. both eta and trait_sel
-        logger.debug(f'scales ll = {ll:.1f}')
+        for item in self.items:
+            ll -= item.relative_entropy_re_prior(self.trait_prob)  # incl. both eta and trait_sel
+        logger.debug(f'items ll = {ll:.1f}')
         return ll
 
     def _adapt_groups(self):
         """One adaptation step for all parameters
         using all response data stored in self.groups.
         :return: ll = scalar lower bound to data log-likelihood
         """
-        adapt_args = (self.scales, self.precision_within, self.precision_among)
+        adapt_args = (self.items,
+                      self.precision_within, self.precision_among,
+                      self.prob_class)
         if usePool:
             n_pool = _pool_size(len(self.groups))
             ch_size = 1
             logger.debug(f'_adapt_groups Pool: n_pool= {n_pool}, ch_size= {ch_size}')
             with Pool(n_pool) as p:
                 self.groups = list(p.imap(_adapt, ((g, adapt_args)
                                                    for g in self.groups),
@@ -415,44 +446,45 @@
     # ------------------------------------------------------- Result Display Functions:
 
     def item_trait_map(self):
         """Mapping with ONE trait corresponding to each item
         :return: itp = 2D boolean array
             itp[i, t] == True <=> i-th item responses were determined by t-th trait
         """
-        return np.array([sc.trait_sel.mean > 0.5 for sc in self.scales])
+        return np.array([sc.trait_sel.mean > 0.5 for sc in self.items])
 
     def prune(self):
         """Reduce model complexity by deleting any latent trait variables
         that did not correspond to any item
         :return: None
         Result: modified internal model properties
         """
         it_map = self.item_trait_map()
         keep = np.any(it_map, axis=0)
+        logger.info(f'Pruning model to {sum(keep)} active traits out of {len(keep)} initially allowed.')
         self.trait_prob.prune(keep)
         self.precision_within.prune(keep)
         self.precision_among.prune(keep)
-        for sc in self.scales:
+        for sc in self.items:
             sc.prune(keep)
         for g in self.groups:
             g.prune(keep)
 
     def standardize(self):
         """Rescale all model parameters, after learning, such that
         predictive individual trait variance is unity for all traits
         :return: None
         """
         s = np.sqrt(self.predictive_individual_var())
-        logger.info(f'Standardizing by factors '
+        logger.info(f'Standardizing trait scales by factors '
                      + np.array2string(s, precision=3))
         for g in self.groups:
             g.standardize(s)
         self._adapt_prec()
-        for sc in self.scales:
+        for sc in self.items:
             sc.standardize(s)
 
     # ------------------------------------------------------ Raw Descriptive Data:
     def item_response_count(self):
         """Total frequency of responses at each ordinal level, for each item,
         by subjects in each included group.
         :return: dict with elements (group_key, g_count), where
@@ -468,28 +500,31 @@
     # ------------------------------------------------------ Predictive Models:
     def predictive_individual_var(self):
         return np.diag(self.predictive_individual_cov())
 
     def predictive_individual_cov(self):
         """Covariance of the zero-mean Predictive distribution of IRT traits
         for a RANDOM INDIVIDUAL in any not yet seen future population,
-        similar to the sub-populations represented by the included subject groups.
+        similar to the populations represented by the included subject groups.
         :return: 2D array with covariance matrix
 
         Method: The exact predictive distribution is a continuous mixture
         of Student-t distributions.
         Samples from the exact distribution can be generated,
         but it may be sufficient to know the exact covariance
         derived from self.precision_within and self.precision_among
         """
         n_g = self.n_groups
         if n_g <= 1:
-            logger.warning(f'Uncertain predictive distribution with only {n_g} groups')
-        return (self.precision_within.mean_inv
-                + self.precision_among.mean_inv * np.eye(self.n_traits))
+            logger.warning(f'Using precision_within, ' +
+                           f'because precision_among is undefined with only {n_g} group')
+            return self.precision_within.mean_inv
+        else:
+            return (self.precision_within.mean_inv
+                    + self.precision_among.mean_inv * np.eye(self.n_traits))
 
     # def predictive_mean(self):
     #     """Predictive distribution of MEAN IRT traits
     #     in any not yet seen future population, similar to any of the sub-populations
     #     represented by the included groups of subjects.
     #     :return: PredictiveTrait instance
     #     """
@@ -509,15 +544,15 @@
                                                         tau=self.precision_among),
                                   tau=self.precision_within)
 
     # ---------------------------------- Descriptive statistics:
 
     def mean_subject_ratings(self):
         """Mean raw ratings, across items, for each respondent in each group
-        NOTE: Only informative: The raw ratings NOT on an interval scale!
+        NOTE: Only informative: The raw ratings are NOT on an interval scale!
         :return: dict with elements (group_key, mean_rating)
             mean_rating[s] = mean rating across items, by s-th subject
         """
         mr = dict()  # space for result
         for g in self.groups:
             try:
                 mr[g.name] = g.mean_response()
@@ -529,15 +564,15 @@
         """Mean ratings, across items, for each respondent in each group,
         with raw ratings re-encoded on point-estimated interval scale.
         NOTE: Only informative, point-estimates are still discrete.
         :return: dict with elements (group_key, mean_rating)
             mean_rating[s] = mean rating across items, by s-th subject
         """
         s = [np.mean(sc.typical_trait(), axis=0)
-             for sc in self.scales]
+             for sc in self.items]
         # s = point-estimated scale values on common interval scale with mean == 0
         # s[i][r] = value for r-th response to i-th item
         return {g.name: np.mean(g.scaled_subject_responses(s), axis=0)
                 for g in self.groups}
 
     def mean_subject_traits(self):
         """Mean latent trait variables in interval-scale domain, range (-inf, +inf),
@@ -548,28 +583,28 @@
         but the trait averaging presumes that separate traits (and items) represent
         measures that make sense to project onto a common uni-dimensional scale.
         :return: dict with elements (group_key, mean_trait), where
             mean_trait = 1D array with individual mean trait values
             mean_trait[s] = mean trait for s-th subject, weighted by item_trait_map
         """
         w = np.sum([sc.trait_sel.mean
-                    for sc in self.scales], axis=0)
+                    for sc in self.items], axis=0)
         w /= np.sum(w)
         # = normalized weight, for fair comparison to raw average rating across items
         return {g.name: np.mean(np.dot(g.theta, w), axis=0)
                 for g in self.groups}
 
     def estim_var_mean_subject_traits(self):
         """Estimation-variance of mean_subject_traits() results,
         used to calculate scale error component of conditional variance given mean rating.
         :return: dict with elements (group_key, estim_var), where
             estim_var = scalar variance estimate for the group
         """
         w = np.sum([sc.trait_sel.mean
-                    for sc in self.scales], axis=0)
+                    for sc in self.items], axis=0)
         w /= np.sum(w)
         # = normalized weight, for fair comparison to raw average rating across items
         # for same weighting as in mean_subject_traits()
         # divide sample variance by n_samples to estimate variance of sample mean
         return {g.name: np.mean(np.var(np.dot(g.theta, w), axis=0)) / g.n_samples
                 for g in self.groups}
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/item_scale.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_graded_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """ Module defining probability distribution of rating-interval thresholds for
 response categories in an OrdinalItemResponseModel,
 implementing the IRT Graded Response Model.
 
 *** Main Class:
-OrdinalItemScale --- defining response intervals for one item
+GradedResponseItem --- defining response intervals for one item
     represented by IRT Graded Response Model.
     Response intervals are defined by a monotonically increasing
     sequence of response thresholds.
 
 Method:
 In this version, response thresholds are indirectly determined by vector
 eta = logarithm of non-normalized width parameters in the logistic-mapped domain.
+This method ensures that thresholds are monotonically increasing,
+for increasing ordinal responses.
+
 The prior distribution of eta is Gaussian,
 and the posterior is approximated by a set of equally probable sample vectors,
 or by a single MAP estimate.
 
 To avoid numerical overflow during sampling,
 the eta samples are also restricted between (wide) fixed bounds,
 so the prior eta distribution is actually a (mildly) truncated Gaussian.
@@ -24,16 +27,17 @@
 2019-07-23, fixed bug in scale.initialize, Initial Trait Scale set externally
 2019-08-10, use a TraitSelector object for item-trait mapping
 2019-08-16, try uniform TraitSelector initialization
 2019-08-24, use np.random.Generator for sampling
 2019-08-25, sample_trait and typical_trait assuming Gaussian inter-individual trait distribution
 2020-02-06, adapt including initial MAP point estimate for faster(?) sampling
 2020-02-13, allow n_samples == 1 in method relative_entropy_re_prior
+2020-06-15, internal changes to use external prob_class for core probability functions
 """
-# **** after testing, include latent_scale as OrdinalItemScale property
+# **** after testing, include latent_scale as GradedResponseItem property
 # **** allow string item_id ? *********************
 
 import numpy as np
 from scipy.stats import norm
 from scipy.optimize import minimize
 
 from .safe_logistic import logistic
@@ -61,75 +65,60 @@
 # = Jeffreys prior for Dirichlet distribution of probability vector,
 # given response counts
 
 RANDOM_G = np.random.default_rng()
 # = module-global random generator, Numpy 1.17
 
 
-# ------------------------------------------- main initialization function:
-def make_scales(item_response_count, trait_prob, n_scale_samples, trait_scale):
-    """Initialize all item scale objects, and corresponding trait mapping objects.
-    :param item_response_count: 1D list of response-count lists
-        item_response_count[i][l] = number of responses == l for i-th item
-    :param trait_prob: prior TraitProb instance initialized by caller
-    :param n_scale_samples: scalar integer number of samples in each scale object
-    :param trait_scale: scalar initially assumed scale of model trait values
-    :return: scales = list with one OrdinalItemScale object for each item
-    """
-    scales = [OrdinalItemScale.initialize(count_i,
-                                          n_samples=n_scale_samples,
-                                          trait_scale=trait_scale,
-                                          trait_prob=trait_prob,
-                                          item_index=i)
-              for (i, count_i) in enumerate(item_response_count)]
-    return scales
-
-
 # --------------------------------------------------------------------
-class OrdinalItemScale:
+class GradedResponseItem:
     """Class defining response thresholds,
     and learning of scale parameters,
     for ONE item in an OrdinalItemResponseModel.
 
     Response interval widths in the logistic-transformed domain
     are proportional to 1D array w, which is represented as
     w = np.exp(eta)
     In each adapt step, the posterior distribution of eta
     is approximated by a set of sample vectors,
     or by a single MAP estimate.
     """
     @classmethod
-    def initialize(cls, response_count, trait_scale, n_samples, trait_prob, item_index):
+    def initialize(cls, response_count, trait_scale, n_samples, trait_prob,
+                   item_index, prob_class):
         """Initialize a scale object crudely to agree with given response counts.
         :param response_count: 1D array with total response counts
             response_count[l] = count of response == l
         :param trait_scale: scalar = initial scale of theta distribution
         :param n_samples: number of samples
         :param trait_prob: single prior TraitProb object for all scale.trait_sel objects
         :param item_index: scalar integer item identifier for this scale
+        :param prob_class: class of response-probability model
         :return: a single cls object
         """
         f = np.cumsum(response_count + PSEUDO_COUNT)
         p_cum = f / f[-1]
         tau = norm.ppf(p_cum[:-1], scale=trait_scale)
         # tau[l] = upper limit of interval for response==l
         cum_w = np.concatenate(([0.], logistic.cdf(tau), [1.]))  # corrected 2019-07-23
         w = np.diff(cum_w)
         eta = np.log(w)
         # eta[l] = log width in transformed domain for l-th response interval
         eta = np.tile(eta, (n_samples, 1))
-        return cls(eta, TraitSelector(trait_prob.mean), item_index)
+        return cls(eta, TraitSelector(trait_prob.mean), item_index, prob_class)
 
-    def __init__(self, eta, trait_sel, item_index):
+    def __init__(self, eta, trait_sel, item_index, prob_class):
         """
         :param eta: log interval width in logistic-transformed domain
             eta[n, l] = n-th sample of log-width for l-th response interval
         :param trait_sel: a TraitSelector object for this item
         :param item_index: scalar integer item identifier for this scale
+        :param prob_class: class of response-probability model
         """
+        self.prob_class = prob_class
         self.item_index = item_index
         eta -= np.mean(eta, axis=1, keepdims=True)
         # forced to zero mean
         too_small = np.log(0.001)
         too_big = np.log(1000.)
         # => ratio about 1e6 between widest and smallest interval width
         b = [(too_small, too_big) for _ in range(eta.shape[-1])]
@@ -139,14 +128,15 @@
                                                      x=eta,
                                                      bounds=b,
                                                      epsilon=0.2,
                                                      n_leapfrog_steps=10)
         # sampler.args to be defined later
         # NOTE: eta is stored only as sampler.x
         self.trait_sel = trait_sel
+        self.latent_scale = 1.
 
     def __repr__(self):
         return (self.__class__.__name__ + f'(item_index= {self.item_index},'
                 + f'\n\teta=\n\t{repr(self.eta)},'
                 + f'\n\ttrait_sel= {repr(self.trait_sel)}'
                 + ')')
 
@@ -168,78 +158,128 @@
         :return: 2D array tau, with
             tau[m, l] = m-th sample of UPPER threshold for l-th interval,
             NOT including extreme values at -inf and +inf
             tau.shape[-1] == self.n_response_levels - 1
         """
         return _tau(np.exp(self.eta))
 
+    def typical_latent(self, theta_scale=1.):
+        """APPROXIMATE point estimates of trait values, given any response,
+        estimated at conditional mean of latent variables within each response interval,
+        assuming Gaussian traits with zero mean and scale = theta_scale,
+        and current latent_scale of logistic latent variable,
+        using current sampled distribution of scale thresholds.
+        :param theta_scale: scalar = current (assumed) scale of theta distribution
+        :return: theta = 2D array, with
+            theta[m, l] = m-th sample of typical trait for response == l
+            theta.shape[-1] == self.n_response_levels
+
+        NOTE: 2020-06-16, include latent variance
+        Method: Expected value of latent variable, given response
+        """
+        latent_var = self.latent_scale**2 * np.pi**2 / 3
+        latent_scale = np.sqrt(theta_scale**2 + latent_var)
+        # = approximate st.dev. of latent-variable scale in population
+        typ_mean = _cond_mean(self.tau, scale=latent_scale)
+        return typ_mean
+
     def typical_trait(self, theta_scale=1.):
-        """Point estimates of trait values, given any response,
-        estimated at conditional mean within each response interval,
+        """APPROXIMATE point estimates of trait values, given any response,
+        estimated at conditional mean of latent variables within each response interval,
         assuming Gaussian traits with zero mean and scale = theta_scale,
+        and current latent_scale of logistic latent variable,
         using current sampled distribution of scale thresholds.
         :param theta_scale: scalar = current (assumed) scale of theta distribution
         :return: theta = 2D array, with
             theta[m, l] = m-th sample of typical trait for response == l
             theta.shape[-1] == self.n_response_levels
+
+        NOTE: Old version, using only trait_scale
+        Method: Expected value of latent variable, given response
         """
-        # typ_median = _cond_median(self.tau, scale=theta_scale)
+        # latent_var = self.latent_scale**2 * np.pi**2 / 3
+        # latent_scale = np.sqrt(theta_scale**2 + latent_var)
+        # # = approximate st.dev. of latent-variable scale in population
         typ_mean = _cond_mean(self.tau, scale=theta_scale)
         return typ_mean
 
+    def mean_trait_ordinal(self, theta_scale=1.):
+        """Point estimates of posterior mean trait values, given each ordinal response,
+        assuming Gaussian traits with zero mean and scale = theta_scale,
+        using current sampled distribution of scale thresholds.
+        :param theta_scale: scalar = current (assumed) scale of theta distribution
+        :return: theta = 1D array, with
+            theta[l] = typical trait for response == l
+            theta.shape == (self.n_response_levels,)
+
+        Method: Expected value of posterior trait distribution, given response,
+        ***** strange results ??? not aligned with typical_latent
+        """
+        th = np.linspace(-10 * theta_scale, 10 * theta_scale, num=10000)
+        p_prior = norm.pdf(th)
+        p_given_th = self.ordinal_prob(th)
+        p_post = p_given_th * p_prior[:, np.newaxis]
+        th_mean = np.sum(p_post * th[:, np.newaxis], axis=0) / np.sum(p_post, axis=0)
+        return th_mean
+
     def sample_trait(self, r, n_samples, trait_scale=1.):
-        """
-        Generate samples of possible trait values, given subjects' responses
+        """Generate crude initial samples of possible trait values,
+        given subjects' responses.
+        Trait samples have truncated Gaussian distribution,
+        restricted to the interval defined by ordinal response and self.tau.
         :param r: 1D array with integer response indices, origin == 0
-            r[s] = l in range(self.n_response_levels
+            r[s] = l in range(self.n_response_levels)
             means s-th subject gave l-th response to this item
         :param n_samples: number of desired samples for each subject
         :param trait_scale: scalar = current (assumed) scale of theta distribution
         :return: th = 2D array of samples
             th[m, s] = m-th sample for s-th subject
         """
         def s_sample(r_s):
             """Sample in transformed (0, 1) range for ONE subject
             :param r_s: scalar integer response by this subject
-            :return: 1D array th_s; len(th_s) == n_samples
+            :return: 1D array th_s with uniform samples in allowed range
+                len(th_s) == n_samples
             """
             if r_s < 0:
                 return RANDOM_G.uniform(low=th_limits[0], high=th_limits[-1], size=n_samples)
             else:
                 return RANDOM_G.uniform(low=th_limits[r_s], high=th_limits[r_s + 1], size=n_samples)
         # ----------------------------------------------------------------------
         th_limits = np.mean(self.tau, axis=0)
         th_limits = np.concatenate(([np.finfo(float).tiny],
                                     norm.cdf(th_limits, scale=trait_scale), [1.]))
         # tiny lowest limit, because RANDOM.uniform samples in [0, 1),
         # but we allow only samples in (0., 1)
         th = [s_sample(r_s) for r_s in r]
         return norm.ppf(np.array(th).T, scale=trait_scale)
 
-    def ordinal_prob(self, theta):
+    def ordinal_prob(self, theta):  # *** done by prob_class ***** ???
         """Conditional probability of ordinal responses, given trait value,
         averaged across scale samples
         :param theta: array of trait values
         :return: pr = array of response probabilities
             pr[..., l] = P{response = l | theta[...]}
             = logistic.cdf(theta[...] - tau[l]) - logistic.cdf(theta[...] - tau[l-1])
             pr.shape == (*theta.shape, self.n_response_levels)
         """
         try:
             s = self.latent_scale
         except NameError:
             s = 1.
-        t = self.tau - theta[..., np.newaxis, np.newaxis]
-        t /= s
-        cdf = np.mean(logistic.cdf(t), axis=-2)  # average across samples
-        p = np.concatenate((np.zeros((*cdf.shape[:-1], 1)),
-                            cdf,
-                            np.ones((*cdf.shape[:-1], 1))),
-                            axis=-1)
-        p = np.diff(p, axis=-1)
+        # t = self.tau - theta[..., np.newaxis, np.newaxis]
+        # t /= s
+        # cdf = np.mean(logistic.cdf(t), axis=-2)  # average across samples
+        # p = np.concatenate((np.zeros((*cdf.shape[:-1], 1)),
+        #                     cdf,
+        #                     np.ones((*cdf.shape[:-1], 1))),
+        #                     axis=-1)
+        # p_old = np.diff(p, axis=-1)
+        p = self.prob_class.response_prob_by_theta(theta, self.tau, s)
+        # p[..., l] = m-th sample of l-th response by theta[...]
         return p
 
     def mean_ordinal(self, theta):
         """Expected value of ordinal response level, given trait
         :param theta: array of trait values
         :return: r = expected "response" on continuous scale
             r[...] = sum_l l * P{response = l | theta[...]}
@@ -253,50 +293,55 @@
         is sometimes used without hesitation in the Rasch research tradition,
         Ref, e.g.: Wright and Masters (1982), Eq. 5.4.1.
         The expected rating plotted vs individual trait value
         is sometimes called Item Characteristic Curve (ICC).
         """
         return np.dot(self.ordinal_prob(theta), np.arange(self.n_response_levels))
 
-    def rating_from_trait(self, theta):  # *** use mean_ordinal instead **********
-        """Calculate mean equivalent continuous-valued "rating",
-        in finite interval (- 0.5, n_rating_levels - 0.5)
-        corresponding to given latent variable(s), such that
-        th = tau[l] -> rating = l + 0.5
-        with linear interpolation in the logistic-transformed (0, 1) range.
-        :param theta: array-like 1D sequence of trait values in range (-inf, +inf)
-        :return: z = rating-transformed values of y
-            z.shape == y.shape
-        """
-        p_theta = logistic.cdf(theta)
-        p_tau = logistic.cdf(np.mean(self.tau, axis=0))
-        p_tau = np.concatenate(([0.], p_tau, [1.]))
-        # = p corresponding to ratings [-0.5, 0.5, ..., n_rating_levels-0.5
-        n_tau = len(p_tau)
-        rp = np.linspace(-0.5, n_tau - 1.5, n_tau)
-        return np.interp(p_theta, p_tau, rp) # + self.min_rating
+    # def rating_from_trait(self, theta):  # *** use mean_ordinal instead **********
+    #     """Calculate mean equivalent continuous-valued "rating",
+    #     in finite interval (- 0.5, n_rating_levels - 0.5)
+    #     corresponding to given latent variable(s), such that
+    #     th = tau[l] -> rating = l + 0.5
+    #     with linear interpolation in the logistic-transformed (0, 1) range.
+    #     :param theta: array-like 1D sequence of trait values in range (-inf, +inf)
+    #     :return: z = rating-transformed values of y
+    #         z.shape == y.shape
+    #     """
+    #     p_theta = logistic.cdf(theta)
+    #     p_tau = logistic.cdf(np.mean(self.tau, axis=0))
+    #     p_tau = np.concatenate(([0.], p_tau, [1.]))
+    #     # = p corresponding to ratings [-0.5, 0.5, ..., n_rating_levels-0.5
+    #     n_tau = len(p_tau)
+    #     rp = np.linspace(-0.5, n_tau - 1.5, n_tau)
+    #     return np.interp(p_theta, p_tau, rp) # + self.min_rating
 
-    def adapt(self, groups, trait_prob):
+    def adapt(self, groups, trait_prob, p_class):
         """One variational-inference update step of sample parameters eta.
         :param groups: list with ResponseGroup instances
             that can calculate log-likelihood values for given response thresholds.
         :param trait_prob: single TraitProb object, prior for self.trait_sel
+        :param p_class: core class calculating response-prob and gradients
         :return: self
             Must call relative_entropy_re_prior later !
         """
         logger.debug(self.__class__.__name__ + f'[{self.item_index}].adapt(...)')
+
         # ------ adapt trait selector first, with old tau:
-        log_trait_resp = sum(np.mean(g.item_logprob_by_tau(self.tau, self.item_index),
+        log_trait_resp = sum(np.mean(p_class.logprob_by_tau(theta=g.theta,
+                                                            tau_i=self.tau,
+                                                            w_i=None,
+                                                            r_i=g.response0[self.item_index]),
                                      axis=0)
                              for g in groups)
         # log_trait_resp[t] = mean logprob given t-th trait
         self.trait_sel.adapt(log_trait_resp, trait_prob)
 
         # ------ adapt self.eta, to define new self.tau:
-        self.sampler.args = (groups, self.item_index, self.trait_sel.mean)
+        self.sampler.args = (groups, self.item_index, self.trait_sel.mean, p_class)
         # ---------- first adjust by point estimate:
         eta_old = np.mean(self.sampler.x, axis=0)
         eta_new = self.adapt_point(eta_old)
         self.sampler.x += eta_new - eta_old
         logger.debug(f'scale[{self.item_index}] point adapted: diff= '
                      + np.array2string(eta_new - eta_old,
                                        precision=2,
@@ -328,33 +373,26 @@
         self.sampler.x -= np.mean(self.sampler.x, axis=-1, keepdims=True)
         # adding a constant to all eta does not change any thresholds
         # --------------------------------- DONE distribution of eta
         if self.n_samples > 10:
             logger.debug(f'Scale[{self.item_index}]: tau percentiles=\n'
                          + np.array2string(np.percentile(self.tau, axis=0, q=[5, 50, 95]),
                                            precision=3, suppress_small=True))
-        # # ------ adapt trait selector AFTER, with new traits:
-        # log_trait_resp = sum(np.mean(g.item_logprob_by_tau(self.tau, item_index),
-        #                              axis=0)
-        #                      for g in groups.values())
-        # # log_trait_resp[t] = mean logprob given t-th trait
-        # self.trait_sel.adapt(log_trait_resp)
-        # # **** self.trait_sel KL_div penalty must be calculated later, after TraitProb update ****
         logger.info(self.__class__.__name__ + f'[{self.item_index}].adapt(...) finished')
         return self
 
     def adapt_point(self, eta_0):
         """Find single MAP point estimate of eta,
         using same objective functions as sampler
         :param eta_0: 1D vector with start value
         :return: eta = 1D vector with new point estimate
             eta.shape == eta_0.shape == self.n_response_levels
         """
         def neg_logprob_1d(eta, *args):
-            """Link to module-global function for 1D input
+            """Link to module function for 1D input
             :param eta: 1D vector with tentative parameter values
             :param args: tuple with additional arguments
             :return: nlp = scalar = - log p(data | eta)
             """
             return neg_logprob(eta[None, :], *args)[0]
 
         def d_neg_logprob_1d(eta, *args):
@@ -415,68 +453,81 @@
         tau = self.tau / s
         n_samples = tau.shape[0]
         # tau[m, l] = m-th sample of new upper limit of l-th response interval
         p = logistic.cdf(tau)  # in (0, 1) domain
         p = np.concatenate((np.zeros((n_samples, 1)), p, np.ones((n_samples, 1))),
                            axis=1)
         w = np.diff(p, axis=1)
+        # ********************** use prob_class.response_prob_by_theta to do this ??? ******
         # w[m, l] = width parameters in (0, 1) domain
         eta = np.log(w)
         self.latent_scale = 1. / s  # *********************
         # = new eta sample values defining rescaled tau values
         logger.debug(f'Scale[{self.item_index}]: Old mean tau = '
                      + np.array2string(np.mean(self.tau, axis=0),
                                        precision=3, suppress_small=True))
         self.sampler.x = eta
         # just to check for new values:
         logger.debug(f'Scale[{self.item_index}]: Rescaled mean tau = '
                      + np.array2string(np.mean(self.tau, axis=0),
                                        precision=3, suppress_small=True))
 
 
-# -------------------------- internal module functions
+# ------------------------------------------- internal module functions
 
-def neg_logprob(eta, groups, item_index, trait_w):
+def neg_logprob(eta, groups, item_index, trait_w, p_class):
     """Negative sum of log prob of observed data, given tentative samples.
     :param eta: 2D array with tentative sample values
         eta[n, l] = n-th sample of l-th log-width parameter
     :param groups: list with ref to all response groups
     :param item_index: integer index for this item
     :param trait_w: 1D weight vector
         trait_w[t] = weight for t-th trait
+        :param p_class: core class calculating response-prob and gradients
     :return: nlp = 1D array
         nlp[n] = negative log-prob for n-th tentative sample
         len(nlp) == eta.shape[0]
     """
     w = np.exp(eta)
     tau = _tau(w)
-    lp = sum(g.item_logprob_by_tau(tau, item_index, trait_w)
+    # lp_old = sum(g.logprob_by_tau(tau, item_index, trait_w)
+    #              for g in groups)
+    lp = sum(p_class.logprob_by_tau(theta=g.theta,
+                                    tau_i=tau,
+                                    w_i=trait_w,
+                                    r_i=g.response0[item_index])
              for g in groups)
     if np.any(np.isnan(lp)):
         logger.warning('Scale[{self.item_index}]: neg_logprob == nan. *** Should never happen!')
     return - lp - prior_logprob(eta)
 
 
-def d_neg_logprob(eta, groups, item_index, trait_w):
+def d_neg_logprob(eta, groups, item_index, trait_w, p_class):
     """Gradient of neg_logprob, given tentative samples.
     :param eta: 2D array with tentative sample values
         eta[n, l] = n-th sample of l-th log-width parameter
     :param groups: list with ref to all response groups
     :param item_index: integer index for this item
     :param trait_w: 1D weight vector
         trait_w[t] = weight for t-th trait
+    :param p_class: core class calculating response-prob and gradients
     :return: dnlp = 2D array
         dnlp[n, l] = d neg_logprob(eta[n]) / d eta[n, l]
         dnlp.shape == eta.shape
     """
     w = np.exp(eta)
     tau = _tau(w)
     if np.any(tau == -np.inf) or np.any(tau == np.inf):
         logger.warning('Scale[{self.item_index}]: Infinite tau. *** Should never happen!')
-    d_lp_d_tau = sum(g.d_item_logprob_by_tau(tau, item_index, trait_w)
+    # d_lp_d_tau_old = sum(g.d_logprob_by_tau(tau, item_index, trait_w)
+    #                      for g in groups)
+    d_lp_d_tau = sum(p_class.d_logprob_by_tau(theta=g.theta,
+                                              tau_i=tau,
+                                              w_i=trait_w,
+                                              r_i=g.response0[item_index])
                      for g in groups)
     dlp = np.einsum('mk, mkl -> ml',
                     d_lp_d_tau, _d_tau_d_eta(w))
     return - dlp - d_prior_logprob(eta)
 
 
 def prior_logprob(eta):
@@ -517,14 +568,15 @@
     """Jacobian of _tau(w)
     :param w: 2D array of non-normalized interval-width parameters = np.exp(eta)
         w[n, l] = proportional to n-th sample of l-th interval width
         in logistic-transformed domain
     :return: 3D array dt_dw, with
         dt_dw[n, l, j] = d _tau[n, l] / dw[n, j]
         dt_dw.shape == (w.shape[0], w.shape[1]-1, w.shape[1])
+
     Method:
     t_l = log(w_0 +...+ w_l) - log(w_{l+1} +...+ w_{L-1}); l = 0,..., L-2, any n
     dt_nlj / d w_nj =
         = +1 / (w_0 +...+ w_l); j <= l
         = -1 / (w_{l+1}+...+w_{L-1}); j > l
     2019-07-04 seems OK
     """
@@ -548,39 +600,41 @@
         dt_d_eta.shape == (w.shape[0], w.shape[1]-1, w.shape[1])
     2019-07-04, sum(_d_tau_d_eta(w), axis=-1) == 0. as it should
     """
     return _d_tau_dw(w) * w[:, None, :]
 
 
 def _cond_mean(tau, scale=1.):
-    """Conditional means of trait values for each ordinal rating,
-    for each rating-interval limits on the latent scale,
-    assuming traits are normal-distributed with given scale
+    """Approximate conditional means of latent variable for each ordinal rating,
+    for each rating interval on the latent scale,
+    assuming traits are normal-distributed with known scale,
+    AND latent variables are APPROXIMATELY normal distributed, given trait.
     :param tau: 2D array with upper interval limits for rating
         tau[m, l] = m-th sample of upper interval limit for rating == l
         lower limit is - inf for l == 0
         upper limit is + inf for l == n_rating_levels-1
         tau.shape[-1] == n_rating_levels - 1
+    :param scale: scalar st.dev. of latent variable in population
     :return: theta = 2D array with mean traits
         theta[m, l] = m-th sample of conditional mean trait, given rating=l
         theta.shape == (tau.shape[0], n_rating_levels)
     """
     n_samples = tau.shape[0]
     n_rating_levels = tau.shape[1] + 1
     tau = np.concatenate((np.full((n_samples,1), - np.inf),
                           tau,
                           np.full((n_samples,1), np.inf)), axis=1)
-    return np.array([[norm.expect(scale=scale, lb=tau_m[l], ub=tau_m[l+1],
+    return np.array([[norm.expect(scale=scale, lb=tau_m[l], ub=tau_m[l + 1],
                                   conditional=True)
                       for l in range(n_rating_levels)]
                      for tau_m in tau])
 
 
 def _cond_median(tau, scale=1.):  # **** not used, but much faster than _cond_mean
-    """Conditional medians of trait values for each ordinal rating,
+    """Conditional medians of latent variable for each ordinal rating,
     for each rating-interval limits on the latent scale,
     assuming traits are normal-distributed with given scale
     :param tau: 2D array with upper interval limits for rating
         tau[m, l] = m-th sample of upper interval limit for rating == l
         lower limit is - inf for l == 0
         upper limit is + inf for l == n_rating_levels-1
         tau.shape[-1] == n_rating_levels - 1
@@ -617,17 +671,17 @@
     print('_d_tau_dw(w)= ', _d_tau_dw(w))
 
     dt_d_eta = _d_tau_d_eta(w)
     print('_d_tau_d_eta(w)= ', dt_d_eta)
     print('sum dt_d_eta= ', np.sum(dt_d_eta, axis=-1))
 
     trait_prob = TraitProb.initialize(5)
-    item_sc = OrdinalItemScale.initialize(10 * w[0], n_samples=3, trait_scale=3.,
-                                          trait_prob=trait_prob,
-                                          item_index=0)
+    item_sc = GradedResponseItem.initialize(10 * w[0], n_samples=3, trait_scale=3.,
+                                            trait_prob=trait_prob,
+                                            item_index=0)
     print('item_sc= ', item_sc)
     print('item_sc.n_samples=', item_sc.n_samples)
     print('item_sc.n_response_levels=', item_sc.n_response_levels)
     print('item_sc.eta=\n', item_sc.eta)
     print('item_sc.tau=\n', item_sc.tau)
     # print('item_sc.typical_trait=\n', item_sc.typical_trait())
     r = [-1, 0, 1, 2, 3, 4]
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/item_trait_selector.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_trait_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # = prior concentration parameters for TraitProb Dirichlet distribution
 
 
 # ----------------------------------------------------------
 class TraitSelector:
     """Probability distribution of a one-of-D boolean switch array
     z = (z_1, ..., z_D) with only ONE element z_d == True,
-    used as property trait_sel of ONE OrdinalItemScale object
+    used as property trait_sel of ONE GradedResponseItem object
     indicating that responses to this object
     are determined by the the d-th trait.
     """
     def __init__(self, weight):
         """
         :param weight: 1D array with un-normalized probability mass elements
         """
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/__init__.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,79 +22,86 @@
 
 NOTE: In most modules of this package,
 the ordinal response to the i-th item is encoded as
 an integer in {0, 1,..., L_i-1},
 where L_i = the number of ordinal response levels for the i-th item.
 Any value outside this range is interpreted as a missing response.
 
-However, in the input data files,
-the recorded responses are usually encoded as integers in {1, 2,..., L_i},
+However, in data files with recorded responses,
+the recorded responses are sometimes encoded as integers in {1, 2,..., L_i},
 with missing values encoded as zero.
-This notation is used in module item_response_data.
-and in some results presentations where response levels are identified.
+Other response files may instead store the actual text labels
+on the response alternatives in the questionnaire.
 
+Therefore, the package user must specify the response encoding
+separately for each input data source.
 
 *** Usage
 
 Copy the template script `run_irt.py` to your working directory, rename it, and
 edit the copy as suggested in the template, to specify
     - your experimental layout,
     - your input data file(s),
     - a directory where all output result files will be stored.
 
 *** Main Modules
 
 item_response_data:
     Interface to one or several data sets containing individual responses
-    from respondents recruited from one or several different population(s).
+    from respondents recruited from one or more separate population(s).
     See this module for information about input files and data formats.
 
 item_response_model:
     The core of the Bayesian IRT model adapted to all observed data.
 
-item_scale:
+item_graded_response:
     Classes representing the item-specific model parameters,
-    defining the connection between traits to ordinal responses, for each item.
+    defining the connection between latent traits and ordinal responses, for each item.
 
 item_respondents:
     Classes representing individual- and population-specific models
     defining trait distributions for each individual and each population.
 
 ir_display:
     Functions and classes to display all analysis results as figures and tables.
     
-table_reader:
-    Defines class Table for input data in several accepted file formats.
-    The present version can read tabulated data from sources of type
-    xlsx, csv, sql, sqlite3.
+ir_source:
+    Implements access methods for input data in several source types,
+    e.g., Excel or CSV files, or SQL database,
+    using reader functions available in package Pandas,
+    or a similar user-defined reader function.
 
 Analysis results are saved as figures and tables in the selected result directory.
 After running an analysis, the logging output briefly explains
 the analysis results presented in figures and tables.
 
 *** References
-Arne Leijon and Harvey Dillon and Louise Hickson
-and Martin Kinkel and Sophia E Kramer and Peter Nordquist (2020):
-    Analysis of Data from the International Outcome Inventory for Hearing Aids (IOI-HA)
-    using Bayesian Item Response Theory.
-    Manuscript in preparation.
 
+A. Leijon, H. Dillon, L. Hickson, M. Kinkel, S. E. Kramer, and P. Nordqvist.
+    Analysis of data from the international outcome inventory for hearing aids (IOI-HA)
+    using Bayesian item response theory. Int J Audiol 60(2):81–88, 2020.
+    doi: 10.1080/14992027.2020.1813338
 J.-P. Fox (2010). *Bayesian Item Response Modeling: Theory and Applications*.
     Statistics for Social and Behavioral Sciences. Springer.
 G. N. Masters (1982). A Rasch model for partial credit scoring.
     *Psychometrika*, 47(2):149–174.
 F. Samejima (1997). Graded response model.
     In W. J. v. D. Linden and R. K. Hambleton, eds.,
     *Handbook of Modern Item Response Theory*, p. 85–100. Springer, New York.
 
 
 *** Version History
 
-2019-08-24, first functional version with automatic selection of trait dimensionality.
+* Version 0.6.0:
+2023-07-07, using package pandas to access input data files, and for tabulated results.
+
+* Version 0.5:
+2020-06-xx, prepare to allow different item response probability models-
 2020-06-08, first version uploaded to PyPi, tested with several IOI-HA data sets.
+2019-08-24, first functional version with automatic selection of trait dimensionality.
 """
 
 __name__ = 'ItemResponseCalc'
-__version__ = '0.5.0'
-__all__ = ['__version__', 'run_irt', 'show_irt']
+__version__ = '0.6.0'
+__all__ = ['__version__', 'run_irt']
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/ir_display_format.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_display_format.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,288 +1,327 @@
 """Functions and classes to display results from an OrdinalItemResponseModel object.
-"""
-# ***** check special chars for latex and txt variants
+** Version history:
+
+* Version 0.6:
+2023-07-07, rely mainly on matplotlib.rcParams for plot styles
+2023-07-06, define name of FigureRef and ResultTable already when created
+2023-07-05, new table result functions using Pandas for result tables
 
+* Version 0.5: first published version
+"""
 import numpy as np
 from itertools import cycle, product
 
 import matplotlib.pyplot as plt
 import logging
 
+import pandas as pd
+
 logger = logging.getLogger(__name__)
 
 # --------------------------- Default format parameters:
-FMT = {'table_format': 'latex',  # or 'tab' for tab-delimited tables
-       'figure_format': 'pdf',   # or 'eps', or 'png', or 'pdf', for saved plots
-       'colors': 'rbg',  # color cycle to separate results in plots
+FMT = {'colors': 'rbg',  # color cycle to separate results in plots
        'line_styles': ['solid', 'dashed', 'dashdot', 'dotted'],
        'markers': 'o^sDv',  # plot symbols, each repeated with each fillstyle
        'fillstyle': ['full', 'none'], # marker style
-       'credibility': 'Credibility',  # heading in tables
-       'correlation': 'Correlation',  # heading in tables
        }
 # = module-global dict with default settings for display details
 # that may be changed by user
-# NOTE: Largest number of combinations of color, line_style, marker, fillstyle
-# is obtained if the number of alternatives are NOT divisible by each other.
 
-TABLE_FILE_SUFFIX = {'latex': '.tex', 'tab': '.txt'}
-# = mapping table_format -> file suffix
+# NOTE: FMT['colors'], FMT['linestyles'], FMT['markers'], and FMT['fillstyle']
+#   override any corresponding properties in matplotlib.rcParams,
+#   because rcParams.axes.prop_cycle allows only equal lengths of property sequences.
+#   Here, the UNEQUAL lengths of FMT default sequences will combine
+#   into a sequence with many combinations, before the style repeats itself.
 
-# ------------------------- Matplotlib settings:
-plt.rcParams.update({'figure.max_open_warning': 0})
-# suppress warning for many open figures
-pad_inches = plt.rcParams['savefig.pad_inches']
-plt.rcParams['savefig.pad_inches'] = 0.
-plt.rcParams['savefig.bbox'] = 'tight'
-# *** allow user to set other plt.rcParams ? ***
-# -----------------------------------------------
-
-
-def set_format_param(**kwargs):
-    """Set / modify module-global format parameters
-    :param kwargs: dict with format variables
-        to replace the default values in FMT
-    :return: None
+
+class FileWriteError(RuntimeError):
+    """Any type of exception while attempting to write a pd.DataFrame table to a file
     """
-    # *** allow user to set other plt.rcParams here ? ***
-    for (k, v) in kwargs.items():
-        k = k.lower()
-        if k not in FMT:
-            logger.warning(f'Format setting {k}={repr(v)} is not known, not used')
-        FMT[k] = v
 
 
-def _percent():
-    """Percent sign for tables
-    :return: str
+def set_format_param(mpl_style=None, mpl_params=None, **kwargs):  # copied from EmaCalc
+    """Set / modify format parameters.
+    Called before any displays are generated.
+    :param mpl_style: (optional) matplotlib style sheet, or list of style sheets
+    :param mpl_params: (optional) dict with matplotlib (k, v) rcParam settings
+    :param kwargs: dict with any formatting variables to be stored in FMT
+    :return: None
     """
-    return '\\%' if FMT['table_format'] == 'latex' else '%'
+    if mpl_style is not None:
+        plt.style.use(mpl_style)
+    if mpl_params is not None:
+        plt.rcParams.update(mpl_params)
+    other_fmt = dict()
+    for (k, v) in kwargs.items():
+        k = k.lower()
+        if k in FMT:
+            FMT[k] = v
+        else:
+            other_fmt[k] = v
+    if len(other_fmt) > 0:
+        logger.warning(f'Parameters {other_fmt} unknown, not used.')
 
 
 # ---------------------------- Main Result Classes
 class FigureRef:
     """Reference to a single graph instance
     """
-    def __init__(self, ax, name=None, path=None):
+    def __init__(self, ax, name=None):  # ***, path=None):
         """
         :param ax: Axes instance containing the graph
-        :param path: Path to directory where figure has been saved
-        :param name: (optional) updated name of figure file
+        :param name: string name of figure
         """
         self.ax = ax
         self.name = name
-        self.path = path
-
-    def __repr__(self):
-        return (f'FigureRef(ax= {repr(self.ax)}, ' +
-                f'name= {repr(self.name)}), path= {repr(self.path)}')
 
     @property
     def fig(self):
         return self.ax.figure
 
-    def save(self, path, name=None):
+    def save(self, path,
+             figure_format):
         """Save figure to given path
         :param path: Path to directory where figure is saved
-        :param name: (optional) updated name of figure file
+        :param figure_format: file format of saved figure
         :return: None
-        Result: updated properties path, name
         """
-        if name is None:
-            name = self.name
-        name = _clean_file_name(name)
-        path.mkdir(parents=True, exist_ok=True)
-        f = (path / name).with_suffix('.' + FMT['figure_format'])
-        self.fig.savefig(str(f))
-        self.path = path
-        self.name = f.name
+        if figure_format is not None:
+            name = _clean_file_name(self.name)
+            path.mkdir(parents=True, exist_ok=True)
+            f = (path / name).with_suffix('.' + figure_format)
+            try:
+                self.fig.savefig(f)
+            except Exception as e:  # any error, just warn and continue
+                logger.warning(f'Could not save plot to {f}. Error: {e}')
 
-    def mapped_y_axis(self, y, y_mapped, y_label='', fontsize=14):
+    def mapped_y_axis(self, y, y_mapped, y_label=''):
         """Add a second y_axis to self.ax with ticks placed at
         y values corresponding to uniform steps in y_mapped values
         but labelled by the y_mapped values
         :param y: long sequence of y_values along original y axis
         :param y_mapped: corresponding transformed y_values for new y_ticks
             len(y_mapped) == len(y)
             y and y_mapped monotonically increasing
         :param y_label: label of second y-axis
-        :param fontsize: (optional) fontsize of y_label
         :return: None
         """
         ax2 = self.ax.twinx()
         ax2.set_ylim(self.ax.get_ylim())
         ymap_ticks = _nice_ticks(np.amin(y_mapped), np.amax(y_mapped))
         # = uniform ticks in y_mapped scale
         ymap_ticklabels = [f'{tick:.1f}' for tick in ymap_ticks]
         y_ticks = np.interp(ymap_ticks, y_mapped, y)
         # = transformed to corresponding y scale positions
         ax2.set_yticks(y_ticks)
         ax2.set_yticklabels(ymap_ticklabels)
-        ax2.set_ylabel(y_label, fontsize=fontsize)
-        self.fig.tight_layout()
+        ax2.set_ylabel(y_label)
+        # self.fig.tight_layout()
 
 
-class TableRef:
-    """Reference to a single table instance,
-    formatted in LaTeX OR plain tabulated txt versions
+# --------------------------------------------------
+class Table(pd.DataFrame):
+    """Subclass adding a general save method,
+    automatically switching to desired file format.
+    """
+    def save(self, file_path,
+             allow_over_write=True,
+             write_fcn=None,
+             **file_kwargs):
+        """Save self to a table-style file.
+        :param file_path: Path instance defining file location and full name incl. suffix.
+        :param allow_over_write: (optional) boolean, if False, find new unused path stem.
+        :param write_fcn: (optional) user-supplied function with signature
+            write_fcn(table, path, **kwargs).
+            If None, default pd.DataFrame method is used, determined by file_path.suffix
+        :param file_kwargs: (optional) any additional arguments for the
+            write function for the specific file format.
+        :return: None
+        """
+        if not allow_over_write:
+            file_path = safe_file_path(file_path)
+        suffix = file_path.suffix
+        try:
+            # ******** file_path.parent.mkdir here? NO, done by container class
+            if write_fcn is None:
+                if suffix in ['.xlsx', '.xls', '.odf', '.ods', '.odt']:
+                    # self.to_excel(file_path, sheet_name=file_path.stem, **file_kwargs) # use default
+                    self.to_excel(file_path, **file_kwargs)
+                elif suffix in ['.csv']:
+                    self.to_csv(file_path, **file_kwargs)
+                elif suffix in ['.txt']:
+                    self.to_string(file_path, **file_kwargs)
+                elif suffix in ['.tex']:
+                    # with warnings.catch_warnings():
+                    #     # suppress Pandas FutureWarning about to_latex method
+                    #     warnings.simplefilter('ignore')
+                    #     self.to_latex(file_path, **file_kwargs)
+                    self.to_latex(file_path, **file_kwargs)
+                else:
+                    raise FileWriteError(f'No DataFrame write method for file type {suffix}')
+            else:
+                write_fcn(self, file_path, **file_kwargs)
+        except Exception as e:
+            raise FileWriteError(f'Could not write to {file_path}. Error: {e}')
+
+class ResultTable(Table):
+    """A pd.DataFrame table subclass, with a name and special save method
     """
-    def __init__(self, text=None, name=None, path=None):
+    def __init__(self, df, name):
         """
-        :param text: single string with all table text incl. newline, tab chars.
-        :param path: (optional) Path to directory where tables are saved
-        :param name: (optional) updated file name, with or without suffix
-            suffix is determined by FMT['table_format'] anyway
+        :param df: a Table(pd.DataFrame) instance
+        :param name: file name for saving the table
         """
-        # store table parts instead *****???
-        self.text = text
+        super().__init__(df)
         self.name = name
-        self.path = path
 
-    def __repr__(self):
-        return (f'TableRef(text= text, ' +    # fmt= {repr(self.fmt)}, ' +
-                f'name= {repr(self.name)}), path= {repr(self.path)}')
+    def save(self, path,
+             table_format=None,
+             **kwargs):
+        """Save table to file.
+        :param path: Path to directory for saving self.
+        :param table_format: table-format string code -> file-name suffix
+        :param kwargs: (optional) any additional arguments to pandas writer function
+        :return: None
+        """
+        if table_format is not None:
+            name = _clean_file_name(self.name)
+            f = (path / name).with_suffix('.' + table_format)
+            try:
+                super().save(f, **kwargs)
+            except Exception as e:  # any error, just warn and continue
+                logger.warning(f'Could not save result table. Error: {e}')
 
-    def save(self, path, name=None):
+
+class DiffTable(ResultTable):
+    """Special subclass suppressing index in save method
+    """
+    def save(self, path,
+             **kwargs):
         """Save table to file.
-        :param path: Path to directory where tables are saved
-        :param name: (optional) updated file name, with or without suffix
-            suffix is determined by FMT['table_format'] anyway
+        :param path: Path to directory for saving self.
+        :param kwargs: (optional) any additional arguments to pandas writer function
         :return: None
-        Result: updated properties path, name
         """
-        if name is None:
-            name = self.name
-        name = _clean_file_name(name)
-        path.mkdir(parents=True, exist_ok=True)   # just in case
-        f = (path / name).with_suffix(TABLE_FILE_SUFFIX[FMT['table_format']])
-        if self.text is not None and len(self.text) > 0:
-            f.write_text(self.text, encoding='utf-8')
-        self.path = path
-        self.name = f.name
+        if 'index' not in kwargs:
+            kwargs['index'] = False  # override Pandas default = True
+        super().save(path, **kwargs)
 
 
 # ------------------------------------------------ plot routines
 
 def fig_log_likelihood(learned_ll, n_users,
+                       name,
                        title='',
-                       # label=None,
-                       fontsize=14,
-                       name=None,
                        **kwargs):
     """plot VI learning result
     :param learned_ll = list log-likelihood values from a learned ItemResponseModel
     :param n_users = scalar number of users included in the total log-likelihood
+    :param name = figure name for file
     :param title = (optional) figure title
-    :param name = (optional) figure name for file
-    :param fontsize = (optional) font size for axis labels
     :param kwargs = (optional) dict with any additional arguments for plot function
     :return: None
     """
     f_logprob, ax = plt.subplots()
     t1 = 1
     # for ll in learned_ll:
     t = [t1 + n for n in range(len(learned_ll))]
     # n_train = ham.n_training_users
     ax.plot(t, np.array(learned_ll) / n_users, **kwargs)
     # t1 = t[-1] + 1
     ax.set_xlim(0, t[-1]+1)
-    ax.set_xlabel('Learning Iterations', fontsize=fontsize)
-    ax.set_ylabel('Log-likelihood / N', fontsize=fontsize)
+    ax.set_xlabel('Learning Iterations')
+    ax.set_ylabel('Log-likelihood / N')
     if 0 < len(title):
         ax.set_title(title)
     return FigureRef(ax, name=name)
 
 
-def fig_response_freq(count, name=None, fontsize=14):
+def fig_response_freq(count, name):
     """Generate a plot with relative frequencies of response counts for all items
     :param count: list of Counter objects  *** dict ?
         count[i][0] = number of missing responses for i-th item
         count[i][l] = number of responses in l-th ordinal level for i-th item
-    :param fontsize = (optional) font size for axis labels
-    :return: figure object *** FigureRef object ???
+    :param name = string name of this figure
+    :return: FigureRef object
     """
     fig, ax = plt.subplots()
     for (i, (c, col, (m, fill_style))) in enumerate(zip(count,  # total_count,
                                                         cycle(FMT['colors']),
                                                         cycle(product(FMT['markers'],
                                                                       FMT['fillstyle'])))):
         x_i = np.arange(1 + max(*c.keys()))  # key = 0 means missing data
         y_i = np.array([c[r] for r in x_i])
         y_i = y_i / np.sum(y_i)
         y_i *= 100  # in percent
         ax.plot(x_i, y_i, label = f'Q{i+1}', color=col,
                 marker=m, fillstyle=fill_style)
     ax.set_xticks(np.arange(0, 6))
     ax.set_xticklabels(['Missing'] + [f'R={i+1}' for i in range(5)])
-    ax.set_xlabel('Item Response', fontsize=fontsize)
-    ax.set_ylabel('Rel. Frequency (%)', fontsize=fontsize)
+    ax.set_xlabel('Item Response')
+    ax.set_ylabel('Rel. Frequency (%)')
     ax.legend(loc='best')
     return FigureRef(ax, name=name)
 
 
 def fig_response_prob(t, p,
+                      name,
                       tau=None,
-                      name=None,
                       x_label='',
-                      y_label='',
-                      fontsize=14
-                      ):
+                      y_label=''):
     """figure with response prob vs. trait
     :param t: 1D array with trait values
     :param p: 2D array with response probabilities
         p[n, l] = P{l-th response | t[n]}
+    :param name: string for plot file name
     :param tau: (optional) 1D array with trait thresholds
-    :param name: (optional) string for plot file name
     :param x_label: string for x-axis label
     :param y_label: string for y-axis label
-    :param fontsize: (optional) fontsize for x_ and y_label
     :return: FigureRef object
     """
     fig, ax = plt.subplots()
     for (l, (p_l, c, ls)) in enumerate(zip(p.T,
                                            cycle(FMT['colors']),
                                            cycle(FMT['line_styles']))):
         ax.plot(t, p_l, color=c, linestyle=ls, label=f'R={1+l}')
     if tau is not None:
         # plot ticks at thresholds
         x = [tau, tau]
         y = [np.zeros(len(tau)), 0.1 * np.ones(len(tau))]
         ax.plot(x, y, color='k', linewidth=1., linestyle='solid')
     ax.set_ylim(0., 1.)
-    ax.set_xlabel(x_label, fontsize=fontsize)
-    ax.set_ylabel(y_label, fontsize=fontsize)
+    ax.set_xlabel(x_label)
+    ax.set_ylabel(y_label)
     ax.legend(loc='best')
     return FigureRef(ax, name=name)
 
 
 def fig_percentiles(perc,
                     y_label,
                     x_ticklabels,
+                    name,
                     case_labels=None,
                     x_label=None,
                     x_offset=0.1,
                     x_space=0.5,
-                    fontsize=14,
-                    name=None,
                     **kwargs):
     """create a figure with trait percentile results
     :param perc: 3D (or 2D) array with trait percentiles
         perc[c, p, t] = p-th percentile of t-th variable for c-th case
         percentiles plotted vertically vs t-variables horizontally,
     :param y_label: string for y axis label
     :param x_label: string for x-axis label
     :param x_ticklabels: list of strings with labels for x_ticks,
         one for each value in rows perc[..., :]
         len(x_ticklabels) == perc.shape[-1] == number of traits
+    :param name: string name of this figure
     :param case_labels: list of strings with labels for cases, if more than one
         len(case_labels) == perc.shape[0] if perc.ndim == 3
     :param x_offset: (optional) horizontal space between case plots for each x_tick
     :param x_space: (optional) min space outside min and max x_tick values
-    :param fontsize: (optional) fontsize for x and theta labels
     :param kwargs: (optional) dict with any additional keyword arguments for plot commands.
     :return: None  # fig object with single plot axis with all results
     """
     fig, ax = plt.subplots()
     if perc.ndim == 2:
         perc = perc[np.newaxis,...]
         case_labels = [None]
@@ -300,41 +339,40 @@
         x += x_offset
     (x_min, x_max) = ax.get_xlim()
     x_min = min(x_min, -x_space)
     x_max = max(x_max, n_xticks - 1 + x_space)
     ax.set_xlim(x_min, x_max)
     ax.set_xticks(np.arange(n_xticks))
     ax.set_xticklabels(x_ticklabels)
-    ax.set_ylabel(y_label, fontsize=fontsize)  # + ' (' + y_unit + ')')
-    ax.set_xlabel(x_label, fontsize=fontsize)
+    ax.set_ylabel(y_label)  # + ' (' + y_unit + ')')
+    ax.set_xlabel(x_label)
     if n_cases > 1:
         # make space for legend
         (x_min, x_max) = ax.get_xlim()
         ax.set_xlim(x_min, x_max + 0.6)
         ax.legend(loc='best')
     if name is None:
         name = _clean_file_name(y_label)
     return FigureRef(ax, name=name)
 
 
 def fig_credible_diff(c_diff,
+                      diff_label,
                       x_labels,
                       x_label=None,
                       title=None,
-                      cred_levels=None,
-                      fontsize=10
-                      ):
+                      cred_levels=None):
     """Nice color plot to show jointly credible differences
     :param c_diff: list of tuples ((i, j), p), indicating that
         x_labels[i] > x-labels[j] with joint credibility p
+    :param diff_label: name for this display figure
     :param x_labels: list of labels of compared categories
     :param x_label: (optional) axis label
     :param title: (optional) string with plot title
     :param cred_levels: (optional) list of joint-credibility values, in DECREASING order
-    :param fontsize: (optional) fontsize for x_labels in plot
     :return:
     """
     if cred_levels is None:
         cred_levels = [.99, .95, .9, .8, .7]
     marker_sizes = [15, 12, 9, 6, 3]
 
     cred_levels = np.asarray(cred_levels)
@@ -360,84 +398,84 @@
             if label is not None:
                 s.set_label(label)
     ax.set_xlim([-0.5, len(x_labels) - 0.5])
     ax.set_ylim([-0.5, len(x_labels) - 0.5])
     ax.set_xticks(np.arange(len(x_labels)))
     ax.set_yticks(np.arange(len(x_labels)))
     ax.set_xticklabels(x_labels,
-                       fontsize=fontsize,
-                       **_x_tick_style(x_labels) )
+                       **_x_tick_style(x_labels)
+                       )
     ax.set_yticklabels(x_labels[::-1],  # reversed order
-                       fontsize=fontsize,
                        rotation='horizontal',
                        horizontalalignment='right'
                        )
     if x_label is not None:
-        ax.set_xlabel(x_label, fontsize=fontsize + 4)
-        ax.set_ylabel(x_label, fontsize=fontsize + 4)
+        ax.set_xlabel(x_label)
+        ax.set_ylabel(x_label)
     ax.set_title(title)
     if len(c_diff) > 0:
         ax.legend(loc='best')
     fig.tight_layout()
-    return FigureRef(ax)
+    return FigureRef(ax, name=diff_label)
 
 
 # --------------------------------------- Table formatting functions
-def tab_correlation_matrix(cov, item_trait_map, name=None):
+def tab_correlation_matrix(cov, item_trait_map, name='Corr', header='Trait'):
     """Normalized correlation matrix between IRT traits corresponding to items.
     :param cov: estimated, possibly un-normalized, covariance matrix,
         possibly including traits that have NO item correspondence
     :param item_trait_map: 2D boolean array mapping trait to item
         item_trait_map[i, t] == True <=> t-th trait determines i-th item response
-    :param name: (optional) string file name of table
-    :return: string with tabulated correlation values by trait = IOI-HA item
+    :param name: (optional) string name of this table
+    :param header: (optional) name for row and column index
+    :return: a ResultTable instance
     """
-    if name is None:
-        name = 'Corr'
     trait_sel = np.any(item_trait_map, axis=0)
     c = cov[:, trait_sel][trait_sel, :]
     std = np.sqrt(np.diag(c))
     # Normalize covariance matrix
     c /= std
     c /= std[:, None]
-    n_traits = c.shape[0]
     trait_labels = _make_trait_labels(item_trait_map)
     # *** use externally defined trait labels? ******
-    align = 'r | ' + (n_traits-1) * 'r '
-    header = ['Trait'] + trait_labels[1:]
-    rows = []
-    for i in range(n_traits-1):
-        rows += [[trait_labels[i]] + i * [' '] + [f'{c[i, j]:.3f}'
-                                                  for j in range(i+1, n_traits)]]
-    return TableRef(_make_table(header, rows, align), name=name)
+    trait_index = pd.Index(trait_labels, name=header)
+    df = pd.DataFrame(c, columns=trait_index, index=trait_index)
+    return ResultTable(df, name=name)
 
 
 def tab_credible_diff(diff,
+                      diff_name,
                       x_labels,
-                      x_label='Population'):
-    """create table with credible trait differences between populations
+                      cred_header='Cred.',
+                      x_label='Population',
+                      and_head=' ',
+                      and_label='AND'):
+    """Create table with credible trait differences between populations
     represented by included group data sets
     :param diff: list of tuples ((i, j), p), indicating that
         x_labels[i] > x-labels[j] with joint credibility p, meaning
         prob{ x_labels[i] > s_labels[j] } AND all previous pairs } == p
+        in quantity = diff_name
+    :param diff_name: string name identifying the difference shown
     :param x_labels: list of category labels of compared data
-    :param x_label: label of category for the difference
-    :return: TableRef object with header lines + one line for each credible difference,
-    """
-    if len(diff) == 0:
-        return None
-    align = 'l l c l r'
-    h = ['', x_label, '$>$', x_label, FMT['credibility']]
-    rows = []
-    col_0 = ''
-    # ((i,j), p) = diff[0]  # separate format for first line
-    for ((i, j), p) in diff:
-        rows.append([col_0, x_labels[i], '$>$', x_labels[j], f'{100*p:.1f}\%'])
-        col_0 = 'AND' # for all except first row
-    return TableRef(_make_table(h, rows, align))
+    :param x_label: string label of category for the difference
+    :param cred_header: string header of credibility column
+    :param and_head: name of column with AND labels
+    :param and_label: label indicating AND condition
+    :return: a ResultTable instance with header lines + one line for each credible difference,
+    """
+    col = {and_head: [''] + (len(diff) -1) * [and_label]}
+    col |= {x_label + ' >': [x_labels[i]
+                             for ((i, j), p) in diff]}  # category with larger value
+    col |= {x_label: [x_labels[j]
+                      for ((i, j), p) in diff]}  # category with smaller value
+    col |= {cred_header: [p for ((i, j), p) in diff]}  # credibility value in (0, 1)
+    df = pd.DataFrame(col)
+    # df.items.name = diff_name  # suppressed anyway, by DiffTable.save()
+    return DiffTable(df, name=diff_name)
 
 
 # ------------------------------------------ internal help functions:
 def _nice_ticks(y_min, y_max):
     """Make nice sequence of equally spaced ticks
     with at most one decimal
     :param y_min: scalar axis min
@@ -471,49 +509,14 @@
     # if len(labels) > 20:
     #     style['fontsize'] = 8
     # else:
     #     style['fontsize'] = 10
     return style
 
 
-table_begin = {'latex': lambda align: '\\begin{tabular}{' + align + '}\n',
-               'tab': lambda align: ''}
-table_head_sep = {'latex':'\hline\n',
-                  'tab':''}
-table_cell_sep = {'latex': ' & ',
-                  'tab':' \t '}
-table_row_sep = {'latex': '\\\\ \n',
-                 'tab': '\n'}
-table_end = {'latex':'\hline\n\end{tabular}',
-             'tab': ''}
-
-
-def _make_table(header, rows, col_alignment):
-    """Generate a string with table text.
-    :param header: list with one string for each table column
-    :param rows: list of rows, where
-        each row is a list of string objects for each column in this row
-    :param col_alignment: list of alignment symbols, l, r, or c
-        len(col_alignment) == len(header) == len(row), for every row in rows
-    :return: single string with complete table
-    """
-    def make_row(cells, fmt):
-        return table_cell_sep[fmt].join(f'{c}' for c in cells) + table_row_sep[fmt]
-    # ------------------------------------------------------------------------
-
-    fmt = FMT['table_format']  # module global constant
-    t = table_begin[fmt](col_alignment)
-    t += table_head_sep[fmt]
-    t += make_row(header, fmt)
-    t += table_head_sep[fmt]
-    t += ''.join((make_row(r, fmt) for r in rows))
-    t += table_end[fmt]
-    return t
-
-
 def _make_trait_labels(item_trait_map):
     """Prepare trait labels for plots and tables
     :param item_trait_map: 2D boolean array mapping trait for each item
     :return: list of strings
     """
     # *** should be done externally ? ***
     trait_sel = np.any(item_trait_map, axis=0)
@@ -529,13 +532,29 @@
     """Make a string that can be used as file name
     :param s: string
     :return: clean_s,
         with whitespace replaced by _,
         and not-allowed chars removed
     """
     clean_s = s.replace(' ', '_')
-    return clean_s.translate({ord(c): None for c in '(),.'})
+    return clean_s.translate({ord(c): None for c in '(),.*'})
+
+
+# ------------------------------------------ help functions:
+def safe_file_path(p):
+    """Ensure previously non-existing file path, to avoid over-writing,
+    by adding a sequence number to the path stem
+    :param p: file path
+    :return: p_safe = similar file path with modified name
+    """
+    f_stem = p.stem
+    f_suffix = p.suffix
+    i = 0
+    while p.exists():
+        i += 1
+        p = p.with_name(f_stem + f'-{i}' + f_suffix)
+    return p
 
 
-# ------------------------------------------------------
+# -----------------------------------------------------
 if __name__ == '__main__':
-    print(_clean_file_name('asd asdf. (asdf), asdf'))
+    print(_clean_file_name('asd asdf. (asdf)*, asdf'))
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/ir_logging.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_logging.py`

 * *Files identical despite different names*

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/run_irt.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/run_irt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,335 +1,301 @@
 """Main template script to analyze ordinal response data using Item Response Theory.
 This template should be copied and edited by the user for the desired application.
 
-Arne Leijon, 2020-05-30, template example based on IOI-HA data analysis
-2020-06-06, standalone version for ItemResponseCalc package
-"""
+The model estimates the distribution of one or more traits underlying responses to a questionnaire,
+for one or several populations, represented by groups of respondents.
+
+The results show trait distributions within and between populations,
+and reveals jointly credible differences between populations.
+
+Populations should preferably be represented by large groups of respondents,
+recruited at random.
 
+Analysis results show the inter-individual variance within and between populations,
+and the mapping between traits and item ratings,
+but individual trait values are not displayed.
+
+The analysis script always includes three main steps:
+1: Define and collect item response data from one or more sources,
+    and specify a top directory for all results.
+2: Learn an OrdinalItemResponseModel instance using the collected response data
+3: Display the main characteristics of the learned model.
+
+*** Version History
+
+* Version 0.6.0
+2023-07-11, cleanup this script template with examples using new ir_source module
+2023-07-06, result file format choice moved from ItemResponseDisplaySet.show() -> .save()
+2023-07-01, new module ir_source for pandas.read_xxx for input files
+2022-09-15, use pandas.read_xxx functions to access input data files.
+2020-06-06, first standalone version for ItemResponseCalc package
+2020-05-30, template example based on IOI-HA data analysis
+"""
 # -------- __main__ check to prevent multiprocessor sub-tasks to re-run this script
 if __name__ == '__main__':
 
     import numpy as np
     import pickle
     from pathlib import Path
     import datetime as dt
     import logging
+    # from sqlalchemy import create_engine  # to read from SQL database
 
+    from ItemResponseCalc import __version__
     from ItemResponseCalc import ir_logging
     from ItemResponseCalc.item_response_data import Questionnaire
     from ItemResponseCalc.item_response_data import ItemResponseDataSet
-    from ItemResponseCalc.item_response_data import item_response_table
-    from ItemResponseCalc.table_reader import Table, Tables
-    # Tables used to join data in teo or more files into one group
+    from ItemResponseCalc.ir_source import item_response_table, Tables
+    # Tables used to join data from two or more sources as one group
     from ItemResponseCalc.item_response_model import OrdinalItemResponseModel
     from ItemResponseCalc.ir_display import ItemResponseDisplaySet
 
-    # ----------------------------------------------- ItemResponseModel parameters:
+    # -------------------------------- ItemResponseModel parameters:
     max_n_traits = 4
     # = max number of traits to explain total set of item responses
     # = 1, if the test instrument is known to measure a uni-dimensional trait
 
     # n_scale_samples = 50
-    # -> sampled set of scale threshold vectors
+    # -> sampled set of scale threshold parameters
     n_scale_samples = 1
-    # -> MAP-estimated single scale threshold vector
-    n_subject_samples = 20
+    # -> MAP-estimated single scale threshold parameters
+    n_subject_samples = 50
     # = number of sampled trait(s) for each respondent
-
     # NOTE: computation time is proportional to
     # n_subjects * n_scale_samples * n_subject_samples
     # n_scale_samples = 1 may give similar result as sampled scale model
 
     TEST_DOWNSAMPLE = 1
     # -> no down-sampling -> all records included
     # TEST_DOWNSAMPLE = 10
-    # -> use smaller data subset only for faster initial test run
+    # -> smaller data subset only for faster initial test run
+
+    # ----------------------------- STEP 1: Define input sources and result path:
+
+    timestamp_result = True  # Prevent over-writing result files
+    # timestamp_result = False  # Repeated runs will save results in same directory
 
-    # ------------------------------------------------------------------------
     TOP_PATH = Path.home() / 'Documents/LeijonKTH/heartech/HA-QualityRegistry'
-    TOP_PATH = TOP_PATH / 'IRT-IOI-HA'
-    # Change this example to top-dir for everything to be read or written here
+    TOP_PATH = TOP_PATH / 'IRT-IOI-HA'  # or whatever...
+    # Change this example to top-dir for everything to be read or written
 
-    ioiha_data_path = TOP_PATH / 'IOI-HA-data'
-    # path to actual item data files OTHER THAN data in sql server
+    ioiha_data_path = TOP_PATH / 'IOI-HA-data'  # or whatever...
+    # path to directory containing item response data files
 
     result_dir = TOP_PATH / 'IOI-HA-results'
     # path where results will be saved, for several runs if needed
 
     ioiha_file = ioiha_data_path / 'IOI-HA-English.txt'
     # text file containing the questions and response alternatives
     # If not available, a Questionnaire object must be created manually
     # as suggested below.
 
-    # ------------------------------------------------------------------------
-    timefmt = '{0.year}-{0.month:02}-{0.day:02}-{0.hour:02}{0.minute:02}'
-    result_run = timefmt.format(dt.datetime.now())
-    # -> name of sub-folder in result_dir
-
-    save_dir = result_dir / result_run
+    if timestamp_result:
+        timefmt = '{0.year}-{0.month:02}-{0.day:02}-{0.hour:02}{0.minute:02}'
+        result_run = timefmt.format(dt.datetime.now())
+        # -> name of sub-folder in result_dir
+        save_dir = result_dir / result_run
+    else:
+        save_dir = result_dir
     save_dir.mkdir(parents=True, exist_ok=True)
     # sub-path for results of this particular run
 
     model_file = 'irt-model.pkl'
     # = name of saved model in save_dir
 
     log_file = 'run_irt_log.txt'
     # = name of log file saved in same sub-folder
-    # -------------------------------------------------------------------------
-
-    # ------------------------------------- setup logging:
     ir_logging.setup(save_dir / log_file)
     logger = logging.getLogger(__name__)
 
-    # -------------------------- common help functions for data input:
+    logger.info('*** Using ItemResponseCalc v.' + __version__)
+    if TEST_DOWNSAMPLE > 1:
+        logger.info(f'*** Test with down-sampling {TEST_DOWNSAMPLE}')
+
     def accept_record(r):
-        """Inclusion criterion for accepting a record,
-        to be called after any other data recoding in each input Table object.
-        :param r: list with responses in ONE record read from file,
-            encoded as integer values
-        :return: boolean == True if record is acceptable
+        """User-defined inclusion criterion for accepting a response record,
+        applied to responses recoded as integer with origin 0,
+        and missing responses encoded as -1.
+        :param r: list with integer-encoded responses in ONE record from a source
+        :return: boolean == True if the record is acceptable
         """
-        n_missing = sum(r_i is None or r_i < 1 or r_i > 5
-                        for r_i in r)
+        n_missing = sum(r_i < 0 for r_i in r)
         return n_missing <= 3
+    # ----------------------------------------------------------
 
-    def recode_missing_as_0(row):
-        """Replace missing data by zero, as required by analysis.
-        Table readers encode missing data as value = None
-        :param row: list with responses in ONE record read from file
-        :return: None, row elements recoded in place
-        """
-        for i in range(len(row)):
-            if row[i] is None or row[i] < 1:  # or row[i] > 5: only for IOI-HA
-                row[i] = 0
-    # --------------------------------------------
-
-    if TEST_DOWNSAMPLE > 1:
-        logging.info(f'*** Test with down-sampling {TEST_DOWNSAMPLE}')
-
-    # ------------------------------- Define questionnaire instrument
+    # ------------------ 1A: Define questionnaire instrument:
     # create a Questionnaire object to specify
     # number of items and response alternatives
-    q_items = Questionnaire.load(ioiha_file)  # load from text file
+
+    # Example: load from text file, edit as needed:
+    q_items = Questionnaire.load(ioiha_file)
 
     # if the text file is not available, create q_items manually, e.g.:
+    # Example: seven items, all with 5 response levels, like the IOI-HA:
     # r_levels = [5, 5, 5, 5, 5, 5, 5]
-    # # = list with number of response levels, one element for each item
-    # # Example: all seven IOI-HA items have 5 response levels
+    # = list with number of response levels, one element for each item
     # q_items = Questionnaire(item_response_levels=r_levels)
 
-    # ------------------------------- Define included data sets:
+    # ------------------ 1B: Define sources of data to be included in analysis:
     data_groups = dict()  # space for all included groups
 
-    # Example: Include two xlsx files from Hickson, Australia:
-    # Responses have already been coded as integers 1,..., 5 in the file
+    # Example: Include xlsx file(s) from Hickson, Australia:
+    # Edit as needed:
     au1_file = ioiha_data_path / 'Hickson' / 'Short_Eartrak AUS.xlsx'
     logger.info(f'AU-H-10: Using {au1_file}')
 
-    au1 = item_response_table(au1_file,
-                              fields=[f'Q0{i}' for i in range(1, 8)],  # labels in header row
-                              field_types=int,
-                              missing_values=['.', ' '],
-                              header_row=1,
+    au1 = item_response_table(source=au1_file,
+                              items={f'Q0{item}': list(range(1, 6))
+                                     for item in range(1, 8)},  # as encoded in the xlsx file
+                              accept_fcn=accept_record,  # None -> no restriction
                               sample_factor=TEST_DOWNSAMPLE,
-                              recode_fcns=recode_missing_as_0,
-                              accept_row=accept_record)
-    data_groups['AU-H-10'] = au1
-
-    au2_file = ioiha_data_path / 'Hickson' / 'Eartrakdata_10_May_08.xlsx'
-    logger.info(f'AU-H-10e: Using {au2_file}')
+                              index_col=0    # with respondent ID, to avoid duplicate records
+                              )
+    # NOTE: items = a dict with column header and a sequence of allowed ordinal responses,
+    #   as encoded in this input source, not necessarily == Questionnaire.responses.
+    # If index_col is defined, only the LAST record from each respondent is included.
 
-    au2 = item_response_table(au2_file,
-                              fields=[f'Q0{i}' for i in range(1, 8)],
-                              field_types=int,
-                              missing_values=['.', ' '],
-                              header_row=1,
-                              sample_factor=TEST_DOWNSAMPLE,
-                              recode_fcns=recode_missing_as_0,
-                              accept_row=accept_record)
-    data_groups['AU-H-10e'] = au2
-
-    # Include two csv files from S Kramer:
-
-    nle_file = ioiha_data_path / 'Kramer' / 'moeder_final - kopieforArne.csv'
-    logger.info(f'NL-02: Using {nle_file}')
-
-    nle1 = item_response_table(file_path=nle_file,
-                               fmt='csv',
-                               fields=[f'ioi_v{i}' for i in range(1, 8)],
-                               field_types=int,
-                               missing_values=[9.0, ''],
-                               sample_factor=TEST_DOWNSAMPLE,
-                               recode_fcns=recode_missing_as_0,
-                               accept_row=accept_record)
-
-    # -------------------------------------------
-    def recode_fields14(row):
-        """IOI-HA items 1 and 4 coded as 0-4 in NLSH-Kramer-T2IOI-HA.csv
-        must be recoded as values 1-5,
-        BEFORE recoding missing-data as zero.
-        """
-        for i in [1, 4]:
-            if row[i - 1] is not None:
-                row[i - 1] += 1
-    # --------------------------------------------
-
-    nle2_file = ioiha_data_path / 'Kramer' / 'NLSH-Kramer-T2IOI-HA.csv'
-    logger.info(f'NL-16: Using {nle2_file}')
-
-    nle2 = item_response_table(file_path=nle2_file,
-                               fmt='csv',
-                               sample_factor=TEST_DOWNSAMPLE,
-                               fields=[f'T2IOIHA{i + 1}' for i in range(7)],
-                               missing_values=[9999999.0],
-                               field_types=int,
-                               recode_fcns=[recode_fields14,
-                                            recode_missing_as_0],
-                               # recode_fcns are called in given order
-                               accept_row=accept_record)
-    # Example: join both data files into ONE group:
-    data_groups['NL-02-16'] = Tables(nle1, nle2)
-
-    # *** Example: include data for one year from an SQL database:
-
-    # from ItemResponseCalc.table_reader_sql import Table
-    # = special Table reader for SQL access
-
-    # haq_config = dict(user='user_id',
-    #                   password='********',
-    #                   host='127.0.0.1',  # IP address of SQL server
-    #                   port='1111',  # access port to SQL server
-    #                   database='hbdb',  # name of database on SQL server
-    #                   connect_timeout=10  # seconds wait in case no access
-    #                   )
-    # = access arguments for SQL database
+    data_groups['AU-H-10'] = au1
 
-    # table = 'prescriptions'  # name of desired table in the database
+    # Example: second input source:
+    # au2_file = ioiha_data_path / 'Hickson' / 'Eartrakdata_10_May_08.xlsx'
+    # logger.info(f'AU-H-10e: Using {au2_file}')
     #
-    # where = ("respondent = 1 " +
-    #          "AND (Q2 = 1 OR Q2 = 2) " +
-    #          "AND date BETWEEN %s AND %s"
-    #          )
-    # # = WHERE section of SELECT statement for SQL database
-    # # with following two dates as arguments:
-    # year_2019 = (dt.date(2019, 1, 1), dt.date(2019, 6, 30))
-
-    # data_groups['SE-19'] = Table(table_id=table,
-    #                              connect_kwargs=haq_config,  # SQL access
-    #                              select_where=where,
-    #                              select_args=year_2019,
-    #                              fields=[f'Q{i}' for i in range(3, 10)],
-    #                              # = IOI-HA field labels in database
-    #                              recode_fcns=recode_missing_as_0,
-    #                              accept_row=accept_record,
-    #                              sample_factor=TEST_DOWNSAMPLE * 10)
+    # au2 = item_response_table(source=au2_file,
+    #                           items={f'Q0{item}': list(range(1, 6))
+    #                                  for item in range(1, 8)},
+    #                           accept_fcn=accept_record,
+    #                           sample_factor=TEST_DOWNSAMPLE,
+    #                           index_col=0)
+    # data_groups['AU-H-10e'] = au2
+
+    # More examples: Combine two csv files into one group:
+    # nle1_file = ioiha_data_path / 'Kramer' / 'moeder_final - kopieforArne.csv'
+    # logger.info(f'NL-02: Using {nle1_file}')
+    #
+    # nle1 = item_response_table(source=nle1_file,
+    #                            items={f'ioi_v{item}': list(range(1, 6))
+    #                                   for item in range(1, 8)},     # as encoded in the csv file
+    #                            accept_fcn=accept_record,
+    #                            sample_factor=TEST_DOWNSAMPLE)   # no respondent ID given
+    #
+    # nle2_file = ioiha_data_path / 'Kramer' / 'NLSH-Kramer-T2IOI-HA.csv'
+    # logger.info(f'NL-16: Using {nle2_file}')
+    #
+    # kramer2_columns = {'T2IOIHA1': range(5),  # responses coded as 0,.., 4
+    #                    'T2IOIHA2': range(1, 6),  # coded as 1,.., 5
+    #                    'T2IOIHA3': range(1, 6),
+    #                    'T2IOIHA4': range(5),  # coded as 0,.., 4
+    #                    'T2IOIHA5': range(1, 6),
+    #                    'T2IOIHA6': range(1, 6),
+    #                    'T2IOIHA7': range(1, 6)}
+    #
+    # nle2 = item_response_table(source=nle2_file,
+    #                            items=kramer2_columns,
+    #                            accept_fcn=accept_record,
+    #                            sample_factor=TEST_DOWNSAMPLE)
+    # data_groups['NL-02-16'] = Tables(nle1, nle2)
+
+    # SQL example: access data from a database:
+    # engine = create_engine("sqlite+pysqlite:///" + str(sql_path / 'testDataBase.db'))
+    # ir_sql = item_response_table(source=engine,
+    #                              sql='ioiha',  # table name in database
+    #                              index_col='EarRowId',
+    #                              items={c: [str(i) for i in range(1, 6)]
+    #                                     for c in column_names}
+    #                              )  # NOTE: string-encoded responses in this DB
+    # data_groups['test'] = ir_sql
 
-    # --------------------------- Collect all groups into ONE DataSet object:
+    # ------------------ 1C: Collect all into ONE DataSet object:
 
-    ids = ItemResponseDataSet(questionnaire=Questionnaire.load(ioiha_file),
+    ids = ItemResponseDataSet(questionnaire=q_items,
                               groups=data_groups)
-    # NOT YET actually reading any data
-    # In case of read error, it will show here:
-    logging.info('Item Response Data collected = \n' + repr(ids))
-
-    total_count = np.array([np.sum(c_i) for c_i in ids.item_response_count])
-    logging.info('Total Response Counts: ' + np.array2string(total_count))
+    # NOT YET reading any response data
+    # In case of any input error, it will show here:
+    logger.info('Item Response Data = \n' + repr(ids))
+
+    # (Optional) Show response counts, to verify that input was OK
+    r_counts = ids.response_counts()
+    # = list with one pandas.DataFrame object for each questionnaire item
+    logger.info('Response Counts =\n'
+                 + '\n\n'.join(item.question + '\n' + c_df.to_string()
+                               for (item, c_df) in zip(ids.questionnaire.items,
+                                                       r_counts)
+                               )
+                 )
 
-    # --------------------------- Create ItemResponseModel from data:
+    # ------------------ STEP 2: Learn ItemResponseModel from data:
 
     irm = OrdinalItemResponseModel.initialize(ids,
                                               n_traits=max_n_traits,
                                               n_scale_samples=n_scale_samples,
                                               n_subject_samples=n_subject_samples,
-                                              trait_scale=3.)  # *** = default
+                                              trait_scale=3.  # *** = default
+                                              )
 
-    logging.info(f'Learning model with max {irm.n_traits} traits'
+    logger.info(f'Learning model with max {irm.n_traits} traits'
                  + f' for {irm.n_groups} groups'
-                 + f' with {irm.n_subjects} subject records in total')
-    logging.info(f'The model uses {n_scale_samples} scale samples'
+                 + f' with {irm.n_subjects} included respondent records in total')
+    logger.info(f'The model uses {n_scale_samples} scale samples'
                  + f' and {n_subject_samples} samples for each subject')
 
-    LL = irm.learn(max_hours=30)
-    # *** It may take MANY hours, try setting shorter time limit first
-    # When learning is complete, it will finish before the time limit
-    # If learning was complete, the LL values should reach a plateau level
+    LL = irm.learn(max_hours=5)
+    # *** Might take MANY hours, try setting shorter time limit first
+    # When learning is complete, it finishes before the time limit.
 
-    logging.info(f'Learned model with {irm.n_groups} groups'
+    logger.info(f'Learned model with {irm.n_groups} groups'
                  + f' with {irm.n_subjects} subjects in total')
-    LL = np.array(LL)
-    logging.info('Log Likelihood: ' + np.array2string(LL, precision=1))
-    # if learning was complete, it should finish before the time limit,
-    # and the LL values should should reach a nearly constant level
+    # LL = np.array(LL)
+    # logger.info('Log Likelihood: ' + np.array2string(LL, precision=1))
 
-    # ------------------ save model for later input to show_irt script
+    # ------------------ Optionally, save model for later display generation
     with (save_dir / model_file).open('wb') as f:
         pickle.dump(irm, f)
+    logger.info(f'Model saved in {save_dir}')
+    logger.info('Learned model = \n' + repr(irm))
 
-    logging.info(f'Result saved in {save_dir}')
-
-    logging.info('Learned model = \n' + repr(irm))
-
-    # ------------------------------------- Display Model Results:
-    # The display can also be done by separate script show_irt.py
-
-    # ------------------------------------- Trait Covariance before standardization
-    # only informative, may be commented out
-    c = irm.precision_within.mean_inv
-    logging.info('Predictive Trait Covariance Within Populations =\n'
-                 + np.array2string(c, precision=3, suppress_small=True))
-
-    c = irm.precision_among.mean_inv
-    logging.info('Predictive Trait Variance Among Populations= '
-                 + np.array2string(c, precision=3, suppress_small=True))
-
-    # ------------------------------------- Global Predictive Covariance
-    c = irm.predictive_individual_cov()
-    logging.info('Predictive Global Trait Cov (before standardization) =\n'
-                 + np.array2string(c, precision=3, suppress_small=True))
-
-    # -------------------------------------  prune and standardize:
     irm.prune()  # keep only traits that were really needed to model the data
+    irm.standardize()  # re-scale all parameters for unity trait variance
 
-    irm.standardize()  # re-scale all parameters for unity global trait variance
-
-    c = irm.predictive_individual_cov()
-    logging.info('Pruned and Standardized Predictive Global Trait Cov =\n'
-                 + np.array2string(c, precision=3, suppress_small=True))
-    s = np.sqrt(np.diag(c))
-    logging.info('Predictive St.Dev. after Standardization = '
-                 + np.array2string(s, precision=3))
-
-    # ------------------------------------- display with standardized scale
-    # mapping_item used to transform trait scale back to ONE item rating scale
+    # ------------------ STEP 3: Display Model Results:
+    # mapping_item used to display trait scales by reference to ONE item rating scale
     ir_display = ItemResponseDisplaySet.show(irm,
                                              mapping_item=-1,  # last questionnaire item
-                                             figure_format='pdf',  # OR eps, png,...
-                                             table_format='latex',  # OR tab
+                                             percentiles=[2.5, 50., 97.5],
+                                             mpl_params={'figure.max_open_warning': 0,  # suppress warning
+                                                         'figure.autolayout': True,  # -> tight layout
+                                                         'axes.labelsize': 'x-large'},  # -> matplotlib.rcParam
+                                             # mpl_style='my_style_sheet',
+                                             # ... any other ema_display.FMT settings
+                                             # ... any ema_display_format.FMT settings
                                              )
-    ir_display.save(save_dir)
+    ir_display.save(save_dir,
+                    figure_format = 'pdf',  # any format that Matplotlib can handle
+                    table_format = 'txt',   # any format that Pandas can handle
+                    float_format = '%.2f')  # any other parameter(s) for pandas.write_xxx
+
+    # --------------------------- (optionally) save in other format(s), too:
+    # ir_display.save(save_dir,
+    #          table_format='csv',  # only tables, for input to other package
+    #          float_format='%.4f',
+    #          )
+    # ir_display.save(save_dir,
+    #          figure_format='eps',  # only figures, for input to other package
+    #          )
+
+    logger.info(f'All results saved in {save_dir}')
 
-    # ------------------------------------- Within-group trait correlation
+    # ------------------ (Optional) PCA of within-population covariance
     if irm.n_traits > 1:
         cov_within = irm.precision_within.mean_inv
-        logging.info('Predictive Trait Covariance Within Populations:\n' +
-                     np.array2string(cov_within, precision=3))
-        s = np.sqrt(np.diag(cov_within))
-        c = cov_within / s
-        c /= s[:, np.newaxis]
-        # = normalized correlation matrix, also tabulated in ir_display:
-        logging.info('Predictive Trait Correlation Within Populations:\n' +
-                     np.array2string(c, precision=3))
-
-        # ------------------------------------- PCA of within-group covariance
-
         (eig_val, eig_vec) = np.linalg.eigh(cov_within)
-        logging.debug('Cov eig_val= ' +
+        logger.debug('Cov eig_val= ' +
                       np.array2string(eig_val, precision=3))
-        logging.debug('Cov eig_vec=\n' +
+        logger.debug('Cov eig_vec=\n' +
                       np.array2string(eig_vec, precision=3))
         eig_val_cum = np.cumsum(eig_val[::-1]) / np.sum(eig_val)
-        logging.info(f'One, Two, etc Principal Trait Factors: ' +
+        logger.info(f'One, Two, etc Principal Trait Factors: ' +
                      ', '.join(f'{ev:.1%}'
                                for ev in eig_val_cum) +
                      ', of Variance within Populations')
 
     logging.shutdown()
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/item_response_data.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_response_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,182 @@
 """This module defines help classes to access responses to questionnaire items.
 Data may be stored in various file formats.
 
 *** Class Overview:
 
-ItemResponseDataSet: container for all response data for selected group(s),
+ItemResponseDataSet: reference to all response data for selected group(s),
     to be used as input for statistical analysis.
     Response data input must be an iterable over response records.
-    A Response Record is a 1D list with integer-coded responses from ONE subject,
-    with one ordinal integer value for each Questionnaire Item.
+    A Response Record is a 1D array-like with ordinal responses from ONE subject,
+    with one ordinal index value for each Questionnaire Item.
     The input data for one group may be
     1) a single list of subject response lists,
-    2) a single table_reader.Table instance, reading from one data file,
-    3) a single table_reader.Tables instance, chaining input from several iterable objects.
+    2) an ir_source.ItemResponseTable (subclass) instance, defining ONE data source,
+    3) an ir_source.Tables instance, chaining input from SEVERAL sources.
 
 Questionnaire: description of a questionnaire, usually with several items
 
 Item: description of a single item (question and answer alternatives)
 
-*** Main File Interface Function:
-
-item_response_table: general function interface to ONE data file in any allowed format
-
-*** Input File Formats:
-
-xlsx: Data can be imported from Excel workbook (xlsx) files,
-    with data stored in ONE worksheet.
-    Item response data are stored in specified columns,
-    as defined by keyword parameter 'fields' to the Table reader class.
-    See module table_reader_xlsx for details.
-
-sql: Data can be imported from sql database files.
-    Item response data are stored in specified database fields,
-    as defined by keyword parameter 'fields' to the Table reader class.
-    See module table_reader_sql for details.
-    (table_reader_sqlite3 is no longer used.)
-
-csv: Data can be imported from a csv text file.
-    Item response data are stored in specified columns,
-    identified by 'fields' string labels in the first line of the file.
-    See module table_reader_csv for details.
-
-spss: Data can be imported from an SSPS (.sav) file.
-    See module table_reader_spss for details.
-    However, SSPS reader might not work with newer python versions.
-    May be easier to first convert the file to .csv format
+*** Input Source Formats:
+Data may be accessed from simple lists, or from any type of source that Pandas can handle,
+e.g., csv or xlsx files, or SQL database(s).
+pandas.read_xxx(...), or similar user-defined function, can be used for actual reading.
 
+Each source may have responses encoded in a specific way, different from other sources.
+Allowed response alternatives must be specified by user, for each input source.
 
 *** Usage Example:
 
 q_file = string or Path identifying questionnaire text (utf8) file
-r_file = string or Path identifying response file
+r_file_xxx = string or Path identifying a response file
 
-group0_file = item_response_table(r_file1, fmt='xlsx')
-group1A_file = item_response_table(r_file1A, ...)  another data file
-group1B_file = item_response_table(r_file1B, ...)  another data file
-etc.
+group0_table = item_response_table(source=r_file0, items=...)
+group1_table = item_response_table(r_file1, items=...)
+group2A_table = item_response_table(r_file2A, items=...)
+group2B_table = item_response_table(r_file2B, items=...)
+
+In each source, items = a dict with elements (column header, list of ordinal response categories)
+exactly as encoded in that data source.
+Any other value is interpreted as a missing response.
+Length of items must agree with number of questionnaire items.
 
 ids = ItemResponseDataSet.load(questionnaire=Questionnaire.load(q_file),
-        groups={'Group0': group0_file,
-                'Group1': Tables(group1A_file, group1B_file,...)
+        groups={'Group0': group0_table,
+                'Group1': group1_table,
+                'Group2', Tables(group2A_table, group2B_table)
                 }
         )
 
-This data-set can then be used as input to create an analysis model, e.g.,
-irm = OrdinalItemResponseModel.initialize(ids, n_traits=3)
-irm.learn()
+This data-set can then be used as input to create an analysis model.
 See run_irt.py for a complete example.
 
+An index_col may be defined for a column with respondent IDs in each input table.
+Duplicate indices will then be removed on reading, but only within each input data chunk.
+
 *** Version History:
 
+* Version 0.6.0:
+2023-07-09, use pandas.read_sql to access database source.
+2022-09-15, use pandas.read_xxx functions to access input data files.
+
+* Version 0.5:
 2019-07-23, functional version, may need some cleanup
 2019-07-29, new version with general table_reader interface
 2019-08-25, minor cleanup
 """
-# **** How to handle duplicate subjectID ??? ********
+# *** use subject_ID for individual displays?
+# *** use item_ID for item displays ?
 
 import numpy as np
 from pathlib import Path
+import pandas as pd
 
 import logging
-from importlib import import_module
-from itertools import chain
-
-ircPackage = 'ItemResponseCalc.'
-# = top ref to sub-modules for selective imports
-
-STORAGE_FMT = {'sqlite3': ircPackage + 'table_reader_sqlite',
-               'sql': ircPackage + 'table_reader_sql',
-               'xlsx': ircPackage + 'table_reader_xlsx',
-               'spss': ircPackage + 'table_reader_spss',
-               'sav': ircPackage + 'table_reader_spss',
-               'csv': ircPackage + 'table_reader_csv'
-               }
-# = mapping of file format code to suitable table_reader module
-# to be imported only if actually needed
 
 logger = logging.getLogger(__name__)
 
 
 # -------------------------------------------------------------------------------
 class Item:
     """Information describing ONE questionnaire item.
     """
     def __init__(self, question, responses, reverse=False):
         """
         :param question: string with explicit question text
-        :param responses: list of strings, one for each possible response
+        :param responses: list of ordinal response categories, one for each possible response
+            as presented in the questionnaire
         :param reverse: boolean = True if responses should be indexed in reverse order
             NOTE: Response data files may or may not already have recoded
             the responses by ordinal indices in the desired analysis order.
         """
         self.question = question
         self.responses = responses
         self.reverse = reverse
 
     def __repr__(self):
         return (self.__class__.__name__ + '(\n\t'
-                + ',\n\t'.join((f'{k}={repr(v)}' for (k,v) in self.__dict__.items()))
+                + ',\n\t'.join((f'{k}={repr(v)}' for (k, v) in self.__dict__.items()))
                 + ')')
 
     @property
     def n_response_levels(self):
         return len(self.responses)
 
+    @property
+    def ordinal_responses(self):
+        """Responses in order of increasing underlying trait
+        :return: iterator over ordinal response categories (NOT a copy)
+        """
+        return reversed(self.responses) if self.reverse else self.responses
+
+    # def response_int(self):
+    #     """Response categories coded as integers 1, ..., n_response_levels
+    #     """
+    #     return list(range(1, 1 + self.n_response_levels))
+
+    def response_codes(self):
+        """Response categories as code values in range(n_response_levels)
+        :return: list
+        """
+        return list(range(self.n_response_levels))
+
 
 class Questionnaire:
     """Container for a questionnaire with several items,
     required to specify number of items and number of response levels for each item,
     even if the actual questions and response alternatives are not included.
     """
     def __init__(self, header=None, items=None, item_response_levels=None):
         """
         :param header: (optional) string describing the questionnaire
         :param items: (optional) list of Item instances
-        :param item_response_levels: (optional) necessary only if items is None:
+        :param item_response_levels: (optional) used only if items is None:
             list with
             item_response_levels[i] = integer number of response levels for i-th item
         """
         self.header = header
-        self.items = items
         if items is None:
-            self.item_response_levels = item_response_levels
+            self.items = [Item(question=f'Question {i+1}',
+                               responses=list(range(1, n_levels +1)))
+                          for (i, n_levels) in enumerate(item_response_levels)]
+            # self.item_response_levels = item_response_levels
         else:
-            self.item_response_levels = [i.n_response_levels for i in self.items]
+            self.items = items
 
     def __repr__(self):
         return (self.__class__.__name__ + '(\n\t'
                 + ',\n\t'.join((f'{k}={repr(v)}' for (k,v) in self.__dict__.items()))
                 + '\n\t)')
 
+    # @property
+    # def item_response_levels(self):  # ******** needed ?
+    #     return [len(item.responses) for item in self.items]
+
     @property
     def n_items(self):
-        return len(self.item_response_levels)
+        return len(self.items)
 
     @classmethod
     def load(cls, file, sep='\t'):
         """Read questions and answers from given file
         :param file: string or Path object identifying input file
         :param sep: (optional) string, separator between response alternatives
         :return: cls instance
         """
         strip = ' \n'  # chars to strip away from end of input lines
-        with Path(file).open('rt', encoding='utf8') as f:  # *********** other txt encodings ??? *****
+        with Path(file).open('rt', encoding='utf8') as f:
             header = f.readline()
             items = []
             while True:
                 q = f.readline()
                 a = f.readline()
                 reverse = f.readline()
                 if a == '':
-                    break  # even if q is non-empty
+                    break  # even if ioiha_q is non-empty
                 else:
                     items.append(Item(question=q.rstrip(strip),
                                       responses=(a.rstrip(strip)).split(sep),
                                       reverse='rev' in reverse))
         return cls(header.rstrip(strip), items)
 
 
@@ -185,214 +188,260 @@
     otherwise the analysis cannot reveal correlations between items.
     """
     def __init__(self, questionnaire, groups):
         """
         :param questionnaire: single Questionnaire object
         :param groups: dict with elements (g_name, g_subjects), where
             g_name = string identifying the group
-            g_subjects = iterable, e.g., a list or responses or an instance of a table_reader.Table subclass,
-                yielding a sequence of subject response_records, one for each subject.
+            g_subjects = iterable of responses, either,
+                (1) a simple list or array,
+                (2) OR an ir_source.ItemResponseTable subclass instance,
+                (3) OR an ir_source.Tables instance
+                    with several join-ed ir_source.ItemResponseTable objects.  **************************
+            Each input table yields a sequence of response_record, one for each subject.
                 response_record = a 1D list with
                 response_record[i] = integer ordinal index of response to i-th item
-                encoded with origin == 1.
-                NOTE: different from python index origin!
-                Missing responses MUST be indicated as 0.
-                The Table object can apply user-supplied recoding functions,
-                in case other response encodings are used in the file.
+                encoded with origin == 0.
+                Missing responses are indicated as -1.
         """
         assert questionnaire is not None, 'Must have a Questionnaire object'
         self.questionnaire = questionnaire
         if groups is None:
             groups = dict()
         self.groups = groups
 
     def __repr__(self):
         return (self.__class__.__name__ + '('
                 + f'\n\t questionnaire= {self.questionnaire.__class__.__name__} '
                 + f'object with {self.questionnaire.n_items} items,'
                 + '\n\t groups= {\n\t\t'
-                + ',\n\t\t'.join(f'{g_key}: {g.__class__.__name__} with about {len(g)} rows'
+                + ',\n\t\t'.join(f'{g_key}: {g.__class__.__name__} object with {len(g)} respondent records'
                                  for (g_key, g) in self.groups.items()) + '}'
                 + ')')
 
-    @property
-    def n_response_levels(self):
-        return self.questionnaire.item_response_levels
+    # @property
+    # def n_response_levels(self):  # ******** needed ?
+    #     return self.questionnaire.item_response_levels
 
     @property
-    def n_items(self):
-        return len(self.n_response_levels)
+    def n_items(self):   # ******** needed
+        return self.questionnaire.n_items
 
     @property
     def n_groups(self):
         return len(self.groups)
 
-    @property
+    def response_counts(self, normalize=False):
+        """Tabulate distributions of response counts by items and groups
+        :param normalize: (optional) True: present relative frequencies,
+            False: absolute response counts
+        :return: list of pd.DataFrame objects,
+            one count table for each item, each with one column for each group
+        """
+        res_df = [pd.DataFrame(index=pd.CategoricalIndex(item.ordinal_responses,
+                                                         copy=True,
+                                                         ordered=True,
+                                                         name='Response'),
+                               columns=[], dtype=int)  # empty df
+                  for item in self.questionnaire.items]
+        # = space for results
+        for (g, g_table) in self.groups.items():
+            g_codes = np.array([row for row in g_table])
+            for (i, item) in enumerate(self.questionnaire.items):
+                gi_series = pd.Series(pd.Categorical.from_codes(g_codes[:, i],
+                                                                categories=item.responses,
+                                                                ordered=True))
+                gi_count = gi_series.value_counts(sort=False,
+                                                  normalize=normalize)
+                res_df[i][g] = gi_count.reindex(item.responses, fill_value=0)
+        return res_df
+
     def item_response_count(self):
-        """Total number of response counts for each item,
+        """Number of response counts for each item,
         summed across all groups.
         :return: c = list of response count arrays, with
             c[i] = 1D array for i-th item,
             with responses encoded with origin == 0, i.e.,
-            c[i][l] = count of response == l+1 for this item
+            c[i][l] = count of l-th ordinal response alternative for this item
         """
-        c = [np.zeros(n_i, dtype=int) for n_i in self.n_response_levels]
-        # counter, NOT including space for missing response coded as zero
-        for (g_key, g_response) in self.groups.items():
-            # g_response is iterable of item-response vectors, one for each subject,
-            # with responses encoded with origin == 1 for the lowest ordinal response alternative
-            for r_s in g_response:
-                for (item, r_si) in enumerate(r_s):
-                    if 1 <= r_si <= len(c[item]):  # i.e., real non-missing response
-                        c[item][r_si - 1] += 1  # count first response alternative at index == 0
-                    elif r_si > len(c[item]):
-                        logger.warning(f'Group {repr(g_key)}: Response={r_si} for item {item} out of range')
-                    # else just a missing data value, not counted
-        return c
-
-
-# ---------------------------------------------- File Interface factory:
-def item_response_table(file_path, fmt=None, **kwargs):
-    """Create interface to input file with individual item response data.
-    :param file_path: Path or string identifying input file
-    :param fmt: (optional) file format code, if not defined by file suffix
-    :param kwargs: keyword arguments to table_reader.Table of selected format
-    :return: a Table object representing the given file,
-        which can be used as an iterator yielding subject response records.
-    """
-    file_path = Path(file_path)
-    assert file_path.exists(), f'{file_path.name} not found'
-    assert file_path.is_file(), f'{file_path.name} is not a file'
-    if fmt is None:
-        fmt = file_path.suffix[1:]
-    if fmt in STORAGE_FMT:
-        m = import_module(STORAGE_FMT[fmt])
-        return m.Table(file_path, **kwargs)
-    else:
-        raise RuntimeError(f'Unknown file format: {repr(fmt)}')
+        return [c_i.sum(axis=1).to_numpy()
+                for c_i in self.response_counts()]
+
+    def item_total_count(self):
+        """Total number of response counts for each item,
+        summed across all response alternatives and all groups.
+        :return: c = list of total response counts,
+            c[i] = scalar integer for i-th item
+        """
+        return [c_i.sum().sum()
+                for c_i in self.response_counts()]
 
 
 # -------------------------------------------------------- Module TEST:
-# if __name__ == '__main__':
-#
-#     def recode_missing_as_0(row):
-#         for i in range(len(row)):
-#             if row[i] is None:
-#                 row[i] = 0
-#     # --------------------------------------------
-#
-#     HAQ_PATH = Path.home() / 'Documents/LeijonKTH/heartech/HA-QualityRegistry/IRT-IOI-HA/IOI-HA-Data'
-#     # ioiha_data_path = HAQ_PATH / 'IRT-IOI-HA' / 'IOI-HA-data'
-#     # to ioi-ha data sets OTHER THAN the Swedish Quality Registry
-#
-#     print('*** Test Load Questionnaire:\n')
-#     q = Questionnaire.load(HAQ_PATH / 'IOI-HA-English.txt')
-#     print(q)
-#     # ------------------------------------------------------------------
-#
-#     print('\n*** Testing table_reader_xlsx with Hickson data set:\n')
-#
-#     test_file = HAQ_PATH / 'Hickson' / 'Short_Eartrak AUS.xlsx'
-#
-#     irf = item_response_table(test_file,
-#                               fields=[f'Q0{i}' for i in range(1, 8)],
-#                               field_types=int,
-#                               header_row=1,
-#                               missing_values=['.', ' '])
-#     print('printing a few records:')
-#     for (i,r) in enumerate(irf):
-#         print(r)
-#         if i > 10:
-#             break
-#     print('printing first few records again:')
-#     for (i,r) in enumerate(irf):
-#         print(r)
-#         if i > 5:
-#             break
-#
-#     all_r = [r for r in irf]
-#     print('number of records=', len(all_r))
-#     print(f'len(irf) = ', len(irf))
-#
-#     # check subject duplicates:
-#     irs = item_response_table(test_file,
-#                               fields=['A'],
-#                               header_row=0)
-#     subjects = set()
-#     dupl_subjects = set()
-#     dupl_records = []
-#     for (i,r) in enumerate(irs):
-#         if r[0] in subjects:
-#             print(f'Duplicate subject ID={repr(r[0])} found in row {i+2}')
-#             dupl_subjects.add(r[0])
-#             dupl_records.append(i)
-#         else:
-#             subjects.add(r[0])
-#     print(f'Found {len(subjects)} unique subject IDs')
-#     print(f'Found {len(dupl_subjects)} duplicate subject IDs in {len(dupl_records)} records')
-#     print(dupl_subjects)
-#
-#     # ----------------------------------------- Use Hickson xlsx in data set:
-#     print('\n*** Testing usin Hickson file in an ItemResponseDataSet object:\n')
-#
-#     irf = item_response_table(test_file,
-#                               fields=[f'Q0{i}' for i in range(1, 8)],
-#                               field_types=int,
-#                               header_row=1,
-#                               missing_values=['.', ' '],
-#                               recode_fcns=recode_missing_as_0)
-#
-#     ids = ItemResponseDataSet(questionnaire=Questionnaire(item_response_levels=[5,5,5,5,5,5,5]),
-#                               groups={'HicksonEarTrak': irf})
-#
-#     print(ids)
-#     print('response_count=\n', ids.item_response_count)
-#     print('total counts: ', [np.sum(c_i) for c_i in ids.item_response_count])
-#
-#     # ----------------------------------------- test Kramer SPSS data set:
-#
-#     print('\n*** Testing table_reader_spss with Kramer data set:\n')
-#
-#     kramer_file = item_response_table(file_path=HAQ_PATH / 'Kramer' / 'moeder_final - kopieforArne.sav',
-#                                       fmt='spss',
-#                                       fields=[f'ioi_v{i}' for i in range(1, 8)],
-#                                       field_types=int,
-#                                       missing_values=[9.0],
-#                                       recode_fcns=recode_missing_as_0)
-#
-#     print(f'Using kramer_file with {len(kramer_file)} records')
-#     print('printing a few records:')
-#     for (i, r) in enumerate(kramer_file):
-#         if i > 10:
-#             break
-#         print(r)
-#
-#     kramer_file2 = item_response_table(file_path=HAQ_PATH / 'Kramer' / 'NLSH-Kramer-T2IOI-HA.sav',
-#                                        fmt='spss',
-#                                        fields=[f'ioi_v{i}' for i in range(1, 8)],
-#                                        field_types=int,
-#                                        missing_values=[9.0],
-#                                        recode_fcns=recode_missing_as_0)
-#
-#     print(f'Using kramer_file with {len(kramer_file2)} records')
-#     print('printing a few records:')
-#     for (i, r) in enumerate(kramer_file2):
-#         if i > 10:
-#             break
-#         print(r)
-#
-#     ids = ItemResponseDataSet(questionnaire=Questionnaire(item_response_levels=[5,5,5,5,5,5,5]),
-#                               groups={'Kramer': kramer_file})
-#
-#     print(ids)
-#     print('response_count=\n', ids.item_response_count)
-#     print('total counts: ', [np.sum(c_i) for c_i in ids.item_response_count])
-#
-#
-# # ------------------------------------------------------- Check using Swedish data set:
+if __name__ == '__main__':
+    from ItemResponseCalc.ir_source import item_response_table, Tables
+    from sqlalchemy import create_engine
+
+    HAQ_PATH = Path.home() / 'Documents/LeijonKTH/heartech/HA-QualityRegistry/IRT-IOI-HA/IOI-HA-Data'
+    # ioiha_data_path = HAQ_PATH / 'IRT-IOI-HA' / 'IOI-HA-data'
+    # to ioi-ha data sets OTHER THAN the Swedish Quality Registry
+
+    print('*** Test Load Questionnaire:\n')
+    ioiha_q = Questionnaire.load(HAQ_PATH / 'IOI-HA-English.txt')
+    print(ioiha_q)
+    # ------------------------------------------------------------------
+
+    print('\n*** Testing Table from Excel with Hickson data set:\n')
+    work_path = HAQ_PATH
+    test_file = HAQ_PATH / 'Hickson' / 'Short_Eartrak AUS.xlsx'
+
+    irf = item_response_table(source=test_file,
+                              items={f'Q0{i}': range(1, 6)
+                                     for i in range(1, 8)},
+                              index_col=0  # integer for read_excel, but string also seems to work
+                              )
+    print('printing a few records:')
+    for (i, r) in enumerate(irf):
+        print(r)
+        if i > 10:
+            break
+    print('printing first few records again:')
+    for (i,r) in enumerate(irf):
+        print(r)
+        if i > 5:
+            break
+
+    all_r = [r for r in irf]
+    print('number of records=', len(all_r))
+    print(f'len(irf) = ', len(irf))
+
+    print('\n*** Test item_response_table using SQLAlchemy engine ***')
+    sql_path = work_path / 'test_sql'
+    engine = create_engine("sqlite+pysqlite:///" + str(sql_path / 'testHickson.db'))
+    ir_sql = item_response_table(source=engine,
+                                 sql='ioiha',  # *** "SELECT * FROM ioiha",
+                                 index_col='EarRowId',
+                                 items={f'Q0{item}': [str(i) for i in range(1, 6)]
+                                        for item in range(1, 8)},
+                                 )  # NOTE: string-encoded integers here
+
+    # ---------------------------------------------------- Test Hickson in data set:
+    print('\n*** Testing using Hickson file(s) in an ItemResponseDataSet object:\n')
+
+    ids = ItemResponseDataSet(questionnaire=ioiha_q, #  Questionnaire(item_response_levels=[5,5,5,5,5,5,5]),
+                              groups={'HicksonEarTrak': irf,
+                                      'Hickson_sql': ir_sql,
+                                      'Hickson_joined': Tables(irf, ir_sql)})
+
+    print(ids)
+    print('\nResponse Counts:')
+    for (i, (q_i, c_df)) in enumerate(zip(ids.questionnaire.items,
+                                          ids.response_counts())
+                                      ):
+        print(f'\nQuestion: ' + q_i.question)
+        print(c_df)
+
+    print('\nitem_response_count=\n', ids.item_response_count())
+    # all items have same n_response_levels:
+    print('item_total_counts: ', ids.item_total_count())
+
+
+    # # ----------------------------------------- test Kramer SPSS data set:
+    #
+    # print('\n*** Testing ItemResponseTable with Kramer data set:\n')
+    #
+    # kramer_file = ItemResponseTable(HAQ_PATH / 'Kramer' / 'moeder_final - kopieforArne.sav',
+    #                                 items={f'ioi_v{i}': range(1, 6)
+    #                                          for i in range(1, 8)},
+    #                                 )
+    #
+    # print(f'Using {kramer_file} with {len(kramer_file)} records')
+    # print('printing a few records:')
+    # for (i, r) in enumerate(kramer_file):
+    #     if i > 10:
+    #         break
+    #     print(r)
+    #
+    # kramer2_columns = {'T2IOIHA1': range(5),  # coded as 0,.., 4
+    #                    'T2IOIHA2': range(1, 6),  # coded as 1,.., 5
+    #                    'T2IOIHA3': range(1, 6),
+    #                    'T2IOIHA4': range(5),  # coded as 0,.., 4
+    #                    'T2IOIHA5': range(1, 6),
+    #                    'T2IOIHA6': range(1, 6),
+    #                    'T2IOIHA7': range(1, 6)}
+    # kramer_file2 = ItemResponseTable(HAQ_PATH / 'Kramer' / 'NLSH-Kramer-T2IOI-HA.csv',  # sav',
+    #                                  items=kramer2_columns,
+    #                                  )
+    #
+    # print(f'Using {kramer_file2} with {len(kramer_file2)} records')
+    # print('printing a few records:')
+    # for (i, r) in enumerate(kramer_file2):
+    #     if i > 10:
+    #         break
+    #     print(r)
+    #
+    # print(f'Testing {kramer_file} in ItemResponseDataSet')
+    # ids = ItemResponseDataSet(questionnaire=Questionnaire(item_response_levels=[5,5,5,5,5,5,5]),
+    #                           groups={'Kramer': kramer_file})
+    #
+    # print(ids)
+    # print('response_count=\n', ids.item_response_count)
+    # print('total counts: ', [np.sum(c_i) for c_i in ids.item_response_count])
+    #
+    # # -------------------- test using Dillon-2010 file
+    # print('\n*** Testing ItemResponseTable with Dillon data set:\n')
+    # dillon10_file = HAQ_PATH / 'Dillon' / 'Final processed file - deidentified_IOIHA.xlsx'
+    # print(f'AU-D-10: Using {dillon10_file}')
+    #
+    # # header = [f'Question{i}' for i in range(1, 8)]
+    # # dillon10 = item_response_table(dillon10_file,
+    # #                                fields=header,
+    # #                                field_types=str,
+    # #                                missing_values=['', 'NS', 'N/A'],
+    # #                                header_row=1,
+    # #                                sample_factor=sample_factor,
+    # #                                accept_row=accept_record,
+    # #                                recode_fcns=[recode_responses, recode_missing])
+    #
+    # dillon10_columns = {f'Question{i+1}': ioiha_q.items[i].responses.copy()
+    #                     for i in range(7)}
+    # dillon10_columns['Question1'][1] = 'less than 1 hour per day'
+    # dillon10_columns['Question1'][2] = '1-4 hours per day'
+    # dillon10_columns['Question1'][3] = '4-8 hours per day'
+    # dillon10_columns['Question2'][0] = 'did not help at all'
+    #
+    # def set_lower_case(v):
+    #     """Ensure lower case in reading strings from Dillon-2010:
+    #     :param v: string cell value
+    #     :return: lower case
+    #     """
+    #     return str(v).lower()
+    #
+    # dillon10 = ItemResponseTable(dillon10_file,
+    #                              items=dillon10_columns,
+    #                              converters={c: set_lower_case
+    #                                          for c in dillon10_columns.keys()})
+    #
+    # print(f'Using {dillon10} with {len(dillon10)} records')
+    # print('printing a few records:')
+    # for (i, r) in enumerate(dillon10):
+    #     if i > 50:
+    #         break
+    #     print(f'{i+2}: ', r)
+    #
+    # print(f'Testing {dillon10} in ItemResponseDataSet')
+    # ids = ItemResponseDataSet(questionnaire=ioiha_q,
+    #                           groups={'Dillon10': dillon10})
+    #
+    # print(ids)
+    # print('response_count=\n', ids.item_response_count)
+    # print('total counts: ', [np.sum(c_i) for c_i in ids.item_response_count])
+
+
+# ------------------------------------------------------- Check using Swedish data set:
 #     print('\n*** Testing table_reader_sqlite with haq data set:\n')
 #
 #     def accept_record(r):
 #         """Inclusion_crit for accepting a record
 #         :param r: dict with all record fields
 #         :param f: list of record field keys to be used
 #         :return: boolean == True if record is acceptable
@@ -445,9 +494,7 @@
 #                                                   'NL': kramer_file,
 #                                                   'SE': haq})
 #
 #     print(ids3)
 #
 #     print('response_count=\n', ids3.item_response_count)
 #     print('total counts: ', [np.sum(c_i) for c_i in ids3.item_response_count])
-
-# ------------------------------------------- plot response distributions
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/safe_logistic.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/safe_logistic.py`

 * *Files identical despite different names*

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/item_respondents.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/item_respondents.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,37 @@
 *** Main Classes:
 
 ResponseGroup -- model for a group of subjects for which
     response data are available for each item for each subject.
 
 GroupMeanTrait -- model for Gaussian distribution of mean trait vector for one group
 
-Arne Leijon, 2019-07-08, first version
+** Version history:
+
+* Version 0.6.0:
+2023-06-24, adapted for new ir_source, responses already encoded with origin=0.
+
+* Version 0.5.0 and earlier:
+2019-07-08, first version
 2019-07-23, cannot use SummaryResponseGroup!
 2019-08-11, delete class SummaryResponseGroup
-2019-08-11, use scales.trait_sel.mean as item_trait_weight
+2019-08-11, use items.trait_sel.mean as item_trait_weight
 2019-08-15, new initialize method, incl. theta randomization
 2019-08-17, single ResponseGroup class, generalized for tied or non-tied prec_among
-2019-08-20, ResponseGroup.adapt returns self, to allow multi-processing
+2019-08-20, ResponseGroup.adapt returns self, to allow multiprocessing
+2020-06-15, internal changes to use external prob_class for core functions
 """
 import numpy as np
 # from scipy.stats import multivariate_normal  # replaced by np.random.Generator
 
 from samppy import hamiltonian_sampler as ham
 from samppy.sample_entropy import entropy_nn_approx as entropy
-from .ir_predictive import GaussianGivenParam
+from ItemResponseCalc.ir_predictive import GaussianGivenParam
 
-from .safe_logistic import logistic
+# from .safe_logistic import logistic
 
 import logging
 logger = logging.getLogger(__name__)
 
 logger.setLevel(logging.INFO)
 # logger.setLevel(logging.DEBUG)
 
@@ -49,42 +56,43 @@
 
 class ResponseGroup:
     """Model representing subjects' latent traits in an OrdinalItemResponseModel,
     learned by adaptation to individual item responses for each subject.
     The trait distribution is represented by sampling.
     """
     @classmethod
-    def initialize_by_item(cls, subject_responses, scales, trait_scale,
+    def initialize_by_item(cls, subject_responses,
+                           items,
+                           trait_scale,
                            name,
                            n_samples=20):
         """Initialize trait values by sampling, on trait for each item
         :param subject_responses: iterable yielding subject responses as a list with
             g_subjects[s][i] = integer index of response to i-th item,
-            coded with origin==1 for the first response alternative,
-            and missing response encoded as 0.
-            Recoded later to python origin 0 for internal use.
-        :param scales: list of ItemScale instances, one for each item
+            re-coded with origin==0 for the first response alternative,
+            and missing response encoded as -1.
+        :param items: list of xxxItem instances, one for each item
         :param trait_scale: scalar initially assumed scale of trait values
         :param n_samples: number of samples of the intra-subject distribution of trait values
         :param name: string identifying this group
         :return: single cls instance
         """
         # collect all response data in one array
-        s_responses = np.array([s_r for s_r in subject_responses]).T
+        s_responses = np.array([s_r for s_r in subject_responses]).T  # *** copy needed?
         # s_responses[i, s] = response-level index for i-th item by s-th subject
-        # still with origin == 1, missing response == 0
+        # with origin == 0, missing response == -1
         # n_items = len(s_responses)
-        th = np.array([sc_i.sample_trait(r_i - 1, n_samples, trait_scale=trait_scale)
-                       for (sc_i, r_i) in zip(scales, s_responses)])
+        th = np.array([i.sample_trait(r_i, n_samples, trait_scale=trait_scale)  # **** deleted -1 here
+                       for (i, r_i) in zip(items, s_responses)])
         # th[i, m, s] = m-th sample for i-th item and s-th subject
         th = th.transpose((1, 2, 0))
         # th[m, s, i] = m-th sample of i-th item for s-th subject
         mu = GroupMeanTrait(loc=np.mean(th, axis=(0, 1)))
         logger.info(f'Initializing {repr(name)}'
-                    + f' with {s_responses.shape[-1]} subjects')
+                    + f' with {s_responses.shape[-1]} respondent records')
         logger.debug('Initial item mu.loc= ' + np.array2string(mu.loc, precision=3))
         return cls(subject_responses=s_responses,
                    theta=th,
                    mu=mu,
                    name=name)
 
     def __init__(self, subject_responses, theta, mu, name):
@@ -92,39 +100,41 @@
         :param subject_responses: 2D array-like list with response data
             response[i, s] = integer ordinal response index for i-th item by s-th subject
             coded with origin==1 for the first response alternative,
         :param theta: 3D array with initial subject latent trait samples
             theta[n, s, t] = n-th sample of t-th trait for s-th subject
         :param mu: GroupMeanTrait instance representing current distribution of mean
         :param name: string with arbitrary label for this object
+
         NOTE: Internal property
-        _response = 2D array of individual response indices, with
+        response0 = 2D array of individual response indices, with
             response[i, s] = integer index of response to i-th item,
             encoded with origin==0, and missing response encoded as -1.
-        The corresponding external property is
-        subject_responses = _response + 1,
-        with origin == 1 and missing response == 0, for external presentation.
+        The corresponding external property
+        subject_responses = response0 + 1,
+        with origin == 1 and missing response == 0, for external presentations.
         """
         assert theta.ndim == 3, 'theta must be 3-dim numpy array'
-        self._response = np.array(subject_responses) - 1
+        self.response0 = np.array(subject_responses) # - 1 # *** done already in ir_source
+        # internal responses always coded with origin 0, missing as -1
         (n_samples, self.n_subjects, self.n_traits) = theta.shape
         self.sampler = ham.HamiltonianSampler(fun=self.neg_logprob,
                                               jac=self.d_neg_logprob,
                                               x=theta.reshape(n_samples, -1),
                                               epsilon=0.3,
                                               n_leapfrog_steps=10)
         # NOTE: theta is stored only as sampler.x
         # args for neg_logprob and d_neg_logprob are defined later, before each call
         self.mu = mu
         self.name = name
         self.ll = None  # log likelihood saved here by adapt step
 
     def __repr__(self):
         return (self.__class__.__name__ + f'(name= {repr(self.name)},'
-                + f'\n\t subject_responses= array with {len(self._response)} responses'
+                + f'\n\t subject_responses= array with {len(self.response0)} responses'
                 + f' by {self.n_subjects} subjects,'
                 + f'\n\t theta= array with shape= {self.theta.shape},'
                 + '\n\t mu= ' + self.mu.__repr__()
                 + ')')
 
     def cov_all(self):
         """Covariance matrix across all samples, all subjects,
@@ -140,32 +150,33 @@
         return c
 
     def transform_traits(self, proj):
         """Transform initial item-traits to (sub-)space defined by external PCA
         :param proj: 2D projection matrix with orthonormal COLUMN vectors
             proj[:, t] = unit vector for t-th trait
         :return: None
-        self.theta and self.mu transformed to proj coordinate system
+
+        Result: self.theta and self.mu transformed to proj coordinate system
         """
         th = np.dot(self.theta, proj)
         self.n_traits = th.shape[-1]
         self.theta = th
         self.mu = GroupMeanTrait(loc=np.mean(th, axis=(0, 1)))
-        logger.info(f'Transformed group {repr(self.name)} self.mu.loc= '
+        logger.debug(f'Transformed group {repr(self.name)} self.mu.loc= '
                     + np.array2string(self.mu.loc, precision=3, suppress_small=True))
 
     @property
     def subject_responses(self):
         """Subject responses as obtained from input files
         using the external encoding {1,..., L_i},
         with missing response == 0
         :return: r = 2D array with responses,
             r[s, i] = response by s-th subject to i-th item
         """
-        return self._response + 1
+        return self.response0 + 1
 
     @property
     def n_samples(self):
         return self.sampler.x.shape[0]
 
     @property
     def theta(self):
@@ -211,49 +222,51 @@
         # But we know distributions are independent among subjects,
         # and Singh et al. (2016) showed convergence is slower with increasing dimension,
         # so an average across all subjects, at low dimension for each subject,
         # is most probably closer to the true value.
         h_sum = sum(entropy(th[:, s, :]) for s in range(th.shape[1]))
         return h_sum
 
-    def adapt(self, scales, precision_within, precision_among):
+    def adapt(self, items,
+              precision_within, precision_among,
+              prob_class):
         """One learning step for distribution of group theta values,
         and group mu property,
         using responses data and current distribution of item scale parameters.
-        :param scales: list of ItemScale objects, one for each item
+        :param items: list of ResponseItem objects, one for each item
         :param precision_within: TraitPrecisionWithinGroup object defining
             current distribution of inter-individual precision matrix within every group
         :param precision_among: TraitPrecisionAmongGroups object defining
             current distribution of psi = scalar precision among group means
+        :param prob_class: core class calculating response-prob and gradients
         :return: self updated, to allow multi-processing
         """
         _id = repr(self.name)  # used for logger output
         logger.debug(self.__class__.__name__ + f'[{_id}].adapt(...)')
         # ---------------------------------- adapt self.theta by Hamilton sampling
-        tau = [sc.tau for sc in scales]
-        weight = [sc.trait_sel.mean for sc in scales]
-        # response thresholds, fixed during theta learning
+        tau = [item.tau for item in items]
+        # = item response thresholds, fixed during theta learning
+        weight = [item.trait_sel.mean for item in items]
         if np.any([np.any(np.isinf(tau_i)) for tau_i in tau]):
             logger.warning(f'{_id}: Infinite tau. Should not happen!')
         mean_precision_within = precision_within.mean
         mean_log_det_prec_within = precision_within.mean_log_det
         # = external parameters, constant during re-sampling of theta
         # but change between calls
-        self.sampler.args = (tau, weight, mean_precision_within, mean_log_det_prec_within)
+        self.sampler.args = (tau, weight,
+                             mean_precision_within, mean_log_det_prec_within,
+                             prob_class)
         max_steps=20
         # logger.debug(f'test sampler._rng.std_normal: {self.sampler._rng.standard_normal()}')
         try:
             self.sampler.safe_sample(min_steps=5, max_steps=max_steps)
             if self.sampler.n_steps >= max_steps:
                 logger.warning(f'{_id}: Done {self.sampler.n_steps} = MAX allowed sampling steps')
             else:
                 logger.debug(f'{_id}: Done {self.sampler.n_steps} sampling steps')
-        #     if self.sampler.accept_rate > 0.95:  # ****** do this in samppy.safe_sample ??? ********
-        #         self.sampler.epsilon *= 1.3
-        #         logger.debug(f'{_id}: High sampler accept_rate; increased epsilon = {self.sampler.epsilon}')
         except ham.AcceptanceError:  # raised by sampler, even after reducing epsilon
             # logger.debug(f'* AcceptanceError {self}.adapt()')
             # self.sampler.epsilon *= (0.7 + 0.2 * uniform.rvs())  # ************** SKIP
             logger.warning((f'{_id}: AcceptanceError: accept_rate= {self.sampler.accept_rate:.2f} ' +
                             f'of {self.sampler.n_trajectories}; ' +
                             f'epsilon reduced to {self.sampler.epsilon:.5f}'))
             # ****** keep going anyway ********
@@ -267,55 +280,57 @@
                             precision_among)
         h = self.entropy_theta
         logger.debug(f'{_id}: LL={LL:.1f}, + entropy={h:.1f}')
         self.ll = LL + h
         logger.debug(self.__class__.__name__ + f'[{_id}].adapt(...) finished')
         return self
 
-    def neg_logprob(self, x, tau, weight, mean_prec, mean_log_det_prec):
+    def neg_logprob(self, x, tau, weight, mean_prec, mean_log_det_prec, prob_class):
         """Negative log-likelihood for any sample subject trait vector
         :param x: 2D array of trait values as stored in self.sampler.x
             x[n, st] = n-th sample of (s,t)-th subject,trait value
         :param tau: list of 2D arrays with UPPER item response thresholds
             tau[i][m, l] = m-th sample of UPPER threshold for l-th response interval of i-th item
             EXCEPT the extreme at +inf
             tau[i].shape[-1] == L_i - 1; L_i = n ordinal response levels
         :param weight: list of 1D arrays of item trait weights
             weight[i][t] = i-th item weight for t-th trait
         :param mean_prec: 2D symmetric intra-group mean precision matrix
         :param mean_log_det_prec: scalar log det(precision matrix)
+        :param prob_class: core class calculating response-prob and gradients
         :return: nlp = 1D vector of negative log-likelihood values
             nlp.shape == (x.shape[0],) == (self.n_samples,)
         """
         th = x.reshape((self.n_samples, self.n_subjects, self.n_traits))
-        return (- self.logprob_by_theta(th, tau, weight)
+        return (- self.logprob_by_theta(th, tau, weight, prob_class)
                 - self.prior_logprob(th, mean_prec, mean_log_det_prec))
 
-    def d_neg_logprob(self, x, tau, weight, mean_prec, mean_log_det_prec):
+    def d_neg_logprob(self, x, tau, weight, mean_prec, mean_log_det_prec, prob_class):
         """Gradient of logprob for any sample subject trait vector
         :param x: 2D array of trait values as stored in self.sampler.x
             x[n, st] = n-th sample of (s,t)-th subject,trait value
         :param tau: list of 2D arrays with UPPER item response thresholds
             tau[i][m, l] = m-th sample of UPPER threshold for l-th response interval of i-th item
             EXCEPT the extreme at +inf
             tau[i].shape[-1] == L_i - 1; L_i = n ordinal response levels
         :param weight: list of 1D arrays of item trait weights
             weight[i][t] = i-th item weight for t-th trait
         :param mean_prec: 2D symmetric intra-group mean precision matrix
         :param mean_log_det_prec: scalar log det(precision matrix)
             NOT NEEDED to calculate gradient w.r.t. theta
+        :param prob_class: core class calculating response-prob and gradients
         :return: dlp = 2D array of gradient row vectors, one for each sample
             dlp.shape == x.shape
         """
         th = x.reshape((self.n_samples, self.n_subjects, self.n_traits))
-        dnlp = (- self.d_logprob_by_theta(th, tau, weight)
+        dnlp = (- self.d_logprob_by_theta(th, tau, weight, prob_class)
                 - self.d_prior_logprob(th, mean_prec))
         return dnlp.reshape((self.n_samples, -1))
 
-    def prior_logprob(self, theta, mean_prec, mean_log_det_prec):
+    def prior_logprob(self, theta, mean_prec, mean_log_det_prec):  # *** module function?
         """Prior log-probability of theta, given current group mu
         :param theta: 3D reshaped array of traits
             theta[n, s, t] = n-th sample of t-th trait for s-th subject
         :param mean_prec: 2D array = mean precision matrix within this group
             externally calculated
         :param mean_log_det_prec: 2D mean log det precision matrix
             externally calculated
@@ -325,15 +340,15 @@
         """
         # th_diff = theta.reshape(self.n_samples, self.n_subjects, -1) - self.mu.loc  # ********
         th_diff = theta - self.mu.loc
         return 0.5 *(self.n_subjects * mean_log_det_prec
                      - np.einsum('nsi, ij, nsj -> n',
                                  th_diff, mean_prec, th_diff))
 
-    def d_prior_logprob(self, theta, mean_prec):
+    def d_prior_logprob(self, theta, mean_prec):  # *** module function?
         """Gradient of prior_log-probability of theta, given current group mu
         :param theta: 3D reshaped array of traits
             theta[n, s, t] = n-th sample of t-th trait for s-th subject
         :param mean_prec: 2D mean precision matrix within this group
         :return: dlp = 2D array with gradient sample vectors
             dlp.shape == theta.shape
         """
@@ -341,120 +356,59 @@
         th_diff = theta - self.mu.loc
         # th_diff[n, s, t] = n-th sample, s-th subject, t-th trait
         # dlp_old = - np.einsum('nsi, ij -> nsj',
         #                       th_diff, mean_prec).reshape(theta.shape)
         dlp = - np.dot(th_diff, mean_prec)  # .reshape(theta.shape)
         return dlp
 
-    def logprob_by_theta(self, theta, tau, weight):
+    def logprob_by_theta(self, theta, tau, weight, prob_class):
         """log-likelihood of observed responses for any sample subject trait vector
         summed across all responses, averaged across threshold samples
         :param theta: 3D reshaped array of traits
             theta[n, s, t] = n-th sample of t-th trait for s-th subject
         :param tau: list of 2D arrays of response thresholds, EXCEPT extremes
             tau[i][m, l] =  m-th sample of UPPER interval limit for l-th response to i-th item
             tau[i].shape[-1] == L_i - 1; L_i = number of ordinal response levels
         :param weight: list of 1D arrays of item trait weights
             weight[i][t] = i-th item weight for t-th trait
+        :param prob_class: core class calculating response-prob and gradients
         :return: lp = 1D vector of log-likelihood values
             lp.shape == (self.n_samples,)
         """
-        # th = theta.reshape((self.n_samples, self.n_subjects, self.n_traits))  # **** already done !
-        lp = [item_logprob_by_theta(theta, tau_i, w_i, r_i)
+        lp = [prob_class.logprob_by_theta(theta, tau_i, w_i, r_i)
               for (tau_i, w_i, r_i) in zip(tau,
                                            weight,
-                                           self._response)]
+                                           self.response0)]
         # lp[i, n] = logprob for n-th theta sample for i-th item
-        # lp = np.dot(self.trait_item_map, lp)
         return np.sum(lp, axis=0)
 
-    def d_logprob_by_theta(self, theta, tau, weight):
+    def d_logprob_by_theta(self, theta, tau, weight, prob_class):
         """Gradient of logprob w.r.t theta, for any given sample subject trait vector
         :param theta: 3D reshaped array of traits
             theta[n, s, t] = n-th sample of t-th trait for s-th subject
         :param tau: list of 2D arrays of response thresholds, EXCEPT extremes
             tau[i][m, l] =  m-th sample of UPPER interval limit for l-th response to i-th item
             tau[i].shape[-1] == L_i - 1; L_i = number of ordinal response levels
         :param weight: list of 1D arrays of item trait weights
             weight[i][t] = i-th item weight for t-th trait
+        :param prob_class: core class calculating response-prob and gradients
         :return: dlp = 3D array of gradients, one for each sample
             dlp[n, s, t] = n-th sample gradient for t-th trait of s-th subject
             dlp[n, s, t] = d logprob(theta[n]) / d theta[n, s, t]
             dlp.shape == theta.shape
         """
-        # th = theta.reshape((self.n_samples, self.n_subjects, self.n_traits))  # **** already done !
-        dlp = [d_item_logprob_by_theta(theta, tau_i, w_i, r_i)
+        dlp = [prob_class.d_logprob_by_theta(theta, tau_i, w_i, r_i)
                for (tau_i, w_i, r_i) in zip(tau,
                                             weight,
-                                            self._response)]
-        # dlp[i, n, s, t] = n-th sample of grad logprob w.r.t theta for i-th item, s-th subject
-        # dlp = np.einsum('ti, ins -> nst',
-        #                 self.trait_item_map, dlp)
+                                            self.response0)]
+        # dlp[i][n, s, :] = n-th sample of grad logprob w.r.t theta for i-th item, s-th subject
         dlp = np.sum(dlp, axis=0)
         # dlp[n, s, t] = n-th d_logprob_by_theta sample for t-th trait, s-th subject
         return dlp  # .reshape(dlp.shape[0], -1)  # shape == theta.shape
 
-    def item_logprob_by_tau(self, tau_i, i, w_i=None):
-        """log prob of observed responses for ONE item,
-        summed across subjects, averaged across theta samples
-        using current theta distribution.
-        :param tau_i: tau_i[m, l] = m-th sample of UPPER interval limit for l-th response
-            tau_i.shape[-1] == L_i - 1
-        :param i: index of selected item
-        :param w_i: (optional) 1D array with trait weights for this item
-        :return: lp = 2D array, with lp[m, t] = m-th sample for t-th trait
-        """
-        r_i = self._response[i]
-        # theta_i = self.theta[..., self.item_trait_index[i]]
-        # theta_i[n, s] = n-th trait sample for s-th subject for this item
-        (tau_low, tau_high) = response_interval(tau_i, r_i)
-        # tau_low[m, s] and tau_high[m, s] are (low, high) interval limits
-        th = self.theta[:, None, :, :]  # to allow broadcast
-        # th[n, 0, s, t] = n-th sample of t-trait for s-th subject
-        lp = log_prob_range(tau_low[..., None] - th, tau_high[..., None] - th)
-        # lp[n, m, s, t] = n-th theta sample, m-th tau sample for s-th subject
-        lp = np.sum(lp, axis=-2)
-        lp = np.mean(lp, axis=0)
-        # lp[m, t] = m-th tau sample, for t-th trait
-        if w_i is None:
-            return lp
-        else:
-            return np.dot(lp, w_i)
-
-    def d_item_logprob_by_tau(self, tau_i, i, w_i):
-        """Gradient of item_logprob_by_tau w.r.t. tau_i,
-        summed across subjects, averaged across theta samples
-        :param tau_i: tau_i[m, l] = m-th sample of UPPER interval limit for l-th response
-            tau_i.shape[-1] == L_i - 1
-        :param i: index of selected item
-        :param w_i: (optional) 1D array with trait weights for this item
-        :return: dlp = 3D array, with
-            dlp[m, l, t] = d logprob(tau_i[m, :] / d tau_i[m, l], given t-th trait
-            dlp.shape == (*tau_i.shape, self.n_traits)
-        """
-        r_i = self._response[i]
-        # theta_i = self.theta[..., self.item_trait_index[i]]
-        (tau_low, tau_high) = response_interval(tau_i, r_i)
-        # tau_low[m, s] and tau_high[m, s] are (low, high) interval limits
-        th = self.theta[:, None, :, :]  # to allow broadcast
-        (da, db) = d_log_prob_range_dab(tau_low[..., None] - th, tau_high[..., None] - th)
-        # da[n, m, s, t] = n-th theta sample, m-th tau sample for t-th trait of s-th subject
-        # of derivative w.r.t. tau_low
-        # db similar for tau_high
-        da = np.dot(np.mean(da, axis=0), w_i)
-        db = np.dot(np.mean(db, axis=0), w_i)
-        # da[n, m, s] = n-th theta sample, m-th tau sample of s-th subject, same for db
-        n_response_levels = tau_i.shape[-1] + 1
-        r_bool = np.array([r_i == l
-                           for l in range(n_response_levels)]).T
-        dlp = np.dot(da, r_bool[:, 1:]) + np.dot(db, r_bool[:, :-1])
-        # dlp[m, l] = derivative w.r.t tau_i[m, l], sum across all responses
-        # when tau[m, l] is LOWER limit PLUS when it is UPPER limit
-        return dlp
-
     # -------------------------------------- Predictive Models for result displays:
     def predictive_individual_cov(self, precision_within):
         """Covariance of the Predictive distribution of IRT traits
         for a RANDOM INDIVIDUAL
         in the sub-population represented by this subject group.
         :param precision_within: TraitPrecisionWithinGroup object defining
             current distribution of inter-individual precision matrix within every group
@@ -506,15 +460,15 @@
         :param item_scale_values: nested list with point-estimated scale values
             item_scale_values[i][r] = value for r-th response to i-th item
             assuming scale mean = 0, to be used for missing responses
         :return: sc_r = 2D array
             sc_r[i, s] = recoded response value for i-th item by s-th subject
             with missing responses recoded as zero
         """
-        r = self._response
+        r = self.response0
         # r[i, s] integer-encoded with origin=0, missing response == -1
         sc_r = np.array([v_i[np.maximum(0, r_i)]
                          for (v_i, r_i) in zip(item_scale_values, r)])
         sc_r[r < 0] = 0.
         return sc_r
 
     def predictive_mean(self):
@@ -629,308 +583,175 @@
         Method: All trait samples to be divided by s
             loc down-scaled, prec up-scaled, i.e., cov downscaled
         """
         self.loc = self.loc / s
         self.prec = self.prec * s * s[:, None]
 
 
-# ---------------------------------------- module help functions
-
-def item_logprob_by_theta(theta, tau_i, w_i, r_i):
-    """sum log prob of observed data for ONE item,
-    averaged across tau samples
-    :param theta: theta[n, s, t] = n-th sample of t-th trait by s-th subject
-    :param tau_i: tau_i[m, l] = m-th sample of UPPER interval limit for l-th response
-        tau_i.shape[-1] == L_i - 1
-    :param w_i: 1D array with w_i[t] = i-th item weight for t-th trait
-    :param r_i: r_i[s] = response index for s-th subject to i-th item
-    :return: lp = 1D array, with lp[n] = n-th sample
-    """
-    (tau_low, tau_high) = response_interval(tau_i, r_i)
-    # tau_low[m, s] and tau_high[m, s] are (low, high) interval limits
-    th = theta[:, None, :, :]  # to allow broadcast
-    # th[n, 0, s, t] = n-th sample of t-th trait for s-th subject
-    lp = log_prob_range(tau_low[..., None] - th, tau_high[..., None] - th)
-    # lp[n, m, s, t] = n-th sample of t-th trait for s-th subject, with m-th tau sample
-    lp = np.sum(lp, axis=-2)  # across subjects
-    # lp[n, m, t]
-    lp = np.mean(lp, axis=-2)
-    # lp[n, t]
-    lp = np.dot(lp, w_i)  # ***** let caller do this ???
-    # lp[n]
-    return lp
-
-
-def d_item_logprob_by_theta(theta, tau_i, w_i, r_i):
-    """d_logprob_by_theta of response data for each item
-    :param theta: theta[n, s, t] = n-th sample of t-th trait by s-th subject
-    :param tau_i: tau_i[m, l] = m-th sample of UPPER interval limit for l-th response
-        tau_i.shape[-1] == L_i - 1
-    :param w_i: 1D array with w_i[t] = i-th item weight for t-th trait
-    :param r_i: list with r_i[s] = response index for s-th subject to i-th item
-    :return: generator yielding dlp = 2D array, with
-        dlp[n, s] = n-th sample of gradient for s-th subject theta value
-    """
-    (tau_low, tau_high) = response_interval(tau_i, r_i)
-    # tau_low[m, s] and tau_high[m, s] are (low, high) interval limits
-    th = theta[:, None, :, :]  # to allow broadcast
-    # th[n, 0, s, t] = n-th sample of t-th trait for s-th subject
-    dlp = d_log_prob_range_dm(tau_low[..., None] - th, tau_high[..., None] - th)
-    # dlp[n, m, s, t] = n-th theta sample, m-th tau sample for s-th subject
-    dlp = np.mean(dlp, axis=1)
-    # dlp[n, s, t] = n-th sample of t-th trait for s-th subject
-    return dlp * w_i    # ***** let caller do the weighting ???
-
-
-def response_interval(tau_i, r_i):
-    """Get response interval for given thresholds and responses for ONE item
-    :param tau_i: 2D array with threshold samples, as
-        tau_i[m, l] = m-th sample of UPPER limit of l-th response interval,
-            EXCEPT extreme limits -infty, +infty
-        tau_i.shape[-1] == L - 1, with L = highest response value
-    :param r_i: 1D array of response indices, with missing response = -1
-        r_i[s] = response index for s-th subject in range(L)
-        except r_[s] = -1 in case of missing response 
-    :return: tuple (tau_low, tau_high) with
-        tau_low[m, s] = m-th sample of lower interval limit for r_i[s]
-        tau_high[m, s] = m-th sample of upper interval limit for r_i[s]
-        tau_low.shape == tau_high.shape
-    """
-    r_i = np.asarray(r_i)
-    max_l = tau_i.shape[-1] - 1
-    # r_i may be -1 for missing response, or = max_l +1 for highest interval
-    tau_low = tau_i[:, np.maximum(0, r_i - 1)]
-    tau_low[:, r_i <= 0] = -np.inf  # lowest interval OR missing response value
-    tau_high = tau_i[:, np.minimum(max_l, r_i)]
-    tau_high[:, r_i > max_l] = np.inf  # highest interval
-    tau_high[:, r_i < 0] = np.inf  # missing response value
-    return tau_low, tau_high
-
-
-def log_prob_range(a, b):
-    """log prob{ a < R <= b },
-    for standard logistic random variable R, i.e.,
-    = log(logistic.cdf(b) - logistic.cdf(a))
-    :param a: array of lower interval limits
-    :param b: array of upper interval limits, such that
-        a.shape == b.shape
-        -inf <= a < b <= +inf
-    :return: lP = array of logprob values
-        lP.shape == a.shape
-    """
-    # Reformulated, numerically safer than use of cdf functions:
-    return (np.log1p(-np.exp(a - b))
-            - np.log1p(np.exp(-b))
-            - np.log1p(np.exp(a))
-            )
-
-
-def d_log_prob_range_dm(am, bm):
-    """Gradient d log_prob_range(am, bm) / dm, where
-    am = a - m, and bm = b - m
-    :param am: array with lower limits
-    :param bm: array with upper limits
-        am.shape == bm.shape
-        -inf <= am  < bm <= +inf
-    :return: d_dm = array of gradient elements
-        d_dm.shape == am.shape == bm.shape
-
-    Method:
-    log_prob_range = log-prob( a < Z <= b),
-    for a logistic-distributed Z with location = m and scale=1,
-    = logprob(a-m < Y <= b-m) for standardized Y with location = 0.
-    = ln(1 - e^(am-bm)) - ln(1 + e^(-bm)) - ln(1 + e^(am))
-    am - bm = a - b is independent of m.
-    Thus,
-    d_dm = - e^{-bm) / (1+ e^{-bm} ) + e^am / (1 + e^am)
-    """
-    return logistic.cdf(am) - logistic.cdf(-bm)
-
-
-def d_log_prob_range_dab(am, bm):
-    """Gradient d log_prob_range(am, bm) w.r.t. interval limits (a, b), where
-    am = a - m, and bm = b - m
-    :param am: array with lower limits
-    :param bm: array with upper limits
-        am.shape == bm.shape
-        -infty <= am  < bm <= +infty
-    :return: tuple (d_da, d_db), where
-        d_da = d logprob(am, bm) w.r.t lower limit a
-        d_db = d logprob(am, bm) w.r.t upper limet b
-        d_da.shape == d_db.shape == am.shape == bm.shape
-
-    Method:
-    log_prob_range = log-prob( a < Z <= b),
-    for a logistic-distributed Z with location = m and scale=1,
-    = logprob(a-m < Y <= b-m) for standardized Y with location = 0.
-    = ln(1 - e^(am-bm)) - ln(1 + e^(-bm)) - ln(1 + e^(am))
-
-    d_da = -1 / (e^{bm - am} - 1 ) - e^am / (1 + e^am)
-    d_db = +1 / (e^{bm - am} - 1 ) + e^bm / (1 + e^bm)
-    """
-
-    c = 1 / np.expm1(bm - am)
-    if np.any(np.logical_not(np.isfinite(c))):
-        logger.warning('Invalid tau, zero interval width')
-    return - c - logistic.cdf(am), c + logistic.cdf(-bm)
-
-
 # -------------------------------------------------------- TEST:
 if __name__ == '__main__':
     # Testing some module functions
 
     from scipy.optimize import check_grad, approx_fprime
 
-    print('\n*** Check logprob_range gradients: ')
-    a = np.array([5.])
-    b = a + 2.
+    from ItemResponseCalc.ir_graded_response_prob import GradedResponse as p_class
 
-    def test_logprob_range_m(y):
-        return log_prob_range(a- y, b- y)
-
-    def test_d_logprob_range_dm(y):
-        return d_log_prob_range_dm(a- y, b- y)
-
-    # ------------------------------------
-    def test_logprob_range_a(y):
-        return log_prob_range(a + y, b)
-
-    def test_d_logprob_range_da(y):
-        return d_log_prob_range_dab(a + y, b)[0]
-
-    # ----------------------------------------
-    def test_logprob_range_b(y):
-        return log_prob_range(a, b + y)
-
-    def test_d_logprob_range_db(y):
-        return d_log_prob_range_dab(a, b + y)[1]
-
-    test_y = np.array([0.])
-    print(f'test_logprob_range_m(test_y) = {test_logprob_range_m(test_y)}')
-
-    err = check_grad(test_logprob_range_m, test_d_logprob_range_dm, test_y)
-    print('d_logprob_range_dm =', test_d_logprob_range_dm(test_y))
-    print('approx_grad = ', approx_fprime(test_y,
-                                          test_logprob_range_m,
-                                          epsilon=1e-6))
-    print('check_grad err = ', err)
-
-    print(f'test_logprob_range_a(test_y) = {test_logprob_range_a(test_y)}')
-    err = check_grad(test_logprob_range_a, test_d_logprob_range_da, test_y)
-    print('d_logprob_range_da =', test_d_logprob_range_da(test_y))
-    print('approx_grad = ', approx_fprime(test_y,
-                                          test_logprob_range_a,
-                                          epsilon=1e-6))
-    print('check_grad err = ', err)
-
-    print(f'test_logprob_range_b(test_y) = {test_logprob_range_b(test_y)}')
-    err = check_grad(test_logprob_range_b, test_d_logprob_range_db, test_y)
-    print('d_logprob_range_db =', test_d_logprob_range_db(test_y))
-    print('approx_grad = ', approx_fprime(test_y,
-                                          test_logprob_range_b,
-                                          epsilon=1e-6))
-    print('check_grad err = ', err)
+    # print('\n*** Check logprob_range gradients: ')
+    # a = np.array([5.])
+    # b = a + 2.
+    #
+    # def test_logprob_range_m(y):
+    #     return log_prob_range(a- y, b- y)
+    #
+    # def test_d_logprob_range_dm(y):
+    #     return d_log_prob_range_dm(a- y, b- y)
+    #
+    # # ------------------------------------
+    # def test_logprob_range_a(y):
+    #     return log_prob_range(a + y, b)
+    #
+    # def test_d_logprob_range_da(y):
+    #     return d_log_prob_range_dab(a + y, b)[0]
+    #
+    # # ----------------------------------------
+    # def test_logprob_range_b(y):
+    #     return log_prob_range(a, b + y)
+    #
+    # def test_d_logprob_range_db(y):
+    #     return d_log_prob_range_dab(a, b + y)[1]
+    #
+    # test_y = np.array([0.])
+    # print(f'test_logprob_range_m(test_y) = {test_logprob_range_m(test_y)}')
+    #
+    # err = check_grad(test_logprob_range_m, test_d_logprob_range_dm, test_y)
+    # print('d_logprob_range_dm =', test_d_logprob_range_dm(test_y))
+    # print('approx_grad = ', approx_fprime(test_y,
+    #                                       test_logprob_range_m,
+    #                                       epsilon=1e-6))
+    # print('check_grad err = ', err)
+    #
+    # print(f'test_logprob_range_a(test_y) = {test_logprob_range_a(test_y)}')
+    # err = check_grad(test_logprob_range_a, test_d_logprob_range_da, test_y)
+    # print('d_logprob_range_da =', test_d_logprob_range_da(test_y))
+    # print('approx_grad = ', approx_fprime(test_y,
+    #                                       test_logprob_range_a,
+    #                                       epsilon=1e-6))
+    # print('check_grad err = ', err)
+    #
+    # print(f'test_logprob_range_b(test_y) = {test_logprob_range_b(test_y)}')
+    # err = check_grad(test_logprob_range_b, test_d_logprob_range_db, test_y)
+    # print('d_logprob_range_db =', test_d_logprob_range_db(test_y))
+    # print('approx_grad = ', approx_fprime(test_y,
+    #                                       test_logprob_range_b,
+    #                                       epsilon=1e-6))
+    # print('check_grad err = ', err)
 
     # ---------------------------------------------------------------
     print('\n*** Testing ResponseGroup ***\n')
     n_samples = 1
     n_subjects = 2
     n_traits = 3
     n_items = 3
 
     theta = np.array([[1., 2., 3.], [0., -1., -2.]])  # 2 subjects, 3 traits
     theta = np.tile(theta, (n_samples, 1, 1))
 
-    s_response = np.array([[1, 2], [3, 4],[0, 4]]) + 1  # 3 items, 5 response levels
+    s_response = np.array([[1, 2], [3, 4],[0, 4]]) # *** + 1  # 3 items, 5 response levels
     # encoded as 1,...,5
     trait_item_map = np.eye(n_traits, dtype=bool)
     mu = GroupMeanTrait(loc=np.zeros(n_traits))
 
     g_ind = ResponseGroup(s_response,
                           theta=theta,
                           mu=mu,
                           name='TEST')
     # NOTE: response encoded with origin == 1 here!  **********************
     print('g_ind=', g_ind)
     print('g_ind.theta=\n', g_ind.theta)
-    print('g_ind._response=\n', g_ind._response)
+    print('g_ind.response0=\n', g_ind.response0)
     print('g_ind.subject_responses=\n', g_ind.subject_responses)
 
     n_tau_samples = 3
     tau = [np.array([[-2., -1., +2., +4]
                      for _ in range(n_tau_samples)])
            for _ in range(3)]  # 3 items, 5 response levels
     print('tau= ', tau)
     r_i = np.arange(-1, 5, dtype=int)
-    (a, b) = response_interval(tau[0], r_i)
-    for (l, a_l, b_l) in zip(r_i, a[0], b[0]):
-        print(f'\tresponse_interval a,b({l})= {a_l, b_l}')
+    # (a, b) = response_interval(tau[0], r_i)
+    # for (l, a_l, b_l) in zip(r_i, a[0], b[0]):
+    #     print(f'\tresponse_interval a,b({l})= {a_l, b_l}')
 
     #  *** th = theta.reshape((n_samples, -1))
     print('sampler theta= ', theta)
     weight = np.eye(n_traits)  # ********** item_i <=> trait_i
     # weight = np.ones((n_items,n_traits))  # ********** item_i <=> trait_i
 
-    lp = g_ind.logprob_by_theta(theta, tau, weight)
+    lp = g_ind.logprob_by_theta(theta, tau, weight, p_class)
     print('logprob_by_theta(theta, tau, weight)= ', lp)
 
     mean_prec_within = np.eye(n_traits)
     mean_log_det_prec = 1.
     lp = g_ind.prior_logprob(theta, mean_prec_within, mean_log_det_prec)
     print('prior_lp(theta, tau)= ', lp)
 
     th = theta.reshape((n_samples, -1))
-    lp = g_ind.neg_logprob(th, tau, weight, mean_prec_within, mean_log_det_prec)
+    lp = g_ind.neg_logprob(th, tau, weight, mean_prec_within, mean_log_det_prec, p_class)
     print('neg_logprob(th, tau)= ', lp)
 
     # -----------------------------------------------
     def test_neg_logprob(y):
-        return g_ind.neg_logprob(y.reshape(1,-1), tau, weight, mean_prec_within, mean_log_det_prec)[0]
+        return g_ind.neg_logprob(y.reshape(1,-1), tau,
+                                 weight,
+                                 mean_prec_within, mean_log_det_prec,
+                                 p_class)[0]
 
     def test_grad_neg_logprob(y):
-         return g_ind.d_neg_logprob(y.reshape(1,-1), tau, weight, mean_prec_within, mean_log_det_prec)[0]
+         return g_ind.d_neg_logprob(y.reshape(1,-1), tau,
+                                    weight,
+                                    mean_prec_within, mean_log_det_prec,
+                                    p_class)[0]
     # -------------------------------------------------
     print('test_neg_logprob(th)= ', test_neg_logprob(th))
 
     y = th[0]  # must be 1D vector for test
     err = check_grad(test_neg_logprob, test_grad_neg_logprob, y)
     print('grad_test =', test_grad_neg_logprob(y))
     print('approx_grad = ', approx_fprime(y,
                                           test_neg_logprob,
                                           epsilon=1e-6))
     print('check_grad err = ', err)
 
-    print('\nTesting item_logprob_by_tau\n')
-
-    item_ind = 0
-    w_i = weight[item_ind]
-
-    # ----------------------------------------
-    def test_logprob_mean_theta(y):
-        tau = y[None, :]
-        return g_ind.item_logprob_by_tau(tau, item_ind, w_i)[0]
-
-    def test_d_logprob_mean_theta(y):
-        tau = y[None, :]
-        return g_ind.d_item_logprob_by_tau(tau, item_ind, w_i)[0]
-
-    test_tau = np.array(tau)[0,0,:]  # must be vector for test
-    print('test_tau= ', test_tau)
-    print('test_logprob_mean_theta(test_tau, item_ind)= ', test_logprob_mean_theta(test_tau))
-
-    err = check_grad(test_logprob_mean_theta, test_d_logprob_mean_theta, test_tau)
-    print('grad_test =', test_d_logprob_mean_theta(test_tau))
-    print('approx_grad = ', approx_fprime(test_tau,
-                                          test_logprob_mean_theta,
-                                          epsilon=1e-6))
-    print('check_grad err = ', err)
-
-    test_tau = np.array(tau)[0, 0, :]  # must be vector for test
-    print('test_tau= ', test_tau)
-    print('test_logprob_mean_theta(test_tau, item_ind)= ', test_logprob_mean_theta(test_tau))
-
-    err = check_grad(test_logprob_mean_theta, test_d_logprob_mean_theta, test_tau)
-    print('grad_test =', test_d_logprob_mean_theta(test_tau))
-    print('approx_grad = ', approx_fprime(test_tau,
-                                          test_logprob_mean_theta,
-                                          epsilon=1e-6))
-    print('check_grad err = ', err)
+    # print('\nTesting item_logprob_by_tau\n')
+    #
+    # item_ind = 0
+    # w_i = weight[item_ind]
+    #
+    # # ----------------------------------------
+    # def test_logprob_mean_theta(y):
+    #     tau = y[None, :]
+    #     return g_ind.item_logprob_by_tau(tau, item_ind, w_i)[0]
+    #
+    # def test_d_logprob_mean_theta(y):
+    #     tau = y[None, :]
+    #     return g_ind.d_item_logprob_by_tau(tau, item_ind, w_i)[0]
+    #
+    # test_tau = np.array(tau)[0,0,:]  # must be vector for test
+    # print('test_tau= ', test_tau)
+    # print('test_logprob_mean_theta(test_tau, item_ind)= ', test_logprob_mean_theta(test_tau))
+    #
+    # err = check_grad(test_logprob_mean_theta, test_d_logprob_mean_theta, test_tau)
+    # print('grad_test =', test_d_logprob_mean_theta(test_tau))
+    # print('approx_grad = ', approx_fprime(test_tau,
+    #                                       test_logprob_mean_theta,
+    #                                       epsilon=1e-6))
+    # print('check_grad err = ', err)
+    #
+    # test_tau = np.array(tau)[0, 0, :]  # must be vector for test
+    # print('test_tau= ', test_tau)
+    # print('test_logprob_mean_theta(test_tau, item_ind)= ', test_logprob_mean_theta(test_tau))
+    #
+    # err = check_grad(test_logprob_mean_theta, test_d_logprob_mean_theta, test_tau)
+    # print('grad_test =', test_d_logprob_mean_theta(test_tau))
+    # print('approx_grad = ', approx_fprime(test_tau,
+    #                                       test_logprob_mean_theta,
+    #                                       epsilon=1e-6))
+    # print('check_grad err = ', err)
```

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/ir_predictive.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_predictive.py`

 * *Files identical despite different names*

### Comparing `ItemResponseCalc-0.5.0/ItemResponseCalc/ir_display.py` & `ItemResponseCalc-0.6.0/src/ItemResponseCalc/ir_display.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,17 +12,22 @@
 
 ItemResponseDisplaySet = a structured container for all display results
 Each display element can be accessed and modified by the user, before saving.
 
 *** Usage Example: see template script run_irt
 
 *** Version History:
+* Version 0.6:
+2023-07-06: Table and figure names set when created. File formats defined in save methods.
+2023-07-06: table results as pandas.DataFrame objects.
+
 2020-06-04, first version for ItemResponseCalc standalone package
 """
 # ********** figure comments table comments
+# **** display individual results ???
 
 import numpy as np
 from collections import Counter
 from pathlib import Path
 
 import logging
 
@@ -39,22 +44,26 @@
        'individual': 'Indiv.',
        'equivalent': 'Equivalent',
        'response': 'Response',
        'probability': 'Prob.',
        'rating': 'Rating',
        'global': 'Global',
        'correlation': 'Correlation',
+       'credibility': 'Credibility',
        }
 # = dict with format parameters that may be changed by user
 # Any other parameters are handled by module ir_display_format
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(logging.INFO)
 # logger.setLevel(logging.DEBUG)  # test
 
+DEFAULT_FIGURE_FORMAT = 'pdf'
+DEFAULT_TABLE_FORMAT = 'txt'
+
 
 # ------------------------------------------------------------
 def set_format_param(**kwargs):
     """Set / modify format parameters for this module
     :param kwargs: dict with any formatting variables
     :return: None
     """
@@ -83,55 +92,73 @@
                  log_likelihood,
                  instrument,
                  traits):
         """
         :param log_likelihood: fmt.FigureRef with log-likelihood plot
         :param instrument: ItemSetDisplay object, showing
             response thresholds, and response_prob plot for each item
+            (only FigureRef displays)
         :param traits: TraitDisplay object with predicted trait distribution
             for population mean, and for random individual in population.
             Traits for individual respondents are NOT (yet) displayed.
+            (containing both FigureRef and ResultTable instances)
         """
         self.log_likelihood = log_likelihood
         self.instrument = instrument
         self.traits = traits
 
     def __repr__(self):
         skip = '\n\t'
         return (self.__class__.__name__ + '(' + skip +
                 (',' + skip).join(f'{key}={repr(v)}'
                                   for (key, v) in vars(self).items()) +
                 skip + ')')
 
-    def save(self, dir_top):
+    def save(self, dir_top,
+             figure_format=None,
+             table_format=None,
+             **kwargs):
         """Save all displays in a directory tree
         :param dir_top: Path or string with top directory for all displays
+        :param figure_format: (optional) single figure-file format string
+        :param table_format: (optional) single table-file format string
+        :param kwargs: (optional) additional parameters passed to ResultTable.save() method.
+            NOTE: NO extra kwargs allowed for plot.save() method!
         :return: None
         """
         dir_top = Path(dir_top)  # just in case
-        self.log_likelihood.save(dir_top)
+        if figure_format is None and table_format is None:
+            figure_format = DEFAULT_FIGURE_FORMAT
+            table_format = DEFAULT_TABLE_FORMAT
+        # One of them may be None -> only the other type of data are saved.
+        dir_top.mkdir(parents=True, exist_ok=True)  # just in case
+        self.log_likelihood.save(dir_top, figure_format=figure_format)
         if self.instrument is not None:
-            self.instrument.save(dir_top)
+            self.instrument.save(dir_top, figure_format=figure_format)
         if self.traits is not None:
-            self.traits.save(dir_top)
+            self.traits.save(dir_top,
+                             figure_format=figure_format,
+                             table_format=table_format,
+                             **kwargs)
 
     @classmethod
     def show(cls, irm, mapping_item=-1, **kwargs):
         """Create displays for all results from an Item Response analysis model,
         and store all display elements in a single structured object.
         :param irm: a single learned OrdinalItemResponseModel instance
-        :param mapping_item: index of irm.scales for item to be used for
+        :param mapping_item: index of irm.items for item to be used for
             mapping non-linear mean rating, given scale trait
         :param: kwargs: (optional) any display formatting parameters
         :return: a single cls instance
         """
         set_format_param(**kwargs)
         logger.info(f'Creating displays for {len(irm.groups)} group(s): ' +
                     ', '.join(g.name for g in irm.groups))
-
+        logger.info(fig_comments())
+        logger.info(table_comments())
         return cls(log_likelihood=fmt.fig_log_likelihood(irm.log_prob,
                                                          irm.n_subjects,
                                                          color='r',
                                                          name='LearnedLL'),
                    instrument=ItemSetDisplay.show(irm),
                    traits=TraitDisplay.show(irm, mapping_item))
 
@@ -146,104 +173,109 @@
         :param response_freq: FigureRef with relative response frequencies, all items
         :param items: dict with elements (item_id, item_display),
             item_display = ItemDisplay object
         """
         self.response_freq = response_freq
         self.items = items
 
-    def save(self, top_path):
+    def save(self, top_path, figure_format):
         """
-        :param top_path:
+        :param top_path: path where plots are saved
+        :param figure_format: file format for saved figures
         :return: None
         """
         items_path = top_path / 'items'
+        items_path.mkdir(parents=True, exist_ok=True)
         if self.response_freq is not None:
-            self.response_freq.save(items_path)
+            self.response_freq.save(items_path, figure_format)
         for item in self.items.values():
-            item.save(items_path)
+            item.save(items_path, figure_format)
 
     @classmethod
     def show(cls, irm):
         """
         :param irm: OrdinalItemResponseModel instance
         :return: a cls instance
         """
         t_min = min(np.min(s.tau) - 2. * s.latent_scale
-                    for s in irm.scales)
+                    for s in irm.items)
         t_max = max(np.max(s.tau) + 2. * s.latent_scale
-                    for s in irm.scales)
+                    for s in irm.items)
         t = np.linspace(t_min, t_max, 100)
         # same trait range across all items
         g_count = irm.item_response_count()
         # = dict with list of Counter objects, one for each item
         total_count = [sum((g_c[i] for g_c in g_count.values()), Counter())
                        for i in range(irm.n_items)]
         # *** use item_id instead of item_index ********************
         return cls(response_freq=fmt.fig_response_freq(total_count,
                                                        name='Response_freq'),
                    items={f'Q{scale.item_index + 1}': ItemDisplay.show(scale,
                                                                        count,
                                                                        trait=t)
-                          for (scale, count) in zip(irm.scales,
+                          for (scale, count) in zip(irm.items,
                                                     total_count)})
 
 
 class ItemDisplay:
     """Container for all displays related to ONE item
     """
     def __init__(self,
                  response_freq=None,
                  response_prob=None,
                  mean_response=None):
         """
         :param response_freq: FigureRef with empirical response freq
-        :param response_prob: FigureRef with predicted response prob vs. trait
+        :param response_prob: FigureRef with predicted response probability vs. trait,
+            like the 'Category Characteristic Curve' in the Rasch tradition.
         :param mean_response: FigureRef with expected response vs. trait
-            like "Item Characteristic Curves" in the Rasch tradition.
             (*** and ? empirical response range vs trait ? *****)
             NOTE: NOT valid, as ordinal responses are NOT on interval scale
             SKIPPING this display variant for now...
         """
         self.response_freq = response_freq
         self.response_prob = response_prob
         self.mean_response = mean_response
 
-    def save(self, save_path):
+    def save(self, save_path, figure_format):
         """
         :param save_path: path where sub-objects are saved
+        :param figure_format: file format of saved figures
         :return:
         """
-        if self.response_freq is not None:
-            self.response_freq.save(save_path)
-        if self.response_prob is not None:
-            self.response_prob.save(save_path)
-        if self.mean_response is not None:
-            self.mean_response.save(save_path)
+        if figure_format is not None:
+            if self.response_freq is not None:
+                self.response_freq.save(save_path, figure_format)
+            if self.response_prob is not None:
+                self.response_prob.save(save_path, figure_format)
+            if self.mean_response is not None:
+                self.mean_response.save(save_path, figure_format)
 
     @classmethod
     def show(cls, item_scale, response_count, trait):
         """Generate displays for given item
-        :param item_scale: OrdinalItemScale object
-        :param response_count: Counter object with response counts
+        :param item_scale: GradedResponseItem object
+        :param response_count: Counter object with response counts  *** needed ? ***
         :param trait: 1D array with dense trait values for plot
         :return: a cls instance
         """
         item_id = f'Q{1+item_scale.item_index}'
         # ***** use item_scale.item_id instead *********************
         tau = np.mean(item_scale.tau, axis=0)
         ord_prob = item_scale.ordinal_prob(trait)
         r_mean = 1. + np.dot(ord_prob, np.arange(item_scale.n_response_levels))
         # response_freq=fmt.fig_response_freq(response_count),
         return cls(response_prob=fmt.fig_response_prob(trait, ord_prob,
-                                                       name=item_id + '_prob',
+                                                       name=item_id + FMT['probability'],
                                                        tau=tau,
                                                        x_label=FMT['trait'],
                                                        y_label=' '.join([FMT['response'],
                                                                          FMT['probability']])
-                                                       ))
+                                                       )
+                   )
 
 
 class TraitDisplay:
     """Container for result displays of predicted trait values
     for all traits and groups,
     with layout depending on number of groups and traits.
     """
@@ -261,92 +293,107 @@
        """
         self.pop_mean = pop_mean
         self.pop_ind = pop_ind
         self.corr_global = corr_global
         self.corr_within = corr_within
         self.group_diff = group_diff
 
-    def save(self, path):
-        if self.pop_mean is not None:
-            self.pop_mean.save(path)
-        if self.pop_ind is not None:
-            self.pop_ind.save(path)
+    def save(self, path, figure_format, table_format, **kwargs):
+        """
+        :param path: to directory where all display objects are saved
+        :param figure_format: file format for saved figures
+        :param table_format: file format for saved tables
+        :param kwargs: (optional) additional parameters to table save method
+        :return:
+        """
+        if figure_format is not None:
+            if self.pop_mean is not None:
+                self.pop_mean.save(path, figure_format)
+            if self.pop_ind is not None:
+                self.pop_ind.save(path, figure_format)
         if self.corr_global is not None:
-            self.corr_global.save(path)
+            self.corr_global.save(path, table_format, **kwargs)
         if self.corr_within is not None:
-            self.corr_within.save(path)
+            self.corr_within.save(path, table_format, **kwargs)
         if self.group_diff is not None:
             for (trait_id, trait_diff) in self.group_diff.items():
-                trait_diff.save(path / 'group_diff', name=trait_id)
+                trait_diff.save(path / 'group_diff',
+                                figure_format=figure_format,
+                                table_format=table_format,
+                                **kwargs)
 
     @classmethod
     def show(cls, irm, mapping_item=-1):
         """
         :param irm: OrdinalItemResponseModel instance
         :param mapping_item: index of item to be used for non-linear scale mapping
         :return: a cls instance
         """
+        # *** show percentiles as table, too ? ***
         def _fig_percentiles(perc, g_labels, t_labels, y_label):
             """Plot trait percentiles vs groups or traits,
             in style depending on n_groups and n_traits
             :param perc: 3D array with percentile trait values
                 perc[g, p, t] = p-th percentile of t-th trait in g-th population
             :param g_labels: list of group label strings
                 len(g_labels) == perc.shape[0]
             :param t_labels: list of trait label strings
                 len[t_labels] == perc.shape[2]
             :param y_label: string with y-axis label
-            :param mapping_item: index of irm.scales to be used for mapping
+            :param mapping_item: index of irm.items to be used for mapping
             :return: FigureRef instance
             """
             (n_groups, n_perc, n_traits) = perc.shape
             if n_traits > 1:  # plot perc vs traits, with populations as sub-cases
                 f = fmt.fig_percentiles(perc,
                                         x_label=FMT['trait'],
                                         x_ticklabels=t_labels,
                                         case_labels=g_labels,
+                                        name=y_label,
                                         y_label=y_label,
                                         x_offset=0.07)
             else:  # plot perc vs groups, with traits as sub-cases
                 f = fmt.fig_percentiles(perc.transpose(2, 1, 0),
                                         x_label=FMT['population'],
                                         x_ticklabels=g_labels,
                                         case_labels=t_labels,
+                                        name=y_label,
                                         y_label=y_label,
                                         x_offset=0.07)
             # ax = f.ax
             # make second corresponding scale with expected response ratings
             (y_min, y_max) = f.ax.get_ylim()
             y_min -= 0.1  # **** fix to make more space for legend
             f.ax.set_ylim(y_min, y_max)
             y = np.linspace(y_min, y_max, 100)
             # use mapping_item and its item_id
-            y_mapped = 1. + irm.scales[mapping_item].mean_ordinal(y)
-            item_id = f'Q{1+irm.scales[mapping_item].item_index}'
-            # item_id = irm.scales[mapping_item].item_id
+            y_mapped = 1. + irm.items[mapping_item].mean_ordinal(y)
+            item_id = f'Q{1+irm.items[mapping_item].item_index}'
+            # item_id = irm.items[mapping_item].item_id
             f.mapped_y_axis(y, y_mapped,
                             y_label=(FMT['equivalent'] + ' ' +
                                      item_id + ' ' +
                                      FMT['rating'])
                             )
             return f
         # -----------------------------------------------------------
         item_trait_map = irm.item_trait_map()
         trait_sel = np.any(item_trait_map, axis=0)
         # = boolean trait index for display, just in case irm has NOT been pruned
-        item_trait_map = item_trait_map[:, trait_sel]
+        # *** should display the non-pruned model?
+        # *** NO, because only traits[trait_sel] are effectively used in the model.
         n_traits = np.sum(trait_sel)
         group_labels = [g.name for g in irm.groups]
         group_mean_samples = np.array([g.predictive_mean().rvs(size=10000)[:, trait_sel]
                                        for g in irm.groups])
         group_mean_perc = np.percentile(group_mean_samples,
                                         FMT['percentiles'],
                                         axis=1)
         # group_mean_perc[p, g, t] = p-th percentile for t-th trait in g-th population
-        trait_labels = fmt._make_trait_labels(item_trait_map)  # **** done by model?
+        trait_labels = fmt._make_trait_labels(item_trait_map[:, trait_sel])
         pop_mean = _fig_percentiles(group_mean_perc.transpose(1, 0, 2),
                                     group_labels,
                                     trait_labels,
                                     y_label=' '.join([FMT['population'],
                                                       FMT['mean'],
                                                       FMT['trait']])
                                     )
@@ -362,38 +409,38 @@
                                                      FMT['trait']])
                                    )
 
         c_global = None
         c_within = None
         if n_traits > 1:
             if irm.n_groups > 1:
-                c_global = fmt.tab_correlation_matrix(irm.predictive_individual_cov(),
-                                                      item_trait_map,
+                c_global = fmt.tab_correlation_matrix(irm.predictive_individual_cov(), item_trait_map,
                                                       name='_'.join((FMT['trait'],
                                                                      FMT['correlation'],
                                                                      FMT['global'])
                                                                     ))
-            c_within = fmt.tab_correlation_matrix(irm.precision_within.mean_inv,
-                                                  item_trait_map,
+            c_within = fmt.tab_correlation_matrix(irm.precision_within.mean_inv, item_trait_map,
                                                   name='_'.join((FMT['trait'],
                                                                  FMT['correlation'],
                                                                  FMT['population'])
                                                                 ))
 
         g_diff = None
         if irm.n_groups > 1:
             g_diff = {trait_id: GroupDiffDisplay.show(t_samples,
-                                                      group_labels)
+                                                      group_labels,
+                                                      trait_label=trait_id)
                       for (trait_id, t_samples) in zip(trait_labels,
                                                        group_mean_samples.transpose(2, 0, 1))
                       }
             if n_traits > 1:
                 g_diff['Mean_Trait'] = GroupDiffDisplay.show(np.mean(group_mean_samples,
                                                                      axis=-1),
-                                                             group_labels)
+                                                             group_labels,
+                                                             trait_label='Mean_Trait')
 
         return cls(pop_mean=pop_mean,
                    pop_ind=pop_ind,
                    corr_global=c_global,
                    corr_within=c_within,
                    group_diff=g_diff)
 
@@ -406,44 +453,99 @@
         """
         :param fig: FigureRef object
         :param tab: TableRef object
         """
         self.fig = fig
         self.tab = tab
 
-    def save(self, path, name):
+    def save(self, path,
+             figure_format,
+             table_format,
+             **kwargs):
         """
         :param path: path to directory for saved plots and tables
-        :param name: string with file name
+        :param figure_format: file format of saved figures
+        :param table_format: file format of saved table
+        :param kwargs: (optional) additional arguments to Table.save method
         :return: None
         """
         if self.fig is not None:
-            self.fig.save(path, name=name)
+            self.fig.save(path, figure_format=figure_format)
         if self.tab is not None:
-            self.tab.save(path, name=name)
+            self.tab.save(path, table_format=table_format, **kwargs)
 
     @classmethod
-    def show(cls, group_samples, group_labels):
+    def show(cls, group_samples, group_labels, trait_label):
         """Display credible differences between groups,
         given samples of predictive distribution
         :param group_samples: 2D array with
             group_samples[g, n] = n-th sample of selected trait for g-th group
         :param group_labels: list of string-valued group labels
             len(group_labels) == group_samples.shape[0]
+        :param trait_label: string identifying the difference to be shown
         :return: a cls instance
         """
-        # **** Sort groups for decreasing median values *************
+        # **** Sort groups for decreasing median values
         s_ind = np.argsort(np.median(group_samples, axis=1))[::-1]
         g_samples = group_samples[s_ind, :]
         g_labels = [group_labels[i] for i in s_ind]
         diff = cred_diff(g_samples,
                          diff_axis=0, sample_axis=1,
                          p_lim=np.amin(FMT['credibility_levels']))
 
         fig = fmt.fig_credible_diff(diff,
+                                    diff_label=trait_label,
                                     x_labels=g_labels,
                                     x_label=FMT['population'],
                                     cred_levels=FMT['credibility_levels'])
-        tab = fmt.tab_credible_diff(diff,
-                                    x_labels=g_labels,
-                                    x_label=FMT['population'])
+        # tab_old = fmt.tab_credible_diff_old(diff, x_labels=g_labels, x_label=FMT['population'])
+        tab = fmt.tab_credible_diff(diff, diff_name=trait_label,
+                                    cred_header=FMT['credibility'],
+                                    x_labels=g_labels, x_label=FMT['population'])
         return cls(fig, tab)
+
+
+# ------------------------------------------------ Result explanations
+def fig_comments():
+    """Generate figure explanations.
+    :return: comment string
+    """
+    p_min = np.amin(FMT['percentiles'])
+    p_max = np.amax(FMT['percentiles'])
+    c = f"""Figure Explanations:
+
+Figure files with a name like Population_Indiv_Trait.xxx or Population_Mean_Trait.xxx
+display user-requested percentiles (markers) and credible intervals (vertical bars)
+for the estimated trait distribution for a random individual and for the population mean.
+The vertical bars show the range between {p_min:.1f}- and {p_max:.1f}- percentiles.
+
+The displayed ranges include all uncertainty
+caused both by real inter-individual perceptual differences
+and by the limited number of items and discrete response categories.
+
+Item-specific figures show the model-estimated probability for each response category
+as a function of the latent trait parameter.
+These plots are sometimes called 'Category Characteristic Curves' in Rasch analysis.
+"""
+    return c
+
+
+def table_comments():
+    c = """Table Explanations:
+
+Files with names like someTrait.txt or, *.csv, tabulate all pairs of populations
+for which the trait difference is JOINTLY credibly different,
+with the tabulated credibility value.
+
+The credibility value in each table row is the JOINT probability
+for the pairs in the same row and all rows above it.
+Thus, the joint probability values already account for multiple comparisons,
+so no further adjustments are needed.
+
+The same information is also saved in figure files with similar names, like someTrait.pdf,
+showing all population pairs with jointly credible trait differences.
+
+If several latent traits are needed to model the response data, 
+table files with names like Trait_Correlation_xxx.xxx 
+show the estimated correlation between traits. 
+"""
+    return c
```

