# Comparing `tmp/NeuralFoil-0.1.3.tar.gz` & `tmp/NeuralFoil-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralFoil-0.1.3.tar", last modified: Mon Jul 10 21:58:11 2023, max compression
+gzip compressed data, was "NeuralFoil-0.1.4.tar", last modified: Wed Jul 12 01:31:53 2023, max compression
```

## Comparing `NeuralFoil-0.1.3.tar` & `NeuralFoil-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.230127 NeuralFoil-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.226127 NeuralFoil-0.1.3/NeuralFoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 21:58:11.000000 NeuralFoil-0.1.3/NeuralFoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-07-10 21:58:11.230127 NeuralFoil-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.226127 NeuralFoil-0.1.3/neuralfoil/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/CL_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/neuralfoil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:58:11.226127 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/
--rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-large.npz
--rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-medium.npz
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-small.npz
--rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:58:11.230127 NeuralFoil-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-10 21:57:56.000000 NeuralFoil-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.902888 NeuralFoil-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.894888 NeuralFoil-0.1.4/NeuralFoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 01:31:53.000000 NeuralFoil-0.1.4/NeuralFoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22899 2023-07-12 01:31:53.902888 NeuralFoil-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21867 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.894888 NeuralFoil-0.1.4/neuralfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/CL_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/neuralfoil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:31:53.898888 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/
+-rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-large.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-medium.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:31:53.902888 NeuralFoil-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-12 01:31:39.000000 NeuralFoil-0.1.4/setup.py
```

### Comparing `NeuralFoil-0.1.3/LICENSE.txt` & `NeuralFoil-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/NeuralFoil.egg-info/PKG-INFO` & `NeuralFoil-0.1.4/NeuralFoil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.3
+Version: 0.1.4
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -101,20 +101,19 @@
 NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
-This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild".
+This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild". The second set of columns gives the runtime speed of the models, both for a single analysis and for a large batch analysis.
 
-<a name="table"></a>
-<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
+<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>1 ms</td><td>0.020 sec</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>3 ms</td><td>0.190 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>4 ms</td><td>0.284 sec</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>4 ms</td><td>0.402 sec</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>5 ms</td><td>0.784 sec</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>6 ms</td><td>1.754 sec</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>10 ms</td><td>3.330 sec</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>13 ms</td><td>4.297 sec</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>38 ms</td><td>8.980 sec</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>73 ms</td><td>42 min</td></tr></tbody></table>
 
-> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may be better than the numbers in this table.
+> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may differ (in either direction) from the numbers in this table.
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
@@ -155,15 +154,15 @@
 
 <a name="xfoil-benefit-question"></a>
 Why not just use XFoil directly?
 
 > XFoil is a truly excellent piece of aerospace software engineering and is the gold standard of airfoil analysis, for good reason. When its assumptions hold (airfoils in subsonic flow without massive separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower computational cost. XFoil shines in particular for human-in-the-loop airfoil design. However, XFoil is not the right tool for all applications, for a few reasons:
 >
 > - XFoil exhibits hysteresis: you can get slightly different solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you sweep $\alpha$ up or down, as Newton iteration is resumed from the last converged solution and uniqueness is not guaranteed. This hysteresis can be a big problem for design optimization.
-> - XFoil is not differentiable, in the sense that it doesn't tell you how performance changes w.r.t. airfoil shape (via, for example, an adjoint). That's okay—NeuralFoil doesn't either, at least out-of-the-box. However, the "path to obtain an efficient gradient" is very straightforward for NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX). In contrast, gradient options XFoil's Fortran code either don't exist or are significantly less advanced (e.g., Tapenade).
+> - XFoil is not differentiable, in the sense that it doesn't tell you how performance changes w.r.t. airfoil shape (via, for example, an adjoint). That's okay—NeuralFoil doesn't either, at least out-of-the-box. However, the "path to obtain an efficient gradient" is very straightforward for NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX). In contrast, gradient options for Fortran code (the language XFoil is in) either don't exist or are significantly less advanced (e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL](https://github.com/mdolab/CMPLXFOIL), which computes complex-step (effectively, forward-mode) gradients. However, even if you can get a gradient, it still may present issues, because...
 > - XFoil's solutions lack $C^1$-continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous by construction. This is critical for gradient-based optimization.
 > 	- Even if one tries to compute gradients of XFoil's outputs by finite-differencing or complex-stepping, these gradients are often inaccurate.
 >   - A bit into the weeds, but: this comes down to how XFoil handles transition (onset of turbulence). XFoil does a cut-cell approach on the transitioning interval, and while this specific cut-cell implementation restores $C^0$-continuity (i.e., transition won't truly "jump" from one node to another discretely), gradients of the laminar and turbulent BL closure functions still change at the cell interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic level. In theory $C^1$-continuity could be restored by also blending the BL shape variables through the transitioning cell interval, but that unleashes some ugly integrals and is not done in XFoil.
 >      - For more on this, see [Adler, Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/~mdolaboratory/pdf/Adler2022c.pdf), Figure 7.
 > - While XFoil is ~1000x faster than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil](#performance). NeuralFoil is also much easier to interface with on a memory level than XFoil, which means you won't find yourself I/O bound from file reading/writing like you will with XFoil.
 > - XFoil is not vectorized, which exacerbates the speed advantage of a (vectorized) neural network when analyzing large batches of airfoil cases simultaneously.
 > - XFoil is not guaranteed to produce a solution. Instead, XFoil often crashes when "ambitious" calculations are attempted, rather than producing a less-accurate answer. In some applications, that's okay or even desirable; in others, that's a dealbreaker. Example applications where this is a problem include:
@@ -172,15 +171,15 @@
 >   - Design optimization, where the optimizer needs "an answer" in order to recover from a bad design point and send the search back to a reasonable design.
 > - XFoil can be a serious pain to compile from source, which is often required if running on Mac or Linux (i.e., all supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so it's easy to install and run anywhere.
 
 Why not use a neural network trained on RANS CFD instead?
 
 > This is not a bad idea, and it has been done (See [Bouhlel, He, and Martins, "Scalable gradient-enhanced artificial..."](https://link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental challenge here, of course, is the cost of training data. RANS CFD is much more expensive than XFoil, so it's much harder to get the training data needed to train a neural network. For example, in the linked work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD runs (and they were sweeping over Mach as well, so the data becomes even sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the airfoil design space, which is critical for accurate predictions on out-of-sample airfoils.
 >
-> One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn directly quantifies the critical Mach number (beyond which simple models, like normal-shock total-pressure-loss relations or the [Korn equation heuristic](https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to extend the Mach region of validity slightly further). But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where XFoil is more accurate than RANS CFD.
+> One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn allows you to estimate the critical Mach number via Prandtl-Glauert correction (beyond which simple models, like normal-shock total-pressure-loss relations or the [Korn equation heuristic](https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to extend the Mach region of validity slightly further). But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where XFoil is more accurate than RANS CFD.
 
 Why not use a neural network trained on wind tunnel data?
 
 > This is a super-cool idea, and I'd love to see someone try it! My guess is that you'd need some kind of morphing wing section (and a way of precisely measuring the shape) in order to get enough data samples to "span" the airfoil design space. Then, you'd just let the wing section sit in the wind tunnel for a few days morphing itself around to collect data, then train a model on that. This would be really awesome, someone should do it!
 
 <a name="compressibility-question"></a>
 NeuralFoil is trained on incompressible ($M=0$) XFoil data. Why not train on compressible ($M>0$) XFoil data? Also, how can I use NeuralFoil to predict compressible airfoil performance?
@@ -190,14 +189,31 @@
 <a name="parameterization-question"></a>
 Why parameterize the airfoil geometry using the CST (Kulfan) parameterization? What exactly does the CST parameterization mean, and how can I convert this parameterization to/from actual airfoil coordinates? Why discretize with 8 CST modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing edges?
 
 > To be written, but in the meantime read:
 > - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
 > - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
 
+What's the underlying neural network architecture used in NeuralFoil?
+
+> To be written, but it is essentially a feed-forward neural network with a varying number of total layers and layer width depending on model size. Layer counts and widths were [determined through extensive trial and error](./training/supercloud_job_id_notes.log), in conjunction with observed test- and train-loss values. All layers are dense (fully connected, with weights and biases). All activation functions between layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and layer width are as follows:
+>
+> * xxsmall: 2 layers,  32 wide.
+> * xsmall:  3 layers,  32 wide.
+> * small:   3 layers,  48 wide.
+> * medium:  4 layers,  64 wide.
+> * large:   4 layers, 128 wide.
+> * xlarge:  4 layers, 256 wide.
+> * xxlarge: 5 layers, 256 wide.
+> * xxxlarge:5 layers, 512 wide.
+
+## Acknowledgements
+
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). 
+
 ## License
 
 NeuralFoil is licensed under the MIT license. Please see the [LICENSE](LICENSE.txt) file for details.
 
 ## Citing NeuralFoil
 
 If you use NeuralFoil in your research, please cite it as follows:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.3 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.4 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -74,65 +74,74 @@
 respect to XFoil more precisely. At a basic level, we care about two things: -
 **Accuracy**: how close are the predictions to XFoil's? - **Computational
 Cost**: how long does it take to run? This table details both of these
 considerations. The first few columns show the error with respect to XFoil on
 the test dataset. [The test dataset is completely isolated from the training
 dataset, and NeuralFoil was not allowed to learn from the test dataset]
 (#geometry-parameterization-and-training-data). Thus, the performance on the
-test dataset gives a good idea of NeuralFoil's performance "in the wild".
-Aerodynamics Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset,  Computational
-Model        with respect to XFoil                                                             Cost to Run
+test dataset gives a good idea of NeuralFoil's performance "in the wild". The
+second set of columns gives the runtime speed of the models, both for a single
+analysis and for a large batch analysis.
+Aerodynamics Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to   Computational
+Model        XFoil                                                                             Cost to Run
                                                                                         Bottom
                                                                              Top        Trans.         Total
              Lift   Fractional Drag   Moment Max Overspeed                   Transition Loc.   Runtime Runtime
              Coeff. Coeff.            Coeff. $u_\max / u_\infty$   â¡ Loc.       $x_    (1 run) (100,000
              $C_L$  $\ln(C_D)$ â  $C_M$                                  $x_{tr,    {tr,           runs)
                                                                              top}/c$    bot}/
                                                                                         c$
-NF Linear    0.116  -                 -      -                               -          -      18 ms   0.020 s
-$C_L$ Model
-NF "xxsmall" 0.065  0.121             0.010  0.215                           0.073      0.100  27 ms   0.204
+NF Linear    0.116  -                 -      -                               -          -      1 ms    0.020
+$C_L$ Model                                                                                            sec
+NF "xxsmall" 0.065  0.121             0.010  0.215                           0.073      0.100  3 ms    0.190
                                                                                                        sec
-NF "xsmall"  0.042  0.075             0.007  0.134                           0.039      0.055  29 ms   0.304 s
-NF "small"   0.039  0.069             0.006  0.122                           0.036      0.050  31 ms   0.437 s
-NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  33 ms   0.749 s
-NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  35 ms   1.542 s
-NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  36 ms   3.495 s
-NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  39 ms   4.557 s
-NF           0.020  0.039             0.003  0.070                           0.016      0.024  65 ms   11.633 s
-"xxxlarge"
-XFoil        0      0                 0      0                               0          0      447 ms  3610 sec
+NF "xsmall"  0.042  0.075             0.007  0.134                           0.039      0.055  4 ms    0.284
+                                                                                                       sec
+NF "small"   0.039  0.069             0.006  0.122                           0.036      0.050  4 ms    0.402
+                                                                                                       sec
+NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  5 ms    0.784
+                                                                                                       sec
+NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  6 ms    1.754
+                                                                                                       sec
+NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  10 ms   3.330
+                                                                                                       sec
+NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  13 ms   4.297
+                                                                                                       sec
+NF           0.020  0.039             0.003  0.070                           0.016      0.024  38 ms   8.980
+"xxxlarge"                                                                                             sec
+XFoil        0      0                 0      0                               0          0      73 ms   42 min
 > â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
 error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm)
 of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to
 within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil
-is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly
+is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly
 not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure
-above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may
-be better than the numbers in this table. > > â¡ This "maximum overspeed" lets
-you compute $C_{p,\min}$, which can be used to calculate the critical Mach
-number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
-Based on these performance numbers, you can select the right tradeoff between
-accuracy and computational cost for your application. In general, I recommend
-starting with the "large" model and adjusting from there. In addition to
-accuracy vs. speed, another consideration when choosing the right model is what
-you're trying to use NeuralFoil for. Larger models will be more complicated
-("less parsimonious," as the math kids would say), which means that they may
-have more "wiggles" in their outputsâthis might be undesirable for gradient-
-based optimization. On the other hand, larger models will be able to capture a
-wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
-be seen mid-optimization), so larger models could have a benefit in that sense.
-If you try a specific application and have better/worse results with a specific
-model, let me know by opening a GitHub issue! Notably, most of the
-computational overhead of calling NeuralFoil is actually in the airfoil
-preprocessing step, where the airfoil is converted from a set of coordinates to
-a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-
-and-training-data)) - not in the aerodynamics analysis itself. This pre-
-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear
-solvers](https://github.com/peterdsharpe/AeroSandbox/blob/
+above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may
+differ (in either direction) from the numbers in this table. > > â¡ This
+"maximum overspeed" lets you compute $C_{p,\min}$, which can be used to
+calculate the critical Mach number $M_\mathrm{crit}$. [More details below.]
+(#compressibility-question) Based on these performance numbers, you can select
+the right tradeoff between accuracy and computational cost for your
+application. In general, I recommend starting with the "large" model and
+adjusting from there. In addition to accuracy vs. speed, another consideration
+when choosing the right model is what you're trying to use NeuralFoil for.
+Larger models will be more complicated ("less parsimonious," as the math kids
+would say), which means that they may have more "wiggles" in their
+outputsâthis might be undesirable for gradient-based optimization. On the
+other hand, larger models will be able to capture a wider range of airfoils
+(e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-
+optimization), so larger models could have a benefit in that sense. If you try
+a specific application and have better/worse results with a specific model, let
+me know by opening a GitHub issue! Notably, most of the computational overhead
+of calling NeuralFoil is actually in the airfoil preprocessing step, where the
+airfoil is converted from a set of coordinates to a CST (Kulfan)
+parameterization ([more info here](#geometry-parameterization-and-training-
+data)) - not in the aerodynamics analysis itself. This pre-processing takes
+around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://
+github.com/peterdsharpe/AeroSandbox/blob/
 c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/
 airfoil_families.py#L265), but in theory a pure-NumPy implementation is
 possible that would be much faster by exploiting linearity (sub-millisecond).
 If you're interested in working on this, open an issue and let me know! In the
 meantime, you can eliminate this overhead by using
 [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to
 one of NeuralFoil's other functions. ## Installation [Install from PyPI](https:
@@ -179,94 +188,112 @@
 sweep $\alpha$ up or down, as Newton iteration is resumed from the last
 converged solution and uniqueness is not guaranteed. This hysteresis can be a
 big problem for design optimization. > - XFoil is not differentiable, in the
 sense that it doesn't tell you how performance changes w.r.t. airfoil shape
 (via, for example, an adjoint). That's okayâNeuralFoil doesn't either, at
 least out-of-the-box. However, the "path to obtain an efficient gradient" is
 very straightforward for NeuralFoil's pure NumPy code, where many excellent
-options exist (e.g., JAX). In contrast, gradient options XFoil's Fortran code
-either don't exist or are significantly less advanced (e.g., Tapenade). > -
-XFoil's solutions lack $C^1$-continuity. NeuralFoil, by contrast, is guaranteed
-to be $C^\infty$-continuous by construction. This is critical for gradient-
-based optimization. > - Even if one tries to compute gradients of XFoil's
-outputs by finite-differencing or complex-stepping, these gradients are often
-inaccurate. > - A bit into the weeds, but: this comes down to how XFoil handles
-transition (onset of turbulence). XFoil does a cut-cell approach on the
-transitioning interval, and while this specific cut-cell implementation
-restores $C^0$-continuity (i.e., transition won't truly "jump" from one node to
-another discretely), gradients of the laminar and turbulent BL closure
-functions still change at the cell interface due to the differing BL parameters
-($H$ and $Re_\theta$) from node to node. This loses $C^1$ continuity, causing a
-"ragged" polar at the microscopic level. In theory $C^1$-continuity could be
-restored by also blending the BL shape variables through the transitioning cell
-interval, but that unleashes some ugly integrals and is not done in XFoil. > -
-For more on this, see [Adler, Gray, and Martins, "To CFD or not to CFD?..."]
-(http://websites.umich.edu/~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > -
-While XFoil is ~1000x faster than RANS CFD, NeuralFoil [can be another ~1000x
-faster to evaluate than XFoil](#performance). NeuralFoil is also much easier to
-interface with on a memory level than XFoil, which means you won't find
-yourself I/O bound from file reading/writing like you will with XFoil. > -
-XFoil is not vectorized, which exacerbates the speed advantage of a
-(vectorized) neural network when analyzing large batches of airfoil cases
-simultaneously. > - XFoil is not guaranteed to produce a solution. Instead,
-XFoil often crashes when "ambitious" calculations are attempted, rather than
-producing a less-accurate answer. In some applications, that's okay or even
-desirable; in others, that's a dealbreaker. Example applications where this is
-a problem include: > - Real-time control, where one wants to estimate forces
-(e.g., for a MPC trajectory), but you can't have the controller crash if XFoil
-fails to converge or hangs the CPU. > - Flight simulation: similar to real-time
-control where "a less-accurate answer" is much better than "no answer." > -
-Design optimization, where the optimizer needs "an answer" in order to recover
-from a bad design point and send the search back to a reasonable design. > -
-XFoil can be a serious pain to compile from source, which is often required if
-running on Mac or Linux (i.e., all supercomputers, some lab computers).
-NeuralFoil is pure Python and NumPy, so it's easy to install and run anywhere.
-Why not use a neural network trained on RANS CFD instead? > This is not a bad
-idea, and it has been done (See [Bouhlel, He, and Martins, "Scalable gradient-
-enhanced artificial..."](https://link.springer.com/article/10.1007/s00158-020-
-02488-5))! The fundamental challenge here, of course, is the cost of training
-data. RANS CFD is much more expensive than XFoil, so it's much harder to get
-the training data needed to train a neural network. For example, in the linked
-work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD
-runs (and they were sweeping over Mach as well, so the data becomes even
-sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil
-runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the
-airfoil design space, which is critical for accurate predictions on out-of-
-sample airfoils. > > One advantage of a RANS CFD approach over the NeuralFoil
-XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get
-around this a little bit by estimating $C_{p, min}$, which in turn directly
-quantifies the critical Mach number (beyond which simple models, like normal-
-shock total-pressure-loss relations or the [Korn equation heuristic](https://
-archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to
-extend the Mach region of validity slightly further). But fundamentally,
-NeuralFoil is likely less accurate in the transonic range because of this. The
-tradeoff is that the much larger training data set allows NeuralFoil to be more
-accurate in the subsonic range, where XFoil is more accurate than RANS CFD. Why
-not use a neural network trained on wind tunnel data? > This is a super-cool
-idea, and I'd love to see someone try it! My guess is that you'd need some kind
-of morphing wing section (and a way of precisely measuring the shape) in order
-to get enough data samples to "span" the airfoil design space. Then, you'd just
-let the wing section sit in the wind tunnel for a few days morphing itself
-around to collect data, then train a model on that. This would be really
-awesome, someone should do it!  NeuralFoil is trained on incompressible ($M=0$)
-XFoil data. Why not train on compressible ($M>0$) XFoil data? Also, how can I
-use NeuralFoil to predict compressible airfoil performance? > To be written.
-But basically: $u_\max / u_\infty$ from NeuralFoil $\longrightarrow C_{p, \min,
-M=0} \longrightarrow C_{p, \min}$ using Prandtl-Glauert correction
-$\longrightarrow$ compare to $C_{p,\mathrm{sonic}}$ to determine the extent to
-which $M_\mathrm{crit}$ is exceeded.  Why parameterize the airfoil geometry
-using the CST (Kulfan) parameterization? What exactly does the CST
-parameterization mean, and how can I convert this parameterization to/from
-actual airfoil coordinates? Why discretize with 8 CST modes per side? Can
-NeuralFoil accurately analyze airfoils with thick trailing edges? > To be
-written, but in the meantime read: > - [D. A. Masters, "Geometric Comparison of
-Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://
-arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal paper on the CST
-(Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric
-Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) ##
-License NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
+options exist (e.g., JAX). In contrast, gradient options for Fortran code (the
+language XFoil is in) either don't exist or are significantly less advanced
+(e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL]
+(https://github.com/mdolab/CMPLXFOIL), which computes complex-step
+(effectively, forward-mode) gradients. However, even if you can get a gradient,
+it still may present issues, because... > - XFoil's solutions lack $C^1$-
+continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous
+by construction. This is critical for gradient-based optimization. > - Even if
+one tries to compute gradients of XFoil's outputs by finite-differencing or
+complex-stepping, these gradients are often inaccurate. > - A bit into the
+weeds, but: this comes down to how XFoil handles transition (onset of
+turbulence). XFoil does a cut-cell approach on the transitioning interval, and
+while this specific cut-cell implementation restores $C^0$-continuity (i.e.,
+transition won't truly "jump" from one node to another discretely), gradients
+of the laminar and turbulent BL closure functions still change at the cell
+interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to
+node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic
+level. In theory $C^1$-continuity could be restored by also blending the BL
+shape variables through the transitioning cell interval, but that unleashes
+some ugly integrals and is not done in XFoil. > - For more on this, see [Adler,
+Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/
+~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster
+than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil]
+(#performance). NeuralFoil is also much easier to interface with on a memory
+level than XFoil, which means you won't find yourself I/O bound from file
+reading/writing like you will with XFoil. > - XFoil is not vectorized, which
+exacerbates the speed advantage of a (vectorized) neural network when analyzing
+large batches of airfoil cases simultaneously. > - XFoil is not guaranteed to
+produce a solution. Instead, XFoil often crashes when "ambitious" calculations
+are attempted, rather than producing a less-accurate answer. In some
+applications, that's okay or even desirable; in others, that's a dealbreaker.
+Example applications where this is a problem include: > - Real-time control,
+where one wants to estimate forces (e.g., for a MPC trajectory), but you can't
+have the controller crash if XFoil fails to converge or hangs the CPU. > -
+Flight simulation: similar to real-time control where "a less-accurate answer"
+is much better than "no answer." > - Design optimization, where the optimizer
+needs "an answer" in order to recover from a bad design point and send the
+search back to a reasonable design. > - XFoil can be a serious pain to compile
+from source, which is often required if running on Mac or Linux (i.e., all
+supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so
+it's easy to install and run anywhere. Why not use a neural network trained on
+RANS CFD instead? > This is not a bad idea, and it has been done (See [Bouhlel,
+He, and Martins, "Scalable gradient-enhanced artificial..."](https://
+link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental
+challenge here, of course, is the cost of training data. RANS CFD is much more
+expensive than XFoil, so it's much harder to get the training data needed to
+train a neural network. For example, in the linked work by Bouhlel et al., the
+authors trained a neural network on 42,000 RANS CFD runs (and they were
+sweeping over Mach as well, so the data becomes even sparser). In contrast,
+NeuralFoil was trained on tens of millions of XFoil runs. Ultimately, this
+exposes NeuralFoil to a much larger "span" of the airfoil design space, which
+is critical for accurate predictions on out-of-sample airfoils. > > One
+advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of
+course, transonic modeling. NeuralFoil attempts to get around this a little bit
+by estimating $C_{p, min}$, which in turn allows you to estimate the critical
+Mach number via Prandtl-Glauert correction (beyond which simple models, like
+normal-shock total-pressure-loss relations or the [Korn equation heuristic]
+(https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be
+used to extend the Mach region of validity slightly further). But
+fundamentally, NeuralFoil is likely less accurate in the transonic range
+because of this. The tradeoff is that the much larger training data set allows
+NeuralFoil to be more accurate in the subsonic range, where XFoil is more
+accurate than RANS CFD. Why not use a neural network trained on wind tunnel
+data? > This is a super-cool idea, and I'd love to see someone try it! My guess
+is that you'd need some kind of morphing wing section (and a way of precisely
+measuring the shape) in order to get enough data samples to "span" the airfoil
+design space. Then, you'd just let the wing section sit in the wind tunnel for
+a few days morphing itself around to collect data, then train a model on that.
+This would be really awesome, someone should do it!  NeuralFoil is trained on
+incompressible ($M=0$) XFoil data. Why not train on compressible ($M>0$) XFoil
+data? Also, how can I use NeuralFoil to predict compressible airfoil
+performance? > To be written. But basically: $u_\max / u_\infty$ from
+NeuralFoil $\longrightarrow C_{p, \min, M=0} \longrightarrow C_{p, \min}$ using
+Prandtl-Glauert correction $\longrightarrow$ compare to $C_{p,\mathrm{sonic}}$
+to determine the extent to which $M_\mathrm{crit}$ is exceeded.  Why
+parameterize the airfoil geometry using the CST (Kulfan) parameterization? What
+exactly does the CST parameterization mean, and how can I convert this
+parameterization to/from actual airfoil coordinates? Why discretize with 8 CST
+modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing
+edges? > To be written, but in the meantime read: > - [D. A. Masters,
+"Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA
+Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal
+paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan,
+"Universal Parametric Geometry Representation Method"](http://
+mx1.brendakulfan.com/docs/CST6.pdf) What's the underlying neural network
+architecture used in NeuralFoil? > To be written, but it is essentially a feed-
+forward neural network with a varying number of total layers and layer width
+depending on model size. Layer counts and widths were [determined through
+extensive trial and error](./training/supercloud_job_id_notes.log), in
+conjunction with observed test- and train-loss values. All layers are dense
+(fully connected, with weights and biases). All activation functions between
+layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and
+layer width are as follows: > > * xxsmall: 2 layers, 32 wide. > * xsmall: 3
+layers, 32 wide. > * small: 3 layers, 48 wide. > * medium: 4 layers, 64 wide. >
+* large: 4 layers, 128 wide. > * xlarge: 4 layers, 256 wide. > * xxlarge: 5
+layers, 256 wide. > * xxxlarge:5 layers, 512 wide. ## Acknowledgements
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster
+operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). ## License
+NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
 (LICENSE.txt) file for details. ## Citing NeuralFoil If you use NeuralFoil in
 your research, please cite it as follows: ``` @misc{neuralfoil, author = {Peter
 Sharpe}, title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using
 physics-informed machine learning}, year = {2023}, publisher = {GitHub},
 journal = {GitHub repository}, howpublished = {\url{https://github.com/
 peterdsharpe/NeuralFoil}}, ```
```

### Comparing `NeuralFoil-0.1.3/NeuralFoil.egg-info/SOURCES.txt` & `NeuralFoil-0.1.4/NeuralFoil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/PKG-INFO` & `NeuralFoil-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.3
+Version: 0.1.4
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -101,20 +101,19 @@
 NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
-This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild".
+This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild". The second set of columns gives the runtime speed of the models, both for a single analysis and for a large batch analysis.
 
-<a name="table"></a>
-<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
+<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>1 ms</td><td>0.020 sec</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>3 ms</td><td>0.190 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>4 ms</td><td>0.284 sec</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>4 ms</td><td>0.402 sec</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>5 ms</td><td>0.784 sec</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>6 ms</td><td>1.754 sec</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>10 ms</td><td>3.330 sec</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>13 ms</td><td>4.297 sec</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>38 ms</td><td>8.980 sec</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>73 ms</td><td>42 min</td></tr></tbody></table>
 
-> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may be better than the numbers in this table.
+> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may differ (in either direction) from the numbers in this table.
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
@@ -155,15 +154,15 @@
 
 <a name="xfoil-benefit-question"></a>
 Why not just use XFoil directly?
 
 > XFoil is a truly excellent piece of aerospace software engineering and is the gold standard of airfoil analysis, for good reason. When its assumptions hold (airfoils in subsonic flow without massive separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower computational cost. XFoil shines in particular for human-in-the-loop airfoil design. However, XFoil is not the right tool for all applications, for a few reasons:
 >
 > - XFoil exhibits hysteresis: you can get slightly different solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you sweep $\alpha$ up or down, as Newton iteration is resumed from the last converged solution and uniqueness is not guaranteed. This hysteresis can be a big problem for design optimization.
-> - XFoil is not differentiable, in the sense that it doesn't tell you how performance changes w.r.t. airfoil shape (via, for example, an adjoint). That's okay—NeuralFoil doesn't either, at least out-of-the-box. However, the "path to obtain an efficient gradient" is very straightforward for NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX). In contrast, gradient options XFoil's Fortran code either don't exist or are significantly less advanced (e.g., Tapenade).
+> - XFoil is not differentiable, in the sense that it doesn't tell you how performance changes w.r.t. airfoil shape (via, for example, an adjoint). That's okay—NeuralFoil doesn't either, at least out-of-the-box. However, the "path to obtain an efficient gradient" is very straightforward for NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX). In contrast, gradient options for Fortran code (the language XFoil is in) either don't exist or are significantly less advanced (e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL](https://github.com/mdolab/CMPLXFOIL), which computes complex-step (effectively, forward-mode) gradients. However, even if you can get a gradient, it still may present issues, because...
 > - XFoil's solutions lack $C^1$-continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous by construction. This is critical for gradient-based optimization.
 > 	- Even if one tries to compute gradients of XFoil's outputs by finite-differencing or complex-stepping, these gradients are often inaccurate.
 >   - A bit into the weeds, but: this comes down to how XFoil handles transition (onset of turbulence). XFoil does a cut-cell approach on the transitioning interval, and while this specific cut-cell implementation restores $C^0$-continuity (i.e., transition won't truly "jump" from one node to another discretely), gradients of the laminar and turbulent BL closure functions still change at the cell interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic level. In theory $C^1$-continuity could be restored by also blending the BL shape variables through the transitioning cell interval, but that unleashes some ugly integrals and is not done in XFoil.
 >      - For more on this, see [Adler, Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/~mdolaboratory/pdf/Adler2022c.pdf), Figure 7.
 > - While XFoil is ~1000x faster than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil](#performance). NeuralFoil is also much easier to interface with on a memory level than XFoil, which means you won't find yourself I/O bound from file reading/writing like you will with XFoil.
 > - XFoil is not vectorized, which exacerbates the speed advantage of a (vectorized) neural network when analyzing large batches of airfoil cases simultaneously.
 > - XFoil is not guaranteed to produce a solution. Instead, XFoil often crashes when "ambitious" calculations are attempted, rather than producing a less-accurate answer. In some applications, that's okay or even desirable; in others, that's a dealbreaker. Example applications where this is a problem include:
@@ -172,15 +171,15 @@
 >   - Design optimization, where the optimizer needs "an answer" in order to recover from a bad design point and send the search back to a reasonable design.
 > - XFoil can be a serious pain to compile from source, which is often required if running on Mac or Linux (i.e., all supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so it's easy to install and run anywhere.
 
 Why not use a neural network trained on RANS CFD instead?
 
 > This is not a bad idea, and it has been done (See [Bouhlel, He, and Martins, "Scalable gradient-enhanced artificial..."](https://link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental challenge here, of course, is the cost of training data. RANS CFD is much more expensive than XFoil, so it's much harder to get the training data needed to train a neural network. For example, in the linked work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD runs (and they were sweeping over Mach as well, so the data becomes even sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the airfoil design space, which is critical for accurate predictions on out-of-sample airfoils.
 >
-> One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn directly quantifies the critical Mach number (beyond which simple models, like normal-shock total-pressure-loss relations or the [Korn equation heuristic](https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to extend the Mach region of validity slightly further). But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where XFoil is more accurate than RANS CFD.
+> One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn allows you to estimate the critical Mach number via Prandtl-Glauert correction (beyond which simple models, like normal-shock total-pressure-loss relations or the [Korn equation heuristic](https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to extend the Mach region of validity slightly further). But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where XFoil is more accurate than RANS CFD.
 
 Why not use a neural network trained on wind tunnel data?
 
 > This is a super-cool idea, and I'd love to see someone try it! My guess is that you'd need some kind of morphing wing section (and a way of precisely measuring the shape) in order to get enough data samples to "span" the airfoil design space. Then, you'd just let the wing section sit in the wind tunnel for a few days morphing itself around to collect data, then train a model on that. This would be really awesome, someone should do it!
 
 <a name="compressibility-question"></a>
 NeuralFoil is trained on incompressible ($M=0$) XFoil data. Why not train on compressible ($M>0$) XFoil data? Also, how can I use NeuralFoil to predict compressible airfoil performance?
@@ -190,14 +189,31 @@
 <a name="parameterization-question"></a>
 Why parameterize the airfoil geometry using the CST (Kulfan) parameterization? What exactly does the CST parameterization mean, and how can I convert this parameterization to/from actual airfoil coordinates? Why discretize with 8 CST modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing edges?
 
 > To be written, but in the meantime read:
 > - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
 > - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
 
+What's the underlying neural network architecture used in NeuralFoil?
+
+> To be written, but it is essentially a feed-forward neural network with a varying number of total layers and layer width depending on model size. Layer counts and widths were [determined through extensive trial and error](./training/supercloud_job_id_notes.log), in conjunction with observed test- and train-loss values. All layers are dense (fully connected, with weights and biases). All activation functions between layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and layer width are as follows:
+>
+> * xxsmall: 2 layers,  32 wide.
+> * xsmall:  3 layers,  32 wide.
+> * small:   3 layers,  48 wide.
+> * medium:  4 layers,  64 wide.
+> * large:   4 layers, 128 wide.
+> * xlarge:  4 layers, 256 wide.
+> * xxlarge: 5 layers, 256 wide.
+> * xxxlarge:5 layers, 512 wide.
+
+## Acknowledgements
+
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). 
+
 ## License
 
 NeuralFoil is licensed under the MIT license. Please see the [LICENSE](LICENSE.txt) file for details.
 
 ## Citing NeuralFoil
 
 If you use NeuralFoil in your research, please cite it as follows:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.3 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.4 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -74,65 +74,74 @@
 respect to XFoil more precisely. At a basic level, we care about two things: -
 **Accuracy**: how close are the predictions to XFoil's? - **Computational
 Cost**: how long does it take to run? This table details both of these
 considerations. The first few columns show the error with respect to XFoil on
 the test dataset. [The test dataset is completely isolated from the training
 dataset, and NeuralFoil was not allowed to learn from the test dataset]
 (#geometry-parameterization-and-training-data). Thus, the performance on the
-test dataset gives a good idea of NeuralFoil's performance "in the wild".
-Aerodynamics Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset,  Computational
-Model        with respect to XFoil                                                             Cost to Run
+test dataset gives a good idea of NeuralFoil's performance "in the wild". The
+second set of columns gives the runtime speed of the models, both for a single
+analysis and for a large batch analysis.
+Aerodynamics Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to   Computational
+Model        XFoil                                                                             Cost to Run
                                                                                         Bottom
                                                                              Top        Trans.         Total
              Lift   Fractional Drag   Moment Max Overspeed                   Transition Loc.   Runtime Runtime
              Coeff. Coeff.            Coeff. $u_\max / u_\infty$   â¡ Loc.       $x_    (1 run) (100,000
              $C_L$  $\ln(C_D)$ â  $C_M$                                  $x_{tr,    {tr,           runs)
                                                                              top}/c$    bot}/
                                                                                         c$
-NF Linear    0.116  -                 -      -                               -          -      18 ms   0.020 s
-$C_L$ Model
-NF "xxsmall" 0.065  0.121             0.010  0.215                           0.073      0.100  27 ms   0.204
+NF Linear    0.116  -                 -      -                               -          -      1 ms    0.020
+$C_L$ Model                                                                                            sec
+NF "xxsmall" 0.065  0.121             0.010  0.215                           0.073      0.100  3 ms    0.190
                                                                                                        sec
-NF "xsmall"  0.042  0.075             0.007  0.134                           0.039      0.055  29 ms   0.304 s
-NF "small"   0.039  0.069             0.006  0.122                           0.036      0.050  31 ms   0.437 s
-NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  33 ms   0.749 s
-NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  35 ms   1.542 s
-NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  36 ms   3.495 s
-NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  39 ms   4.557 s
-NF           0.020  0.039             0.003  0.070                           0.016      0.024  65 ms   11.633 s
-"xxxlarge"
-XFoil        0      0                 0      0                               0          0      447 ms  3610 sec
+NF "xsmall"  0.042  0.075             0.007  0.134                           0.039      0.055  4 ms    0.284
+                                                                                                       sec
+NF "small"   0.039  0.069             0.006  0.122                           0.036      0.050  4 ms    0.402
+                                                                                                       sec
+NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  5 ms    0.784
+                                                                                                       sec
+NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  6 ms    1.754
+                                                                                                       sec
+NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  10 ms   3.330
+                                                                                                       sec
+NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  13 ms   4.297
+                                                                                                       sec
+NF           0.020  0.039             0.003  0.070                           0.016      0.024  38 ms   8.980
+"xxxlarge"                                                                                             sec
+XFoil        0      0                 0      0                               0          0      73 ms   42 min
 > â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
 error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm)
 of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to
 within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil
-is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly
+is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly
 not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure
-above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may
-be better than the numbers in this table. > > â¡ This "maximum overspeed" lets
-you compute $C_{p,\min}$, which can be used to calculate the critical Mach
-number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
-Based on these performance numbers, you can select the right tradeoff between
-accuracy and computational cost for your application. In general, I recommend
-starting with the "large" model and adjusting from there. In addition to
-accuracy vs. speed, another consideration when choosing the right model is what
-you're trying to use NeuralFoil for. Larger models will be more complicated
-("less parsimonious," as the math kids would say), which means that they may
-have more "wiggles" in their outputsâthis might be undesirable for gradient-
-based optimization. On the other hand, larger models will be able to capture a
-wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
-be seen mid-optimization), so larger models could have a benefit in that sense.
-If you try a specific application and have better/worse results with a specific
-model, let me know by opening a GitHub issue! Notably, most of the
-computational overhead of calling NeuralFoil is actually in the airfoil
-preprocessing step, where the airfoil is converted from a set of coordinates to
-a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-
-and-training-data)) - not in the aerodynamics analysis itself. This pre-
-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear
-solvers](https://github.com/peterdsharpe/AeroSandbox/blob/
+above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may
+differ (in either direction) from the numbers in this table. > > â¡ This
+"maximum overspeed" lets you compute $C_{p,\min}$, which can be used to
+calculate the critical Mach number $M_\mathrm{crit}$. [More details below.]
+(#compressibility-question) Based on these performance numbers, you can select
+the right tradeoff between accuracy and computational cost for your
+application. In general, I recommend starting with the "large" model and
+adjusting from there. In addition to accuracy vs. speed, another consideration
+when choosing the right model is what you're trying to use NeuralFoil for.
+Larger models will be more complicated ("less parsimonious," as the math kids
+would say), which means that they may have more "wiggles" in their
+outputsâthis might be undesirable for gradient-based optimization. On the
+other hand, larger models will be able to capture a wider range of airfoils
+(e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-
+optimization), so larger models could have a benefit in that sense. If you try
+a specific application and have better/worse results with a specific model, let
+me know by opening a GitHub issue! Notably, most of the computational overhead
+of calling NeuralFoil is actually in the airfoil preprocessing step, where the
+airfoil is converted from a set of coordinates to a CST (Kulfan)
+parameterization ([more info here](#geometry-parameterization-and-training-
+data)) - not in the aerodynamics analysis itself. This pre-processing takes
+around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://
+github.com/peterdsharpe/AeroSandbox/blob/
 c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/
 airfoil_families.py#L265), but in theory a pure-NumPy implementation is
 possible that would be much faster by exploiting linearity (sub-millisecond).
 If you're interested in working on this, open an issue and let me know! In the
 meantime, you can eliminate this overhead by using
 [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to
 one of NeuralFoil's other functions. ## Installation [Install from PyPI](https:
@@ -179,94 +188,112 @@
 sweep $\alpha$ up or down, as Newton iteration is resumed from the last
 converged solution and uniqueness is not guaranteed. This hysteresis can be a
 big problem for design optimization. > - XFoil is not differentiable, in the
 sense that it doesn't tell you how performance changes w.r.t. airfoil shape
 (via, for example, an adjoint). That's okayâNeuralFoil doesn't either, at
 least out-of-the-box. However, the "path to obtain an efficient gradient" is
 very straightforward for NeuralFoil's pure NumPy code, where many excellent
-options exist (e.g., JAX). In contrast, gradient options XFoil's Fortran code
-either don't exist or are significantly less advanced (e.g., Tapenade). > -
-XFoil's solutions lack $C^1$-continuity. NeuralFoil, by contrast, is guaranteed
-to be $C^\infty$-continuous by construction. This is critical for gradient-
-based optimization. > - Even if one tries to compute gradients of XFoil's
-outputs by finite-differencing or complex-stepping, these gradients are often
-inaccurate. > - A bit into the weeds, but: this comes down to how XFoil handles
-transition (onset of turbulence). XFoil does a cut-cell approach on the
-transitioning interval, and while this specific cut-cell implementation
-restores $C^0$-continuity (i.e., transition won't truly "jump" from one node to
-another discretely), gradients of the laminar and turbulent BL closure
-functions still change at the cell interface due to the differing BL parameters
-($H$ and $Re_\theta$) from node to node. This loses $C^1$ continuity, causing a
-"ragged" polar at the microscopic level. In theory $C^1$-continuity could be
-restored by also blending the BL shape variables through the transitioning cell
-interval, but that unleashes some ugly integrals and is not done in XFoil. > -
-For more on this, see [Adler, Gray, and Martins, "To CFD or not to CFD?..."]
-(http://websites.umich.edu/~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > -
-While XFoil is ~1000x faster than RANS CFD, NeuralFoil [can be another ~1000x
-faster to evaluate than XFoil](#performance). NeuralFoil is also much easier to
-interface with on a memory level than XFoil, which means you won't find
-yourself I/O bound from file reading/writing like you will with XFoil. > -
-XFoil is not vectorized, which exacerbates the speed advantage of a
-(vectorized) neural network when analyzing large batches of airfoil cases
-simultaneously. > - XFoil is not guaranteed to produce a solution. Instead,
-XFoil often crashes when "ambitious" calculations are attempted, rather than
-producing a less-accurate answer. In some applications, that's okay or even
-desirable; in others, that's a dealbreaker. Example applications where this is
-a problem include: > - Real-time control, where one wants to estimate forces
-(e.g., for a MPC trajectory), but you can't have the controller crash if XFoil
-fails to converge or hangs the CPU. > - Flight simulation: similar to real-time
-control where "a less-accurate answer" is much better than "no answer." > -
-Design optimization, where the optimizer needs "an answer" in order to recover
-from a bad design point and send the search back to a reasonable design. > -
-XFoil can be a serious pain to compile from source, which is often required if
-running on Mac or Linux (i.e., all supercomputers, some lab computers).
-NeuralFoil is pure Python and NumPy, so it's easy to install and run anywhere.
-Why not use a neural network trained on RANS CFD instead? > This is not a bad
-idea, and it has been done (See [Bouhlel, He, and Martins, "Scalable gradient-
-enhanced artificial..."](https://link.springer.com/article/10.1007/s00158-020-
-02488-5))! The fundamental challenge here, of course, is the cost of training
-data. RANS CFD is much more expensive than XFoil, so it's much harder to get
-the training data needed to train a neural network. For example, in the linked
-work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD
-runs (and they were sweeping over Mach as well, so the data becomes even
-sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil
-runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the
-airfoil design space, which is critical for accurate predictions on out-of-
-sample airfoils. > > One advantage of a RANS CFD approach over the NeuralFoil
-XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get
-around this a little bit by estimating $C_{p, min}$, which in turn directly
-quantifies the critical Mach number (beyond which simple models, like normal-
-shock total-pressure-loss relations or the [Korn equation heuristic](https://
-archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to
-extend the Mach region of validity slightly further). But fundamentally,
-NeuralFoil is likely less accurate in the transonic range because of this. The
-tradeoff is that the much larger training data set allows NeuralFoil to be more
-accurate in the subsonic range, where XFoil is more accurate than RANS CFD. Why
-not use a neural network trained on wind tunnel data? > This is a super-cool
-idea, and I'd love to see someone try it! My guess is that you'd need some kind
-of morphing wing section (and a way of precisely measuring the shape) in order
-to get enough data samples to "span" the airfoil design space. Then, you'd just
-let the wing section sit in the wind tunnel for a few days morphing itself
-around to collect data, then train a model on that. This would be really
-awesome, someone should do it!  NeuralFoil is trained on incompressible ($M=0$)
-XFoil data. Why not train on compressible ($M>0$) XFoil data? Also, how can I
-use NeuralFoil to predict compressible airfoil performance? > To be written.
-But basically: $u_\max / u_\infty$ from NeuralFoil $\longrightarrow C_{p, \min,
-M=0} \longrightarrow C_{p, \min}$ using Prandtl-Glauert correction
-$\longrightarrow$ compare to $C_{p,\mathrm{sonic}}$ to determine the extent to
-which $M_\mathrm{crit}$ is exceeded.  Why parameterize the airfoil geometry
-using the CST (Kulfan) parameterization? What exactly does the CST
-parameterization mean, and how can I convert this parameterization to/from
-actual airfoil coordinates? Why discretize with 8 CST modes per side? Can
-NeuralFoil accurately analyze airfoils with thick trailing edges? > To be
-written, but in the meantime read: > - [D. A. Masters, "Geometric Comparison of
-Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://
-arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal paper on the CST
-(Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric
-Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) ##
-License NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
+options exist (e.g., JAX). In contrast, gradient options for Fortran code (the
+language XFoil is in) either don't exist or are significantly less advanced
+(e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL]
+(https://github.com/mdolab/CMPLXFOIL), which computes complex-step
+(effectively, forward-mode) gradients. However, even if you can get a gradient,
+it still may present issues, because... > - XFoil's solutions lack $C^1$-
+continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous
+by construction. This is critical for gradient-based optimization. > - Even if
+one tries to compute gradients of XFoil's outputs by finite-differencing or
+complex-stepping, these gradients are often inaccurate. > - A bit into the
+weeds, but: this comes down to how XFoil handles transition (onset of
+turbulence). XFoil does a cut-cell approach on the transitioning interval, and
+while this specific cut-cell implementation restores $C^0$-continuity (i.e.,
+transition won't truly "jump" from one node to another discretely), gradients
+of the laminar and turbulent BL closure functions still change at the cell
+interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to
+node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic
+level. In theory $C^1$-continuity could be restored by also blending the BL
+shape variables through the transitioning cell interval, but that unleashes
+some ugly integrals and is not done in XFoil. > - For more on this, see [Adler,
+Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/
+~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster
+than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil]
+(#performance). NeuralFoil is also much easier to interface with on a memory
+level than XFoil, which means you won't find yourself I/O bound from file
+reading/writing like you will with XFoil. > - XFoil is not vectorized, which
+exacerbates the speed advantage of a (vectorized) neural network when analyzing
+large batches of airfoil cases simultaneously. > - XFoil is not guaranteed to
+produce a solution. Instead, XFoil often crashes when "ambitious" calculations
+are attempted, rather than producing a less-accurate answer. In some
+applications, that's okay or even desirable; in others, that's a dealbreaker.
+Example applications where this is a problem include: > - Real-time control,
+where one wants to estimate forces (e.g., for a MPC trajectory), but you can't
+have the controller crash if XFoil fails to converge or hangs the CPU. > -
+Flight simulation: similar to real-time control where "a less-accurate answer"
+is much better than "no answer." > - Design optimization, where the optimizer
+needs "an answer" in order to recover from a bad design point and send the
+search back to a reasonable design. > - XFoil can be a serious pain to compile
+from source, which is often required if running on Mac or Linux (i.e., all
+supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so
+it's easy to install and run anywhere. Why not use a neural network trained on
+RANS CFD instead? > This is not a bad idea, and it has been done (See [Bouhlel,
+He, and Martins, "Scalable gradient-enhanced artificial..."](https://
+link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental
+challenge here, of course, is the cost of training data. RANS CFD is much more
+expensive than XFoil, so it's much harder to get the training data needed to
+train a neural network. For example, in the linked work by Bouhlel et al., the
+authors trained a neural network on 42,000 RANS CFD runs (and they were
+sweeping over Mach as well, so the data becomes even sparser). In contrast,
+NeuralFoil was trained on tens of millions of XFoil runs. Ultimately, this
+exposes NeuralFoil to a much larger "span" of the airfoil design space, which
+is critical for accurate predictions on out-of-sample airfoils. > > One
+advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of
+course, transonic modeling. NeuralFoil attempts to get around this a little bit
+by estimating $C_{p, min}$, which in turn allows you to estimate the critical
+Mach number via Prandtl-Glauert correction (beyond which simple models, like
+normal-shock total-pressure-loss relations or the [Korn equation heuristic]
+(https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be
+used to extend the Mach region of validity slightly further). But
+fundamentally, NeuralFoil is likely less accurate in the transonic range
+because of this. The tradeoff is that the much larger training data set allows
+NeuralFoil to be more accurate in the subsonic range, where XFoil is more
+accurate than RANS CFD. Why not use a neural network trained on wind tunnel
+data? > This is a super-cool idea, and I'd love to see someone try it! My guess
+is that you'd need some kind of morphing wing section (and a way of precisely
+measuring the shape) in order to get enough data samples to "span" the airfoil
+design space. Then, you'd just let the wing section sit in the wind tunnel for
+a few days morphing itself around to collect data, then train a model on that.
+This would be really awesome, someone should do it!  NeuralFoil is trained on
+incompressible ($M=0$) XFoil data. Why not train on compressible ($M>0$) XFoil
+data? Also, how can I use NeuralFoil to predict compressible airfoil
+performance? > To be written. But basically: $u_\max / u_\infty$ from
+NeuralFoil $\longrightarrow C_{p, \min, M=0} \longrightarrow C_{p, \min}$ using
+Prandtl-Glauert correction $\longrightarrow$ compare to $C_{p,\mathrm{sonic}}$
+to determine the extent to which $M_\mathrm{crit}$ is exceeded.  Why
+parameterize the airfoil geometry using the CST (Kulfan) parameterization? What
+exactly does the CST parameterization mean, and how can I convert this
+parameterization to/from actual airfoil coordinates? Why discretize with 8 CST
+modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing
+edges? > To be written, but in the meantime read: > - [D. A. Masters,
+"Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA
+Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal
+paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan,
+"Universal Parametric Geometry Representation Method"](http://
+mx1.brendakulfan.com/docs/CST6.pdf) What's the underlying neural network
+architecture used in NeuralFoil? > To be written, but it is essentially a feed-
+forward neural network with a varying number of total layers and layer width
+depending on model size. Layer counts and widths were [determined through
+extensive trial and error](./training/supercloud_job_id_notes.log), in
+conjunction with observed test- and train-loss values. All layers are dense
+(fully connected, with weights and biases). All activation functions between
+layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and
+layer width are as follows: > > * xxsmall: 2 layers, 32 wide. > * xsmall: 3
+layers, 32 wide. > * small: 3 layers, 48 wide. > * medium: 4 layers, 64 wide. >
+* large: 4 layers, 128 wide. > * xlarge: 4 layers, 256 wide. > * xxlarge: 5
+layers, 256 wide. > * xxxlarge:5 layers, 512 wide. ## Acknowledgements
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster
+operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). ## License
+NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
 (LICENSE.txt) file for details. ## Citing NeuralFoil If you use NeuralFoil in
 your research, please cite it as follows: ``` @misc{neuralfoil, author = {Peter
 Sharpe}, title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using
 physics-informed machine learning}, year = {2023}, publisher = {GitHub},
 journal = {GitHub repository}, howpublished = {\url{https://github.com/
 peterdsharpe/NeuralFoil}}, ```
```

### Comparing `NeuralFoil-0.1.3/README.md` & `NeuralFoil-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -79,20 +79,19 @@
 NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=0.75$ at $Re=\mathrm{1M}$, or $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is obviously incorrect, which would otherwise make optimization difficult. 
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
-This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild".
+This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild". The second set of columns gives the runtime speed of the models, both for a single analysis and for a large batch analysis.
 
-<a name="table"></a>
-<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>18 ms</td><td>0.020 s</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>27 ms</td><td>0.204 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>29 ms</td><td>0.304 s</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>31 ms</td><td>0.437 s</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>33 ms</td><td>0.749 s</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>35 ms</td><td>1.542 s</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>36 ms</td><td>3.495 s</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>39 ms</td><td>4.557 s</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>65 ms</td><td>11.633 s</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>447 ms</td><td>3610 sec</td></tr></tbody></table>
+<table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>1 ms</td><td>0.020 sec</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>3 ms</td><td>0.190 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>4 ms</td><td>0.284 sec</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>4 ms</td><td>0.402 sec</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>5 ms</td><td>0.784 sec</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>6 ms</td><td>1.754 sec</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>10 ms</td><td>3.330 sec</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>13 ms</td><td>4.297 sec</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>38 ms</td><td>8.980 sec</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>73 ms</td><td>42 min</td></tr></tbody></table>
 
-> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may be better than the numbers in this table.
+> † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may differ (in either direction) from the numbers in this table.
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
 
 Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
@@ -133,15 +132,15 @@
 
 <a name="xfoil-benefit-question"></a>
 Why not just use XFoil directly?
 
 > XFoil is a truly excellent piece of aerospace software engineering and is the gold standard of airfoil analysis, for good reason. When its assumptions hold (airfoils in subsonic flow without massive separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower computational cost. XFoil shines in particular for human-in-the-loop airfoil design. However, XFoil is not the right tool for all applications, for a few reasons:
 >
 > - XFoil exhibits hysteresis: you can get slightly different solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you sweep $\alpha$ up or down, as Newton iteration is resumed from the last converged solution and uniqueness is not guaranteed. This hysteresis can be a big problem for design optimization.
-> - XFoil is not differentiable, in the sense that it doesn't tell you how performance changes w.r.t. airfoil shape (via, for example, an adjoint). That's okay—NeuralFoil doesn't either, at least out-of-the-box. However, the "path to obtain an efficient gradient" is very straightforward for NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX). In contrast, gradient options XFoil's Fortran code either don't exist or are significantly less advanced (e.g., Tapenade).
+> - XFoil is not differentiable, in the sense that it doesn't tell you how performance changes w.r.t. airfoil shape (via, for example, an adjoint). That's okay—NeuralFoil doesn't either, at least out-of-the-box. However, the "path to obtain an efficient gradient" is very straightforward for NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX). In contrast, gradient options for Fortran code (the language XFoil is in) either don't exist or are significantly less advanced (e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL](https://github.com/mdolab/CMPLXFOIL), which computes complex-step (effectively, forward-mode) gradients. However, even if you can get a gradient, it still may present issues, because...
 > - XFoil's solutions lack $C^1$-continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous by construction. This is critical for gradient-based optimization.
 > 	- Even if one tries to compute gradients of XFoil's outputs by finite-differencing or complex-stepping, these gradients are often inaccurate.
 >   - A bit into the weeds, but: this comes down to how XFoil handles transition (onset of turbulence). XFoil does a cut-cell approach on the transitioning interval, and while this specific cut-cell implementation restores $C^0$-continuity (i.e., transition won't truly "jump" from one node to another discretely), gradients of the laminar and turbulent BL closure functions still change at the cell interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic level. In theory $C^1$-continuity could be restored by also blending the BL shape variables through the transitioning cell interval, but that unleashes some ugly integrals and is not done in XFoil.
 >      - For more on this, see [Adler, Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/~mdolaboratory/pdf/Adler2022c.pdf), Figure 7.
 > - While XFoil is ~1000x faster than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil](#performance). NeuralFoil is also much easier to interface with on a memory level than XFoil, which means you won't find yourself I/O bound from file reading/writing like you will with XFoil.
 > - XFoil is not vectorized, which exacerbates the speed advantage of a (vectorized) neural network when analyzing large batches of airfoil cases simultaneously.
 > - XFoil is not guaranteed to produce a solution. Instead, XFoil often crashes when "ambitious" calculations are attempted, rather than producing a less-accurate answer. In some applications, that's okay or even desirable; in others, that's a dealbreaker. Example applications where this is a problem include:
@@ -150,15 +149,15 @@
 >   - Design optimization, where the optimizer needs "an answer" in order to recover from a bad design point and send the search back to a reasonable design.
 > - XFoil can be a serious pain to compile from source, which is often required if running on Mac or Linux (i.e., all supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so it's easy to install and run anywhere.
 
 Why not use a neural network trained on RANS CFD instead?
 
 > This is not a bad idea, and it has been done (See [Bouhlel, He, and Martins, "Scalable gradient-enhanced artificial..."](https://link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental challenge here, of course, is the cost of training data. RANS CFD is much more expensive than XFoil, so it's much harder to get the training data needed to train a neural network. For example, in the linked work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD runs (and they were sweeping over Mach as well, so the data becomes even sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the airfoil design space, which is critical for accurate predictions on out-of-sample airfoils.
 >
-> One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn directly quantifies the critical Mach number (beyond which simple models, like normal-shock total-pressure-loss relations or the [Korn equation heuristic](https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to extend the Mach region of validity slightly further). But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where XFoil is more accurate than RANS CFD.
+> One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn allows you to estimate the critical Mach number via Prandtl-Glauert correction (beyond which simple models, like normal-shock total-pressure-loss relations or the [Korn equation heuristic](https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to extend the Mach region of validity slightly further). But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where XFoil is more accurate than RANS CFD.
 
 Why not use a neural network trained on wind tunnel data?
 
 > This is a super-cool idea, and I'd love to see someone try it! My guess is that you'd need some kind of morphing wing section (and a way of precisely measuring the shape) in order to get enough data samples to "span" the airfoil design space. Then, you'd just let the wing section sit in the wind tunnel for a few days morphing itself around to collect data, then train a model on that. This would be really awesome, someone should do it!
 
 <a name="compressibility-question"></a>
 NeuralFoil is trained on incompressible ($M=0$) XFoil data. Why not train on compressible ($M>0$) XFoil data? Also, how can I use NeuralFoil to predict compressible airfoil performance?
@@ -168,14 +167,31 @@
 <a name="parameterization-question"></a>
 Why parameterize the airfoil geometry using the CST (Kulfan) parameterization? What exactly does the CST parameterization mean, and how can I convert this parameterization to/from actual airfoil coordinates? Why discretize with 8 CST modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing edges?
 
 > To be written, but in the meantime read:
 > - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
 > - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
 
+What's the underlying neural network architecture used in NeuralFoil?
+
+> To be written, but it is essentially a feed-forward neural network with a varying number of total layers and layer width depending on model size. Layer counts and widths were [determined through extensive trial and error](./training/supercloud_job_id_notes.log), in conjunction with observed test- and train-loss values. All layers are dense (fully connected, with weights and biases). All activation functions between layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and layer width are as follows:
+>
+> * xxsmall: 2 layers,  32 wide.
+> * xsmall:  3 layers,  32 wide.
+> * small:   3 layers,  48 wide.
+> * medium:  4 layers,  64 wide.
+> * large:   4 layers, 128 wide.
+> * xlarge:  4 layers, 256 wide.
+> * xxlarge: 5 layers, 256 wide.
+> * xxxlarge:5 layers, 512 wide.
+
+## Acknowledgements
+
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). 
+
 ## License
 
 NeuralFoil is licensed under the MIT license. Please see the [LICENSE](LICENSE.txt) file for details.
 
 ## Citing NeuralFoil
 
 If you use NeuralFoil in your research, please cite it as follows:
```

#### html2text {}

```diff
@@ -60,65 +60,74 @@
 respect to XFoil more precisely. At a basic level, we care about two things: -
 **Accuracy**: how close are the predictions to XFoil's? - **Computational
 Cost**: how long does it take to run? This table details both of these
 considerations. The first few columns show the error with respect to XFoil on
 the test dataset. [The test dataset is completely isolated from the training
 dataset, and NeuralFoil was not allowed to learn from the test dataset]
 (#geometry-parameterization-and-training-data). Thus, the performance on the
-test dataset gives a good idea of NeuralFoil's performance "in the wild".
-Aerodynamics Mean Absolute Error ("MAE", or $L^1$ norm) of Given Metric, on the Test Dataset,  Computational
-Model        with respect to XFoil                                                             Cost to Run
+test dataset gives a good idea of NeuralFoil's performance "in the wild". The
+second set of columns gives the runtime speed of the models, both for a single
+analysis and for a large batch analysis.
+Aerodynamics Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to   Computational
+Model        XFoil                                                                             Cost to Run
                                                                                         Bottom
                                                                              Top        Trans.         Total
              Lift   Fractional Drag   Moment Max Overspeed                   Transition Loc.   Runtime Runtime
              Coeff. Coeff.            Coeff. $u_\max / u_\infty$   â¡ Loc.       $x_    (1 run) (100,000
              $C_L$  $\ln(C_D)$ â  $C_M$                                  $x_{tr,    {tr,           runs)
                                                                              top}/c$    bot}/
                                                                                         c$
-NF Linear    0.116  -                 -      -                               -          -      18 ms   0.020 s
-$C_L$ Model
-NF "xxsmall" 0.065  0.121             0.010  0.215                           0.073      0.100  27 ms   0.204
-                                                                                                       sec
-NF "xsmall"  0.042  0.075             0.007  0.134                           0.039      0.055  29 ms   0.304 s
-NF "small"   0.039  0.069             0.006  0.122                           0.036      0.050  31 ms   0.437 s
-NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  33 ms   0.749 s
-NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  35 ms   1.542 s
-NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  36 ms   3.495 s
-NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  39 ms   4.557 s
-NF           0.020  0.039             0.003  0.070                           0.016      0.024  65 ms   11.633 s
-"xxxlarge"
-XFoil        0      0                 0      0                               0          0      447 ms  3610 sec
+NF Linear    0.116  -                 -      -                               -          -      1 ms    0.020
+$C_L$ Model                                                                                            sec
+NF "xxsmall" 0.065  0.121             0.010  0.215                           0.073      0.100  3 ms    0.190
+                                                                                                       sec
+NF "xsmall"  0.042  0.075             0.007  0.134                           0.039      0.055  4 ms    0.284
+                                                                                                       sec
+NF "small"   0.039  0.069             0.006  0.122                           0.036      0.050  4 ms    0.402
+                                                                                                       sec
+NF "medium"  0.027  0.051             0.004  0.088                           0.022      0.033  5 ms    0.784
+                                                                                                       sec
+NF "large"   0.024  0.045             0.004  0.079                           0.020      0.029  6 ms    1.754
+                                                                                                       sec
+NF "xlarge"  0.023  0.043             0.004  0.076                           0.019      0.028  10 ms   3.330
+                                                                                                       sec
+NF "xxlarge" 0.021  0.040             0.003  0.071                           0.018      0.025  13 ms   4.297
+                                                                                                       sec
+NF           0.020  0.039             0.003  0.070                           0.016      0.024  38 ms   8.980
+"xxxlarge"                                                                                             sec
+XFoil        0      0                 0      0                               0          0      73 ms   42 min
 > â  The deviation of $\ln(C_D)$ can be thought of as "the typical relative
 error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm)
 of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to
 within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil
-is *less* accurate than XFoil; although XFoil is quite accurate, it is clearly
+is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly
 not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure
-above](#clcd-polar)) - so NeuralFoil's true accuracy compared to experiment may
-be better than the numbers in this table. > > â¡ This "maximum overspeed" lets
-you compute $C_{p,\min}$, which can be used to calculate the critical Mach
-number $M_\mathrm{crit}$. [More details below.](#compressibility-question)
-Based on these performance numbers, you can select the right tradeoff between
-accuracy and computational cost for your application. In general, I recommend
-starting with the "large" model and adjusting from there. In addition to
-accuracy vs. speed, another consideration when choosing the right model is what
-you're trying to use NeuralFoil for. Larger models will be more complicated
-("less parsimonious," as the math kids would say), which means that they may
-have more "wiggles" in their outputsâthis might be undesirable for gradient-
-based optimization. On the other hand, larger models will be able to capture a
-wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
-be seen mid-optimization), so larger models could have a benefit in that sense.
-If you try a specific application and have better/worse results with a specific
-model, let me know by opening a GitHub issue! Notably, most of the
-computational overhead of calling NeuralFoil is actually in the airfoil
-preprocessing step, where the airfoil is converted from a set of coordinates to
-a CST (Kulfan) parameterization ([more info here](#geometry-parameterization-
-and-training-data)) - not in the aerodynamics analysis itself. This pre-
-processing takes around 20 milliseconds using [AeroSandbox's general nonlinear
-solvers](https://github.com/peterdsharpe/AeroSandbox/blob/
+above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may
+differ (in either direction) from the numbers in this table. > > â¡ This
+"maximum overspeed" lets you compute $C_{p,\min}$, which can be used to
+calculate the critical Mach number $M_\mathrm{crit}$. [More details below.]
+(#compressibility-question) Based on these performance numbers, you can select
+the right tradeoff between accuracy and computational cost for your
+application. In general, I recommend starting with the "large" model and
+adjusting from there. In addition to accuracy vs. speed, another consideration
+when choosing the right model is what you're trying to use NeuralFoil for.
+Larger models will be more complicated ("less parsimonious," as the math kids
+would say), which means that they may have more "wiggles" in their
+outputsâthis might be undesirable for gradient-based optimization. On the
+other hand, larger models will be able to capture a wider range of airfoils
+(e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-
+optimization), so larger models could have a benefit in that sense. If you try
+a specific application and have better/worse results with a specific model, let
+me know by opening a GitHub issue! Notably, most of the computational overhead
+of calling NeuralFoil is actually in the airfoil preprocessing step, where the
+airfoil is converted from a set of coordinates to a CST (Kulfan)
+parameterization ([more info here](#geometry-parameterization-and-training-
+data)) - not in the aerodynamics analysis itself. This pre-processing takes
+around 20 milliseconds using [AeroSandbox's general nonlinear solvers](https://
+github.com/peterdsharpe/AeroSandbox/blob/
 c20bea3b142b61a7ad284dbe7632fbd9d5e232a6/aerosandbox/geometry/airfoil/
 airfoil_families.py#L265), but in theory a pure-NumPy implementation is
 possible that would be much faster by exploiting linearity (sub-millisecond).
 If you're interested in working on this, open an issue and let me know! In the
 meantime, you can eliminate this overhead by using
 [`get_aero_from_kulfan_parameters()`](./neuralfoil/neuralfoil.py) as opposed to
 one of NeuralFoil's other functions. ## Installation [Install from PyPI](https:
@@ -165,94 +174,112 @@
 sweep $\alpha$ up or down, as Newton iteration is resumed from the last
 converged solution and uniqueness is not guaranteed. This hysteresis can be a
 big problem for design optimization. > - XFoil is not differentiable, in the
 sense that it doesn't tell you how performance changes w.r.t. airfoil shape
 (via, for example, an adjoint). That's okayâNeuralFoil doesn't either, at
 least out-of-the-box. However, the "path to obtain an efficient gradient" is
 very straightforward for NeuralFoil's pure NumPy code, where many excellent
-options exist (e.g., JAX). In contrast, gradient options XFoil's Fortran code
-either don't exist or are significantly less advanced (e.g., Tapenade). > -
-XFoil's solutions lack $C^1$-continuity. NeuralFoil, by contrast, is guaranteed
-to be $C^\infty$-continuous by construction. This is critical for gradient-
-based optimization. > - Even if one tries to compute gradients of XFoil's
-outputs by finite-differencing or complex-stepping, these gradients are often
-inaccurate. > - A bit into the weeds, but: this comes down to how XFoil handles
-transition (onset of turbulence). XFoil does a cut-cell approach on the
-transitioning interval, and while this specific cut-cell implementation
-restores $C^0$-continuity (i.e., transition won't truly "jump" from one node to
-another discretely), gradients of the laminar and turbulent BL closure
-functions still change at the cell interface due to the differing BL parameters
-($H$ and $Re_\theta$) from node to node. This loses $C^1$ continuity, causing a
-"ragged" polar at the microscopic level. In theory $C^1$-continuity could be
-restored by also blending the BL shape variables through the transitioning cell
-interval, but that unleashes some ugly integrals and is not done in XFoil. > -
-For more on this, see [Adler, Gray, and Martins, "To CFD or not to CFD?..."]
-(http://websites.umich.edu/~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > -
-While XFoil is ~1000x faster than RANS CFD, NeuralFoil [can be another ~1000x
-faster to evaluate than XFoil](#performance). NeuralFoil is also much easier to
-interface with on a memory level than XFoil, which means you won't find
-yourself I/O bound from file reading/writing like you will with XFoil. > -
-XFoil is not vectorized, which exacerbates the speed advantage of a
-(vectorized) neural network when analyzing large batches of airfoil cases
-simultaneously. > - XFoil is not guaranteed to produce a solution. Instead,
-XFoil often crashes when "ambitious" calculations are attempted, rather than
-producing a less-accurate answer. In some applications, that's okay or even
-desirable; in others, that's a dealbreaker. Example applications where this is
-a problem include: > - Real-time control, where one wants to estimate forces
-(e.g., for a MPC trajectory), but you can't have the controller crash if XFoil
-fails to converge or hangs the CPU. > - Flight simulation: similar to real-time
-control where "a less-accurate answer" is much better than "no answer." > -
-Design optimization, where the optimizer needs "an answer" in order to recover
-from a bad design point and send the search back to a reasonable design. > -
-XFoil can be a serious pain to compile from source, which is often required if
-running on Mac or Linux (i.e., all supercomputers, some lab computers).
-NeuralFoil is pure Python and NumPy, so it's easy to install and run anywhere.
-Why not use a neural network trained on RANS CFD instead? > This is not a bad
-idea, and it has been done (See [Bouhlel, He, and Martins, "Scalable gradient-
-enhanced artificial..."](https://link.springer.com/article/10.1007/s00158-020-
-02488-5))! The fundamental challenge here, of course, is the cost of training
-data. RANS CFD is much more expensive than XFoil, so it's much harder to get
-the training data needed to train a neural network. For example, in the linked
-work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD
-runs (and they were sweeping over Mach as well, so the data becomes even
-sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil
-runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the
-airfoil design space, which is critical for accurate predictions on out-of-
-sample airfoils. > > One advantage of a RANS CFD approach over the NeuralFoil
-XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get
-around this a little bit by estimating $C_{p, min}$, which in turn directly
-quantifies the critical Mach number (beyond which simple models, like normal-
-shock total-pressure-loss relations or the [Korn equation heuristic](https://
-archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be used to
-extend the Mach region of validity slightly further). But fundamentally,
-NeuralFoil is likely less accurate in the transonic range because of this. The
-tradeoff is that the much larger training data set allows NeuralFoil to be more
-accurate in the subsonic range, where XFoil is more accurate than RANS CFD. Why
-not use a neural network trained on wind tunnel data? > This is a super-cool
-idea, and I'd love to see someone try it! My guess is that you'd need some kind
-of morphing wing section (and a way of precisely measuring the shape) in order
-to get enough data samples to "span" the airfoil design space. Then, you'd just
-let the wing section sit in the wind tunnel for a few days morphing itself
-around to collect data, then train a model on that. This would be really
-awesome, someone should do it!  NeuralFoil is trained on incompressible ($M=0$)
-XFoil data. Why not train on compressible ($M>0$) XFoil data? Also, how can I
-use NeuralFoil to predict compressible airfoil performance? > To be written.
-But basically: $u_\max / u_\infty$ from NeuralFoil $\longrightarrow C_{p, \min,
-M=0} \longrightarrow C_{p, \min}$ using Prandtl-Glauert correction
-$\longrightarrow$ compare to $C_{p,\mathrm{sonic}}$ to determine the extent to
-which $M_\mathrm{crit}$ is exceeded.  Why parameterize the airfoil geometry
-using the CST (Kulfan) parameterization? What exactly does the CST
-parameterization mean, and how can I convert this parameterization to/from
-actual airfoil coordinates? Why discretize with 8 CST modes per side? Can
-NeuralFoil accurately analyze airfoils with thick trailing edges? > To be
-written, but in the meantime read: > - [D. A. Masters, "Geometric Comparison of
-Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://
-arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal paper on the CST
-(Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric
-Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) ##
-License NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
+options exist (e.g., JAX). In contrast, gradient options for Fortran code (the
+language XFoil is in) either don't exist or are significantly less advanced
+(e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL]
+(https://github.com/mdolab/CMPLXFOIL), which computes complex-step
+(effectively, forward-mode) gradients. However, even if you can get a gradient,
+it still may present issues, because... > - XFoil's solutions lack $C^1$-
+continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous
+by construction. This is critical for gradient-based optimization. > - Even if
+one tries to compute gradients of XFoil's outputs by finite-differencing or
+complex-stepping, these gradients are often inaccurate. > - A bit into the
+weeds, but: this comes down to how XFoil handles transition (onset of
+turbulence). XFoil does a cut-cell approach on the transitioning interval, and
+while this specific cut-cell implementation restores $C^0$-continuity (i.e.,
+transition won't truly "jump" from one node to another discretely), gradients
+of the laminar and turbulent BL closure functions still change at the cell
+interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to
+node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic
+level. In theory $C^1$-continuity could be restored by also blending the BL
+shape variables through the transitioning cell interval, but that unleashes
+some ugly integrals and is not done in XFoil. > - For more on this, see [Adler,
+Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/
+~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster
+than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil]
+(#performance). NeuralFoil is also much easier to interface with on a memory
+level than XFoil, which means you won't find yourself I/O bound from file
+reading/writing like you will with XFoil. > - XFoil is not vectorized, which
+exacerbates the speed advantage of a (vectorized) neural network when analyzing
+large batches of airfoil cases simultaneously. > - XFoil is not guaranteed to
+produce a solution. Instead, XFoil often crashes when "ambitious" calculations
+are attempted, rather than producing a less-accurate answer. In some
+applications, that's okay or even desirable; in others, that's a dealbreaker.
+Example applications where this is a problem include: > - Real-time control,
+where one wants to estimate forces (e.g., for a MPC trajectory), but you can't
+have the controller crash if XFoil fails to converge or hangs the CPU. > -
+Flight simulation: similar to real-time control where "a less-accurate answer"
+is much better than "no answer." > - Design optimization, where the optimizer
+needs "an answer" in order to recover from a bad design point and send the
+search back to a reasonable design. > - XFoil can be a serious pain to compile
+from source, which is often required if running on Mac or Linux (i.e., all
+supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so
+it's easy to install and run anywhere. Why not use a neural network trained on
+RANS CFD instead? > This is not a bad idea, and it has been done (See [Bouhlel,
+He, and Martins, "Scalable gradient-enhanced artificial..."](https://
+link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental
+challenge here, of course, is the cost of training data. RANS CFD is much more
+expensive than XFoil, so it's much harder to get the training data needed to
+train a neural network. For example, in the linked work by Bouhlel et al., the
+authors trained a neural network on 42,000 RANS CFD runs (and they were
+sweeping over Mach as well, so the data becomes even sparser). In contrast,
+NeuralFoil was trained on tens of millions of XFoil runs. Ultimately, this
+exposes NeuralFoil to a much larger "span" of the airfoil design space, which
+is critical for accurate predictions on out-of-sample airfoils. > > One
+advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of
+course, transonic modeling. NeuralFoil attempts to get around this a little bit
+by estimating $C_{p, min}$, which in turn allows you to estimate the critical
+Mach number via Prandtl-Glauert correction (beyond which simple models, like
+normal-shock total-pressure-loss relations or the [Korn equation heuristic]
+(https://archive.aoe.vt.edu/mason/Mason_f/ConfigAeroTransonics.pdf), can be
+used to extend the Mach region of validity slightly further). But
+fundamentally, NeuralFoil is likely less accurate in the transonic range
+because of this. The tradeoff is that the much larger training data set allows
+NeuralFoil to be more accurate in the subsonic range, where XFoil is more
+accurate than RANS CFD. Why not use a neural network trained on wind tunnel
+data? > This is a super-cool idea, and I'd love to see someone try it! My guess
+is that you'd need some kind of morphing wing section (and a way of precisely
+measuring the shape) in order to get enough data samples to "span" the airfoil
+design space. Then, you'd just let the wing section sit in the wind tunnel for
+a few days morphing itself around to collect data, then train a model on that.
+This would be really awesome, someone should do it!  NeuralFoil is trained on
+incompressible ($M=0$) XFoil data. Why not train on compressible ($M>0$) XFoil
+data? Also, how can I use NeuralFoil to predict compressible airfoil
+performance? > To be written. But basically: $u_\max / u_\infty$ from
+NeuralFoil $\longrightarrow C_{p, \min, M=0} \longrightarrow C_{p, \min}$ using
+Prandtl-Glauert correction $\longrightarrow$ compare to $C_{p,\mathrm{sonic}}$
+to determine the extent to which $M_\mathrm{crit}$ is exceeded.  Why
+parameterize the airfoil geometry using the CST (Kulfan) parameterization? What
+exactly does the CST parameterization mean, and how can I convert this
+parameterization to/from actual airfoil coordinates? Why discretize with 8 CST
+modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing
+edges? > To be written, but in the meantime read: > - [D. A. Masters,
+"Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA
+Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal
+paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan,
+"Universal Parametric Geometry Representation Method"](http://
+mx1.brendakulfan.com/docs/CST6.pdf) What's the underlying neural network
+architecture used in NeuralFoil? > To be written, but it is essentially a feed-
+forward neural network with a varying number of total layers and layer width
+depending on model size. Layer counts and widths were [determined through
+extensive trial and error](./training/supercloud_job_id_notes.log), in
+conjunction with observed test- and train-loss values. All layers are dense
+(fully connected, with weights and biases). All activation functions between
+layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and
+layer width are as follows: > > * xxsmall: 2 layers, 32 wide. > * xsmall: 3
+layers, 32 wide. > * small: 3 layers, 48 wide. > * medium: 4 layers, 64 wide. >
+* large: 4 layers, 128 wide. > * xlarge: 4 layers, 256 wide. > * xxlarge: 5
+layers, 256 wide. > * xxxlarge:5 layers, 512 wide. ## Acknowledgements
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster
+operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). ## License
+NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
 (LICENSE.txt) file for details. ## Citing NeuralFoil If you use NeuralFoil in
 your research, please cite it as follows: ``` @misc{neuralfoil, author = {Peter
 Sharpe}, title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using
 physics-informed machine learning}, year = {2023}, publisher = {GitHub},
 journal = {GitHub repository}, howpublished = {\url{https://github.com/
 peterdsharpe/NeuralFoil}}, ```
```

### Comparing `NeuralFoil-0.1.3/neuralfoil/CL_linear_regression.py` & `NeuralFoil-0.1.4/neuralfoil/CL_linear_regression.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/neuralfoil.py` & `NeuralFoil-0.1.4/neuralfoil/neuralfoil.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 npz_file_directory = Path(__file__).parent / "nn_weights_and_biases"
 
 
 def get_aero_from_kulfan_parameters(
         kulfan_parameters: Dict[str, Union[float, np.ndarray]],
         alpha: Union[float, np.ndarray],
         Re: Union[float, np.ndarray],
-        model_size="medium"
+        model_size="large"
 ) -> Dict[str, Union[float, np.ndarray]]:
 
     ### Load the neural network parameters
     filename = npz_file_directory / f"nn-{model_size}.npz"
     if not filename.exists():
         raise FileNotFoundError(f"Could not find the neural network file {filename}, which contains the weights and biases.")
 
@@ -126,15 +126,15 @@
     }
 
 
 def get_aero_from_airfoil(
         airfoil: asb.Airfoil,
         alpha: Union[float, np.ndarray],
         Re: Union[float, np.ndarray],
-        model_size="medium",
+        model_size="large",
 ) -> Dict[str, Union[float, np.ndarray]]:
     from aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters
 
     kulfan_parameters = get_kulfan_parameters(
         airfoil.coordinates,
         n_weights_per_side=8
     )
@@ -147,15 +147,15 @@
     )
 
 
 def get_aero_from_coordinates(
         coordinates: np.ndarray,
         alpha: Union[float, np.ndarray],
         Re: Union[float, np.ndarray],
-        model_size="medium",
+        model_size="large",
 ):
     return get_aero_from_airfoil(
         airfoil=asb.Airfoil(
             coordinates=coordinates
         ),
         alpha=alpha,
         Re=Re,
@@ -163,15 +163,15 @@
     )
 
 
 def get_aero_from_dat_file(
         filename,
         alpha: Union[float, np.ndarray],
         Re: Union[float, np.ndarray],
-        model_size="medium",
+        model_size="large",
 ):
     with open(filename, "r") as f:
         raw_text = f.readlines()
 
     from aerosandbox.geometry.airfoil.airfoil_families import get_coordinates_from_raw_dat
     return get_aero_from_coordinates(
         coordinates=get_coordinates_from_raw_dat(raw_text=raw_text),
```

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-large.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-large.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-medium.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-medium.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-small.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-small.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xlarge.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xsmall.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz` & `NeuralFoil-0.1.4/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.3/setup.py` & `NeuralFoil-0.1.4/setup.py`

 * *Files identical despite different names*

