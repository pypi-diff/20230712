# Comparing `tmp/Ekidna-0.0.7.tar.gz` & `tmp/Ekidna-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ekidna-0.0.7.tar", last modified: Fri Jun 30 22:55:03 2023, max compression
+gzip compressed data, was "Ekidna-0.0.8.tar", last modified: Wed Jul 12 16:36:44 2023, max compression
```

## Comparing `Ekidna-0.0.7.tar` & `Ekidna-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 22:55:03.743853 Ekidna-0.0.7/
--rw-rw-rw-   0        0        0      639 2023-06-30 21:48:21.000000 Ekidna-0.0.7/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 22:55:03.686032 Ekidna-0.0.7/Ekidna/
--rw-rw-rw-   0        0        0    86635 2023-06-30 22:54:12.000000 Ekidna-0.0.7/Ekidna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:55:03.740769 Ekidna-0.0.7/Ekidna.egg-info/
--rw-rw-rw-   0        0        0     1532 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 22:55:03.000000 Ekidna-0.0.7/Ekidna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1059 2023-06-29 21:10:14.000000 Ekidna-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-29 18:41:11.000000 Ekidna-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    36509 2023-06-30 21:51:21.000000 Ekidna-0.0.7/Module Contents.txt
--rw-rw-rw-   0        0        0     1532 2023-06-30 22:55:03.743166 Ekidna-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-06-29 21:10:51.000000 Ekidna-0.0.7/README.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 22:55:03.744355 Ekidna-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-06-30 21:48:32.000000 Ekidna-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:36:44.346912 Ekidna-0.0.8/
+-rw-rw-rw-   0        0        0      354 2023-07-12 16:31:57.000000 Ekidna-0.0.8/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 16:36:44.315759 Ekidna-0.0.8/Ekidna/
+-rw-rw-rw-   0        0        0   102688 2023-07-12 16:35:40.000000 Ekidna-0.0.8/Ekidna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:36:44.344471 Ekidna-0.0.8/Ekidna.egg-info/
+-rw-rw-rw-   0        0        0     1245 2023-07-12 16:36:44.000000 Ekidna-0.0.8/Ekidna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-12 16:36:44.000000 Ekidna-0.0.8/Ekidna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:36:44.000000 Ekidna-0.0.8/Ekidna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 16:36:44.000000 Ekidna-0.0.8/Ekidna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1059 2023-06-29 21:10:14.000000 Ekidna-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 18:41:11.000000 Ekidna-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    42273 2023-07-12 16:35:09.000000 Ekidna-0.0.8/Module Contents.txt
+-rw-rw-rw-   0        0        0     1245 2023-07-12 16:36:44.346912 Ekidna-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-29 21:10:51.000000 Ekidna-0.0.8/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:36:44.347916 Ekidna-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-07-12 16:35:24.000000 Ekidna-0.0.8/setup.py
```

### Comparing `Ekidna-0.0.7/Ekidna/__init__.py` & `Ekidna-0.0.8/Ekidna/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -654,15 +654,20 @@
                                           if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)          : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                           if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)            : details regarding the smoothing procedure used when building the curve
         - baseline     (str)            : details regarding the baseline procedure used when building the curve  
         - calibration  (str)            : details regarding the calibration procedure used when building the curve
+
+        - fit_data     (list)           : a list containing the x,y data for the data used to fit the parabolic model
+        - full_data    (list)           : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. It is not necessary to fit.
     Methods/Functions:
+        - fit               : performs least-squares regression using scipy.optimize.curve_fit. The function returns estimated fit coefficients, their covariance matrix,
+                              and populates various attributes of the linear_std_curve object including s, standard range, estimation range.
         - predict           : returns the value, y, of the standard curve at a particular input, x. This is essentially the MLE for the system response to the input, x.
         - details           : prints out a summary of the details of the standard curve
         - errprop           : the error propagation formula for a parabola. This method returns the value of the variance of the response variable, y, at a given input, x.
         - upper_pred_edge   : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                               This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge   : analogous to upper_pred_edge but for the lower edge of the prediction interval
         - conc_est_min_loss : This function returns zero when the horizontal minimum current line intersects the best fit line. The concentration at the point of intersection is the 
@@ -929,16 +934,29 @@
                                              if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)             : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                              if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)               : details regarding the smoothing procedure used when building the curve
         - baseline     (str)               : details regarding the baseline procedure used when building the curve  
         - calibration  (str)               : details regarding the calibration procedure used when building the curve
-   
+        - fit_data     (list)              : a list containing the x,y data of the linear fit
+        - full_data    (list)              : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. This is not
+                                             necessary for fitting
+        
     Methods:
+        - fit             : performs quantile regression on x,y data
+                            The function returns estimated fit coefficients for three specified quantiles (default 0.025, 0.5, 0.975)
+                            and populates various attributes of the power_std_curve object including fit_params, low_edge_params,
+                            upp_edge_params, models, imin_std, imax_Std, imin_est, imax_est, conc_est_min, conc_est_max.
+
+                            Output: 3-entry list (one for each quantile). Each entry is of the form,
+                                                                    [
+                                                                    quantile (float), 
+                                                                    np.array([est of p0, est of p1, est of p2])
+                                                                    ]
         - predict         : returns the median quantile for the prediction, y, of the standard curve at a particular input, x.
         - details         : prints out a summary of the details of the standard curve
         - set_params      : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                             where the user is prompeted to enter each parameter, one after the other.
         - upper_pred_edge : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                             This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge : analogous to upper_pred_edge but for the lower edge of the prediction interval
@@ -948,15 +966,16 @@
    '''
     
     
     # How an instance of the class is initiated:
     def __init__(self, fit_params = np.array([0.,0.,0.]), low_edge_params = np.array([0.,0.,0.]), upp_edge_params = np.array([0.,0.,0.]), 
                  Elow=-2., Eupp=2., imin_est=0., imax_est=100., imin_std=0., imax_std=100.,
                  conc_est_min=0., conc_est_max=5., conc_std_min=0., conc_std_max=100., 
-                 smoothing='None', baseline='None', calibration='None'):
+                 smoothing='None', baseline='None', calibration='None', fit_data = [np.zeros(4), np.zeros(4)],
+                full_data=[]):
 
         self.fit_params      = fit_params
         self.low_edge_params = low_edge_params
         self.upp_edge_params = upp_edge_params
         self.Elow            = Elow
         self.Eupp            = Eupp
         self.imin_est        = imin_est
@@ -968,29 +987,125 @@
         self.conc_std_min    = conc_std_min
         self.conc_std_max    = conc_std_max
 
         self.smoothing       = smoothing
         self.baseline        = baseline
         self.calibration     = calibration
         
+        self.fit_data = fit_data
+        self.full_data = full_data
+        
                                          
         return
 
+    def fit(self, x_data, y_data, quantiles=[0.025, 0.5, 0.975], show_summary=True):     
+        def power_model(x, p0=0, p1=1, p2=1):
+            '''
+            Purpose: 
+                Map an argument, x, to a response, y, with a power law relationship given by:   f(x) = y = alpha*x^beta + gamma
+
+            Input:
+                - x  (float - array) : The argument for the power law function
+                - p2 (float)         : the coefficient in the power law function
+                - p1 (float)         : the exponent of the power law function
+                - p0 (float)         : the intercept of the power law function
+            Output:
+                - y  (float)         : The response of the argument, x, under the power law function/mapping
+            '''
+
+            y = p1*(x**p2) + p0
+            return y
+
+        def quantile_loss(q, y, f):
+            # q: Quantile to be evaluated, e.g., 0.5 for median.
+            # y: True value.
+            # f: Fitted (predicted) value.
+            e = y - f
+            return np.maximum(q * e, (q - 1) * e)
+
+
+        from scipy.optimize import curve_fit
+        bestest, covar = curve_fit(power_model, x_data, y_data, maxfev=2000) # the output of this is used as an intial guess in our quantile loss algorithm
+        from scipy.optimize import minimize as minimize
+        fit_results = []
+        for q in quantiles:
+            def power_quantileLoss(p):
+                obs  = y_data
+                nobs = len(obs)
+                loss = 0
+                for i in range(nobs):
+                    f = power_model(x_data[i], *p)
+                    loss+=quantile_loss(q, y_data[i], f)
+                return loss
+            fit_results.append([q, minimize(power_quantileLoss, x0=bestest,method='Nelder-Mead').x])
+
+        
+
+
+        p0_low = fit_results[0][1][0]
+        p0_mid = fit_results[1][1][0]
+        p0_upp = fit_results[2][1][0]
+        
+        p1_low = fit_results[0][1][1]
+        p1_mid = fit_results[1][1][1]
+        p1_upp = fit_results[2][1][1]
+        
+        p2_low = fit_results[0][1][2]
+        p2_mid = fit_results[1][1][2]
+        p2_upp = fit_results[2][1][2]
+        
+        
+       
+        
+        
+        self.fit_params[0]      = p0_mid
+        self.fit_params[1]      = p1_mid
+        self.fit_params[2]      = p2_mid
+        
+        self.low_edge_params[0]      = p0_low
+        self.low_edge_params[1]      = p1_low
+        self.low_edge_params[2]      = p2_low
+        
+        self.upp_edge_params[0]      = p0_upp
+        self.upp_edge_params[1]      = p1_upp
+        self.upp_edge_params[2]      = p2_upp
+       
+    
+        self.conc_std_min = min(x_data)
+        self.conc_std_max = max(x_data)
+        self.fit_data[0]  = x_data
+        self.fit_data[1]  = y_data
+
+        self.imin_std = self.predict(self.conc_std_min)
+        self.imax_std = self.predict(self.conc_std_max)
+        self.imin_est = self.upper_pred_edge(self.conc_std_min)
+        self.imax_est = self.lower_pred_edge(self.conc_std_max) 
+        
+        self.conc_est_min = least_squares(self.conc_est_min_loss, bounds = (self.conc_std_min, self.conc_std_max), x0 = (self.conc_std_min+self.conc_std_max)/2).x[0]
+        self.conc_est_max = least_squares(self.conc_est_max_loss, bounds = (self.conc_std_min, self.conc_std_max), x0 = (self.conc_std_min+self.conc_std_max)/2).x[0]
+
+        
+    
+        
+    
+        return fit_results
+    
+    
     # Function for printing out the attributes of the object
     def details(self):
-        print('Model : parabolic        --- y = p0 + p1*x^p2')                                                                           
-        print('[p0, p1, p2]     = {}'.format(self.fit_params))   
+        print('Model : power --- y = p0 + p1*x^p2')                                                                           
+        print('[p0, p1, p2]       = {}'.format(self.fit_params))   
         print('[p0_l, p1_l, p2_l] = {}'.format(self.low_edge_params))   
         print('[p0_u, p1_u, p2_u] = {}'.format(self.upp_edge_params))   
         print('')
         print('Elow                           = {}'.format(self.Elow))
         print('Eupp                           = {}'.format(self.Eupp))
         print('imin_est                       = {}'.format(self.imin_est))
         print('imax_est                       = {}'.format(self.imax_est))
-        print('imin_std                       = {}'.format(self.imax_std))
+        print('imin_std                       = {}'.format(self.imin_std))
         print('imax_std                       = {}'.format(self.imax_std))
         print('conc_est_min                   = {}'.format(self.conc_est_min))
         print('conc_est_max                   = {}'.format(self.conc_est_max))
         print('conc_std_min                   = {}'.format(self.conc_std_min))
         print('conc_std_max                   = {}'.format(self.conc_std_max))
         
         print('Smoothing Procedure            : {}'.format(self.smoothing))
@@ -1116,40 +1231,54 @@
                                           if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)          : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                           if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)            : details regarding the smoothing procedure used when building the curve
         - baseline     (str)            : details regarding the baseline procedure used when building the curve  
         - calibration  (str)            : details regarding the calibration procedure used when building the curve
+        - fit_data     (list)           : a list containing the x,y data of the linear fit
+        - full_data    (list)           : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. This is not
+                                          necessary for fitting
+        - models       (list)           : a list of the fitted linear models for each quantile - models are of statsmodels.formula.api.quantreg
    
     Methods:
+        - fit             : performs quantile regression using statsmodels.formula.api.quantreg.
+                            The function returns estimated fit coefficients for three specified quantiles (default 0.025, 0.5, 0.975)
+                            and populates various attributes of the linear_QR object including fit_params, low_edge_params,
+                            upp_edge_params, models, imin_std, imax_Std, imin_est, imax_est, conc_est_min, conc_est_max.
+
+                            Output: 3-entry list (one for each quantile). Each entry is of the form
+                                                                    [quantile (float), 
+                                                                    np.array([lower lim of intercept , est of intercept, upper lim of intercept]), 
+                                                                    np.array([lower lim of slope, est of slope, upper lim of slope]),
+                                                                    a linear quantile regression model from statsmodels.formula.api.quantreg]
+
+                                                                    where the intercept and slope limits are at alpha level 0.05
+
         - predict         : returns the median quantile for the prediction, y, of the standard curve at a particular input, x.
         - details         : prints out a summary of the details of the standard curve
         - set_params      : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                             where the user is prompeted to enter each parameter, one after the other.
         - upper_pred_edge : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                             This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge : analogous to upper_pred_edge but for the lower edge of the prediction interval
         - inv_pred        : Invert the predict function to obtain an estimate for x given a measured y
         - inv_low         : Invert the upper quantile function (upper_pred_edge) to obtain the lower limit for the estimate of x given a measured y
         - inv_upp         : Invert the lower quantile function (lower_pred_edge) to obtain the upper limit for the estimate of x given a measured y
     '''
     
-    '''
-    Future Ideas:
-        1 - Make quantiles customizable. I.e. instead of a fixed
-    
-    '''
+ 
 
 
-    # How an instance of the class is initiated:
+    # How an instance of the class is instatiated:
     def __init__(self, fit_params = np.array([0.,0.]), low_edge_params = np.array([0.,0.]), upp_edge_params = np.array([0.,0.]), 
                  Elow=-2., Eupp=2., imin_est=0., imax_est=100., imin_std=0., imax_std=100.,
                  conc_est_min=0., conc_est_max=5., conc_std_min=0., conc_std_max=100., 
-                 smoothing='None', baseline='None', calibration='None'):
+                 smoothing='None', baseline='None', calibration='None', fit_data = [np.zeros(3), np.zeros(3)],
+                full_data=[], models = []):
 
         self.fit_params      = fit_params
         self.low_edge_params = low_edge_params
         self.upp_edge_params = upp_edge_params
         self.Elow            = Elow
         self.Eupp            = Eupp
         self.imin_est        = imin_est
@@ -1161,17 +1290,96 @@
         self.conc_std_min    = conc_std_min
         self.conc_std_max    = conc_std_max
 
         self.smoothing       = smoothing
         self.baseline        = baseline
         self.calibration     = calibration
         
+        self.fit_data  = fit_data
+        self.full_data = full_data
+        self.models    = models
+        
                                          
         return
 
+    def fit(self, x_data, y_data, quantiles=[0.025, 0.5, 0.975], show_summary=True):     
+        import statsmodels.formula.api as smf
+        import pandas as pd
+        import math
+        data = pd.DataFrame(data={'X': x_data, 'Y':y_data})
+
+
+        mod = smf.quantreg('Y ~ X', data)
+        def fit_model(q):
+            modfit = mod.fit(q=q)
+            if show_summary:
+                print('---------------------------------------------')
+                print('---------------------------------------------')
+                print('---------------------------------------------')
+                print('---------------------------------------------')
+                print('Quantile: {}'.format(q))
+                print(modfit.summary())
+            return [q, 
+                    np.array([modfit.conf_int().loc['Intercept'][0], modfit.params['Intercept'], modfit.conf_int().loc['Intercept'][1]]), 
+                    np.array([modfit.conf_int().loc['X'][0], modfit.params['X'], modfit.conf_int().loc['X'][1]]),
+                    modfit] 
+        
+        fit_results = [fit_model(q) for q in quantiles]
+
+
+        slope_low = fit_results[0][2][1]
+        slope_mid = fit_results[1][2][1]
+        slope_upp = fit_results[2][2][1]
+        
+        int_low   = fit_results[0][1][1]
+        int_mid   = fit_results[1][1][1]
+        int_upp   = fit_results[2][1][1]
+        
+        mod_low   = fit_results[0][3]
+        mod_mid   = fit_results[1][3]
+        mod_upp   = fit_results[2][3]
+        
+        
+        
+        self.fit_params[0]      = int_mid
+        self.fit_params[1]      = slope_mid
+        
+        self.low_edge_params[0] = int_low
+        self.low_edge_params[1] = slope_low
+        
+        self.upp_edge_params[0] = int_upp
+        self.upp_edge_params[1] = slope_upp
+        self.models = [x[3] for x in fit_results]
+        
+        checklist = [int_low, slope_low, int_upp, slope_upp]
+        
+        checks = [math.isnan(x) for x in checklist]
+        
+        if any(checks):
+            print('Unable to compute some estimates. You may have insufficient data for chosen quantiles.\nTry raising lower quantile and/or lowering upper quantile.')
+            print('Recommend checking model summaries of output.')
+            return fit_results
+        self.conc_std_min = min(x_data)
+        self.conc_std_max = max(x_data)
+        self.fit_data[0]  = x_data
+        self.fit_data[1]  = y_data
+
+        self.imin_std = self.predict(self.conc_std_min)
+        self.imax_std = self.predict(self.conc_std_max)
+        self.imin_est = self.upper_pred_edge(self.conc_std_min)
+        self.imax_est = self.lower_pred_edge(self.conc_std_max) 
+        
+        self.conc_est_min = least_squares(self.conc_est_min_loss, bounds = (self.conc_std_min, self.conc_std_max), x0 = (self.conc_std_min+self.conc_std_max)/2).x[0]
+        self.conc_est_max = least_squares(self.conc_est_max_loss, bounds = (self.conc_std_min, self.conc_std_max), x0 = (self.conc_std_min+self.conc_std_max)/2).x[0]
+
+        
+       
+        return fit_results
+    
+    
     # Function for printing out the attributes of the object
     def details(self):
         print('Model : linear         --- y = p0 + p1*x')                                                                           
         print('[p0, p1]     = {}'.format(self.fit_params))   
         print('[p0_l, p1_l] = {}'.format(self.low_edge_params))   
         print('[p0_u, p1_u] = {}'.format(self.upp_edge_params))   
         print('')
@@ -1320,40 +1528,53 @@
                                              if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)             : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                              if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)               : details regarding the smoothing procedure used when building the curve
         - baseline     (str)               : details regarding the baseline procedure used when building the curve  
         - calibration  (str)               : details regarding the calibration procedure used when building the curve
+        - fit_data     (list)              : a list containing the x,y data of the lparabolic fit
+        - full_data    (list)              : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. This is not
+                                             necessary for fitting
+        - models       (list)              : a list of the fitted parabolic models for each quantile - models are of statsmodels.formula.api.quantreg
    
     Methods:
+        - fit             : performs quantile regression using statsmodels.formula.api.quantreg.
+                            The function returns estimated fit coefficients for three specified quantiles (default 0.025, 0.5, 0.975)
+                            and populates various attributes of the parabolic_QR object including fit_params, low_edge_params,
+                            upp_edge_params, models, imin_std, imax_Std, imin_est, imax_est, conc_est_min, conc_est_max.
+
+                        Output: 3-entry list (one for each quantile). Each entry is of the form
+                                                                    [quantile (float), 
+                                                                    np.array([lower lim of p0 , est of p0, upper lim of p0]), 
+                                                                    np.array([lower lim of p1 , est of p1, upper lim of p1]),
+                                                                    np.array([lower lim of p2 , est of p2, upper lim of p2])
+                                                                    a linear quantile regression model from statsmodels.formula.api.quantreg]
+
+                                                                where the p0, p1, p2 limits are at alpha level 0.05
+                                                                
         - predict         : returns the median quantile for the prediction, y, of the standard curve at a particular input, x.
         - details         : prints out a summary of the details of the standard curve
         - set_params      : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                             where the user is prompeted to enter each parameter, one after the other.
         - upper_pred_edge : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                             This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge : analogous to upper_pred_edge but for the lower edge of the prediction interval
         - inv_pred        : Invert the predict function to obtain an estimate for x given a measured y
         - inv_low         : Invert the upper quantile function (upper_pred_edge) to obtain the lower limit for the estimate of x given a measured y
         - inv_upp         : Invert the lower quantile function (lower_pred_edge) to obtain the upper limit for the estimate of x given a measured y
     '''
     
-    '''
-    Future Ideas:
-        1 - Make quantiles customizable. I.e. instead of a fixed
-    
-    '''
-
 
     # How an instance of the class is initiated:
     def __init__(self, fit_params = np.array([0.,0.,0.]), low_edge_params = np.array([0.,0.,0.]), upp_edge_params = np.array([0.,0.,0.]), 
                  Elow=-2., Eupp=2., imin_est=0., imax_est=100., imin_std=0., imax_std=100.,
                  conc_est_min=0., conc_est_max=5., conc_std_min=0., conc_std_max=100., 
-                 smoothing='None', baseline='None', calibration='None'):
+                 smoothing='None', baseline='None', calibration='None', fit_data = [np.zeros(4), np.zeros(4)],
+                full_data = [], models = []):
 
         self.fit_params      = fit_params
         self.low_edge_params = low_edge_params
         self.upp_edge_params = upp_edge_params
         self.Elow            = Elow
         self.Eupp            = Eupp
         self.imin_est        = imin_est
@@ -1365,29 +1586,117 @@
         self.conc_std_min    = conc_std_min
         self.conc_std_max    = conc_std_max
 
         self.smoothing       = smoothing
         self.baseline        = baseline
         self.calibration     = calibration
         
+        self.fit_data  = fit_data
+        self.full_data = full_data
+        self.models    = models
+        
                                          
         return
 
+    def fit(self, x_data, y_data, quantiles=[0.025, 0.5, 0.975], show_summary=True):     
+        import statsmodels.formula.api as smf
+        import pandas as pd
+        import math
+        data = pd.DataFrame(data={'X': x_data, 'X2' : x_data**2, 'Y':y_data})
+        mod  = smf.quantreg('Y ~ X2 + X', data)
+        
+        def fit_model(q):
+            modfit = mod.fit(q=q)
+            if show_summary:
+                print('---------------------------------------------')
+                print('---------------------------------------------')
+                print('---------------------------------------------')
+                print('---------------------------------------------')
+                print('Quantile: {}'.format(q))
+                print(modfit.summary())
+            return [q,
+                    np.array([modfit.conf_int().loc['Intercept'][0], modfit.params['Intercept'], modfit.conf_int().loc['Intercept'][1]]), 
+                    np.array([modfit.conf_int().loc['X'][0]        , modfit.params['X']        , modfit.conf_int().loc['X'][1]]), 
+                    np.array([modfit.conf_int().loc['X2'][0]       , modfit.params['X2']       , modfit.conf_int().loc['X2'][1]]),
+                    modfit
+                   ] 
+        models = [fit_model(x) for x in quantiles]
+        
+        fit_results = [fit_model(q) for q in quantiles]
+
+
+        p0_low = fit_results[0][1][1]
+        p0_mid = fit_results[1][1][1]
+        p0_upp = fit_results[2][1][1]
+        
+        p1_low = fit_results[0][2][1]
+        p1_mid = fit_results[1][2][1]
+        p1_upp = fit_results[2][2][1]
+        
+        p2_low = fit_results[0][3][1]
+        p2_mid = fit_results[1][3][1]
+        p2_upp = fit_results[2][3][1]
+        
+        
+       
+        
+        
+        self.fit_params[0]      = p0_mid
+        self.fit_params[1]      = p1_mid
+        self.fit_params[2]      = p2_mid
+        
+        self.low_edge_params[0]      = p0_low
+        self.low_edge_params[1]      = p1_low
+        self.low_edge_params[2]      = p2_low
+        
+        self.upp_edge_params[0]      = p0_upp
+        self.upp_edge_params[1]      = p1_upp
+        self.upp_edge_params[2]      = p2_upp
+        
+        self.models = [x[4] for x in fit_results]
+        
+        checklist = [p0_low, p1_low, p2_low, p0_upp, p1_upp, p2_upp]
+        
+        checks = [math.isnan(x) for x in checklist]
+        
+        if any(checks):
+            print('Unable to compute some estimates. You may have insufficient data for chosen quantiles.\nTry raising lower quantile and/or lowering upper quantile.')
+            print('Recommend checking model summaries of output.')
+            return fit_results
+        
+        self.conc_std_min = min(x_data)
+        self.conc_std_max = max(x_data)
+        self.fit_data[0]  = x_data
+        self.fit_data[1]  = y_data
+
+        self.imin_std = self.predict(self.conc_std_min)
+        self.imax_std = self.predict(self.conc_std_max)
+        self.imin_est = self.upper_pred_edge(self.conc_std_min)
+        self.imax_est = self.lower_pred_edge(self.conc_std_max) 
+        
+        self.conc_est_min = least_squares(self.conc_est_min_loss, bounds = (self.conc_std_min, self.conc_std_max), x0 = (self.conc_std_min+self.conc_std_max)/2).x[0]
+        self.conc_est_max = least_squares(self.conc_est_max_loss, bounds = (self.conc_std_min, self.conc_std_max), x0 = (self.conc_std_min+self.conc_std_max)/2).x[0]
+
+        
+       
+        return fit_results
+    
+    
     # Function for printing out the attributes of the object
     def details(self):
         print('Model : parabolic        --- y = p0 + p1*x + p2*x^2')                                                                           
         print('[p0, p1, p2]     = {}'.format(self.fit_params))   
         print('[p0_l, p1_l, p2_l] = {}'.format(self.low_edge_params))   
         print('[p0_u, p1_u, p2_u] = {}'.format(self.upp_edge_params))   
         print('')
         print('Elow                           = {}'.format(self.Elow))
         print('Eupp                           = {}'.format(self.Eupp))
         print('imin_est                       = {}'.format(self.imin_est))
         print('imax_est                       = {}'.format(self.imax_est))
-        print('imin_std                       = {}'.format(self.imax_std))
+        print('imin_std                       = {}'.format(self.imin_std))
         print('imax_std                       = {}'.format(self.imax_std))
         print('conc_est_min                   = {}'.format(self.conc_est_min))
         print('conc_est_max                   = {}'.format(self.conc_est_max))
         print('conc_std_min                   = {}'.format(self.conc_std_min))
         print('conc_std_max                   = {}'.format(self.conc_std_max))
         
         print('Smoothing Procedure            : {}'.format(self.smoothing))
@@ -1475,15 +1784,14 @@
         t2 = self.upp_edge_params[2]*x**2.
         t1 = self.upp_edge_params[1]*x
         t0 = self.upp_edge_params[0]
         y  =  t0 + t1 + t2
         return y
     
     def lower_pred_edge(self, x):   
-        
         t0 = self.low_edge_params[0]
         t1 = self.low_edge_params[1]*x
         t2 = self.low_edge_params[2]*x**2.
         
         y = t0 + t1 + t2
         return y
```

### Comparing `Ekidna-0.0.7/Ekidna.egg-info/PKG-INFO` & `Ekidna-0.0.8/Ekidna.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ekidna
-Version: 0.0.7
+Version: 0.0.8
 Summary: Electrochemistry data analysis tools
 Home-page: 
 Author: OzymandiasTheDead
 Author-email: jacob@ekidnasensing.com
 License: MIT
 Keywords: Ekidna
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,20 +21,17 @@
 
 The code is developed by researchers at Ekidna Sensing.
 
 
 
 Change Log
 ===========
-0.0.7 (June 30, 2023)
+0.0.8 (July 12, 2023)
 -------------------------
-- Seventh Release
+- Eighth Release
 
 Notes:
 ------
-Added standard curve classes: parabolic_QR, linear_QR, power_std_curve, parabolic_std_curve
+Added a fitting function to  classes parabolic_QR, linear_QR, power_std_curve, parabolic_std_curve, linear_std_curve
 
-The classes can be used to fit models to data. The classes also contain attriburtes such as estimation limits for inverse regression.
-Information such as smoothing, baseline subtraction, calibration procedures employed to process the data prior to fitting can also be stored.
 
-The prediction band edges of the standard curve are callable as methods within the objects. See documentation for full list of methods
-and attributes. 
+These classes can now use an internal curve fitting function and populate their parameters automatically after fitting.
```

### Comparing `Ekidna-0.0.7/LICENSE.txt` & `Ekidna-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ekidna-0.0.7/Module Contents.txt` & `Ekidna-0.0.8/Module Contents.txt`

 * *Files 14% similar despite different names*

```diff
@@ -26,16 +26,34 @@
                                              if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)             : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                              if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)               : details regarding the smoothing procedure used when building the curve
         - baseline     (str)               : details regarding the baseline procedure used when building the curve  
         - calibration  (str)               : details regarding the calibration procedure used when building the curve
+        - fit_data     (list)              : a list containing the x,y data of the lparabolic fit
+        - full_data    (list)              : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. This is not
+                                             necessary for fitting
+        - models       (list)              : a list of the fitted parabolic models for each quantile - models are of statsmodels.formula.api.quantreg
    
     Methods:
+        - fit             : performs quantile regression using statsmodels.formula.api.quantreg.
+                            The function returns estimated fit coefficients for three specified quantiles (default 0.025, 0.5, 0.975)
+                            and populates various attributes of the parabolic_QR object including fit_params, low_edge_params,
+                            upp_edge_params, models, imin_std, imax_Std, imin_est, imax_est, conc_est_min, conc_est_max.
+
+                        Output: 3-entry list (one for each quantile). Each entry is of the form
+                                                                    [quantile (float), 
+                                                                    np.array([lower lim of p0 , est of p0, upper lim of p0]), 
+                                                                    np.array([lower lim of p1 , est of p1, upper lim of p1]),
+                                                                    np.array([lower lim of p2 , est of p2, upper lim of p2])
+                                                                    a linear quantile regression model from statsmodels.formula.api.quantreg]
+
+                                                                where the p0, p1, p2 limits are at alpha level 0.05
+                                                                
         - predict         : returns the median quantile for the prediction, y, of the standard curve at a particular input, x.
         - details         : prints out a summary of the details of the standard curve
         - set_params      : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                             where the user is prompeted to enter each parameter, one after the other.
         - upper_pred_edge : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                             This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge : analogous to upper_pred_edge but for the lower edge of the prediction interval
@@ -70,16 +88,33 @@
                                           if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)          : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                           if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)            : details regarding the smoothing procedure used when building the curve
         - baseline     (str)            : details regarding the baseline procedure used when building the curve  
         - calibration  (str)            : details regarding the calibration procedure used when building the curve
+        - fit_data     (list)           : a list containing the x,y data of the linear fit
+        - full_data    (list)           : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. This is not
+                                          necessary for fitting
+        - models       (list)           : a list of the fitted linear models for each quantile - models are of statsmodels.formula.api.quantreg
    
     Methods:
+        - fit             : performs quantile regression using statsmodels.formula.api.quantreg.
+                            The function returns estimated fit coefficients for three specified quantiles (default 0.025, 0.5, 0.975)
+                            and populates various attributes of the linear_QR object including fit_params, low_edge_params,
+                            upp_edge_params, models, imin_std, imax_Std, imin_est, imax_est, conc_est_min, conc_est_max.
+
+                            Output: 3-entry list (one for each quantile). Each entry is of the form
+                                                                    [quantile (float), 
+                                                                    np.array([lower lim of intercept , est of intercept, upper lim of intercept]), 
+                                                                    np.array([lower lim of slope, est of slope, upper lim of slope]),
+                                                                    a linear quantile regression model from statsmodels.formula.api.quantreg]
+
+                                                                    where the intercept and slope limits are at alpha level 0.05
+
         - predict         : returns the median quantile for the prediction, y, of the standard curve at a particular input, x.
         - details         : prints out a summary of the details of the standard curve
         - set_params      : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                             where the user is prompeted to enter each parameter, one after the other.
         - upper_pred_edge : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                             This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge : analogous to upper_pred_edge but for the lower edge of the prediction interval
@@ -114,27 +149,41 @@
                                              if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)             : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                              if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)               : details regarding the smoothing procedure used when building the curve
         - baseline     (str)               : details regarding the baseline procedure used when building the curve  
         - calibration  (str)               : details regarding the calibration procedure used when building the curve
-   
+        - fit_data     (list)              : a list containing the x,y data of the linear fit
+        - full_data    (list)              : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. This is not
+                                             necessary for fitting
+        
     Methods:
+        - fit             : performs quantile regression on x,y data
+                            The function returns estimated fit coefficients for three specified quantiles (default 0.025, 0.5, 0.975)
+                            and populates various attributes of the power_std_curve object including fit_params, low_edge_params,
+                            upp_edge_params, models, imin_std, imax_Std, imin_est, imax_est, conc_est_min, conc_est_max.
+
+                            Output: 3-entry list (one for each quantile). Each entry is of the form,
+                                                                    [
+                                                                    quantile (float), 
+                                                                    np.array([est of p0, est of p1, est of p2])
+                                                                    ]
         - predict         : returns the median quantile for the prediction, y, of the standard curve at a particular input, x.
         - details         : prints out a summary of the details of the standard curve
         - set_params      : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                             where the user is prompeted to enter each parameter, one after the other.
         - upper_pred_edge : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                             This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge : analogous to upper_pred_edge but for the lower edge of the prediction interval
         - inv_pred        : Invert the predict function to obtain an estimate for x given a measured y
         - inv_low         : Invert the upper quantile function (upper_pred_edge) to obtain the lower limit for the estimate of x given a measured y
         - inv_upp         : Invert the lower quantile function (lower_pred_edge) to obtain the upper limit for the estimate of x given a measured y
 
+    
  --------------------------------------------------------------------------------------------------------------------
  --------------------------------------------------------------------------------------------------------------------
 class parabola_std_curve:
     Purpose:
         - To define a parabolic standard curve complete with prediction intervals, an error propagation formula for use with the delta method, 
           limits of estimation, and details about the creation of the curve, including smoothing parameters, baseline subtraction parameters,
           and calibration procedures.
@@ -158,34 +207,38 @@
                                           if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)          : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                           if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)            : details regarding the smoothing procedure used when building the curve
         - baseline     (str)            : details regarding the baseline procedure used when building the curve  
         - calibration  (str)            : details regarding the calibration procedure used when building the curve
+
+        - fit_data     (list)           : a list containing the x,y data for the data used to fit the parabolic model
+        - full_data    (list)           : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data. It is not necessary to fit.
     Methods/Functions:
+        - fit               : performs least-squares regression using scipy.optimize.curve_fit. The function returns estimated fit coefficients, their covariance matrix,
+                              and populates various attributes of the linear_std_curve object including s, standard range, estimation range.
         - predict           : returns the value, y, of the standard curve at a particular input, x. This is essentially the MLE for the system response to the input, x.
         - details           : prints out a summary of the details of the standard curve
         - errprop           : the error propagation formula for a parabola. This method returns the value of the variance of the response variable, y, at a given input, x.
         - upper_pred_edge   : returns the value of the upper edge of the prediction interval, with confidence alpha specified by the user, at a particular input, x.
                               This calculation makes use of the 'Delta Method' and uses the errprop method above within its calculation.
         - lower_pred_edge   : analogous to upper_pred_edge but for the lower edge of the prediction interval
         - conc_est_min_loss : This function returns zero when the horizontal minimum current line intersects the best fit line. The concentration at the point of intersection is the 
                               minimum concentration estimate that can be reported with a valid lower limit. We solve for the point of intersection via least-squares minimization
                               and use the result to instantiate the conc_est_min parameter of the curve object
         - conc_est_max_loss : This function returns zero when the horizontal maximum current line intersects the best fit line. The concentration at the point of intersection is the 
                               maximum concentration estimate that can be reported with a valid upper limit. We solve for the point of intersecgtions via least-squares minimization
                               and use the result to instatiate the conc_est_max parameter of the curve object.
         - set_params        : This function can be used to manually adjust the values of the curve's parameters. The user will be queried with a simple i/o question & answer algorithm
                               where the user is prompeted to enter each parameter, one after the other.
- 
  --------------------------------------------------------------------------------------------------------------------
  --------------------------------------------------------------------------------------------------------------------
 class linear_std_curve:
-    Purpose:
+     Purpose:
         - To define a linear standard curve complete with prediction intervals, an error propagation formula for use with the delta method, 
           limits of estimation, and details about the creation of the curve, including smoothing parameters, baseline subtraction parameters,
           and calibration procedures.
     
     Attributes:
         - fit_params   (1D array/float) : An array containing the values of the fit coefficients of the linear model. form: [p0, p1], where linear(x) = p0 + p1*x
         - covar        (2D array/float) : the covariance matrix of the fit coefficients
@@ -205,14 +258,16 @@
                                           if the MLE is between conc_std_min and conc_est_min (i.e. the lower limit will require extrapolation of the prediction band's upper edge to be calculated... this is risky and is not recommended)
         - conc_std_max (float)          : the largest concentration of all the std pts. Any MLE below this value and above conc_std_min is a valid MLE. However, the upper limit on the estimate will not be valid
                                           if the MLE is between conc_std_ax and conc_est_max (i.e. the upper limit will require extrapolation of the prediction band's lower edge to be calculated... this is risky and is not recommended)
       
         - smoothing    (str)            : details regarding the smoothing procedure used when building the curve
         - baseline     (str)            : details regarding the baseline procedure used when building the curve  
         - calibration  (str)            : details regarding the calibration procedure used when building the curve
+        - fit_data     (list)           : a list containing the x,y data for fitting a linear model
+        - full_data    (list)           : if fit_data is a result of processing an original dataset, this attribute can be used to house the original, unprocessed data
    
     Methods/Functions:
         - fit             : performs least-squares regression using scipy.optimize.curve_fit. The function returns estimated fit coefficients, their covariance matrix,
                             and also populate various attributes of the linear_std_curve object including s, standard range, estimation range.
         - predict         : returns the value, y, of the standard curve at a particular input, x. This is essentially the MLE for the system response to the input, x.
         - details         : prints out a summary of the details of the standard curve
         - errprop         : the error propagation formula for a parabola. This method returns the value of the variance of the response variable, y, at a given input, x.
```

### Comparing `Ekidna-0.0.7/PKG-INFO` & `Ekidna-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ekidna
-Version: 0.0.7
+Version: 0.0.8
 Summary: Electrochemistry data analysis tools
 Home-page: 
 Author: OzymandiasTheDead
 Author-email: jacob@ekidnasensing.com
 License: MIT
 Keywords: Ekidna
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -21,20 +21,17 @@
 
 The code is developed by researchers at Ekidna Sensing.
 
 
 
 Change Log
 ===========
-0.0.7 (June 30, 2023)
+0.0.8 (July 12, 2023)
 -------------------------
-- Seventh Release
+- Eighth Release
 
 Notes:
 ------
-Added standard curve classes: parabolic_QR, linear_QR, power_std_curve, parabolic_std_curve
+Added a fitting function to  classes parabolic_QR, linear_QR, power_std_curve, parabolic_std_curve, linear_std_curve
 
-The classes can be used to fit models to data. The classes also contain attriburtes such as estimation limits for inverse regression.
-Information such as smoothing, baseline subtraction, calibration procedures employed to process the data prior to fitting can also be stored.
 
-The prediction band edges of the standard curve are callable as methods within the objects. See documentation for full list of methods
-and attributes. 
+These classes can now use an internal curve fitting function and populate their parameters automatically after fitting.
```

### Comparing `Ekidna-0.0.7/setup.py` & `Ekidna-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Ekidna',
-    version='0.0.7',
+    version='0.0.8',
     description='Electrochemistry data analysis tools',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='OzymandiasTheDead',
     author_email='jacob@ekidnasensing.com',
     license='MIT',
     classifiers=classifiers,
```

