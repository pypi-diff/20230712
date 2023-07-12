# Comparing `tmp/CEEMDAN_LSTM-1.2b2.tar.gz` & `tmp/CEEMDAN_LSTM-1.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CEEMDAN_LSTM-1.2b2.tar", last modified: Sat Jul  8 13:25:37 2023, max compression
+gzip compressed data, was "CEEMDAN_LSTM-1.2b3.tar", last modified: Wed Jul 12 08:08:59 2023, max compression
```

## Comparing `CEEMDAN_LSTM-1.2b2.tar` & `CEEMDAN_LSTM-1.2b3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.215470 CEEMDAN_LSTM-1.2b2/
-drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.203455 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/
--rw-rw-rw-   0        0        0      916 2022-11-18 01:34:52.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/__init__.py
--rw-rw-rw-   0        0        0    27877 2023-06-28 09:46:22.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/core.py
--rw-rw-rw-   0        0        0    41842 2023-06-28 02:14:57.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/data_preprocessor.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.213968 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/
--rw-rw-rw-   0        0        0    30846 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/beijing_ets.csv
--rw-rw-rw-   0        0        0    56764 2023-03-15 06:59:29.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ftse.csv
--rw-rw-rw-   0        0        0    97722 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/guangzhou_ets.csv
--rw-rw-rw-   0        0        0    59837 2023-03-15 06:59:12.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hsi.csv
--rw-rw-rw-   0        0        0    60602 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hubei_ets.csv
--rw-rw-rw-   0        0        0    57605 2023-06-08 11:49:39.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/n225.csv
--rw-rw-rw-   0        0        0    61006 2023-06-08 11:48:36.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/nasdaq.csv
--rw-rw-rw-   0        0        0    60683 2023-03-15 06:59:00.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sp500.csv
--rw-rw-rw-   0        0        0   536253 2022-08-31 07:05:12.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sse_index.csv
--rw-rw-rw-   0        0        0    55845 2023-03-15 06:57:54.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ssec.csv
--rw-rw-rw-   0        0        0    26696 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/tianjin_ets.csv
--rw-rw-rw-   0        0        0    52234 2023-06-28 10:01:40.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/keras_predictor.py
--rw-rw-rw-   0        0        0    32567 2023-06-28 05:07:59.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/sklearn_predictor.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:25:37.206966 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/
--rw-rw-rw-   0        0        0     9996 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-08 13:25:37.000000 CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b2/LICENSE
--rw-rw-rw-   0        0        0     9996 2023-07-08 13:25:37.214966 CEEMDAN_LSTM-1.2b2/PKG-INFO
--rw-rw-rw-   0        0        0     9161 2023-06-14 11:10:49.000000 CEEMDAN_LSTM-1.2b2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 13:25:37.216475 CEEMDAN_LSTM-1.2b2/setup.cfg
--rw-rw-rw-   0        0        0     1374 2023-07-08 13:25:18.000000 CEEMDAN_LSTM-1.2b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:08:59.655016 CEEMDAN_LSTM-1.2b3/
+drwxrwxrwx   0        0        0        0 2023-07-12 08:08:59.627845 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/
+-rw-rw-rw-   0        0        0      917 2023-07-10 18:54:14.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/__init__.py
+-rw-rw-rw-   0        0        0    29901 2023-07-12 04:54:12.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/core.py
+-rw-rw-rw-   0        0        0    42026 2023-07-12 02:38:33.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/data_preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:08:59.652015 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/
+-rw-rw-rw-   0        0        0    30846 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/beijing_ets.csv
+-rw-rw-rw-   0        0        0    56764 2023-03-15 06:59:29.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/ftse.csv
+-rw-rw-rw-   0        0        0    97722 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/guangzhou_ets.csv
+-rw-rw-rw-   0        0        0    59837 2023-03-15 06:59:12.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/hsi.csv
+-rw-rw-rw-   0        0        0    60602 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/hubei_ets.csv
+-rw-rw-rw-   0        0        0    57605 2023-06-08 11:49:39.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/n225.csv
+-rw-rw-rw-   0        0        0    61006 2023-06-08 11:48:36.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/nasdaq.csv
+-rw-rw-rw-   0        0        0    60683 2023-03-15 06:59:00.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/sp500.csv
+-rw-rw-rw-   0        0        0   536253 2022-08-31 07:05:12.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/sse_index.csv
+-rw-rw-rw-   0        0        0    55845 2023-03-15 06:57:54.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/ssec.csv
+-rw-rw-rw-   0        0        0    26696 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/tianjin_ets.csv
+-rw-rw-rw-   0        0        0    52151 2023-07-11 16:00:13.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/keras_predictor.py
+-rw-rw-rw-   0        0        0    27493 2023-07-12 01:28:10.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/sklearn_predictor.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:08:59.630353 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/
+-rw-rw-rw-   0        0        0     9996 2023-07-12 08:08:59.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-07-12 08:08:59.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:08:59.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-12 08:08:59.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 08:08:59.000000 CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1067 2022-08-31 06:31:07.000000 CEEMDAN_LSTM-1.2b3/LICENSE
+-rw-rw-rw-   0        0        0     9996 2023-07-12 08:08:59.654017 CEEMDAN_LSTM-1.2b3/PKG-INFO
+-rw-rw-rw-   0        0        0     9161 2023-06-14 11:10:49.000000 CEEMDAN_LSTM-1.2b3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 08:08:59.655016 CEEMDAN_LSTM-1.2b3/setup.cfg
+-rw-rw-rw-   0        0        0     1374 2023-07-10 18:54:29.000000 CEEMDAN_LSTM-1.2b3/setup.py
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/__init__.py` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ﻿# __init__.py
 
-__version__ = '1.2b'
+__version__ = '1.2b3'
 __module_name__ = 'CEEMDAN_LSTM'
 
 # Basic
 from CEEMDAN_LSTM.core import (
     help,
     show_keras_example,
     show_keras_example_model,
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/core.py` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -280,15 +280,15 @@
     """
     Name the predictor for convenient saving.
     """
     redecom_mode = ''
     if redecom_list is not None: # Check redecom_list and get redecom_mode
         try: redecom_list = pd.DataFrame(redecom_list, index=[0]) 
         except: raise ValueError("Invalid input for redecom_list! Please input eg. None, '{'co-imf0':'vmd', 'co-imf1':'emd'}'.")
-        for i in range(redecom_list.size): redecom_mode = redecom_mode+redecom_list.values.ravel()[i]+'-'
+        for i in (redecom_list+redecom_list.columns.str[-1]).values.ravel(): redecom_mode = redecom_mode+i+'-'
 
     if type(model) == str and '.h5' not in str(model):
         if 'Single' not in name:
             if decom_mode is not None: 
                 name = name + ' ' + decom_mode.upper() + '-' 
                 name = name + redecom_mode.upper()
         else: name = name + ' '
@@ -298,59 +298,89 @@
     name = name + ' ' + module+' Forecasting'
     print('==============================================================================')
     print(str(now.strftime('%Y-%m-%d %H:%M:%S'))+' '+ name +' is running...')
     print('==============================================================================')
     return name
 
 # Output Result
-def output_result(df_result, name, time, imf='', type='Result'):
+def output_result(df_result, name, time, imf='', next_day=False, run=None):
     # Output Result and add Runtime
     """
     Input and Parameters:
     ---------------------
     name            - predictor_name
     time            - end-start
+    imf             - Final or Co-imf0 or ...
+    run             - multiple run times mark
 
     Output
     ---------------------
     df_result 
     """
-    imf_name = ''
+
+    imf_name, run_name = '', ''
+    if run is not None: run_name = 'Run'+str(run)+'-'
     if imf != '' and imf != 'Final': 
         imf_name = ' of '+imf
         print('\n----------'+name+imf_name+' Finished----------')
     else: print('\n================'+name+' Finished================')
-    if isinstance(df_result, tuple) and len(df_result)==3: # (df_result, df_eval, df_loss)
-        df_result[1]['Runtime'] = time # Output Runtime
-        df_result[1]['IMF'] = imf
-        df_result[0].name, df_result[1].name, df_result[2].name = name+' Result'+imf_name, name+' Evaluation'+imf_name, name+' Loss'+imf_name
-        print(df_result[1]) # print df_eval
-    elif isinstance(df_result, tuple) and len(df_result)==2 and type=='Evaluation': # (df_pred_result, df_eval_result)
+    
+    def finish_evaluation(final_pred, df_eval=None):
         from CEEMDAN_LSTM.data_preprocessor import eval_result
-        df_pred_result = df_result[0]
-        final_eval = eval_result(df_pred_result['predict'], df_pred_result['real'])
-        final_eval['Runtime'] = time # Output Runtime
-        final_eval['IMF'] = imf
+        if df_eval is None: # single method
+            final_eval = eval_result(final_pred['real'], final_pred['predict'])
+            final_eval['Runtime'], final_eval['IMF'] = time, imf
+        elif len(df_eval)==1: 
+            final_eval = df_eval # multiple method
+            final_eval['Runtime'], final_eval['IMF'] = time, imf
+        elif 'Final' in df_eval['IMF'].values: final_eval = df_eval # multiple method
+        else: # respective method
+            final_eval = eval_result(final_pred['real'], final_pred['predict'])
+            final_eval['Runtime'], final_eval['IMF'] = time, imf
+            final_eval = pd.concat((final_eval, df_result[1]))
+        final_eval.name = name+' Evaluation'+imf_name
         print(final_eval)
-        df_plot = df_pred_result[['real', 'predict']]
-        final_eval = pd.concat((final_eval, df_result[1]))
-        df_pred_result.name, final_eval.name, df_plot.name = name+' Result', name+' Evaluation', name+' Result'
-        df_result = [df_pred_result, final_eval, df_plot]
-    elif isinstance(df_result, tuple) and len(df_result)==2 and type=='Result': # (df_result, df_next_result)
-        df_result[0]['Runtime'] = time # Output Runtime
-        df_result[0]['IMF'] = imf
-        df_result = pd.concat((df_result[0], df_result[1]))
-        df_result.name = name+' Result'
-        print(df_result)
-    elif isinstance(df_result, pd.DataFrame) and type=='Result': # (df_result)
-        df_result['Runtime'] = time # Output Runtime
-        df_result['IMF'] = imf
-        df_result.name = name+' Result'+imf_name
-        print(df_result)
-    else: raise ValueError('Unknown Error.')
+        return final_eval
+
+    if not next_day:
+        if isinstance(df_result, tuple) and len(df_result)==3: # input (df_result, df_eval, df_loss)
+            final_pred, final_pred.name = df_result[0], name+' Result'+imf_name
+            df_result[2].name = name+' Loss'+imf_name
+            final_eval = finish_evaluation(final_pred, df_result[1]) # evaluation for final
+            final_pred.columns = run_name+final_pred.columns
+            if 'of' in imf_name: # not Final
+                final_pred.columns = run_name+imf+'-'+final_pred.columns 
+                df_result[2].columns = run_name+imf+'-'+df_result[2].columns 
+            final_eval['IMF'] = run_name + final_eval['IMF']
+            df_result = (final_pred, final_eval, df_result[2]) # return (final_pred, final_eval)
+        elif isinstance(df_result, tuple) and len(df_result)==2: # input (df_pred, df_eval) 
+            final_pred, final_pred.name = df_result[0], name+' Result'+imf_name
+            final_eval = finish_evaluation(final_pred, df_result[1]) # evaluation for final
+            final_pred.columns = run_name+final_pred.columns
+            if 'of' in imf_name: final_pred.columns = run_name+imf+'-'+final_pred.columns # not Final
+            final_eval['IMF'] = run_name + final_eval['IMF']
+            df_result = (final_pred, final_eval) # return (final_pred, final_eval)
+        elif isinstance(df_result, pd.DataFrame): # input df_pred 
+            final_pred, final_pred.name = df_result, name+' Result'
+            final_eval = finish_evaluation(final_pred)
+            df_result = (final_pred, final_eval) # return (final_pred, final_eval)
+        else: raise ValueError('Unknown Error.')
+    else: # for next-day predict
+        if isinstance(df_result, tuple) and len(df_result)==2 and next_day==True: # (df_result, df_next_result) for next-day predict
+            df_result[0]['Runtime'] = time 
+            df_result[0]['IMF'] = imf
+            df_result = pd.concat((df_result[0], df_result[1]))
+            df_result.name = name+' Result'
+            df_result['IMF'] = run_name + df_result['IMF']
+            print(df_result)
+        elif isinstance(df_result, pd.DataFrame) and next_day==True: # input df_next_pred
+            if len(df_result)==1: df_result['Runtime'], df_result['IMF'], df_result.name  = time, imf, name+' Result'+imf_name
+            df_result['IMF'] = run_name + df_result['IMF']
+            print(df_result)
+        else: raise ValueError('Unknown Error.')
     return df_result
     
 
 
 # Plot and save data
 def plot_save_result(data, name=None, plot=True, save=True, path=None, type=None): 
     """
@@ -373,43 +403,44 @@
     elif isinstance(name, datetime):
         name = name.strftime('%Y%m%d_%H%M%S_')
     else: name = ''
     if PATH is None: save = False
 
     def default_output(df, file_name): 
         if 'Evaluation' not in df.name and 'Next' not in df.name and plot:
-            df.plot(figsize=(6,3))
+            if df.columns.size<3: df.plot(figsize=(7,4))
+            elif 'real' in df.columns and 'predict' in df.columns: df[['real', 'predict']].plot(figsize=(8,4))
             plt.title(df.name, fontsize=12, y=1)
             if save: plt.savefig(FIG_PATH + file_name +'.jpg', dpi=300, bbox_inches='tight') # Save figure
             plt.show()
-        if save: pd.DataFrame.to_csv(df, LOG_PATH + file_name +'.csv', encoding='utf-8') # Save log
+        if save: pd.DataFrame.to_csv(df, LOG_PATH+file_name+'.csv', encoding='utf-8') # Save log
 
     # Ouput
     if isinstance(data, tuple):
         for df in data: # plot and save forecasting result
             try: file_name = name + df.name.replace('-','_').replace(' ','_') # Check df Name
             except: df.name, file_name = 'output', name+'output'
             default_output(df, file_name)
     elif isinstance(data, pd.DataFrame):
         try: file_name = name + data.name.replace('-','_').replace(' ','_') # Check data Name
         except: data.name, file_name = 'output', name+'output'
         if 'decom' in data.name: # plot and save plot EMD result
             if plot:
-                data.plot(figsize=(6,1*data.columns.size), subplots=True)
+                data.plot(figsize=(7,1*data.columns.size), subplots=True)
                 plt.gcf().suptitle(data.name, fontsize=12, y=0.9) # Enlarge and Move the title     
                 if save: plt.savefig(FIG_PATH + file_name +'.jpg', dpi=300, bbox_inches='tight') # Save figure
                 plt.show()
             if save: pd.DataFrame.to_csv(data, LOG_PATH + file_name +'.csv', encoding='utf-8') # Save log
         else:
             try: default_output(data, file_name)
             except: print('Data is:\n', data)
     else:
         try: series = pd.Series(data)
         except: raise ValueError('Sorry! %s is not supported to plot and save, please input pd.DataFrame, pd.Series, nd.array(<=2D)'%type(data))
-        default_output(series)
+        default_output(series, file_name)
     if PATH is not None and save: print('The figures and logs of forecasting results have been saved into', PATH)
 
 
 
 # Run the qucik forecasting
 def quick_keras_predict(data=None, **kwargs):
     """
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/data_preprocessor.py` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/data_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,76 +239,108 @@
     try: df_decom = pd.DataFrame(df_decom)
     except: raise ValueError('Invalid input of df_decom!')
     if 'target' in df_decom.columns: 
         tmp_target = df_decom['target']
         df_decom = df_decom.drop('target', axis=1, inplace=False)
     else: tmp_target = None
 
-    if df_decom.columns.size > num_clusters:
-        df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
-
-        # Check inte_list
-        if inte_list is not None:
-            if str(inte_list).lower() == 'auto': # Without 
-                df_sampen = inte_sampen(df_decom)
-                inte_list = inte_kmeans(df_sampen, num_clusters)
-            elif isinstance(inte_list, pd.DataFrame):
-                if len(inte_list) == 1: inte_list = inte_list.T
-            elif type(inte_list) == str and len(inte_list) < df_decom.columns.size:
-                df_list, n, c, s = {}, 0, 0, 0
-                for i in inte_list: s = s + int(i) 
-                if s != df_decom.columns.size: raise ValueError('Invalid inte_list! %s (%s columns) does not match the number of dataset columns=%s.'%(inte_list, s, df_decom.columns.size)) 
-                for i in inte_list:
-                    for j in ['imf'+str(x) for x in range(n, n+int(i))]: 
-                        df_list[j], n = c, n + 1
-                    c += 1
-                inte_list = pd.DataFrame(df_list, index=['Cluster']).T
-            elif type(inte_list) == str and len(inte_list) == df_decom.columns.size:
-                inte_list = pd.DataFrame([int(x) for x in inte_list], columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
-            elif type(inte_list) == int and inte_list < df_decom.columns.size:
-                print('Integrate %d columns to be %d columns by K-means.'%(df_decom.columns.size, inte_list))
-                df_sampen = inte_sampen(df_decom)
-                inte_list = inte_kmeans(df_sampen, inte_list)
-            else:
-                try: inte_list = pd.DataFrame(inte_list, columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
-                except: raise ValueError('Invalid inte_list of %s with type %s. Check your input or length.'%(inte_list, type(inte_list)))
-
-            # Integrate, name, and resort
-            df_tmp = pd.DataFrame()
-            for i in range(inte_list.values.max()+1):
-                df_tmp['imf'+str(i)] = df_decom[inte_list[(inte_list['Cluster']==i)].index].sum(axis=1)
-                df_tmp_list = pd.DataFrame(df_tmp['imf'+str(i)])
-                df_tmp_list.columns = ['target']
-                df_inte_list.append(pd.concat((df_tmp_list, df_decom[inte_list[(inte_list['Cluster']==i)].index]), axis=1))
-            df_inte = df_tmp.T # Use Sample Entropy sorting the Co-IMFs
-            df_inte['sampen'] = inte_sampen(df_tmp).values
-            df_inte.sort_values(by=['sampen'], ascending=False, inplace=True)
-            df_inte.index = ['co-imf'+str(i) for i in range(inte_list.values.max()+1)]
-            df_inte = df_inte.drop('sampen', axis=1, inplace=False).T
-
-            # Rename df_inte_list
-            for i in range(len(df_inte.columns)):
-                for j in range(len(df_inte.columns)):
-                    try:
-                        if df_inte_list[i]['target'].sum() == df_inte['co-imf'+str(j)].sum():
-                            df_inte_list[i].columns = ['co-imf'+str(j)] + list(df_inte_list[i].columns)[1:]
-                    except: break
-
-            # Output
-            df_inte.name = 'df_inte_list_is_'+''.join(str(x) for x in inte_list.values.ravel()) # record integrate list
-            df_inte.index = df_decom.index
-        else: df_inte = df_decom
+    # Convert inte_list
+    if inte_list is not None:
+        if str(inte_list).lower() == 'auto': # Without 
+            inte_list = inte_kmeans(df_decom, num_clusters=num_clusters)
+        elif isinstance(inte_list, pd.DataFrame):
+            if len(inte_list) == 1: inte_list = inte_list.T
+        elif type(inte_list) == str and len(inte_list) < df_decom.columns.size:
+            df_list, n, c, s = {}, 0, 0, 0
+            for i in inte_list: s = s + int(i) 
+            if s != df_decom.columns.size: raise ValueError('Invalid inte_list! %s (%s columns) does not match the number of dataset columns=%s.'%(inte_list, s, df_decom.columns.size)) 
+            for i in inte_list:
+                for j in ['imf'+str(x) for x in range(n, n+int(i))]: 
+                    df_list[j], n = c, n + 1
+                c += 1
+            inte_list = pd.DataFrame(df_list, index=['Cluster']).T
+        elif type(inte_list) == str and len(inte_list) == df_decom.columns.size:
+            inte_list = pd.DataFrame([int(x) for x in inte_list], columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
+        elif type(inte_list) == int and inte_list < df_decom.columns.size:
+            print('Integrate %d columns to be %d columns by K-means.'%(df_decom.columns.size, inte_list))
+            inte_list = inte_kmeans(df_decom, num_clusters=inte_list)
+        else:
+            try: inte_list = pd.DataFrame(inte_list, columns=['Cluster'], index=['imf'+str(x) for x in range(len(inte_list))])
+            except: raise ValueError('Invalid inte_list of %s with type %s. Check your input or length.'%(inte_list, type(inte_list)))
+
+    # Integrate, resort, and output
+    if inte_list is not None: # Check inte_list after Convert
+        # Integrate
+        df_inte = pd.DataFrame()
+        for i in range(inte_list.values.max()+1):
+            df_inte['co-imf'+str(i)] = df_decom[inte_list[(inte_list['Cluster']==i)].index].sum(axis=1)
+            df_tmp = pd.concat((df_inte['co-imf'+str(i)], df_decom[inte_list[(inte_list['Cluster']==i)].index]), axis=1)
+            df_tmp.name = 'co-imf'+str(i)
+            df_inte_list.append(df_tmp)
+
+        # Use Sample Entropy resorting the Co-IMFs
+        df_tmp = df_inte.T
+        df_tmp['sampen'] = inte_sampen(df_tmp.T).values
+        df_tmp.sort_values(by=['sampen'], ascending=False, inplace=True)
+        df_tmp['related'] = [x for x in range(len(df_tmp))]
+        df_related = pd.DataFrame(df_tmp['related']).T
+        for df in df_inte_list: # rename df_inte_list
+            imf_name = 'co-imf'+str(df_related[df.name]['related'])
+            df.rename(columns={df.name:imf_name}, inplace=True)
+            df.name = imf_name
+        df_inte_list.sort(key=lambda x: x.name)
+        df_tmp.index = ['co-imf'+str(i) for i in range(len(df_tmp))]
+        df_inte = df_tmp.drop(['related', 'sampen'], axis=1, inplace=False).T
+
+        # output
+        df_inte.name = 'df_inte_list_'+''.join(str(x) for x in inte_list.values.ravel()) # record integrate list
+        df_inte.index = df_decom.index
     else: 
         df_decom.columns = ['co-imf'+str(i) for i in range(df_decom.columns.size)] # less than num_clusters, stop inte and output
         df_inte = df_decom
-    if tmp_target is not None: df_inte['target'] = tmp_target # add tmp target column
+        for col in df_inte.columns: 
+            df_tmp = pd.DataFrame(df_inte[col])
+            df_tmp.name = col
+            df_inte_list.append(df_tmp)
+    if tmp_target is not None: df_inte.insert(0, 'target', tmp_target.values) # add tmp target column
     return df_inte, df_inte_list
     
+# 2.1 K-Means
+def inte_kmeans(df_decom=None, num_clusters=3, random_state=0, **kwargs):
+    """
+    Get integrating form by K-Means by sklearn.cluster.
+    Example: inte_list = cl.inte_kmeans(df_sampen)
+    Print: print(inte_list)
+
+    Input and Parameters:
+    ---------------------
+    df_decom     - the decomposing results in pd.Dataframe, or a group of series
+    df_sampen    - the Sample Entropy of each time series in pd.Dataframe, or an one-column Dataframe with specific index
+    num_clusters - number of categories/clusters eg. num_clusters = 3
+    random_state - control the random state to guarantee the same result every time
+    **kwargs     - any parameters of sklearn.cluster.KMeans()
+
+    Output:
+    ---------------------
+    inte_list    - the integrating form of each time series in pd.Dataframe
+    """
+
+    # Get integrating form by K-Means
+    try: from sklearn.cluster import KMeans
+    except ImportError: raise ImportError('Cannot import sklearn, run: pip install sklearn!')
+    if df_decom.columns.size > num_clusters:
+        df_sampen = inte_sampen(df_decom)
+        try: df_sampen = pd.DataFrame(df_sampen)
+        except: raise ValueError('Invalid input of df_sampen!')
+        np_inte_list = KMeans(n_clusters=num_clusters, random_state=random_state, **kwargs).fit_predict(df_sampen)
+        inte_list = pd.DataFrame(np_inte_list, index=['imf'+str(i) for i in range(df_sampen.index.size)], columns=['Cluster'])
+    else: inte_list = None
+    return inte_list
 
-# 2.1 Sample Entropy
+# 2.2 Sample Entropy
 def inte_sampen(df_decom=None, max_len=1, tol=0.1, nor=True, **kwargs):
     """
     Calculate Sample Entropy for each IMF or series by sampen.sampen2.
     Example: df_sampen = cl.inte_sampen(df_decom)
     Plot by pandas: df_sampen.plot(title='Sample Entropy')
 
     Input and Parameters:
@@ -322,53 +354,26 @@
     Output:
     ---------------------
     df_sampen  - the Sample Entropy of each time series in pd.Dataframe
     """
     try: 
         df_decom = pd.DataFrame(df_decom)
         if 'target' in df_decom.columns: df_decom = df_decom.drop('target', axis=1, inplace=False)
-        if 'imf0' not in df_decom.columns: df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
+        if 'imf0' not in df_decom.columns or 'co-imf0' not in df_decom.columns: 
+            df_decom.columns = ['imf'+str(i) for i in range(df_decom.columns.size)]
     except: raise ValueError('Invalid input of df_decom!') 
     try: import sampen
     except ImportError: raise ImportError('Cannot import sampen, run: pip install sampen!')
     np_sampen = []
     for i in range(df_decom.columns.size):
         sample_entropy = sampen.sampen2(list(df_decom['imf'+str(i)].values), mm=max_len, r=tol, normalize=nor, **kwargs)
         np_sampen.append(sample_entropy[1][1])
     df_sampen = pd.DataFrame(np_sampen, index=['imf'+str(i) for i in range(df_decom.columns.size)])
     return df_sampen
 
-# 2.2 K-Means
-def inte_kmeans(df_sampen=None, num_clusters=3, random_state=0, **kwargs):
-    """
-    Get integrating form by K-Means by sklearn.cluster.
-    Example: inte_list = cl.inte_kmeans(df_sampen)
-    Print: print(inte_list)
-
-    Input and Parameters:
-    ---------------------
-    df_sampen    - the Sample Entropy of each time series in pd.Dataframe, or an one-column Dataframe with specific index
-    num_clusters - number of categories/clusters eg. num_clusters = 3
-    random_state - control the random state to guarantee the same result every time
-    **kwargs     - any parameters of sklearn.cluster.KMeans()
-
-    Output:
-    ---------------------
-    inte_list    - the integrating form of each time series in pd.Dataframe
-    """
-
-    # Get integrating form by K-Means
-    try: from sklearn.cluster import KMeans
-    except ImportError: raise ImportError('Cannot import sklearn, run: pip install sklearn!')
-    try: df_sampen = pd.DataFrame(df_sampen)
-    except: raise ValueError('Invalid input of df_sampen!')
-    np_inte_list = KMeans(n_clusters=num_clusters, random_state=random_state, **kwargs).fit_predict(df_sampen)
-    inte_list = pd.DataFrame(np_inte_list, index=['imf'+str(i) for i in range(df_sampen.index.size)], columns=['Cluster'])
-    return inte_list
-
 
 
 # 3.Other Mains
 # ------------------------------------------------------
 # 3.Main. Redecompose (inculd decom() and inte())
 def redecom(data=None, show=False, decom_mode='ceemdan', inte_list='auto', redecom_list={'co-imf0':'ovmd'}, vmd_params=None, FORECAST_LENGTH=None, **kwargs):
     """
@@ -397,39 +402,43 @@
     if vmd_params is not None and type(vmd_params) != dict: raise ValueError('Invalid input of vmd_params!') 
     if len(data.columns) == 1: 
         df_decom = decom(data[data.columns[0]], decom_mode=decom_mode, FORECAST_LENGTH=FORECAST_LENGTH)
     else: df_decom = data # pd.DataFrame
     df_inte, df_inte_list = inte(df_decom, inte_list=inte_list)
 
     # Re-decompose 
-    df_redecom_list, best_params_dict, inte_columns = [], {}, str(df_inte.columns.to_list())
+    best_params_dict, inte_columns = {}, str(df_inte.columns.to_list())
     if redecom_list is not None:
         try: redecom_list = pd.DataFrame(redecom_list, index=range(1))
         except: raise ValueError("Invalid input for redecom_list! Please input eg. None, '{'co-imf0':'vmd', 'co-imf1':'emd'}'.")
         for i in redecom_list.columns:
             try: df_inte[i]
             except: raise ValueError('Invalid input for redecom_list! Please check your key value of column name.')
-            if vmd_params is None: df_redecom = decom(df_inte[i], decom_mode=redecom_list[i][0], FORECAST_LENGTH=FORECAST_LENGTH, **kwargs)
+            if vmd_params is None: df_imf_decom = decom(df_inte[i], decom_mode=redecom_list[i][0], FORECAST_LENGTH=FORECAST_LENGTH, **kwargs)
             else: 
                 print('Get vmd_params:', vmd_params)
-                df_redecom = decom(df_inte[i], decom_mode=redecom_list[i][0], vmd_params=vmd_params[i], FORECAST_LENGTH=FORECAST_LENGTH, **kwargs)
-            best_params_dict[i] = eval(df_redecom.name.split('_')[1])
-            df_redecom = df_redecom.drop('target', axis=1, inplace=False)
-            df_redecom.columns = [i+'-'+redecom_list[i][0].lower()+str(x) for x in range(df_redecom.columns.size)]# rename
-            for x in df_redecom.columns[::-1]: df_inte.insert(int(i[-1]), x, df_redecom[x].values)
-            df_redecom['target'] = df_inte[i] # record each imf redecompose result and itself as target
-            df_redecom.name = i
-            df_redecom_list.append(df_redecom) 
-            df_inte = df_inte.drop(i, axis=1, inplace=False)
-        df_inte.name = inte_columns+'_'+str(best_params_dict) # record redecomposition parameters
-    else: df_inte.name = 'None'
+                df_imf_decom = decom(df_inte[i], decom_mode=redecom_list[i][0], vmd_params=vmd_params[i], FORECAST_LENGTH=FORECAST_LENGTH, **kwargs)
+            best_params_dict[i] = eval(df_imf_decom.name.split('_')[1]) # get best_params_dict
+            df_imf_decom = df_imf_decom.drop('target', axis=1, inplace=False)
+            df_imf_decom.columns = [i+'-'+redecom_list[i][0].lower()+str(x) for x in range(df_imf_decom.columns.size)] # rename
+            df_imf_decom.insert(0, i, df_inte[i].values)
+            df_imf_decom.name = 'redecom_'+i
+            for j in range(len(df_inte_list)):
+                if df_inte_list[j].name == i: df_inte_list[j] = df_imf_decom # record each redecomposition result
+        df_redecom = df_inte['target']
+        for df in df_inte_list: df_redecom = pd.concat((df_redecom, df.iloc[:,1:]),axis=1)
+        df_redecom.name = inte_columns+'_'+str(best_params_dict) # record redecomposition parameters
+    else: df_redecom = df_inte
+        
     if show:
         print('\nPart of preprocessing dataset (inculde training and test set):')
-        print(df_inte)
-    return df_inte, df_redecom_list
+        print(df_redecom)
+    return df_redecom, df_inte_list
+
+
 
 # 3.Main. Evaluate
 def eval_result(y_real, y_pred): 
     """
     Evaluate forecasting result by sklearn.metrics, eg.'R2', 'RMSE', 'MAE', 'MAPE'.
     Example: df_eval = cl.eval_result(y_real, y_pred)
     Print: print(df_eval)
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/beijing_ets.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/beijing_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ftse.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/ftse.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/guangzhou_ets.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/guangzhou_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hsi.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/hsi.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/hubei_ets.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/hubei_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/n225.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/n225.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/nasdaq.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/nasdaq.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sp500.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/sp500.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/sse_index.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/sse_index.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/ssec.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/ssec.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/datasets/tianjin_ets.csv` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/datasets/tianjin_ets.csv`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/keras_predictor.py` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/keras_predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         tf.config.experimental_connect_to_cluster(tpu)
         tf.tpu.experimental.initialize_tpu_system(tpu)
         strategy = tf.distribute.TPUStrategy(tpu)
         with strategy.scope(): # Change Keras model to TPU form
             model = self.build_model(shape, model_name, model_file) # Build the model # Use model.summary() to show the model structure
         return model
 
-    # 1.Main Forecast by Keras
+    # 1.3 Main Forecast by Keras
     def keras_predict(self, data=None, show_model=False, fitting_set=None, **kwargs): # GRU forecasting function
         """
         Forecast by Keras
         
         Input and Parameters:
         ---------------------
         data               - data set (include training set and test set)
@@ -276,27 +276,27 @@
         """
 
         # Initialize
         from CEEMDAN_LSTM.data_preprocessor import create_train_test_set
         x_train, x_test, y_train, y_test, scalarY, next_x = create_train_test_set(data, self.FORECAST_LENGTH, self.FORECAST_HORIZONS, self.NEXT_DAY, self.NOR_METHOD, self.DAY_AHEAD, fitting_set) 
 
         # Convert to tensor = tf.constant()
-        today_x = x_train[-1].reshape(1, x_train.shape[1], x_train.shape[2]) # aviod resahpe tf.constant - tensor
+        today_x = x_train[-1].reshape(1, x_train.shape[1], x_train.shape[2]) # aviod resahpe tf.constant -> tensor
         x_train = constant(x_train) # x_train = x_train.reshape((x_train.shape[0], x_train.shape[1], x_train.shape[2])) 
         if not self.NEXT_DAY: x_test = constant(x_test) # x_test = x_test.reshape((x_test.shape[0], x_test.shape[1], x_test.shape[2])) 
         
         # Set callbacks
         Reduce = ReduceLROnPlateau(monitor=self.callbacks_monitor, patience=self.opt_patience, verbose=self.verbose, mode='auto') # Adaptive learning rate
         EarlyStop = EarlyStopping(monitor=self.callbacks_monitor, patience=self.stop_patience, verbose=self.verbose, mode='auto') # Early stop at small learning rate 
         callbacks_list = [Reduce, EarlyStop]
 
         # Name model
         try: 
             data.name = data.name.replace('-','_').replace(' ','_')
-            if '.h5' not in str(data.name): data.name = data.name + '.h5'
+            if '.h5' not in str(data.name): data.name = data.name+'.h5'
         except: data.name = 'Keras_model.h5'
         
         # Load and save model
         model_file = None
         if self.PATH is not None:
             # Load model if get input of self.KERAS_MODEL
             if isinstance(self.KERAS_MODEL, dict): self.KERAS_MODEL = pd.DataFrame(self.KERAS_MODEL, index=[0])
@@ -336,21 +336,21 @@
 
         # Get results and evaluate
         from CEEMDAN_LSTM.data_preprocessor import eval_result
         df_loss = pd.DataFrame({'loss': history.history['loss'], 'val_loss': history.history['val_loss']}, index=range(len(history.history['val_loss'])))
         if not self.NEXT_DAY:
             # Get general results and evaluate
             y_predict = model(x_test) # Predict # replace y_predict = model.predict(x_test) to aviod warning
-            df_eval = eval_result(y_test, y_predict) # Evaluate model
             y_predict = np.array(y_predict).ravel().reshape(-1,1) 
             if scalarY is not None: 
                 y_test = scalarY.inverse_transform(y_test)
                 y_predict = scalarY.inverse_transform(y_predict) # De-normalize 
             if self.TARGET is not None: result_index = self.TARGET.index[-self.FORECAST_LENGTH:] # Forecasting result idnex
             else: result_index = range(len(y_test.ravel()))
+            df_eval = eval_result(y_test, y_predict) # Evaluate model
             df_result = pd.DataFrame({'real': y_test.ravel(), 'predict': y_predict.ravel()}, index=result_index) # Output
             return df_result, df_eval, df_loss
         else:
             # Get next day's results
             today_y = np.array(model(today_x))
             next_y = np.array(model(next_x.reshape(1, today_x.shape[1], today_x.shape[2])))
             if scalarY is not None: # De-normalize 
@@ -363,15 +363,15 @@
             df_result = pd.DataFrame({'today_real': today_real.ravel()[0], 'today_pred': today_y.ravel()[0], 'next_pred': next_y.ravel()[0]}, index=next_index) # Output
             return df_result
 
 
 
     # 2.Advanced forecasting functions
     # ------------------------------------------------------
-    # 2.1. Single Method (directly forecast)
+    # 2.1 Single Method (directly forecast)
     def single_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
         """
         Single Method (directly forecast)
         Use Keras model to directly forecast with vector input
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.single_keras_predict(data, show=True, plot=True, save=True)
@@ -394,30 +394,30 @@
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name and set 
         now = datetime.now()
         predictor_name = name_predictor(now, 'Single', 'Keras', self.KERAS_MODEL, None, None, self.NEXT_DAY)
         data = check_dataset(data, show, self.DECOM_MODE, None)
-        data.name = (predictor_name+'_model.h5').replace('-','_').replace(' ','_')
-        self.TARGET = data['target']
+        data.name = (predictor_name+' model.h5')
+        if self.TARGET is None: self.TARGET = data['target']
 
         # Forecast
         start = time.time()
         df_result = self.keras_predict(data=data, show_model=show, **kwargs)
         end = time.time()
 
         # Output
-        df_result = output_result(df_result, predictor_name, end-start)
+        df_result = output_result(df_result, predictor_name, end-start, imf='Final', next_day=self.NEXT_DAY) # (df_result, df_eval, df_loss) for keras_predict()
         plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
         return df_result
 
 
 
-    # 2.2. Ensemble Method (decompose then directly forecast)
+    # 2.2 Ensemble Method (decompose then directly forecast)
     def ensemble_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
         """
         Ensemble Method (decompose then directly forecast)
         Use decomposition-integration Keras model to directly forecast with matrix input
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.ensemble_keras_predict(data, show=True, plot=True, save=True)
@@ -444,29 +444,29 @@
         now = datetime.now()
         predictor_name = name_predictor(now, 'Ensemble', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
-        df_redecom.name = (predictor_name+'_model.h5').replace('-','_').replace(' ','_') # model name input to self.keras_predict
-        self.TARGET = df_redecom['target']
+        df_redecom.name = predictor_name+'_model.h5' # model name input to self.keras_predict
+        if self.TARGET is None: self.TARGET = df_redecom['target']
 
         # Forecast
         df_result = self.keras_predict(data=df_redecom, show_model=show, **kwargs)
         end = time.time()
 
         # Output
-        df_result = output_result(df_result, predictor_name, end-start)
+        df_result = output_result(df_result, predictor_name, end-start, imf='Final', next_day=self.NEXT_DAY) # return (df_result, df_eval, df_loss)
         plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
         return df_result
 
 
     
-    # 2.3. Respective Method (decompose then respectively forecast each IMFs)
+    # 2.3 Respective Method (decompose then respectively forecast each IMFs)
     def respective_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
         """
         Respective Method (decompose then respectively forecast each IMFs)
         Use decomposition-integration Keras model to respectively forecast each IMFs with vector input
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.respective_keras_predict(data, show=True, plot=True, save=True)
@@ -493,59 +493,51 @@
         now = datetime.now()
         predictor_name = name_predictor(now, 'Respective', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
-        self.TARGET = df_redecom['target']
-        # set target and model
-        try: 
-            if 'Keras_Forecasting' in data.name: predictor_name = data.name
-            else: data.name, self.TARGET = '', df_redecom['target']
-        except: data.name, self.TARGET = '', df_redecom['target']
+        if self.TARGET is None: self.TARGET = df_redecom['target']
 
         # Forecast and ouput each Co-IMF
         df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
         df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'IMF']) # df for storing Next-day forecasting result
         for imf in df_redecom.columns.difference(['target']):
-            df_redecom[imf].name = (predictor_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_')
+            df_redecom[imf].name = predictor_name+'_of_'+imf+'_model.h5'
             time1 = time.time()
             df_result = self.keras_predict(data=df_redecom[imf], show_model=show, **kwargs)
             time2 = time.time()
-            df_result = output_result(df_result, predictor_name, time2-time1, imf)
+            df_result = output_result(df_result, predictor_name, time2-time1, imf, next_day=self.NEXT_DAY) # return (imf_pred, imf_eval, imf_loss)
             if not self.NEXT_DAY:
-                df_pred_result[imf+'-real'] = df_result[0]['real'] # add real values
-                df_pred_result[imf+'-predict'] = df_result[0]['predict'] # add forecasting result
+                df_pred_result = pd.concat((df_pred_result, df_result[0]), axis=1) # add forecasting result
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
                 plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
             else: df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
             print('')
         end = time.time()
 
         # Final Output
-        # Final Output
         if not self.NEXT_DAY: 
-            df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
+            df_pred_result['real'] = df_redecom['target'][-self.FORECAST_LENGTH:]
             df_pred_result['predict'] = df_pred_result[[x for x in df_pred_result.columns if 'predict' in x]].sum(axis=1)
-            df_result = output_result((df_pred_result,df_eval_result), predictor_name, end-start, imf='Final', type='Evaluation')
-            plot_save_result(df_result[2], name=now, plot=plot, save=save, path=self.PATH) # only plot result
-            df_result = (df_result[0], df_result[1])
+            df_result = (df_pred_result, df_eval_result)
         else:
-            df_result = pd.DataFrame({'today_real': self.TARGET.values[-1], 'today_pred': df_next_result['today_pred'].sum(), 
-                                      'next_pred': df_next_result['next_pred'].sum()}, index=[df_next_result.index[0]]) # Output
-            df_result = output_result((df_result, df_next_result), predictor_name, end-start, imf='Final', type='Result')
-        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH) # save result 
-        return df_result
+            df_result = pd.DataFrame({'today_real': df_redecom['target'][-1:], 'today_pred': df_next_result['today_pred'].sum(), 
+                                      'next_pred': df_next_result['next_pred'].sum()}) # Output
+            df_result = (df_result, df_next_result)
+        df_result = output_result(df_result, predictor_name, end-start, imf='Final', next_day=self.NEXT_DAY)
+        plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
+        return df_result 
 
 
 
-    # 2.4. Hybrid Method (decompose then forecast high-frequency IMF by ensemble method and forecast other by respective method)
-    def hybrid_keras_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
+    # 2.4 Hybrid Method (decompose then forecast high-frequency IMF by ensemble method and forecast other by respective method)
+    def hybrid_keras_predict(self, data=None, show=False, plot=False, save=False, method='respective', **kwargs):
         """
         Hybrid Method (decompose then forecast high-frequency IMF by ensemble method and forecast others by respective method)
         Use the ensemble method to forecast high-frequency IMF and the respective method for other IMFs.
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.hybrid_keras_predict(data, show=True, plot=True, save=True)
 
@@ -566,111 +558,107 @@
         df_train_loss   - training loss log
         next_y          - forecasting result of the next day when NEXT_DAY=Ture
         """
 
         # Name
         now = datetime.now()
         predictor_name = name_predictor(now, 'Hybrid', 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
+        if method != 'ensemble' and method != 'respective': raise ValueError("Please input a vaild predict method! eg. 'ensemble', 'respective'.")
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
-        df_rest_columns, df_rest_list = [], []
-        for x in df_redecom_list: # create df_rest_list
-            df_redecom[x.name] = x['target']
-            df_rest_columns.append(x.name)
-            df_redecom = df_redecom[df_redecom.columns.difference(x.columns.difference(['target']))]
-        for x in df_redecom.columns.difference(df_rest_columns): 
-            if x != 'target': df_rest_list.append(df_redecom[x])
-        self.TARGET = df_redecom['target']
+        if self.TARGET is None: self.TARGET = df_redecom['target']
 
         # Forecast
         df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
         df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'IMF']) # df for storing Next-day forecasting result
-        for df in df_redecom_list+df_rest_list: # both ensemble (matrix-input) and respective (vector-input) method 
+        for df in df_redecom_list: # both ensemble (matrix-input) and respective (vector-input) method 
             imf = df.name
-            df.name = (predictor_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_') # Save model
+            if 'redecom' not in imf:
+                if method=='respective': df = pd.DataFrame(df[imf]) # if method=='ensemble': df = df
+            else: imf = imf[8:]
+            df.rename(columns={imf: 'target'}, inplace=True)
+            df.name = predictor_name+'_of_'+imf+'_model.h5' # Save model
             time1 = time.time()
             df_result = self.keras_predict(data=df, show_model=show, **kwargs) # the ensemble method with matrix input 
             time2 = time.time()
-            df_result = output_result(df_result, predictor_name, time2-time1, imf)
-            if not self.NEXT_DAY: 
-                df_pred_result[imf+'-real'] = df_result[0]['real'] # add real values
-                df_pred_result[imf+'-predict'] = df_result[0]['predict'] # add forecasting result
+            df_result = output_result(df_result, predictor_name, time2-time1, imf, next_day=self.NEXT_DAY) # return (imf_pred, imf_eval, imf_loss)
+            if not self.NEXT_DAY:
+                df_pred_result = pd.concat((df_pred_result, df_result[0]), axis=1) # add forecasting result
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
                 plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
             else: df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
             print('')
 
         # Fitting 
         if not self.NEXT_DAY: 
+            df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
             if self.FIT_METHOD == 'ensemble': # fitting method
                 print('Fitting of the ensemble method is running...')        
                 fitting_set = df_pred_result[[x for x in df_pred_result.columns if '-predict' in x]]
-                df_redecom.name = (predictor_name+'_of_Fitting_model.h5').replace('-','_').replace(' ','_') # Save model
+                df_redecom.name = predictor_name+'_of_Fitting_model.h5' # Save model
                 time1 = time.time()
                 df_result = self.keras_predict(data=df_redecom, show_model=show, fitting_set=fitting_set, **kwargs) # the ensemble method with matrix input 
                 time2 = time.time()
-                df_result = output_result(df_result, predictor_name, time2-time1, 'fitting')
-                df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
-                df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
+                df_result = output_result(df_result, predictor_name, time2-time1, imf='fitting', next_day=self.NEXT_DAY)
+                df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result of fitting
                 df_pred_result['add-predict'] = df_pred_result[[x for x in df_pred_result.columns if '-predict' in x]].sum(axis=1) # add all imf predict result
-                df_pred_result['predict'] = df_result[0]['predict']
+                df_pred_result['predict'] = df_result[0]['fitting-predict']
                 plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
             else: # adding method
-                df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
                 df_pred_result['predict'] = df_pred_result[[x for x in df_pred_result.columns if '-predict' in x]].sum(axis=1) # add all imf predict result
         else: # if self.NEXT_DAY:
             if self.FIT_METHOD == 'ensemble': # fitting method
                 print('Fitting of the ensemble method is running...')        
                 fitting_set = df_redecom[df_redecom.columns.difference(['target'])][-self.FORECAST_LENGTH+1:]
                 fitting_set_next_index = fitting_set.index[-1]+(fitting_set.index[-1]-fitting_set.index[-2])
                 fitting_set.loc[fitting_set_next_index] = [x for x in range(fitting_set.columns.size)] # create blank row
                 for i in range(df_next_result.index.size): # add next_pred of each imf to fitting_set
                     point_row = df_next_result[i:i+1]
                     fitting_set[point_row['IMF'][0]][fitting_set_next_index] = point_row['next_pred'][0]
-                df_redecom.name = (predictor_name+'_of_Fitting_model.h5').replace('-','_').replace(' ','_') # Save model
+                df_redecom.name = predictor_name+'_of_Fitting_model.h5' # Save model
                 time1 = time.time()
                 df_result = self.keras_predict(data=df_redecom, show_model=show, fitting_set=fitting_set, **kwargs) # the ensemble method with matrix input 
                 time2 = time.time()
-                df_result = output_result(df_result, predictor_name, time2-time1, imf='fitting')
+                df_result = output_result(df_result, predictor_name, time2-time1, imf='fitting', next_day=self.NEXT_DAY)
                 df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
                 today_result = df_result['today_pred']
                 next_reuslt = df_result['next_pred']
             else: # adding method
                 today_result = df_next_result['today_pred'].sum()
                 next_reuslt = df_next_result['next_pred'].sum() # adding method
         end = time.time()
 
         # Final Output
-        if not self.NEXT_DAY: 
-            df_result = output_result((df_pred_result,df_eval_result), predictor_name, end-start, imf='Final', type='Evaluation')
-            plot_save_result(df_result[2], name=now, plot=plot, save=save, path=self.PATH) # only plot result 
-            df_result = (df_result[0], df_result[1])
+        if not self.NEXT_DAY: df_result = (df_pred_result, df_eval_result)
         else:
-            df_result = pd.DataFrame({'today_real': self.TARGET.values[-1], 'today_pred': today_result, 'next_pred': next_reuslt}, index=[df_next_result.index[0]]) # Output
-            df_result = output_result((df_result, df_next_result), predictor_name, end-start, imf='Final', type='Result')
-        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH) # save result 
-        return df_result
+            df_result = pd.DataFrame({'today_real': df_redecom['target'][-1:], 'today_pred': today_result, 'next_pred': next_reuslt}) # Output                
+            df_result = (df_result, df_next_result)
+        df_result = output_result(df_result, predictor_name, end-start, imf='Final', next_day=self.NEXT_DAY)
+        plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
+        return df_result 
+
+
 
     # A class used to hide the print
     class HiddenPrints: 
         """
         A class used to hide the print
         """
         def __enter__(self):
             self._original_stdout = sys.stdout
             sys.stdout = open(os.devnull, 'w')
         def __exit__(self, exc_type, exc_val, exc_tb):
             sys.stdout.close()
             sys.stdout = self._original_stdout
 
-    # 2.5. Multiple Run Predictor
+    # 2.5 Multiple Run Predictor
     def multiple_keras_predict(self, data=None, run_times=10, predict_method=None, **kwargs):
         """
         Multiple Run Predictor, multiple run of above method
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.multiple_keras_predict(data, run_times=10, predict_method='single')
 
@@ -690,52 +678,58 @@
         ---------------------
         df_eval_result     - evaluating forecasting results of each run
         """
 
         # Initialize 
         now = datetime.now()
         data = check_dataset(data, False, self.DECOM_MODE, self.REDECOM_LIST)
-        self.TARGET = data['target']
+        if self.TARGET is None: self.TARGET = data['target']
         
         if self.PATH is None: print('Do not set a PATH! It is recommended to set a PATH to prevent the loss of running results')
         if predict_method is None: raise ValueError("Please input a predict method! eg. 'single', 'ensemble', 'respective', 'hybrid'.")
         else: predict_method = predict_method.capitalize()
         if predict_method == 'Single': predictor_name = name_predictor(now, 'Multiple Single', 'Keras', self.KERAS_MODEL, None, None, self.NEXT_DAY)
         else: predictor_name = name_predictor(now, 'Multiple '+predict_method, 'Keras', self.KERAS_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)    
 
         # Forecast
         start = time.time()
         df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
-        df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
+        df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'IMF']) # df for storing Next-day forecasting result
         for i in range(run_times):
             print('Run %d is running...'%i, end='')
             time1 = time.time()
             with self.HiddenPrints():
                 if predict_method == 'Single': df_result = self.single_keras_predict(data=data, **kwargs)
-                if predict_method == 'Ensemble': df_result = self.ensemble_keras_predict(data=data, **kwargs) 
-                if predict_method == 'Respective': df_result = self.respective_keras_predict(data=data, **kwargs)
-                if predict_method == 'Hybrid': df_result = self.hybrid_keras_predict(data=data, **kwargs)
-                df_result[1]['IMF'] = predict_method + '-Run' + str(i)
-                df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
-                df_pred_result['Run'+str(i)+'-predict'] = df_result[0]['predict']
-                df_result = (df_pred_result, df_eval_result)
-                df_pred_result.name, df_eval_result.name = predictor_name+' Result', predictor_name+' Evaluation'
-                plot_save_result(df_result, name=now, plot=False, save=True, path=self.PATH)
-            time2 = time.time()
+                elif predict_method == 'Ensemble': df_result = self.ensemble_keras_predict(data=data, **kwargs) 
+                elif predict_method == 'Respective': df_result = self.respective_keras_predict(data=data, **kwargs)
+                elif predict_method == 'Hybrid': df_result = self.hybrid_keras_predict(data=data, **kwargs)
+                elif predict_method == 'Hybrid-ensemble': df_result = self.hybrid_keras_predict(data=data, method='ensemble', **kwargs)
+                else: raise ValueError("Please input a vaild predict method! eg. 'single', 'ensemble', 'respective', 'hybrid'.")
+                time2 = time.time()
+                df_result = output_result(df_result, predictor_name, time2-time1, imf='Final', run=i, next_day=self.NEXT_DAY)
+                if not self.NEXT_DAY:
+                    df_pred_result = pd.concat((df_pred_result, df_result[0]), axis=1) # add forecasting result
+                    df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
+                    df_pred_result.name, df_eval_result.name = predictor_name+' Result', predictor_name+' Evaluation'
+                    df_result = (df_pred_result, df_eval_result)
+                else: 
+                    df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
+                    df_next_result.name = predictor_name+' Result'
+                    df_result = df_next_result
+                plot_save_result(df_result, name=now, plot=False, save=True, path=self.PATH) # Temporary storage
             print('taking time: %.3fs'%(time2-time1))
         end = time.time()
         print('\n============='+predictor_name+' Finished=============')
         print('Running time: %.3fs'%(end-start))
-        plot_save_result(df_result, name=now, plot=False, save=True, path=self.PATH)
         return df_result
 
 
 
-    # 2.6.Rolling Method (forecast each value one by one)
+    # 2.6 Rolling Method (forecast each value one by one)
     def rolling_keras_predict(self, data=None, predict_method=None, transfer_learning=False, out_of_sample=False, **kwargs):
         """
         Rolling Method (forecast each value one by one to avoid lookahead bias)
         Rolling run of above method to avoid the look-ahead bias, but take a long long time
         Example: 
         kr = cl.keras_predictor(epochs=10, verbose=1)
         df_result = kr.rolling_keras_predict(data, predict_method='single', transfer_learning=True)
@@ -841,15 +835,15 @@
         print('\n============='+predictor_name+' Finished=============')
         print('Running time: %.3fs'%(end-start))
         from CEEMDAN_LSTM.data_preprocessor import eval_result
         df_pred_result = pd.DataFrame()
         df_pred_result['real'] = data[-self.FORECAST_LENGTH:]
         if predict_method == 'Single' or predict_method == 'Ensemble': df_pred_result['predict'] = df_next_result['next_pred'].values
         else: df_pred_result['predict'] = df_next_result.loc[df_next_result['IMF'] == 'Final']['next_pred'].values
-        df_eval_result = eval_result(df_pred_result['predict'], df_pred_result['real'])
+        df_eval_result = eval_result(df_pred_result['real'], df_pred_result['predict'])
         df_eval_result['Runtime'] = end-start # Output Runtime
         df_eval_result['Run'] = 'Final'
         print(df_eval_result)
         df_result = (df_pred_result, df_eval_result, df_next_result)
         df_pred_result.name, df_eval_result.name = predictor_name+' Result', predictor_name+' Evaluation'
         plot_save_result(df_result[:2], name=now, plot=True, save=True, path=self.PATH)
         return df_result
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM/sklearn_predictor.py` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM/sklearn_predictor.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,30 +20,29 @@
 # Import modules for sklearn_predictor
 import os
 import sys
 import time
 import numpy as np
 import pandas as pd
 from datetime import datetime
-import matplotlib.pyplot as plt
 import warnings
 warnings.filterwarnings("ignore") # Ignore some annoying warnings
 # CEEMDAN_LSTM
-from CEEMDAN_LSTM.core import check_dataset, check_path, plot_save_result, name_predictor
+from CEEMDAN_LSTM.core import check_dataset, check_path, plot_save_result, name_predictor, output_result
 # Sklearn
+# import joblib # load and save model 
 from sklearn.svm import SVR
 from sklearn.linear_model import Lasso
 from sklearn.model_selection import cross_val_score, GridSearchCV
-from sklearn.metrics import mean_squared_error, r2_score
 
 class sklearn_predictor:
     # 0.Initialize
     # ------------------------------------------------------
-    def __init__(self, PATH=None, FORECAST_HORIZONS=30, FORECAST_LENGTH=30, SKLEARN_MODEL='SVM', OPTIMIZER='Bayes',
-                 DECOM_MODE='VMD', INTE_LIST='auto', REDECOM_LIST=None, 
+    def __init__(self, PATH=None, FORECAST_HORIZONS=30, FORECAST_LENGTH=30, SKLEARN_MODEL='LASSO', OPTIMIZER='Bayes',
+                 DECOM_MODE='OVMD', INTE_LIST='auto', REDECOM_LIST=None, 
                  NEXT_DAY=False, DAY_AHEAD=1, NOR_METHOD='minmax', FIT_METHOD='add', **kwargs):
         """
         Initialize the sklearn_predictor.
         Configuration can be passed as kwargs (keyword arguments).
 
         Input and HyperParameters:
         ---------------------
@@ -56,14 +55,17 @@
         DECOM_MODE         - the decomposition method, eg.'EMD', 'VMD', 'CEEMDAN'
         INTE_LIST          - the integration list, eg. pd.Dataframe, (int) 3, (str) '233', (list) [0,0,1,1,1,2,2,2], ...
         REDECOM_LIST       - the re-decomposition list, eg. '{'co-imf0':'vmd', 'co-imf1':'emd'}', pd.DataFrame
         NEXT_DAY           - set True to only predict next out-of-sample value
         DAY_AHEAD          - define to forecast n days' ahead, eg. 0, 1 (default int 1)
         NOR_METHOD         - the normalizing method, eg. 'minmax'-MinMaxScaler, 'std'-StandardScaler, otherwise without normalization
         FIT_METHOD         - the fitting method to stablize the forecasting result (not necessarily useful), eg. 'add', 'ensemble'
+        trials             - optimizer search times, trials//10 for GridSearch
+        opt_cv             - optimizer cross validation division number, cross_val_score(cv=opt_cv), eg.5-20
+        opt_score          - optimizer cross validation scoring method,  cross_val_score(scoring=opt_score), eg.'r2', 'explained_variance', 'neg_mean_absolute_error'
 
         Temp global variables (cannot directly change):
         ---------------------
         TARGET             - saving target column from input data['target']
         REDECOM_MODE       - the re-decomposition method from REDECOM_LIST
         FIG_PATH           - saving path of figures from PATH
         LOG_PATH           - saving path of logs from PATH
@@ -82,289 +84,208 @@
         self.DAY_AHEAD = int(DAY_AHEAD)
         self.NOR_METHOD = str(NOR_METHOD)
         self.FIT_METHOD = str(FIT_METHOD)
         
         self.TARGET = None
         self.VMD_PARAMS = None
 
+        # Declare Sklearn parameters
+        self.opt_trials = int(kwargs.get('opt_trials', 100))
+        self.opt_cv = int(kwargs.get('opt_cv', 5))
+        self.opt_score = str(kwargs.get('opt_score', 'r2')) 
+        self.opt_direction = str(kwargs.get('opt_direction', 'maximize')) 
+
         # Check parameters
         self.PATH, self.FIG_PATH, self.LOG_PATH = check_path(PATH) # Check PATH
         if self.FORECAST_HORIZONS <= 0: raise ValueError("Invalid input for FORECAST_HORIZONS! Please input a positive integer >0.")
         if self.FORECAST_LENGTH <= 0: raise ValueError("Invalid input for FORECAST_LENGTH! Please input a positive integer >0.")
         if self.DAY_AHEAD < 0: raise ValueError("Invalid input for DAY_AHEAD! Please input a integer >=0.")
 
         if type(SKLEARN_MODEL) == str: 
             self.SKLEARN_MODEL = SKLEARN_MODEL.upper()
             if self.SKLEARN_MODEL not in ['LASSO', 'SVM', 'LGB']: raise ValueError("Invalid input for SKLEARN_MODEL! Please input eg. 'LASSO', 'SVM', 'LGB'.")
         if type(OPTIMIZER) == str: 
             self.OPTIMIZER = OPTIMIZER.upper()
             if self.OPTIMIZER not in ['BAYES', 'GS']: raise ValueError("Invalid input for OPTIMIZER! Please input eg. 'BAYES', 'GS'.")
         if type(DECOM_MODE) == str: self.DECOM_MODE = str(DECOM_MODE).upper() # Check DECOM_MODE
-        if REDECOM_LIST is not None:# Check REDECOM_LIST and Input REDECOM_MODE
+        if REDECOM_LIST is not None: # Check REDECOM_LIST and Input REDECOM_MODE
             REDECOM_MODE = ''
             try:
                 REDECOM_LIST = pd.DataFrame(REDECOM_LIST, index=range(1)) 
                 for i in range(REDECOM_LIST.size): REDECOM_MODE = REDECOM_MODE+REDECOM_LIST.values.ravel()[i]+REDECOM_LIST.columns[i][-1]+'-'
             except: raise ValueError("Invalid input for redecom_list! Please input eg. None, '{'co-imf0':'vmd', 'co-imf1':'emd'}'.")
             self.REDECOM_MODE = str(REDECOM_MODE).upper()
         else: REDECOM_MODE = None
 
+        if self.opt_score == 'r2': self.opt_direction = 'maximize' # Check opt_direction
+        else: self.opt_direction = 'minimize'
+
         if self.NEXT_DAY == True:
             print('Sklearn predictor does not support next day. Maybe update in the future.')
             self.NEXT_DAY = False
 
 
-
-    # Lasso (Least Absolute Shrinkage and Selection Operator regression)
-    def lasso_predict(self, data=None, optimizer='GridSearch', trials=100, show=False, plot=False, save=False):
+    # 1.Basic functions
+    # ------------------------------------------------------
+    # 1.1 Lasso (Least Absolute Shrinkage and Selection Operator regression)
+    def lasso_predict(self, train_test_set=None, show=False):
         """
         Single Method (directly forecast)
         Use sklearn Lasso to directly forecast wiht vector input
         Example: 
         sr = cl.sklearn_predictor()
         df_result = sr.lasso_predict(data, show=True, plot=True)
 
         Input and Parameters:
         ---------------------
         Note important hyperparameters of class cl.sklearn_predictor()
-        data               - data set (include training set and test set)
-        optimzer           - optimizer of model, eg. GridSearch and Bayes
-        trials             - optimizer search times, trials//10 for GridSearch
-        show               - show the inputting data set
-        plot               - show figure result or not
-        save               - save forecasting result or not
+        train_test_set     - data set (include training set and test set)
+        show               - show optimzing process
 
         Output
         ---------------------
-        df_result = (df_predict_real, df_eval) or next_y
-        df_predict_real   - forecasting results and the original real series set
-        df_eval           - evaluating results of forecasting 
-        next_y            - forecasting result of the next day when NEXT_DAY=Ture
+        y_predict         - forecasting result
         """
 
-        # Name and set target
-        now = datetime.now()
-        predictor_name = name_predictor(now, '', 'Sklearn', 'LASSO', None, None, False)
-        data = check_dataset(data, show)
-        self.TARGET = data['target']
-
-        # Divide the training and test set
-        from CEEMDAN_LSTM.data_preprocessor import create_train_test_set, eval_result
-        start = time.time()
-        x_train, x_test, y_train, y_test, scalarY, next_x = create_train_test_set(data, self.FORECAST_LENGTH, self.FORECAST_HORIZONS, self.NEXT_DAY, self.NOR_METHOD, self.DAY_AHEAD) 
-        x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
-        x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
+        # Get the training and test set
+        x_train, x_test, y_train, y_test, scalarY, next_x = train_test_set 
 
         # Grid Search of K-Fold CV
         # logspace(a,b,N)Divide the interval from the a power of 10 to the b power of 10 into N parts
         if self.OPTIMIZER == 'GS':
             alpha_range = np.logspace(-9, 3, 15)
             best_alpha = 1
-            for i in range(trials//10):
+            for i in range(self.opt_trials//10):
                 param_grid = dict(alpha=alpha_range)
-                grid = GridSearchCV(Lasso(max_iter=10000), param_grid=param_grid, cv=10)
+                grid = GridSearchCV(Lasso(max_iter=10000), param_grid=param_grid, cv=self.opt_cv, scoring=self.opt_score)
                 grid.fit(x_train, y_train)
                 print('Iteration',i)
                 print('Best parameters:', grid.best_params_)
                 if best_alpha == grid.best_params_['alpha']: break
                 best_alpha = grid.best_params_['alpha']
                 alpha_range = np.append(np.linspace(best_alpha/10,best_alpha*0.9,9), np.linspace(best_alpha,best_alpha*10,10)).ravel()
         
         # Bayes optimization
         if self.OPTIMIZER == 'BAYES':
             try: import optuna
             except: raise ImportError('Cannot import optuna, run: pip install optuna!')
             def objective(trial):
                 alpha = trial.suggest_float('alpha', 0, 1) 
-                clf = Lasso(alpha=alpha).fit(x_train, y_train)
-                score = cross_val_score(clf, x_train, y_train, cv=5, scoring='r2')
+                model = Lasso(alpha=alpha).fit(x_train, y_train)
+                score = cross_val_score(model, x_train, y_train, cv=self.opt_cv, scoring=self.opt_score)
                 return score.mean() 
-            study = optuna.create_study(study_name='LASSO alpha', direction='maximize') # TPESampler is used
+            study = optuna.create_study(study_name='LASSO alpha', direction=self.opt_direction) # TPESampler is used
             if not show:optuna.logging.set_verbosity(optuna.logging.WARNING) # not to print
-            study.optimize(objective, n_trials=trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
+            study.optimize(objective, n_trials=self.opt_trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
             best_alpha = study.best_params['alpha']
+            # training_loss = study.trials_dataframe()['value']
 
         # Predict
-        clf = Lasso(alpha=best_alpha)
-        clf.fit(x_train, y_train)
-        y_predict = clf.predict(x_test)
-        end = time.time()
-
-        # De-normalize and Evaluate
-        y_predict = y_predict.ravel().reshape(-1,1) 
-        if scalarY is not None: 
-            y_test = scalarY.inverse_transform(y_test)
-            y_predict = scalarY.inverse_transform(y_predict) # De-normalize           
-        if self.TARGET is not None: result_index = self.TARGET.index[-self.FORECAST_LENGTH:] # Forecasting result idnex
-        else: result_index = range(len(y_test.ravel()))
-        df_eval = eval_result(y_predict, y_test)
-        df_eval['Runtime'] = end-start
-        df_predict_result = pd.DataFrame({'real': y_test.ravel(), 'predict': y_predict.ravel()}, index=result_index) # Output
-
-        # Plot observation figures
-        print('\n=========='+predictor_name+' Finished==========')
-        df_predict_result.name, df_eval.name = predictor_name+' Result', predictor_name+' Evaluation'
-        print(df_eval) # print df_eval
-        df_result = (df_predict_result, df_eval)
-        plot_save_result(df_result, name=now, plot=plot, save=save ,path=self.PATH)
-        return df_result
-
+        model = Lasso(alpha=best_alpha)
+        model.fit(x_train, y_train)
+        y_predict = model.predict(x_test)
+        return y_predict
 
 
 
-    # SVM (Support Vector Machine Regression)
-    def svm_predict(self, data=None, optimizer='GridSearch', trials=100, show=False, plot=False, save=False):
+    # 1.2 SVM (Support Vector Machine Regression)
+    def svm_predict(self, train_test_set=None, show=False):
         """
         Single Method (directly forecast)
         Use sklearn SVR to directly forecast wiht vector input
         Example: 
         sr = cl.sklearn_predictor()
         df_result = sr.svm_predict(data, show=True, plot=True)
 
         Input and Parameters:
         ---------------------
         Note important hyperparameters of class cl.sklearn_predictor()
-        data               - data set (include training set and test set)
-        optimzer           - optimizer of model, eg. GridSearch and Bayes
-        trials             - optimizer search times, trials//10 for GridSearch
-        show               - show the inputting data set
-        plot               - show figure result or not
-        save               - save forecasting result or not
+        train_test_set     - data set (include training set and test set)
+        show               - show optimzing process
 
         Output
         ---------------------
-        df_result = (df_predict_real, df_eval) or next_y
-        df_predict_real   - forecasting results and the original real series set
-        df_eval           - evaluating results of forecasting 
-        next_y            - forecasting result of the next day when NEXT_DAY=Ture
+        y_predict         - forecasting result
         """
 
-        # Name and set target
-        now = datetime.now()
-        predictor_name = name_predictor(now, '', 'Sklearn', 'SVM', None, None, False)
-        data = check_dataset(data, show)
-        self.TARGET = data['target']
-
-        # Divide the training and test set
-        from CEEMDAN_LSTM.data_preprocessor import create_train_test_set, eval_result
-        start = time.time()
-        x_train, x_test, y_train, y_test, scalarY, next_x = create_train_test_set(data, self.FORECAST_LENGTH, self.FORECAST_HORIZONS, self.NEXT_DAY, self.NOR_METHOD, self.DAY_AHEAD) 
-        x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
-        x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
+        # Get the training and test set
+        x_train, x_test, y_train, y_test, scalarY, next_x = train_test_set 
 
         # Grid Search of K-Fold CV
         # logspace(a,b,N)Divide the interval from the a power of 10 to the b power of 10 into N parts
         if self.OPTIMIZER == 'GS':
             C_range = np.logspace(-2, 10, 13)
             gamma_range = np.logspace(-9, 3, 13)
             best_gamma, best_C = 0, 0
-            for i in range(trials//10):
+            for i in range(self.opt_trials//10):
                 param_grid = dict(gamma=gamma_range, C=C_range)
-                grid = GridSearchCV(SVR(), param_grid=param_grid, cv=10)
+                grid = GridSearchCV(SVR(), param_grid=param_grid, cv=self.opt_cv, scoring=self.opt_score)
                 grid.fit(x_train, y_train)
                 print('Iteration',i)
                 print('Best parameters:', grid.best_params_)
                 if best_gamma == grid.best_params_['gamma'] and best_C == grid.best_params_['C']: break
                 best_gamma = grid.best_params_['gamma']
                 best_C = grid.best_params_['C']
                 gamma_range = np.append(np.linspace(best_gamma/10,best_gamma*0.9,9), np.linspace(best_gamma,best_gamma*10,10)).ravel()
                 C_range = np.append(np.linspace(best_C/10,best_C*0.9,9), np.linspace(best_C,best_C*10,10)).ravel()
-        
+
         # Bayes optimization
         if self.OPTIMIZER == 'BAYES':
             try: import optuna
             except: raise ImportError('Cannot import optuna, run: pip install optuna!')
             def objective(trial):
                 # kernel = trial.suggest_categorical('kernel', ['linear','rbf','poly','sigmoid'])
                 gamma = trial.suggest_loguniform('gamma',1e-5,1e5)
                 C = trial.suggest_loguniform('C',1e-5,1e5)
                 epsilon = trial.suggest_loguniform('epsilon',1e-5,1e5)
-                clf = SVR(kernel='rbf', gamma=gamma, C=C, epsilon=epsilon).fit(x_train, y_train)
-                score = cross_val_score(clf, x_train, y_train, cv=5, scoring='r2')
+                model = SVR(kernel='rbf', gamma=gamma, C=C, epsilon=epsilon).fit(x_train, y_train)
+                score = cross_val_score(model, x_train, y_train, cv=self.opt_cv, scoring=self.opt_score)
                 return score.mean() 
-            study = optuna.create_study(study_name='SVR C gamma epsilon', direction='maximize') # TPESampler is used
+            study = optuna.create_study(study_name='SVR C gamma epsilon', direction=self.opt_direction) # TPESampler is used
             if not show: optuna.logging.set_verbosity(optuna.logging.WARNING) # not to print
-            study.optimize(objective, n_trials=trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
+            study.optimize(objective, n_trials=self.opt_trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
             # best_kernel = study.best_params['kernel']
             best_gamma = study.best_params['gamma']
             best_C = study.best_params['C']
             best_epsilon = study.best_params['epsilon']
 
         # Predict
-        clf = SVR(kernel='rbf', gamma=best_gamma, C=best_C, epsilon=best_epsilon)
-        clf.fit(x_train, y_train)
-        y_predict = clf.predict(x_test)
-        end = time.time()
-
-        # De-normalize and Evaluate
-        y_predict = y_predict.ravel().reshape(-1,1) 
-        if scalarY is not None: 
-            y_test = scalarY.inverse_transform(y_test)
-            y_predict = scalarY.inverse_transform(y_predict) # De-normalize           
-        if self.TARGET is not None: result_index = self.TARGET.index[-self.FORECAST_LENGTH:] # Forecasting result idnex
-        else: result_index = range(len(y_test.ravel()))
-        df_eval = eval_result(y_predict, y_test)
-        df_eval['Runtime'] = end-start
-        df_predict_result = pd.DataFrame({'real': y_test.ravel(), 'predict': y_predict.ravel()}, index=result_index) # Output
-
-        # Plot observation figures
-        print('\n=========='+predictor_name+' Finished==========')
-        df_predict_result.name, df_eval.name = predictor_name+' Result', predictor_name+' Evaluation'
-        print(df_eval) # print df_eval
-        df_result = (df_predict_result, df_eval)
-        plot_save_result(df_result, name=now, plot=plot, save=save ,path=self.PATH)
-        return df_result
+        model = SVR(kernel='rbf', gamma=best_gamma, C=best_C, epsilon=best_epsilon)
+        model.fit(x_train, y_train)
+        y_predict = model.predict(x_test)
+        return y_predict
 
 
 
-    # LGB or LightGBM (Light Gradient Boosting Machine)
-    def lgb_predict(self, data=None, optimizer='Bayes', trials=100, show=False, plot=False, save=False):
+    # 1.3 LGB or LightGBM (Light Gradient Boosting Machine)
+    def lgb_predict(self, train_test_set=None, show=False):
         """
         Single Method (directly forecast)
         Use LGB to directly forecast wiht vector input
         Example: 
         sr = cl.sklearn_predictor()
         df_result = sr.lgb_predict(data, show=True, plot=True)
 
         Input and Parameters:
         ---------------------
         Note important hyperparameters of class cl.sklearn_predictor()
-        data               - data set (include training set and test set)
-        optimzer           - optimizer of model, eg. GridSearch and Bayes
-        trials             - optimizer search times, trials//10 for GridSearch
-        show               - show the inputting data set
-        plot               - show figure result or not
-        save               - save forecasting result or not
+        train_test_set     - data set (include training set and test set)
+        show               - show optimzing process
 
         Output
         ---------------------
-        df_result = (df_predict_real, df_eval) or next_y
-        df_predict_real   - forecasting results and the original real series set
-        df_eval           - evaluating results of forecasting 
-        next_y            - forecasting result of the next day when NEXT_DAY=Ture
+        y_predict         - forecasting result
         """
 
         # Name and set target
         try: import lightgbm as lgb
         except: raise ImportError('Cannot import lightgbm, run: pip install lightgbm!')
 
-        self.SKLEARN_MODEL = 'LGB'
-        now = datetime.now()
-        predictor_name = name_predictor(now, '', 'Sklearn', 'LGB', None, None, False)
-        data = check_dataset(data, show)
-        self.TARGET = data['target']
-
-        # Divide the training and test set
-        from CEEMDAN_LSTM.data_preprocessor import create_train_test_set, eval_result
-        start = time.time()
-        x_train, x_test, y_train, y_test, scalarY, next_x = create_train_test_set(data, self.FORECAST_LENGTH, self.FORECAST_HORIZONS, self.NEXT_DAY, self.NOR_METHOD, self.DAY_AHEAD) 
-        x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
-        x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
-        # lgb_train = lgb.Dataset(x_train, y_train)
-        # lgb_test = lgb.Dataset(x_test, y_test, reference=lgb_train)
+        # Get the training and test set
+        x_train, x_test, y_train, y_test, scalarY, next_x = train_test_set 
 
         # Grid Search of K-Fold CV
         # logspace(a,b,N)Divide the interval from the a power of 10 to the b power of 10 into N parts
         if self.OPTIMIZER == 'GS':
             print('Grid search is not recommended. Change to Bayes optimization...')
             self.OPTIMIZER = 'BAYES'
         
@@ -381,54 +302,94 @@
                     'num_leaves': trial.suggest_categorical('num_leaves', [5, 6, 7, 12, 13, 14, 15, 28, 29, 30, 31]),
                     'learning_rate': trial.suggest_float('learning_rate', 0.01, 0.3),
                     'reg_alpha': trial.suggest_loguniform('reg_alpha', 1e-3, 10.0),
                     'reg_lambda': trial.suggest_loguniform('reg_lambda', 1e-3, 10.0),
                     'colsample_bytree': trial.suggest_categorical('colsample_bytree', [0.6,0.7,0.8,0.9,1.0]),
                     'subsample': trial.suggest_categorical('subsample', [0.6,0.7,0.8,1.0]),
                 }
-                clf = lgb.LGBMRegressor(**param_grid).fit(x_train, y_train, eval_set=[(x_test, y_test)], early_stopping_rounds=100, verbose=False)
-                score = cross_val_score(clf, x_train, y_train, cv=5, scoring='r2')
+                model = lgb.LGBMRegressor(**param_grid).fit(x_train, y_train, eval_set=[(x_test, y_test)], early_stopping_rounds=100, verbose=False)
+                score = cross_val_score(model, x_train, y_train, cv=self.opt_cv, scoring=self.opt_score)
                 return score.mean() 
-            study = optuna.create_study(study_name='LGB hyperparameters', direction='maximize') # TPESampler is used
+            study = optuna.create_study(study_name='LGB hyperparameters', direction=self.opt_direction) # TPESampler is used
             if not show: optuna.logging.set_verbosity(optuna.logging.WARNING) # not to print
-            study.optimize(objective, n_trials=100, n_jobs=-1, gc_after_trial=True)  # number of iterations
+            study.optimize(objective, n_trials=self.opt_trials, n_jobs=-1, gc_after_trial=True)  # number of iterations
             best_params = study.best_params
 
         # Predict
-        clf = lgb.LGBMRegressor(**best_params)
-        clf.fit(x_train, y_train, eval_set=[(x_test, y_test)], early_stopping_rounds=100, verbose=False)
-        y_predict = clf.predict(x_test)
+        model = lgb.LGBMRegressor(**best_params)
+        model.fit(x_train, y_train, eval_set=[(x_test, y_test)], early_stopping_rounds=100, verbose=False)
+        y_predict = model.predict(x_test)
+        return y_predict
+
+
+
+    # 2.Advanced forecasting functions
+    # ------------------------------------------------------
+    # 2.1. Single Method (directly forecast)
+    def single_sklearn_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
+        """
+        Single Method (directly forecast)
+        Use Sklearn models to directly forecast with vector input
+        Example: 
+        sr = cl.sklearn_predictor()
+        df_result = sr.single_sklearn_predict(data, show=True, plot=True, save=False)
+
+        Input and Parameters:
+        ---------------------
+        Note important hyperarameters of class cl.sklearn_predictor()
+        data            - data set (include training set and test set)
+        show            - show the inputting data set and Keras model structure
+        plot            - show figure result or not
+        save            - save forecasting result when set PATH
+        **kwargs        - any parameters of self.lasso_predict() or self.svm_predict() or ...
+
+        Output
+        ---------------------
+        df_result = (df_pred_result, df_eval_result)
+        df_pred_result  - forecasting results and the original real series set
+        df_eval_result  - evaluating results of forecasting 
+        """
+
+        # Name and set 
+        now = datetime.now()
+        predictor_name = name_predictor(now, 'Single', 'Sklearn', self.SKLEARN_MODEL, None, None, self.NEXT_DAY)
+        data = check_dataset(data, show, self.DECOM_MODE, None)
+        data.name = predictor_name+' model.pkl'
+
+        # Divide the training and test set
+        from CEEMDAN_LSTM.data_preprocessor import create_train_test_set
+        start = time.time()
+        x_train, x_test, y_train, y_test, scalarY, next_x = create_train_test_set(data, self.FORECAST_LENGTH, self.FORECAST_HORIZONS, self.NEXT_DAY, self.NOR_METHOD, self.DAY_AHEAD) 
+        x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
+        x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
+        train_test_set = (x_train, x_test, y_train, y_test, scalarY, next_x)
+
+        # Forecast
+        if self.SKLEARN_MODEL == 'LASSO': y_predict = self.lasso_predict(train_test_set, show=show, **kwargs)
+        if self.SKLEARN_MODEL == 'SVM': y_predict = self.svm_predict(train_test_set, show=show, **kwargs) 
+        if self.SKLEARN_MODEL == 'LGB': y_predict = self.lgb_predict(train_test_set, show=show, **kwargs)
         end = time.time()
 
-        # De-normalize and Evaluate
+        # De-normalize
         y_predict = y_predict.ravel().reshape(-1,1) 
-        if scalarY is not None: 
-            y_test = scalarY.inverse_transform(y_test)
-            y_predict = scalarY.inverse_transform(y_predict) # De-normalize           
-        if self.TARGET is not None: result_index = self.TARGET.index[-self.FORECAST_LENGTH:] # Forecasting result idnex
-        else: result_index = range(len(y_test.ravel()))
-        df_eval = eval_result(y_predict, y_test)
-        df_eval['Runtime'] = end-start
-        df_predict_result = pd.DataFrame({'real': y_test.ravel(), 'predict': y_predict.ravel()}, index=result_index) # Output
-
-        # Plot observation figures
-        print('\n=========='+predictor_name+' Finished==========')
-        df_predict_result.name, df_eval.name = predictor_name+' Result', predictor_name+' Evaluation'
-        print(df_eval) # print df_eval
-        df_result = (df_predict_result, df_eval)
-        plot_save_result(df_result, name=now, plot=plot, save=save ,path=self.PATH)
+        if scalarY is not None: y_predict = scalarY.inverse_transform(y_predict)         
+
+        # Output and Evaluate
+        df_predict_result = pd.DataFrame({'real': data['target'][-self.FORECAST_LENGTH:], 'predict': y_predict.ravel()}) # Output
+        df_result = output_result(df_predict_result, predictor_name, end-start, imf='Final') # return (final_pred, final_eval)
+        plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
         return df_result
 
 
 
-    # 2.3. Respective Method (decompose then respectively forecast each IMFs)
+    # 2.2. Respective Method (decompose then respectively forecast each IMFs)
     def respective_sklearn_predict(self, data=None, show=False, plot=False, save=False, **kwargs):
         """
         Respective Method (decompose then respectively forecast each IMFs)
-        Use decomposition-integration Sklearn model to respectively forecast each IMFs with vector input
+        Use decomposition-integration method and Sklearn models to respectively forecast each IMFs with vector input
         Example: 
         sr = cl.sklearn_predictor()
         df_result = sr.respective_sklearn_predict(data, show=True, plot=True, save=False)
 
         Input and Parameters:
         ---------------------
         Note important hyperarameters of class cl.sklearn_predictor()
@@ -436,96 +397,58 @@
         show            - show the inputting data set and Sklearn model structure
         plot            - show figure result or not
         save            - save forecasting result when set PATH
         **kwargs        - any parameters of self.sklearn_predictor()
 
         Output
         ---------------------
-        df_result = (df_predict_real, df_eval, df_train_loss) or next_y
-        df_predict_real - forecasting results and the original real series set
-        df_eval         - evaluating results of forecasting 
-        df_train_loss   - training loss log
-        next_y          - forecasting result of the next day when NEXT_DAY=Ture
+        df_result = (df_pred_result, df_eval_result)
+        df_pred_result  - forecasting results and the original real series set
+        df_eval_result  - evaluating results of forecasting 
         """
 
         # Name
         now = datetime.now()
         predictor_name = name_predictor(now, 'Respective', 'Sklearn', self.SKLEARN_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)
 
         # Decompose, integrate, re-decompose
         start = time.time()
         from CEEMDAN_LSTM.data_preprocessor import redecom
         df_redecom, df_redecom_list = redecom(data, show, self.DECOM_MODE, self.INTE_LIST, self.REDECOM_LIST, self.VMD_PARAMS, self.FORECAST_LENGTH)
-        
-        # set target and model
-        try: 
-            if 'Sklearn_Forecasting' in data.name: predictor_name = data.name
-            else:
-                data.name = ''
-                self.TARGET = df_redecom['target']
-        except: 
-            data.name = ''
-            self.TARGET = df_redecom['target']
 
         # Forecast and ouput each Co-IMF
-        df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
+        df_pred_result = pd.DataFrame(index = df_redecom['target'].index[-self.FORECAST_LENGTH:]) # df for storing forecasting result
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
         df_next_result = pd.DataFrame(columns=['today_real', 'today_pred', 'next_pred', 'Runtime', 'IMF']) # df for storing Next-day forecasting result
         for imf in df_redecom.columns.difference(['target']):
             df_redecom[imf].name = (predictor_name+'_of_'+imf+'_model.h5').replace('-','_').replace(' ','_')
             time1 = time.time()
             with self.HiddenPrints():
-                if self.SKLEARN_MODEL == 'LASSO': df_result = self.lasso_predict(data=df_redecom[imf], **kwargs)
-                if self.SKLEARN_MODEL == 'SVM': df_result = self.svm_predict(data=df_redecom[imf], **kwargs) 
-                if self.SKLEARN_MODEL == 'LGB': df_result = self.lgb_predict(data=df_redecom[imf], **kwargs)
+                df_result = self.single_sklearn_predict(data=df_redecom[imf], **kwargs) # return (df_pred, df_eval)
             time2 = time.time()
-            print('----'+predictor_name+' of '+imf+' Finished----')
-            if not self.NEXT_DAY: 
-                df_result[1]['Runtime'] = time2-time1 # Output Runtime
-                df_result[1]['IMF'] = imf
-                df_result[0].name, df_result[1].name = predictor_name+' Result of '+imf, predictor_name+' Evaluation of '+imf
-                print(df_result[1]) # print df_eval
-                df_pred_result[imf+'-real'] = df_result[0]['real'] # add real values
-                df_pred_result[imf+'-predict'] = df_result[0]['predict'] # add forecasting result
+            df_result = output_result(df_result, predictor_name, time2-time1, imf) # return (imf_pred, imf_eval)
+            if not self.NEXT_DAY:
+                df_pred_result = pd.concat((df_pred_result, df_result[0]), axis=1) # add forecasting result
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
-            else: 
-                df_result['Runtime'] = time2-time1 # Output Runtime
-                df_result['IMF'] = imf
-                df_result.name = predictor_name+' Result of '+imf
-                print(df_result)
-                df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
-            plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
+                plot_save_result(df_result, name=now, plot=plot, save=False, path=self.PATH) # do not save Co-IMF results
+            else: df_next_result = pd.concat((df_next_result, df_result)) # add Next-day forecasting result
             print('')
         end = time.time()
 
         # Final Output
-        print('=========='+predictor_name+' Finished==========')
-        from CEEMDAN_LSTM.data_preprocessor import eval_result
         if not self.NEXT_DAY: 
-            df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
+            df_pred_result['real'] = df_redecom['target'][-self.FORECAST_LENGTH:]
             df_pred_result['predict'] = df_pred_result[[x for x in df_pred_result.columns if 'predict' in x]].sum(axis=1)
-            final_eval = eval_result(df_pred_result['predict'], df_pred_result['real'])
-            final_eval['Runtime'] = end-start # Output Runtime
-            final_eval['IMF'] = 'Final'
-            print(final_eval) # print df_eval
-            final_eval = pd.concat((final_eval, df_eval_result))
-            df_plot = df_pred_result[['real', 'predict']]
-            df_pred_result.name, final_eval.name, df_plot.name = predictor_name+' Result', predictor_name+' Evaluation', predictor_name+' Result'
-            plot_save_result(df_plot, name=now, plot=plot, save=False, path=self.PATH)
-            df_result = (df_pred_result, final_eval)
+            df_result = output_result((df_pred_result, df_eval_result), predictor_name, end-start, imf='Final')
         else:
-            df_result = pd.DataFrame({'today_real': self.TARGET.values[-1], 'today_pred': df_next_result['today_pred'].sum(), 
-                                      'next_pred': df_next_result['next_pred'].sum()}, index=[df_next_result.index[0]]) # Output
-            df_result['Runtime'] = end-start # Output Runtime
-            df_result['IMF'] = 'Final'
-            df_result = pd.concat((df_result, df_next_result))
-            df_result.name = predictor_name+' Result'
-            print(df_result)
-        plot_save_result(df_result, name=now, plot=False, save=save, path=self.PATH)
-        return df_result
+            df_result = pd.DataFrame({'today_real': df_redecom['target'][-1:], 'today_pred': df_next_result['today_pred'].sum(), 
+                                      'next_pred': df_next_result['next_pred'].sum()}) # Output
+            df_result = output_result((df_result, df_next_result), predictor_name, end-start, imf='Final')
+        plot_save_result(df_result, name=now, plot=plot, save=save, path=self.PATH)
+        return df_result 
 
 
 
     # A class used to hide the print
     class HiddenPrints: 
         """
         A class used to hide the print
@@ -533,21 +456,21 @@
         def __enter__(self):
             self._original_stdout = sys.stdout
             sys.stdout = open(os.devnull, 'w')
         def __exit__(self, exc_type, exc_val, exc_tb):
             sys.stdout.close()
             sys.stdout = self._original_stdout
 
-    # 2.5. Multiple Run Predictor
+    # 2.3. Multiple Run Predictor
     def multiple_sklearn_predict(self, data=None, run_times=10, predict_method=None, **kwargs):
         """
         Multiple Run Predictor, multiple run of above method
         Example: 
-        kr = cl.sklearn_predictor()
-        df_result = kr.multiple_sklearn_predict(data, run_times=10, predict_method='lasso')
+        sr = cl.sklearn_predictor()
+        df_result = sr.multiple_sklearn_predict(data, run_times=10, predict_method='respective')
 
         Input and Parameters:
         ---------------------
         Note important hyperarameters of class cl.sklearn_predictor()
         data               - data set (include training set and test set)
         run_times          - running times
         predict_method     - run different method eg. 'lasso', 'svm', 'lgb'
@@ -559,43 +482,35 @@
         ---------------------
         df_eval_result     - evaluating forecasting results of each run
         """
 
         # Initialize 
         now = datetime.now()
         data = check_dataset(data, False, self.DECOM_MODE, self.REDECOM_LIST)
-        self.TARGET = data['target']
-        
         if self.PATH is None: print('Do not set a PATH! It is recommended to set a PATH to prevent the loss of running results')
         if predict_method is None: raise ValueError("Please input a predict method! eg. 'single', 'ensemble', 'respective'.")
         else: predict_method = predict_method.capitalize()
         if predict_method == 'Single': predictor_name = name_predictor(now, 'Multiple Single', 'Sklearn', self.SKLEARN_MODEL, None, None, self.NEXT_DAY)
         else: predictor_name = name_predictor(now, 'Multiple '+predict_method, 'Sklearn', self.SKLEARN_MODEL, self.DECOM_MODE, self.REDECOM_LIST, self.NEXT_DAY)    
 
         # Forecast
         start = time.time()
-        df_pred_result = pd.DataFrame(index = self.TARGET.index[-self.FORECAST_LENGTH:0]) # df for storing forecasting result
-        df_pred_result['real'] = self.TARGET[-self.FORECAST_LENGTH:]
+        df_pred_result = pd.DataFrame(index = data['target'].index[-self.FORECAST_LENGTH:]) # df for storing forecasting result
         df_eval_result = pd.DataFrame(columns=['Scale', 'R2', 'RMSE', 'MAE', 'MAPE', 'Runtime', 'IMF']) # df for storing evaluation result
         for i in range(run_times):
             print('Run %d is running...'%i, end='')
             time1 = time.time()
             with self.HiddenPrints():
-                if predict_method == 'Single':
-                    if self.SKLEARN_MODEL == 'LASSO': df_result = self.lasso_predict(data=data, **kwargs)
-                    if self.SKLEARN_MODEL == 'SVM': df_result = self.svm_predict(data=data, **kwargs) 
-                    if self.SKLEARN_MODEL == 'LGB': df_result = self.lgb_predict(data=data, **kwargs)
-                if predict_method == 'Respective': df_result = self.respective_sklearn_predict(data=data, **kwargs)
-                if 'IMF' not in df_result[1].columns: df_result[1]['IMF'] = predict_method + '-Run' + str(i)
-                else: df_result[1]['IMF'] = predict_method + '-Run' + str(i) + '-' + df_result[1]['IMF']
+                if predict_method == 'Single': df_result = self.single_sklearn_predict(data=data, **kwargs) # return (df_pred, df_eval)
+                elif predict_method == 'Respective': df_result = self.respective_sklearn_predict(data=data, **kwargs) # return (df_all_pred, df_eval)
+                else: raise ValueError("Please input a vaild predict method! eg. 'single', 'respective'.")
+                time2 = time.time()
+                df_result = output_result(df_result, predictor_name, time2-time1, imf='Final', run=i)
+                df_pred_result = pd.concat((df_pred_result, df_result[0]), axis=1) # add forecasting result
                 df_eval_result = pd.concat((df_eval_result, df_result[1])) # add evaluation result
-                df_pred_result['Run'+str(i)+'-predict'] = df_result[0]['predict']
-                df_result = (df_pred_result, df_eval_result)
                 df_pred_result.name, df_eval_result.name = predictor_name+' Result', predictor_name+' Evaluation'
-                plot_save_result(df_result, name=now, plot=False, save=True, path=self.PATH)
-            time2 = time.time()
+                plot_save_result((df_pred_result, df_eval_result), name=now, plot=False, save=True, path=self.PATH) # Temporary storage
             print('taking time: %.3fs'%(time2-time1))
         end = time.time()
         print('\n============='+predictor_name+' Finished=============')
         print('Running time: %.3fs'%(end-start))
-        plot_save_result(df_result, name=now, plot=False, save=True, path=self.PATH)
-        return df_result
+        return (df_pred_result, df_eval_result)
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/PKG-INFO` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEMDAN-LSTM
-Version: 1.2b2
+Version: 1.2b3
 Summary: CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.
 Home-page: http://github.com/FateMurphy/CEEMDAN_LSTM
 Author: Feite Zhou
 Author-email: jupiterzhou@foxmail.com
 Keywords: CEEMDAN,VMD,LSTM,decomposition,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CEEMDAN_LSTM-1.2b2/CEEMDAN_LSTM.egg-info/SOURCES.txt` & `CEEMDAN_LSTM-1.2b3/CEEMDAN_LSTM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/LICENSE` & `CEEMDAN_LSTM-1.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/PKG-INFO` & `CEEMDAN_LSTM-1.2b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CEEMDAN_LSTM
-Version: 1.2b2
+Version: 1.2b3
 Summary: CEEMDAN_LSTM is a Python project for decomposition-integration forecasting models based on EMD methods and LSTM.
 Home-page: http://github.com/FateMurphy/CEEMDAN_LSTM
 Author: Feite Zhou
 Author-email: jupiterzhou@foxmail.com
 Keywords: CEEMDAN,VMD,LSTM,decomposition,forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `CEEMDAN_LSTM-1.2b2/README.md` & `CEEMDAN_LSTM-1.2b3/README.md`

 * *Files identical despite different names*

### Comparing `CEEMDAN_LSTM-1.2b2/setup.py` & `CEEMDAN_LSTM-1.2b3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='CEEMDAN_LSTM',
-    version='1.2b2',
+    version='1.2b3',
     packages=setuptools.find_packages(),
     install_requires=['numpy >= 1.17.3',
                       'pandas >= 1.2.0',
                       'EMD-signal >= 1.2.3',
                       'optuna >= 3.0.0',
                       'vmdpy',
                       'sampen',
```

