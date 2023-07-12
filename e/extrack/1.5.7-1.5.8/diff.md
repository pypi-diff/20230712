# Comparing `tmp/extrack-1.5.7.tar.gz` & `tmp/extrack-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrack-1.5.7.tar", last modified: Fri May 19 21:03:40 2023, max compression
+gzip compressed data, was "extrack-1.5.8.tar", last modified: Wed Jul 12 18:46:59 2023, max compression
```

## Comparing `extrack-1.5.7.tar` & `extrack-1.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.794831 extrack-1.5.7/
--rw-rw-rw-   0        0        0     1074 2023-05-19 15:53:57.000000 extrack-1.5.7/LICENSE
--rw-rw-rw-   0        0        0     6889 2023-05-19 21:03:40.794831 extrack-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     6083 2023-05-19 15:53:57.000000 extrack-1.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.725797 extrack-1.5.7/Tutorials/
--rw-rw-rw-   0        0        0        1 2023-05-19 15:54:45.000000 extrack-1.5.7/Tutorials/__init__.py
--rw-rw-rw-   0        0        0     3979 2023-05-19 15:54:45.000000 extrack-1.5.7/Tutorials/automated_fitting.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.757049 extrack-1.5.7/extrack/
--rw-rw-rw-   0        0        0      367 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/__init__.py
--rw-rw-rw-   0        0        0     6484 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/auto_fitting.py
--rw-rw-rw-   0        0        0    23781 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/exporters.py
--rw-rw-rw-   0        0        0    24031 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/histograms.py
--rw-rw-rw-   0        0        0    40699 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/old_tracking.py
--rw-rw-rw-   0        0        0    10492 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/readers.py
--rw-rw-rw-   0        0        0    22606 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/refined_loc_old.py
--rw-rw-rw-   0        0        0    25414 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/refined_localization.py
--rw-rw-rw-   0        0        0    10688 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/simulate_tracks.py
--rw-rw-rw-   0        0        0    73026 2023-05-19 15:54:45.000000 extrack-1.5.7/extrack/tracking.py
--rw-rw-rw-   0        0        0    58805 2023-05-19 15:54:46.000000 extrack-1.5.7/extrack/tracking_0.py
--rw-rw-rw-   0        0        0       22 2023-05-19 15:54:46.000000 extrack-1.5.7/extrack/version.py
--rw-rw-rw-   0        0        0     5227 2023-05-19 15:54:46.000000 extrack-1.5.7/extrack/visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:03:40.794831 extrack-1.5.7/extrack.egg-info/
--rw-rw-rw-   0        0        0     6889 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-19 21:03:40.000000 extrack-1.5.7/extrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2023-05-19 15:53:57.000000 extrack-1.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-19 21:03:40.794831 extrack-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-19 15:53:57.000000 extrack-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:46:59.034444 extrack-1.5.8/
+-rw-rw-rw-   0        0        0     1074 2023-07-12 18:27:38.000000 extrack-1.5.8/LICENSE
+-rw-rw-rw-   0        0        0     6889 2023-07-12 18:46:59.034444 extrack-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6083 2023-07-12 18:27:38.000000 extrack-1.5.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:46:58.981034 extrack-1.5.8/Tutorials/
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:27:38.000000 extrack-1.5.8/Tutorials/__init__.py
+-rw-rw-rw-   0        0        0     3979 2023-07-12 18:27:38.000000 extrack-1.5.8/Tutorials/automated_fitting.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:46:58.996658 extrack-1.5.8/extrack/
+-rw-rw-rw-   0        0        0      367 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/__init__.py
+-rw-rw-rw-   0        0        0     6484 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/auto_fitting.py
+-rw-rw-rw-   0        0        0    23781 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/exporters.py
+-rw-rw-rw-   0        0        0    24031 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/histograms.py
+-rw-rw-rw-   0        0        0    40699 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/old_tracking.py
+-rw-rw-rw-   0        0        0    10492 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/readers.py
+-rw-rw-rw-   0        0        0    22606 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/refined_loc_old.py
+-rw-rw-rw-   0        0        0    25414 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/refined_localization.py
+-rw-rw-rw-   0        0        0    10688 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/simulate_tracks.py
+-rw-rw-rw-   0        0        0    73925 2023-07-12 18:44:27.000000 extrack-1.5.8/extrack/tracking.py
+-rw-rw-rw-   0        0        0    58805 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/tracking_0.py
+-rw-rw-rw-   0        0        0       23 2023-07-12 18:28:46.000000 extrack-1.5.8/extrack/version.py
+-rw-rw-rw-   0        0        0     5227 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:46:59.034444 extrack-1.5.8/extrack.egg-info/
+-rw-rw-rw-   0        0        0     6889 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2023-07-12 18:27:38.000000 extrack-1.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 18:46:59.034444 extrack-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-07-12 18:27:38.000000 extrack-1.5.8/setup.py
```

### Comparing `extrack-1.5.7/LICENSE` & `extrack-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/PKG-INFO` & `extrack-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrack
-Version: 1.5.7
+Version: 1.5.8
 Summary: SPT kinetic modelling and states annotation of tracks
 Home-page: https://github.com/FrancoisSimon/ExTrack-python3
 Author: Francois Simon
 Author-email: simon.francois@protonmail.com
 Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `extrack-1.5.7/README.md` & `extrack-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/Tutorials/automated_fitting.py` & `extrack-1.5.8/Tutorials/automated_fitting.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/auto_fitting.py` & `extrack-1.5.8/extrack/auto_fitting.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/exporters.py` & `extrack-1.5.8/extrack/exporters.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/histograms.py` & `extrack-1.5.8/extrack/histograms.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/old_tracking.py` & `extrack-1.5.8/extrack/old_tracking.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/readers.py` & `extrack-1.5.8/extrack/readers.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/refined_loc_old.py` & `extrack-1.5.8/extrack/refined_loc_old.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/refined_localization.py` & `extrack-1.5.8/extrack/refined_localization.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/simulate_tracks.py` & `extrack-1.5.8/extrack/simulate_tracks.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/tracking.py` & `extrack-1.5.8/extrack/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -599,14 +599,15 @@
         # repeat the previous matrix to account for the states variations due to the new position
         m_arr = cp.repeat(m_arr, nb_states**nb_substeps , axis = 1)
         s2_arr = cp.repeat(s2_arr, nb_states**nb_substeps, axis = 1)
         LP = cp.repeat(LP, nb_states**nb_substeps, axis = 1)
         
         end_p_stay = p_stay[cur_states[:,None:,:-1]][:,:,0]
         LL = cp.log(pBL + (1-end_p_stay) - pBL * (1-end_p_stay)) + LT
+        cur_Bs_cat = cur_Bs_cat[:,:,1:]
     
     new_s2_arr = cp.array((s2_arr + LocErr2[:,:, min(LocErr_index, nb_locs-current_step)]))
     log_integrated_term = cp.sum(-0.5*cp.log(2*np.pi*new_s2_arr) - (Cs[:,:,0] - m_arr)**2/(2*new_s2_arr),axis=2)
     #LF = cp.log(Fs[cur_Bs[:,:,0].astype(int)]) # Log proba of starting in a given state (fractions)
     #LF = cp.log(0.5)
     # cp.mean(cp.log(Fs[cur_Bs[:,:,:].astype(int)]), 2) # Log proba of starting in a given state (fractions)
     LP += log_integrated_term + LL
@@ -639,45 +640,53 @@
     
     for Bs_ID in range(m_arr.shape[1]):
         if not np.isin(Bs_ID, grouped_IDs):
             cur_m_arr = m_arr[:,Bs_ID]
             cur_s_arr = s_arr[:,Bs_ID]
             
             cur_cur_Bs_cat = cur_Bs_cat[:,Bs_ID]
+            current_state = np.argmax(cur_cur_Bs_cat[0,0])
+            cur_state_mask = np.argmax(cur_Bs_cat[0, :,0],1) == current_state
             
             test_chunks = np.min([np.max([10, int(nb_Tracks**0.4)]), 50])
             test_chunks = 30
             
             if cur_cur_Bs_cat.shape[1] > frame_len:
-                state_mask = np.mean(np.all((cur_cur_Bs_cat[:test_chunks,None,:frame_len] == cur_Bs_cat[:test_chunks,:,:frame_len]), (2, 3)), 0) > 0.999
+                #state_mask = np.mean(np.all((cur_cur_Bs_cat[:test_chunks,None,:frame_len] == cur_Bs_cat[:test_chunks,:,:frame_len]), (2, 3)), 0) > 0.999
+                state_mask = np.mean(np.all(np.argmax(cur_cur_Bs_cat[:test_chunks,None,:frame_len], -1) == np.argmax(cur_Bs_cat[:test_chunks,:,:frame_len], -1), (2)), 0) > 0.999
+            #cur_Bs_cat[:,np.where(state_mask)[0]]
+            
+            #(np.argmax(cur_cur_Bs_cat[:test_chunks,None,:frame_len], -1) == np.argmax(cur_Bs_cat[:test_chunks,:,:frame_len], -1)).shape
+            
             else:
                 state_mask = False
             
             m_mask_relative = np.mean((np.mean(np.abs(m_arr[:test_chunks] - cur_m_arr[:test_chunks,None]), 2, keepdims = True)/s_arr[:test_chunks]) < threshold, (0, 2)) > 0.8
             #s_mask_relative = ((cur_s_arr[:,None] > (1 - threshold) * s_arr)*(cur_s_arr[:,None] < (1 + threshold) * s_arr))[0,:,0]
             s_mask_relative = np.mean((np.mean(np.abs(s_arr[:test_chunks] - cur_s_arr[:test_chunks,None]), 2, keepdims = True)/s_arr[:test_chunks]) < threshold, (0, 2)) > 0.8
             
-            args = np.where(m_mask_relative * s_mask_relative + state_mask)[0]
+            args = np.where(m_mask_relative * s_mask_relative * cur_state_mask + state_mask)[0]
 
             args = args[np.isin(args, grouped_IDs) == False] # remove elements that already belongs to a group
             
             groups.append(args)
             grouped_IDs = grouped_IDs + list(args)
-            
+    
     if len(grouped_IDs) != m_arr.shape[1]:
         raise ValueError('problem with grouping: len(grouped_IDs)=' + str(len(grouped_IDs)) + ' and m_arr.shape[1]=' + str( m_arr.shape[1]))
 
-    subgroups = []
-    for group in groups:
-        for state in range(nb_states):
-            subgroup = group[cur_Bs[:, group][0,:,0] == state]
-            if len(subgroup)>0:
-                subgroups.append(subgroup)
+    #subgroups = []
+    #for group in groups:
+    #    for state in range(nb_states):
+    #        subgroup = group[cur_Bs[:, group][0,:,0] == state]
+    #        if len(subgroup)>0:
+    #            subgroups.append(subgroup)
     
     # part that is too time consuming, find a way to make it faster
+    subgroups = groups
     nb_subgroups = len(subgroups)
     new_cur_Bs = np.empty((1, nb_subgroups, 1), dtype=(int))
     if not do_preds:
         cur_Bs_cat = cur_Bs_cat[:,:,:frame_len]
 
     new_cur_Bs_cat = np.zeros((nb_Tracks, nb_subgroups, cur_Bs_cat.shape[2], nb_states), dtype = cur_Bs_cat.dtype)
     
@@ -703,14 +712,15 @@
         
         new_m_arr[:, Bs_ID] = np.sum(weights[:,:,None] * m_arr[:, subgroup, :], 1) / sum_weights
         new_s2_arr[:, Bs_ID] = np.sum(weights[:,:,None] * s2_arr[:, subgroup, :], 1) / sum_weights
         new_LP[:, Bs_ID] = np.log(np.sum(np.exp(LP[:, subgroup]-max_LP), axis = 1)) + np.squeeze(max_LP, axis = 1)
         
     return new_m_arr, new_s2_arr, new_LP, new_cur_Bs, new_cur_Bs_cat
 
+
 def get_all_Bs(nb_Cs, nb_states):
     '''
     produces a matrix of the possible sequences of states
     '''
     Bs_ID = np.arange(nb_states**nb_Cs)
     all_Bs = np.zeros((nb_states**nb_Cs, nb_Cs), int)
     
@@ -747,24 +757,27 @@
     max_LP = max_LP[:,0]
     P_CB = np.exp(LP_CB)
     P_C = cp.sum(P_CB, axis = 1) # sum over B
     LP_C = np.log(P_C) + max_LP # back to log proba of C without overflow due to exponential
     return LP_C
 
 def Pool_star_P_inter(args):
-    return P_Cs_inter_bound_stats(*args)[2] # returns the 3rd output which is the predictions
+    return P_Cs_inter_bound_stats_th(*args)[2] # returns the 3rd output which is the predictions
 
 def predict_Bs(all_tracks,
                dt,
                params,
                cell_dims=[1],
-               nb_states=2,
-               frame_len=8,
+               nb_states=4,
+               frame_len=5,
+               max_nb_states = 200,
+               threshold = 0.1,
                workers = 1,
-               input_LocErr = None):
+               input_LocErr = None,
+               verbose = 0):
     '''
     inputs the observed localizations and parameters and determines the proba
     of each localization to be in a given state.
     
     arguments:
     all_tracks: dict describing the tracks with track length as keys (number of time positions, e.g. '23') of 3D arrays: dim 0 = track, dim 1 = time position, dim 2 = x, y position.
     params: lmfit parameters used for the model.
@@ -799,58 +812,58 @@
             param_kwargs.append({'name' : param, 'value' : params[param], 'vary': False})
         new_params = Parameters()
         [new_params.add(**param_kwargs[k]) for k in range(len(params))]
         LocErr, ds, Fs, TrMat, pBL = extract_params(new_params, dt, nb_states, nb_substeps)'''
     else:
         raise TypeError("params must be either of the class 'lmfit.parameter.Parameters' or a dictionary of the relevant parameters")
     all_pred_Bs = []
-
+    
     min_len = int(l_list[0])
     max_len = int(l_list[-1])
     
     Csss = []
     sigss = []
     isBLs = []
     for k in range(len(all_tracks)):
-        if k == len(all_tracks)-1:
-            isBL = 0 # last position correspond to tracks which didn't disapear within maximum track length
-        else:
-            isBL = 1
         Css = all_tracks[k]
         if input_LocErr != None:
             sigs = LocErr[k]
-        nb_max = 500
+        nb_max = 1
         for n in range(int(np.ceil(len(Css)/nb_max))):
             Csss.append(Css[n*nb_max:(n+1)*nb_max])
             if input_LocErr != None:
                 sigss.append(sigs[n*nb_max:(n+1)*nb_max])
             if Css.shape[1] == max_len:
                 isBLs.append(0) # last position correspond to tracks which didn't disapear within maximum track length
             else:
                 isBLs.append(1)
     do_preds = 1
-    args_prod = np.array(list(product(Csss, [0], [ds], [Fs], [TrMat],[pBL], [0],[cell_dims], [nb_substeps], [frame_len], [do_preds], [min_len])), dtype=object)
+    #Cs, LocErr, ds, Fs, TrMat,pBL,isBL, cell_dims, nb_substeps, frame_len, min_len, threshold, max_nb_states = args_prod[0]
+    #Cs, LocErr, ds, Fs, TrMat, pBL, isBL, cell_dims, nb_substeps, frame_len, do_preds, min_len, threshold, max_nb_states = args_prod[0]
+    args_prod = np.array(list(product(Csss, [0], [ds], [Fs], [TrMat],[pBL], [0],[cell_dims], [nb_substeps], [frame_len], [do_preds], [min_len], [threshold], [max_nb_states])), dtype=object)
     args_prod[:, 6] = isBLs
     if input_LocErr != None:
         args_prod[:,1] = sigss
     else:
         args_prod[:,1] = LocErr
     
     if workers >= 2:
         with multiprocessing.Pool(workers) as pool:
             all_pred_Bs = pool.map(Pool_star_P_inter, args_prod)
     else:
         all_pred_Bs = []
         for args in args_prod:
             all_pred_Bs.append(Pool_star_P_inter(args))
+            if verbose:
+                print('.', end = '')
     
     all_pred_Bs_dict = {}
     for l in l_list:
         all_pred_Bs_dict[l] = np.empty((0,int(l),nb_states))
-    for pred_Bs in all_pred_Bs:
+    for i, pred_Bs in enumerate(all_pred_Bs):
         all_pred_Bs_dict[str(pred_Bs.shape[1])] = np.concatenate((all_pred_Bs_dict[str(pred_Bs.shape[1])],pred_Bs))
 
     return all_pred_Bs_dict
 
 def extract_params(params, dt, nb_states, nb_substeps, input_LocErr = None, Matrix_type = 1):
     '''
     turn the parameters which differ deppending on the number of states into lists
```

### Comparing `extrack-1.5.7/extrack/tracking_0.py` & `extrack-1.5.8/extrack/tracking_0.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack/visualization.py` & `extrack-1.5.8/extrack/visualization.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/extrack.egg-info/PKG-INFO` & `extrack-1.5.8/extrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extrack
-Version: 1.5.7
+Version: 1.5.8
 Summary: SPT kinetic modelling and states annotation of tracks
 Home-page: https://github.com/FrancoisSimon/ExTrack-python3
 Author: Francois Simon
 Author-email: simon.francois@protonmail.com
 Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `extrack-1.5.7/extrack.egg-info/SOURCES.txt` & `extrack-1.5.8/extrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extrack-1.5.7/setup.py` & `extrack-1.5.8/setup.py`

 * *Files identical despite different names*

