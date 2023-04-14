# Comparing `tmp/tupa123-1.2.9.tar.gz` & `tmp/tupa123-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.2.9.tar", last modified: Tue Apr  4 19:24:19 2023, max compression
+gzip compressed data, was "tupa123-1.3.0.tar", last modified: Fri Apr 14 21:02:26 2023, max compression
```

## Comparing `tupa123-1.2.9.tar` & `tupa123-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 19:24:19.590237 tupa123-1.2.9/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0     6636 2023-04-04 19:24:19.590237 tupa123-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     6273 2023-04-04 17:40:49.000000 tupa123-1.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 19:24:19.590237 tupa123-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-04-04 19:24:09.000000 tupa123-1.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:24:19.580202 tupa123-1.2.9/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.2.9/tupa123/__init__.py
--rw-rw-rw-   0        0        0    38979 2023-04-04 19:20:04.000000 tupa123-1.2.9/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-04 19:24:19.590237 tupa123-1.2.9/tupa123.egg-info/
--rw-rw-rw-   0        0        0     6636 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 21:02:26.448205 tupa123-1.3.0/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     7490 2023-04-14 21:02:26.448205 tupa123-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7127 2023-04-14 21:01:08.000000 tupa123-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 21:02:26.448205 tupa123-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-04-14 21:01:41.000000 tupa123-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 21:02:26.438202 tupa123-1.3.0/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.0/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    60174 2023-04-14 13:18:14.000000 tupa123-1.3.0/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-14 21:02:26.448205 tupa123-1.3.0/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     7490 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 21:02:26.000000 tupa123-1.3.0/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.2.9/LICENSE.txt` & `tupa123-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.2.9/PKG-INFO` & `tupa123-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-Metadata-Version: 2.1
-Name: tupa123
-Version: 1.2.9
-Summary: fully connected neural network with four layers
-Author: Leandro Schemmer
-Author-email: leandro.schemmer@gmail.com
-License: MIT
-Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
 The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
 <br>
+<br>
+#Manual = https://www.mediafire.com/file/vtzpb8ne1g92mgz/Manual_Tupa123.pdf <br>
+<br>
+#Excel example data = https://www.mediafire.com/file/k8xkw4592tb9uab/ALETAS.xlsx <br>
+<br>
+<br>
 #<b>-----Files without comments:--------------------------------------- </b><br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
 <br>
 import tupa123 as tu <br>
 <br>
-X = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
-y = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
+X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
+y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
 <br>
 model = tu.nnet4(norma=5, coef=0, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0) <br>
 model.Fit_ADAM(X, y) <br>
 model.Plotconv() <br>
 <br>
 input('end') <br>
 <br>
 #-----FILE TO APPLICATION OF MACHINE LEARNING <br>
 <br>
 import tupa123 as tu <br>
 <br>
 model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, fa2c=5, fa3c=5, fa4c=0) <br>
-X_new = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
-y_resposta = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
+X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
+y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
 y_pred = model.Predict(X_new) <br>
 <br>
 tu.Statistics(y_pred, y_resposta) <br>
 tu.PlotCorrelation(y_pred, y_resposta) <br>
 tu.PlotComparative(y_pred, y_resposta) <br>
 input('end') <br>
 <br>
 #<b>------Commented file:------------------------------------------</b> <br>
 <br>
 #-----MACHINE LEARNING <br>
 <br>
 <b>import tupa123 as tu</b> <br>
 #import the library <br>
 <br>
-<b>X = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300)</b> <br>
-<b>y = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300)</b> <br>
+<b>X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300)</b> <br>
+<b>y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300)</b> <br>
 #learning data <br>
 #The data can come from any source, but the ExcelMatrix function allows a practical interaction with Excel <br>
 #ExcelMatrix = collect data from excel, the spreadsheet needs to be in the same folder as the python file <br>
 #'ALETAS.xlsm' = example name of the excel file / 'Sheet1' = example name of the tab where the data are <br>
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
-<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0)</b> <br>
+<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='')</b> <br>
 #creates the Neural Network model <br>
+<br>
 #norma = type of data normalization: (default=2)<br>
 #=-1, standardization <br>
 #=0, do anything <br>
 #=1, between 0 and 1 <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
-#normout = if 1 normalizes the output (default=1) <br>
+#normout = if 1 normalizes the output (default=1), 0 dont <br>
+<br>
 #nn1c=5, nn2c=7, nn3c=5, nn4c=2 = number of neurons from the first to the fourth layer (default=1,5,5,1) <br>
 #rate = learning rate (default=0.01) <br>
 #epochs = number of epochs (default=1000)<br>
 #fa2c=5, fa3c=5, fa4c=0 = second to fourth layer activation functions (default=5,5,0) <br>
 #for regression the fourth layer is recommended as linear = 0 <br>
+#cost=0, cost function, (default=0). 0 = MSE, mean squared error for regression and classification / 1 = BCE, binary cross entropy for classification <br>
+#regu= regularization, (default=0). Usual value for regression = 0.01 <br>
+#namenet= name of the folder where the weights are saved, default is the same directory as the .py file, necessary when working with more than one neural network <br>
+<br>
 #Activation functions: <br>
 #=0 linear <br> 
 #=1 Sigmoide <br>
 #=2 softpluss <br>
 #=3 gaussinana <br>
 #=4 ReLU <br>
 #=5 tanh <br>
@@ -97,14 +98,15 @@
 #=14 X**3 <br>
 #=15 Symmetric Rectified Linear <br>
 <br>
 <b>model.Fit_ADAM(X, y) </b><br>
 #machine learning <br>
 #model.Fit_ADAM(X, y) = single batch interpolation of all learning data, with ADAM accelerator <br>
 #model.Fit_STOC(X, y) = case-by-case interpolation, stochastic gradient descent <br>
+#model.Fit_STOC_ADAM(X, y) = case-by-case interpolation, stochastic with ADAM <br>
 <br>
 <b>model.Plotconv()</b> <br>
 #Plot the convergence process <br>
 <br>
 input('End') <br>
 <br>
 #-----APPLICATION OF MACHINE LEARNING <br>
@@ -112,18 +114,18 @@
 <b>import tupa123 as tu</b> <br>
 <br>
 <b>model = tu.nnet4(norma=5, coef=0, nn1c=5, nn2c=7, nn3c=5, nn4c=2, fa2c=5, fa3c=5, fa4c=0) </b><br>
 #application file must be in the same folder as the learning file <br>
 #where some .txt files were generated with the neural network settings <br>
 #neural network must have the same configuration that was used in the learning phase <br>
 <br>
-<b>X_new = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000)</b> <br>
+<b>X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000)</b> <br>
 #variables to be predicted <br>
 <br>
-<b>y_resposta = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) </b><br>
+<b>y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) </b><br>
 #right answer to compare, to evaluate neural network performance <br>
 <br>
 <b>y_pred = model.Predict(X_new) </b><br>
 #prediction, neural network result <br>
 <br>
 <b>tu.Statistics(y_pred, y_resposta) </b><br>
 #Statistical evaluation of the results <br>
@@ -134,23 +136,26 @@
 <br>
 <b>tu.PlotCorrelation2(y_pred, y_resposta) </b><br>
 #Calculated and target correlation plot with standard deviation lines<br>
 <br>
 <b>tu.PlotComparative(y_pred, y_resposta) </b><br>
 #Calculated and target comparative plot <br>
 <br>
-<b>tu.PlotComparative2(y_pred, y_resposta) </b><br>
-#Calculated and target comparative plot <br>
+<b>tu.PlotComparative2(y_pred, y_resposta, window_size=1000) </b><br>
+#Error plot with movel average<br>
 <br>
 <b>tu.PlotComparative3(y_pred, y_resposta) </b><br>
 #Calculated and target comparative plot with standard deviation areas <br>
 <br>
+<b>tu.PlotComparative4(y_pred, y_resposta) </b><br>
+#Plot 2 sigma tandard deviation areas with target <br>
+<br>
 <b>tu.PlotDispe(y_pred, y_resposta) </b><br>
 #Error dispersion <br>
 <br>
 <b>tu.PlotDispe2(y_pred, y_resposta) </b><br>
 #Error dispersion with error proportion<br>
 <br>
 <b>tu.PlotHisto(y_pred, y_resposta) </b><br>
 #Percentage error histogram <br>
 <br>
-input('end') <br>
+input('end') <br>
```

### Comparing `tupa123-1.2.9/README.md` & `tupa123-1.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,100 @@
+Metadata-Version: 2.1
+Name: tupa123
+Version: 1.3.0
+Summary: fully connected neural network with four layers
+Author: Leandro Schemmer
+Author-email: leandro.schemmer@gmail.com
+License: MIT
+Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
 The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
 <br>
+<br>
+#Manual = https://www.mediafire.com/file/vtzpb8ne1g92mgz/Manual_Tupa123.pdf <br>
+<br>
+#Excel example data = https://www.mediafire.com/file/k8xkw4592tb9uab/ALETAS.xlsx <br>
+<br>
+<br>
 #<b>-----Files without comments:--------------------------------------- </b><br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
 <br>
 import tupa123 as tu <br>
 <br>
-X = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
-y = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
+X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
+y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
 <br>
 model = tu.nnet4(norma=5, coef=0, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0) <br>
 model.Fit_ADAM(X, y) <br>
 model.Plotconv() <br>
 <br>
 input('end') <br>
 <br>
 #-----FILE TO APPLICATION OF MACHINE LEARNING <br>
 <br>
 import tupa123 as tu <br>
 <br>
 model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, fa2c=5, fa3c=5, fa4c=0) <br>
-X_new = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
-y_resposta = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
+X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
+y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
 y_pred = model.Predict(X_new) <br>
 <br>
 tu.Statistics(y_pred, y_resposta) <br>
 tu.PlotCorrelation(y_pred, y_resposta) <br>
 tu.PlotComparative(y_pred, y_resposta) <br>
 input('end') <br>
 <br>
 #<b>------Commented file:------------------------------------------</b> <br>
 <br>
 #-----MACHINE LEARNING <br>
 <br>
 <b>import tupa123 as tu</b> <br>
 #import the library <br>
 <br>
-<b>X = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300)</b> <br>
-<b>y = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300)</b> <br>
+<b>X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300)</b> <br>
+<b>y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300)</b> <br>
 #learning data <br>
 #The data can come from any source, but the ExcelMatrix function allows a practical interaction with Excel <br>
 #ExcelMatrix = collect data from excel, the spreadsheet needs to be in the same folder as the python file <br>
 #'ALETAS.xlsm' = example name of the excel file / 'Sheet1' = example name of the tab where the data are <br>
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
-<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0)</b> <br>
+<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='')</b> <br>
 #creates the Neural Network model <br>
+<br>
 #norma = type of data normalization: (default=2)<br>
 #=-1, standardization <br>
 #=0, do anything <br>
 #=1, between 0 and 1 <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
-#normout = if 1 normalizes the output (default=1) <br>
+#normout = if 1 normalizes the output (default=1), 0 dont <br>
+<br>
 #nn1c=5, nn2c=7, nn3c=5, nn4c=2 = number of neurons from the first to the fourth layer (default=1,5,5,1) <br>
 #rate = learning rate (default=0.01) <br>
 #epochs = number of epochs (default=1000)<br>
 #fa2c=5, fa3c=5, fa4c=0 = second to fourth layer activation functions (default=5,5,0) <br>
 #for regression the fourth layer is recommended as linear = 0 <br>
+#cost=0, cost function, (default=0). 0 = MSE, mean squared error for regression and classification / 1 = BCE, binary cross entropy for classification <br>
+#regu= regularization, (default=0). Usual value for regression = 0.01 <br>
+#namenet= name of the folder where the weights are saved, default is the same directory as the .py file, necessary when working with more than one neural network <br>
+<br>
 #Activation functions: <br>
 #=0 linear <br> 
 #=1 Sigmoide <br>
 #=2 softpluss <br>
 #=3 gaussinana <br>
 #=4 ReLU <br>
 #=5 tanh <br>
@@ -86,14 +109,15 @@
 #=14 X**3 <br>
 #=15 Symmetric Rectified Linear <br>
 <br>
 <b>model.Fit_ADAM(X, y) </b><br>
 #machine learning <br>
 #model.Fit_ADAM(X, y) = single batch interpolation of all learning data, with ADAM accelerator <br>
 #model.Fit_STOC(X, y) = case-by-case interpolation, stochastic gradient descent <br>
+#model.Fit_STOC_ADAM(X, y) = case-by-case interpolation, stochastic with ADAM <br>
 <br>
 <b>model.Plotconv()</b> <br>
 #Plot the convergence process <br>
 <br>
 input('End') <br>
 <br>
 #-----APPLICATION OF MACHINE LEARNING <br>
@@ -101,18 +125,18 @@
 <b>import tupa123 as tu</b> <br>
 <br>
 <b>model = tu.nnet4(norma=5, coef=0, nn1c=5, nn2c=7, nn3c=5, nn4c=2, fa2c=5, fa3c=5, fa4c=0) </b><br>
 #application file must be in the same folder as the learning file <br>
 #where some .txt files were generated with the neural network settings <br>
 #neural network must have the same configuration that was used in the learning phase <br>
 <br>
-<b>X_new = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000)</b> <br>
+<b>X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000)</b> <br>
 #variables to be predicted <br>
 <br>
-<b>y_resposta = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) </b><br>
+<b>y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) </b><br>
 #right answer to compare, to evaluate neural network performance <br>
 <br>
 <b>y_pred = model.Predict(X_new) </b><br>
 #prediction, neural network result <br>
 <br>
 <b>tu.Statistics(y_pred, y_resposta) </b><br>
 #Statistical evaluation of the results <br>
@@ -123,23 +147,26 @@
 <br>
 <b>tu.PlotCorrelation2(y_pred, y_resposta) </b><br>
 #Calculated and target correlation plot with standard deviation lines<br>
 <br>
 <b>tu.PlotComparative(y_pred, y_resposta) </b><br>
 #Calculated and target comparative plot <br>
 <br>
-<b>tu.PlotComparative2(y_pred, y_resposta) </b><br>
-#Calculated and target comparative plot <br>
+<b>tu.PlotComparative2(y_pred, y_resposta, window_size=1000) </b><br>
+#Error plot with movel average<br>
 <br>
 <b>tu.PlotComparative3(y_pred, y_resposta) </b><br>
 #Calculated and target comparative plot with standard deviation areas <br>
 <br>
+<b>tu.PlotComparative4(y_pred, y_resposta) </b><br>
+#Plot 2 sigma tandard deviation areas with target <br>
+<br>
 <b>tu.PlotDispe(y_pred, y_resposta) </b><br>
 #Error dispersion <br>
 <br>
 <b>tu.PlotDispe2(y_pred, y_resposta) </b><br>
 #Error dispersion with error proportion<br>
 <br>
 <b>tu.PlotHisto(y_pred, y_resposta) </b><br>
 #Percentage error histogram <br>
 <br>
-input('end') <br>
+input('end') <br>
```

### Comparing `tupa123-1.2.9/setup.py` & `tupa123-1.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.2.9',
+    version='1.3.0',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy>=1.23.5','matplotlib>=3.6.3','pandas>=1.5.3'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.2.9/tupa123/tupa123.py` & `tupa123-1.3.0/tupa123/tupa123.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os 
 import pandas as pd
 import numpy as np 
 import time
 import matplotlib.pyplot as plt
+import matplotlib.colors as mcolors
 
 
 
 
 
 
 
@@ -31,24 +33,33 @@
     print('------------------------')
     print ('Statistics between predictor variables and target variables:')
     print('------------------------')
       
     for j in range(0,numevar):
         
         erroari = Calculated[:,j] - Targeted[:,j]
-        erroper = (( Calculated[:,j] - Targeted[:,j] ) / Targeted[:,j])*100
+        erroper = ( ( Calculated[:,j] - Targeted[:,j] ) / (Targeted[:,j] + 1e-7)  )*100
         coefcorrelacao = np.corrcoef(Targeted[:,j], Calculated[:,j])[1][0]
         
         print ('Correlation coefficient, variable ' + str(j+1) +' = ' + str(coefcorrelacao))
         print('')
         print ('Mean difference, variable ' + str(j+1) +' = ' + str(np.mean(erroari)) + ' (' + str(np.mean(erroper)) + '%)')
         print('')
         print ('Standard deviation, variable ' + str(j+1) +' = ' + str(np.std(erroari)) + ' (' + str(np.std(erroper)) + '%)')
         print('')
         print ('Biggest absolute point difference, variable ' + str(j+1) +' = ' + str(np.max(abs(erroari))) + ' ('  + str(np.max(abs(erroper))) + '%)' )
+        print('')
+
+        conta=0
+        for i in range(0,numdata):
+            if abs(erroari[i]) <= 0.1:
+                conta=conta+1
+        result = 100*conta/numdata
+        print('For classification 0 to 1, number of hits for a maximum difference of 10% = ' + str(result) + '%' )
+
         print('------------------------')
 
 
 
 
 
 
@@ -76,29 +87,37 @@
 
 
 
 
 
 
 #Plot the differences of two variables in a sequential series
-def PlotComparative2(Calculated, Targeted):
+def PlotComparative2(Calculated, Targeted, window_size=10):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
-
+            
     for j in range(0,numevar):    
         eixoY1= Targeted[:,j]
         eixoY2= Calculated[:,j]
+        
         eixoY3 = eixoY2 - eixoY1
-    
+
+
+        # preparação para a média móvel
+        rolling_mean = pd.Series(eixoY3).rolling(window_size).mean()
+
         plt.figure(figsize=(12, 5))
         plt.title('Comparison chart calculated variable vs targeted')
         plt.xlabel('Sequence of events')
-        plt.ylabel('Target and predicted variable ' + str(j+1))
-        plt.plot(eixoX, eixoY3, marker = '', color = 'darkblue', label='Targeted')  
+        plt.ylabel('Error, Calculated - Targeted ' + str(j+1))
+        plt.plot(eixoX, eixoY3, marker = '', color = 'darkblue', label='Targeted')
+        # plota a med movel
+        plt.plot(eixoX, rolling_mean, marker='', color = mcolors.to_hex((1, 0, 0)), label='Rolling mean', linestyle='dashed') 
+
         plt.legend(loc = "upper left")
         plt.show()
 
 
 
 
 
@@ -137,14 +156,58 @@
         plt.show()
 
 
 
 
 
 
+
+
+#Plot 2 sigma lines
+def PlotComparative4(Calculated, Targeted):
+
+    numdata,numevar = Calculated.shape
+    eixoX = np.arange(0, numdata, dtype=int)
+
+    for j in range(0,numevar):    
+        eixoY1= Targeted[:,j]
+        eixoY2= Calculated[:,j]
+
+        # Cálculo do erro médio e desvio padrão
+        erro_medio = np.mean(eixoY2 - eixoY1)
+        sigma = np.std(eixoY2 - eixoY1)
+    
+        plt.figure(figsize=(12, 5))
+        plt.title('Comparison chart calculated variable vs targeted')
+        plt.xlabel('Sequence of events')
+        plt.ylabel('Target and predicted variable ' + str(j+1))
+        plt.plot(eixoX, eixoY1, marker = '',  label='Targeted')
+
+        plt.plot(eixoX, eixoY1 + erro_medio - 2*sigma, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected minimum, -2S')
+        plt.plot(eixoX, eixoY1 + erro_medio + 2*sigma, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected maximum, +2S')
+        plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.1)
+                
+        #plt.plot(eixoX, eixoY2, linestyle='none', c='black', marker = '.', label='Calculated', alpha=0.33)
+        plt.legend(loc = "upper right")
+
+        # Preenchendo a área entre as curvas
+        #plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - sigma, eixoY1 + erro_medio + sigma, color='gray', alpha=0.3)
+        #plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.2)
+        #plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 3*sigma, eixoY1 + erro_medio + 3*sigma, color='gray', alpha=0.1)
+
+        # Adicionando o valor do desvio padrão ao canto superior esquerdo do gráfico
+        plt.text(0.025, 0.95, "sigma = {:.2f}".format(sigma) + ", average = {:.2f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
+        
+        plt.show()
+
+
+        
+
+
+
 #Plot correlation between calculated variables and objectives
 def PlotCorrelation(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
@@ -218,25 +281,27 @@
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
         
         valormax = np.max(eixoY1)
         valormin = np.min(eixoY1)
         volormed =(valormin+valormax)/2
         eixoY1norma = (eixoY1 - volormed)/(valormax - volormed)                        
+
+        plt.figure(figsize=(15, 5))
         
-        plt.scatter(eixoY1norma,erro,color='blue',s=15,edgecolor='red')
+        plt.scatter(eixoY1norma,erro,color='blue', s=15, edgecolor='red')
         
         plt.plot([-1,1], [0,0], color='black', alpha=0.9, linestyle='dashed')                
 
         # Preenchendo a área entre as curvas
         plt.fill_between((-1,1), erro_medio - sigma, erro_medio + sigma, color='gray', alpha=0.3)
         plt.fill_between((-1,1), erro_medio - 2*sigma, erro_medio + 2*sigma, color='gray', alpha=0.2)
         plt.fill_between((-1,1), erro_medio - 3*sigma, erro_medio + 3*sigma, color='gray', alpha=0.1)
         
-        plt.title('Dispersion plot, 3 sigma colors, variable '+ str(j+1))
+        plt.title('Dispersion plot, 3 sigma gray gradients, variable '+ str(j+1))
         plt.xlabel('Variable normalized: -1,1')
         plt.ylabel('Variable error (calculated-targeted)')
         
         plt.show()
 
         
 
@@ -261,15 +326,15 @@
         eixoY3 = eixoY2 - eixoY1        
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
         eixoY4 = eixoY3/sigma
         
                         
         plt.title('Target vs sniper, variable '+ str(j+1))
-        plt.scatter(eixoY4,razao,color='blue',s=15,edgecolor='red') #grafico de correlação entre as variaveis procuradas e alvo---
+        plt.scatter(eixoY4,razao,color='red', s=15 , marker = '.', alpha=0.1) #grafico de correlação entre as variaveis procuradas e alvo---
         plt.xlabel('Standard deviation sigma')
         plt.ylabel('Proportion = calculated/targeted')
 
         plt.plot([-1,1], [1,1], color='black', alpha=0.9, linestyle='dashed')
         plt.plot([0,0], [1-(np.max(razao)-1)*0.5,1+(np.max(razao)-1)*0.5], color='black', alpha=0.9, linestyle='dashed')
         
         plt.show()
@@ -313,35 +378,37 @@
 
         plt.show()
 
 
 
 
 
+
+
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=2, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0):
+    def __init__ (self, norma=2, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet=''):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
         self.fa2c=fa2c
         self.fa3c=fa3c
         self.fa4c=fa4c
         self.norma=norma
         self.coef=coef
         self.normout=normout
-
-
-
+        self.cost=cost
+        self.regu=regu
+        self.namenet=namenet
 
 
 
 
 
     #data normalization by calculating maximums and minimums-----------------------------------------------
     def Normalize(self, data, maxiname, mininame, medianame, desvioname):          
@@ -669,49 +736,81 @@
         e2= np.zeros((self.nn2c))
         e3= np.zeros((self.nn3c))
         e4= np.zeros((self.nn4c))
 
         #resultados
         R = np.zeros((self.nn4c))
 
+
+        #ajuste do local de salvamento, se especificado
+        if (self.namenet==''):
+            nomepasta=''
+        else:
+            nomepasta = self.namenet + '/'
+            if not os.path.exists(self.namenet):
+                os.mkdir(self.namenet)
+
+
+
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
     
-            if self.nn1c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = np.array([np.loadtxt("P12.txt")])        
+            if self.nn1c ==1: #garante o formato matricial 
+                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
+            else:
+                P12 = np.loadtxt(nomepasta + "P12.txt")
+
+            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P12 = P12aux.T
+            
+            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
+                P23 = P23aux.T
             else:
-                P12 = np.loadtxt("P12.txt")  
-            P23 = np.loadtxt("P23.txt")
+                P23 = np.loadtxt(nomepasta + "P23.txt") 
+            
             if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt("P34.txt")])
+                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
                 P34 = P34aux.T
             else:
-                P34 = np.loadtxt("P34.txt")
-            B2 = np.loadtxt("B2.txt")
-            B3 = np.loadtxt("B3.txt")
-            B4 = np.loadtxt("B4.txt")
+                P34 = np.loadtxt(nomepasta + "P34.txt")              
+
+            if self.nn2c ==1: #garante o formato matricial 
+                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
+            else:
+                B2 = np.loadtxt(nomepasta + "B2.txt")
+                
+            if self.nn3c ==1: #garante o formato matricial 
+                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
+            else:
+                B3 = np.loadtxt(nomepasta + "B3.txt")
+                
+            if self.nn4c ==1: #garante o formato matricial 
+                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
+            else:
+                B4 = np.loadtxt(nomepasta + "B4.txt")  
 
         except: #Inicializa randomicamente-------------------------------
 
             B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))
             B4 = -0.1 + 2*0.1*(np.random.rand(self.nn4c))    
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
-        matX = self.Normalize(matX,"vmax_in.txt","vmin_in.txt","media_in.txt","desvio_in.txt")
+        matX = self.Normalize(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt")
         if (self.normout==1):
-            matY = self.Normalize(matY,"vmax_out.txt","vmin_out.txt","media_out.txt","desvio_out.txt")
+            matY = self.Normalize(matY,nomepasta + "vmax_out.txt",nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt")
 
 
         #Processo de aprendizado------------------------------------------------------------
 
-        VetorErro = np.zeros((self.epochs))
+        VetorErro = np.zeros((self.epochs+1))
         MenorErro = 999999999
 
         NumdataEstudo = len(matX)
 
         monit=0
         for ite in range(0,self.epochs): #Processo iterativo global, epocas, cada epoca passa por todos os dados de aprendizagem-----------------
             Tempo = ite+1
@@ -736,24 +835,33 @@
 
                 c3 = np.dot(c2,P23)- B3
                 c3 = self.Activation(self.fa3c,c3)
         
                 c4 = np.dot(c3,P34)- B4
                 c4 = self.Activation(self.fa4c,c4)         
 
+                regulariza=0
+                if (self.regu!=0): #adiciona a regularização se houver                    
+                    regulariza = self.regu*( np.sum(P12*P12) + np.sum(P23*P23) + np.sum(P34*P34) + np.sum(B2*B2) + np.sum(B3*B3) + np.sum(B4*B4) )
+
                 #calculo efetivo do erro ------------
-                m_aux = (R - c4)**2
-                EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)
-                   
-            VetorErro[ite] = EMQ 
+                if (self.cost==0):#erro medio quadratico                   
+                    m_aux = 0.5*((R - c4))**2 + regulariza
+                else: #BCE, entropia cruzada binaria
+                    m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
+                
+                EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)                    
 
- 
+                
+            VetorErro[ite+1] = EMQ 
+
+            
             #memorização dos melhores pesos-----------
             if (EMQ < MenorErro):
-                itememo = ite
+                itememo = ite+1
                 MenorErro = EMQ
                 P12m = P12*1
                 P23m = P23*1
                 P34m = P34*1
                 B2m = B2*1
                 B3m = B3*1
                 B4m = B4*1
@@ -774,17 +882,24 @@
                 d3 = self.DeActivation(self.fa3c,c3)
                 c3 = self.Activation(self.fa3c,c3)
         
                 c4 = np.dot(c3,P34)- B4
                 d4 = self.DeActivation(self.fa4c,c4)
                 c4 = self.Activation(self.fa4c,c4)          
 
-                #Calcula o erro da ultima camada 
-                e4 = d4 * ( R - c4 )
-                 
+                regulariza=0
+                if (self.regu!=0): #adiciona a regularização se houver                    
+                    regulariza = 2*self.regu*( np.sum(P12) + np.sum(P23) + np.sum(P34) + np.sum(B2) + np.sum(B3) + np.sum(B4) )
+
+                #Calcula o erro da ultima camada
+                if (self.cost==0):#EMQ
+                    e4 = d4 * ( (R - c4) + regulariza )
+                else: #BCE
+                    e4 = d4 * ( (R/(c4 +1e-7)) - ((1-R)/(1-c4 +1e-7)) + regulariza )
+                
                 #Propagação do erro para traz, backprop     
                 e3 = np.dot(e4, np.transpose(P34))
                 e3 = d3 * e3
             
                 e2 = np.dot(e3, np.transpose(P23))
                 e2 = d2 * e2
 
@@ -850,21 +965,22 @@
         P34 = P34m*1
         B2 = B2m*1
         B3 = B3m*1
         B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
-        np.savetxt("P12.txt", P12)
-        np.savetxt("P23.txt", P23)
-        np.savetxt("P34.txt", P34)
-        np.savetxt("B2.txt", B2)
-        np.savetxt("B3.txt", B3)
-        np.savetxt("B4.txt", B4)
-        np.savetxt("Convergencia.txt", VetorErro)
+        np.savetxt(nomepasta + "P12.txt", P12)
+        np.savetxt(nomepasta + "P23.txt", P23)
+        np.savetxt(nomepasta + "P34.txt", P34)
+        np.savetxt(nomepasta + "B2.txt", B2)
+        np.savetxt(nomepasta + "B3.txt", B3)
+        np.savetxt(nomepasta + "B4.txt", B4)
+        VetorErro[0] = itememo
+        np.savetxt(nomepasta + "Convergencia.txt", VetorErro)
 
         tfim = time.time()
         print('runtime(s) = ' , tfim-tinicio)
 
 
 
 
@@ -916,49 +1032,80 @@
         e2= np.zeros((self.nn2c))
         e3= np.zeros((self.nn3c))
         e4= np.zeros((self.nn4c))
 
         #resultados
         R = np.zeros((self.nn4c))
 
+
+        #ajuste do local de salvamento, se especificado
+        if (self.namenet==''):
+            nomepasta=''
+        else:
+            nomepasta = self.namenet + '/'
+            if not os.path.exists(self.namenet):
+                os.mkdir(self.namenet)
+
+
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
     
-            if self.nn1c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = np.array([np.loadtxt("P12.txt")])        
+            if self.nn1c ==1: #garante o formato matricial 
+                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
             else:
-                P12 = np.loadtxt("P12.txt")  
-            P23 = np.loadtxt("P23.txt")
+                P12 = np.loadtxt(nomepasta + "P12.txt")
+
+            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P12 = P12aux.T
+            
+            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
+                P23 = P23aux.T
+            else:
+                P23 = np.loadtxt(nomepasta + "P23.txt") 
+            
             if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt("P34.txt")])
+                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
                 P34 = P34aux.T
             else:
-                P34 = np.loadtxt("P34.txt")
-            B2 = np.loadtxt("B2.txt")
-            B3 = np.loadtxt("B3.txt")
-            B4 = np.loadtxt("B4.txt")
+                P34 = np.loadtxt(nomepasta + "P34.txt")              
+
+            if self.nn2c ==1: #garante o formato matricial 
+                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
+            else:
+                B2 = np.loadtxt(nomepasta + "B2.txt")
+                
+            if self.nn3c ==1: #garante o formato matricial 
+                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
+            else:
+                B3 = np.loadtxt(nomepasta + "B3.txt")
+                
+            if self.nn4c ==1: #garante o formato matricial 
+                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
+            else:
+                B4 = np.loadtxt(nomepasta + "B4.txt")  
 
         except: #Inicializa randomicamente-------------------------------
 
             B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))
             B4 = -0.1 + 2*0.1*(np.random.rand(self.nn4c))    
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
-        matX = self.Normalize(matX,"vmax_in.txt","vmin_in.txt","media_in.txt","desvio_in.txt")
+        matX = self.Normalize(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt")
         if (self.normout==1):
-            matY = self.Normalize(matY,"vmax_out.txt","vmin_out.txt","media_out.txt","desvio_out.txt") 
+            matY = self.Normalize(matY,nomepasta + "vmax_out.txt",nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt") 
 
 
         #Processo de aprendizado------------------------------------------------------------
 
-        VetorErro = np.zeros((self.epochs))
+        VetorErro = np.zeros((self.epochs+1))
         MenorErro = 999999999
 
         NumdataEstudo = len(matX)
 
         monit=0
         for ite in range(0,self.epochs): #iteração global, cada epoca varred todos os casos de estudo-------------------------
             Tempo = ite+1
@@ -983,24 +1130,32 @@
 
                 c3 = np.dot(c2,P23)- B3
                 c3 = self.Activation(self.fa3c,c3)
         
                 c4 = np.dot(c3,P34)- B4
                 c4 = self.Activation(self.fa4c,c4)         
 
-                #calculo efetivo do erro -------
-                m_aux = (R - c4)**2
+                regulariza=0
+                if (self.regu!=0): #adiciona a regularização se houver                    
+                    regulariza = self.regu*( np.sum(P12*P12) + np.sum(P23*P23) + np.sum(P34*P34) + np.sum(B2*B2) + np.sum(B3*B3) + np.sum(B4*B4) )
+
+                #calculo efetivo do erro ------------
+                if (self.cost==0):#erro medio quadratico                   
+                    m_aux = 0.5*((R - c4))**2 + regulariza
+                else: #BCE, entropia cruzada binaria
+                    m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
+               
                 EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)
                    
-            VetorErro[ite] = EMQ 
+            VetorErro[ite+1] = EMQ 
 
  
             #memorização dos melhores pesos------------
             if (EMQ < MenorErro):
-                itememo = ite
+                itememo = ite+1
                 MenorErro = EMQ
                 P12m = P12*1
                 P23m = P23*1
                 P34m = P34*1
                 B2m = B2*1
                 B3m = B3*1
                 B4m = B4*1
@@ -1021,16 +1176,23 @@
                 d3 = self.DeActivation(self.fa3c,c3)
                 c3 = self.Activation(self.fa3c,c3)
         
                 c4 = np.dot(c3,P34)- B4
                 d4 = self.DeActivation(self.fa4c,c4)
                 c4 = self.Activation(self.fa4c,c4)          
 
-                #Calcula o erro da ultima camada 
-                e4 = d4 * ( R - c4 )
+                regulariza=0
+                if (self.regu!=0): #adiciona a regularização se houver                    
+                    regulariza = 2*self.regu*( np.sum(P12) + np.sum(P23) + np.sum(P34) + np.sum(B2) + np.sum(B3) + np.sum(B4) )
+
+                #Calcula o erro da ultima camada
+                if (self.cost==0):#EMQ
+                    e4 = d4 * ( (R - c4) + regulariza )
+                else: #BCE
+                    e4 = d4 * ( (R/(c4 +1e-7)) - ((1-R)/(1-c4 +1e-7)) + regulariza )
                  
                 #Propagação do erro para traz, backprop     
                 e3 = np.dot(e4, np.transpose(P34))
                 e3 = d3 * e3
             
                 e2 = np.dot(e3, np.transpose(P23))
                 e2 = d2 * e2
@@ -1051,21 +1213,22 @@
         P34 = P34m*1
         B2 = B2m*1
         B3 = B3m*1
         B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
-        np.savetxt("P12.txt", P12)
-        np.savetxt("P23.txt", P23)
-        np.savetxt("P34.txt", P34)
-        np.savetxt("B2.txt", B2)
-        np.savetxt("B3.txt", B3)
-        np.savetxt("B4.txt", B4)
-        np.savetxt("Convergencia.txt", VetorErro)
+        np.savetxt(nomepasta + "P12.txt", P12)
+        np.savetxt(nomepasta + "P23.txt", P23)
+        np.savetxt(nomepasta + "P34.txt", P34)
+        np.savetxt(nomepasta + "B2.txt", B2)
+        np.savetxt(nomepasta + "B3.txt", B3)
+        np.savetxt(nomepasta + "B4.txt", B4)
+        VetorErro[0] = itememo
+        np.savetxt(nomepasta + "Convergencia.txt", VetorErro)
 
         tfim = time.time()
         print('runtime(s) = ' , tfim-tinicio)
 
 
 
 
@@ -1089,37 +1252,65 @@
         #camadas
         c1= np.zeros((self.nn1c))
         c2= np.zeros((self.nn2c))
         c3= np.zeros((self.nn3c))
         c4= np.zeros((self.nn4c))
 
 
+        #ajuste do local de salvamento, se especificado
+        if (self.namenet==''):
+            nomepasta=''
+        else:
+            nomepasta = self.namenet + '/'
+            
+
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
     
-            if self.nn1c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = np.array([np.loadtxt("P12.txt")])        
+            if self.nn1c ==1: #garante o formato matricial 
+                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
             else:
-                P12 = np.loadtxt("P12.txt")  
-            P23 = np.loadtxt("P23.txt")
+                P12 = np.loadtxt(nomepasta + "P12.txt")
+
+            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P12 = P12aux.T
+            
+            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
+                P23 = P23aux.T
+            else:
+                P23 = np.loadtxt(nomepasta + "P23.txt") 
+            
             if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt("P34.txt")])
+                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
                 P34 = P34aux.T
             else:
-                P34 = np.loadtxt("P34.txt")
-            B2 = np.loadtxt("B2.txt")
-            B3 = np.loadtxt("B3.txt")
-            B4 = np.loadtxt("B4.txt")
+                P34 = np.loadtxt(nomepasta + "P34.txt")              
 
+            if self.nn2c ==1: #garante o formato matricial 
+                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
+            else:
+                B2 = np.loadtxt(nomepasta + "B2.txt")
+                
+            if self.nn3c ==1: #garante o formato matricial 
+                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
+            else:
+                B3 = np.loadtxt(nomepasta + "B3.txt")
+                
+            if self.nn4c ==1: #garante o formato matricial 
+                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
+            else:
+                B4 = np.loadtxt(nomepasta + "B4.txt")
+                
         except: #se nao tem pesos salvos encerra o programa-------------------------------
 
            input('No saved weight files')
            exit()
 
         #Normaliza a entrada de data----------------------
-        matX = self.Normalize2(matX,"vmax_in.txt","vmin_in.txt","media_in.txt","desvio_in.txt") 
+        matX = self.Normalize2(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt") 
 
         
         #Predição----------------------------
         numdata = len(matX)
         Calculated = np.zeros((numdata, self.nn4c)) #inicializa a matriz dos resultados Calculated
         
         for caso in range (0, numdata):
@@ -1137,43 +1328,370 @@
             c4 = np.dot(c3,P34)- B4
             c4 = self.Activation(self.fa4c,c4)         
 
             # saida----------------------------
             Calculated[caso][:] = c4[:]
 
         if (self.normout==1):            
-            Calculated = self.DesNormalize(Calculated, "vmax_out.txt", "vmin_out.txt","media_out.txt","desvio_out.txt") 
+            Calculated = self.DesNormalize(Calculated, nomepasta + "vmax_out.txt", nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt") 
 
         return Calculated
 
 
 
 
 
 
 
 
 
 
+
+    #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
+    def Fit_STOC_ADAM(self, matX, matY):
+
+        tinicio = time.time()
+        
+        #Criação ou leitura da matriz dos pesos--------
+
+        #pesos
+        P12 = np.zeros((self.nn1c,self.nn2c))
+        P23 = np.zeros((self.nn2c,self.nn3c))
+        P34 = np.zeros((self.nn3c,self.nn4c))
+
+        #bias
+        B2= np.zeros((self.nn2c))
+        B3= np.zeros((self.nn3c))
+        B4= np.zeros((self.nn4c))
+
+        #pesos memorizados
+        P12m = np.zeros((self.nn1c,self.nn2c))
+        P23m = np.zeros((self.nn2c,self.nn3c))
+        P34m = np.zeros((self.nn3c,self.nn4c))
+
+        #bias memorizados
+        B2m = np.zeros((self.nn2c))
+        B3m = np.zeros((self.nn3c))
+        B4m = np.zeros((self.nn4c))
+
+        #variaçao pesos
+        VP12 = np.zeros((self.nn1c,self.nn2c))
+        VP23 = np.zeros((self.nn2c,self.nn3c))
+        VP34 = np.zeros((self.nn3c,self.nn4c))
+
+        #variaçao bias
+        VB2= np.zeros((self.nn2c))
+        VB3= np.zeros((self.nn3c))
+        VB4= np.zeros((self.nn4c))
+
+        #velocidade pesos
+        veloP12 = np.zeros((self.nn1c,self.nn2c))
+        veloP23 = np.zeros((self.nn2c,self.nn3c))
+        veloP34 = np.zeros((self.nn3c,self.nn4c))
+
+        #velocidade bias
+        veloB2= np.zeros((self.nn2c))
+        veloB3= np.zeros((self.nn3c))
+        veloB4= np.zeros((self.nn4c))
+
+        #massa pesos
+        massaP12 = np.zeros((self.nn1c,self.nn2c))
+        massaP23 = np.zeros((self.nn2c,self.nn3c))
+        massaP34 = np.zeros((self.nn3c,self.nn4c))
+
+        #massa bias
+        massaB2= np.zeros((self.nn2c))
+        massaB3= np.zeros((self.nn3c))
+        massaB4= np.zeros((self.nn4c))
+
+        #camadas
+        c1= np.zeros((self.nn1c))
+        c2= np.zeros((self.nn2c))
+        c3= np.zeros((self.nn3c))
+        c4= np.zeros((self.nn4c))
+
+        #derivadas
+        d1= np.zeros((self.nn1c))
+        d2= np.zeros((self.nn2c))
+        d3= np.zeros((self.nn3c))
+        d4= np.zeros((self.nn4c))
+
+        #erros
+        e1= np.zeros((self.nn1c))
+        e2= np.zeros((self.nn2c))
+        e3= np.zeros((self.nn3c))
+        e4= np.zeros((self.nn4c))
+
+        #resultados
+        R = np.zeros((self.nn4c))
+
+
+        #ajuste do local de salvamento, se especificado
+        if (self.namenet==''):
+            nomepasta=''
+        else:
+            nomepasta = self.namenet + '/'
+            if not os.path.exists(self.namenet):
+                os.mkdir(self.namenet)
+
+
+
+        try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
+    
+            if self.nn1c ==1: #garante o formato matricial 
+                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
+            else:
+                P12 = np.loadtxt(nomepasta + "P12.txt")
+
+            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P12 = P12aux.T
+            
+            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
+                P23 = P23aux.T
+            else:
+                P23 = np.loadtxt(nomepasta + "P23.txt") 
+            
+            if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
+                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
+                P34 = P34aux.T
+            else:
+                P34 = np.loadtxt(nomepasta + "P34.txt")              
+
+            if self.nn2c ==1: #garante o formato matricial 
+                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
+            else:
+                B2 = np.loadtxt(nomepasta + "B2.txt")
+                
+            if self.nn3c ==1: #garante o formato matricial 
+                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
+            else:
+                B3 = np.loadtxt(nomepasta + "B3.txt")
+                
+            if self.nn4c ==1: #garante o formato matricial 
+                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
+            else:
+                B4 = np.loadtxt(nomepasta + "B4.txt")  
+
+        except: #Inicializa randomicamente-------------------------------
+
+            B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
+            B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))
+            B4 = -0.1 + 2*0.1*(np.random.rand(self.nn4c))    
+            P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
+            P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
+            P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
+
+
+        #Normaliza os parametros-------------------------
+        matX = self.Normalize(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt")
+        if (self.normout==1):
+            matY = self.Normalize(matY,nomepasta + "vmax_out.txt",nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt")
+
+
+        #Processo de aprendizado------------------------------------------------------------
+
+        VetorErro = np.zeros((self.epochs+1))
+        MenorErro = 999999999
+
+        NumdataEstudo = len(matX)
+
+        monit=0
+        for ite in range(0,self.epochs): #Processo iterativo global, epocas, cada epoca passa por todos os dados de aprendizagem-----------------
+            Tempo = ite+1
+    
+            if ite > (self.epochs*monit/100): #só um monitor de progresso
+                print(str(monit) + '%')
+                monit=monit+10
+
+
+            #Calculo do erro----------------------------
+
+            EMQ = 0
+            for caso in range (0, NumdataEstudo): #Verificação do aprendizado---
+
+                #Camada 1, data de entrada
+                c1 = matX[caso,:self.nn1c]
+                R = matY[caso,:]  
+                
+                #propagacao sinal
+                c2 = np.dot(c1,P12)- B2        
+                c2 = self.Activation(self.fa2c,c2)
+
+                c3 = np.dot(c2,P23)- B3
+                c3 = self.Activation(self.fa3c,c3)
+        
+                c4 = np.dot(c3,P34)- B4
+                c4 = self.Activation(self.fa4c,c4)         
+
+                regulariza=0
+                if (self.regu!=0): #adiciona a regularização se houver                    
+                    regulariza = self.regu*( np.sum(P12*P12) + np.sum(P23*P23) + np.sum(P34*P34) + np.sum(B2*B2) + np.sum(B3*B3) + np.sum(B4*B4) )
+
+                #calculo efetivo do erro ------------
+                if (self.cost==0):#erro medio quadratico                   
+                    m_aux = 0.5*((R - c4))**2 + regulariza
+                else: #BCE, entropia cruzada binaria
+                    m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
+                
+                EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)                    
+
+                
+            VetorErro[ite+1] = EMQ 
+
+            
+            #memorização dos melhores pesos-----------
+            if (EMQ < MenorErro):
+                itememo = ite+1
+                MenorErro = EMQ
+                P12m = P12*1
+                P23m = P23*1
+                P34m = P34*1
+                B2m = B2*1
+                B3m = B3*1
+                B4m = B4*1
+
+        
+            for caso in range (0, NumdataEstudo): #varredura em todos os casos de estudo--------
+
+                #Camada 1, data de entrada
+                c1 = matX[caso,:self.nn1c]
+                R = matY[caso,:]                        
+                
+                #propagacao sinal
+                c2 = np.dot(c1,P12)- B2
+                d2 = self.DeActivation(self.fa2c,c2)
+                c2 = self.Activation(self.fa2c,c2)
+
+                c3 = np.dot(c2,P23)- B3
+                d3 = self.DeActivation(self.fa3c,c3)
+                c3 = self.Activation(self.fa3c,c3)
+        
+                c4 = np.dot(c3,P34)- B4
+                d4 = self.DeActivation(self.fa4c,c4)
+                c4 = self.Activation(self.fa4c,c4)          
+
+                regulariza=0
+                if (self.regu!=0): #adiciona a regularização se houver                    
+                    regulariza = 2*self.regu*( np.sum(P12) + np.sum(P23) + np.sum(P34) + np.sum(B2) + np.sum(B3) + np.sum(B4) )
+
+                #Calcula o erro da ultima camada
+                if (self.cost==0):#EMQ
+                    e4 = d4 * ( (R - c4) + regulariza )
+                else: #BCE
+                    e4 = d4 * ( (R/(c4 +1e-7)) - ((1-R)/(1-c4 +1e-7)) + regulariza )
+                
+                #Propagação do erro para traz, backprop     
+                e3 = np.dot(e4, np.transpose(P34))
+                e3 = d3 * e3
+            
+                e2 = np.dot(e3, np.transpose(P23))
+                e2 = d2 * e2
+                                     
+        
+                #Atualização efetiva dos pesos----------------------------------
+
+                Gd12 = np.dot(c1.reshape(-1, 1), e2.reshape(1, -1))  
+                Gd23 = np.dot(c2.reshape(-1, 1), e3.reshape(1, -1)) 
+                Gd34 = np.dot(c3.reshape(-1, 1), e4.reshape(1, -1))
+
+                massaP12 = 0.9*massaP12 + (1-0.9)*Gd12
+                massaP23 = 0.9*massaP23 + (1-0.9)*Gd23
+                massaP34 = 0.9*massaP34 + (1-0.9)*Gd34
+
+                veloP12 = 0.999*veloP12 + (1-0.999)*(Gd12**2)
+                veloP23 = 0.999*veloP23 + (1-0.999)*(Gd23**2)
+                veloP34 = 0.999*veloP34 + (1-0.999)*(Gd34**2)
+
+                aux1= 1-(0.9**Tempo)
+                aux2 = 1 - (0.999**Tempo)
+    
+                P12 = P12 + self.rate*( (massaP12/aux1) / np.sqrt(veloP12/aux2) )
+                P23 = P23 + self.rate*( (massaP23/aux1) / np.sqrt(veloP23/aux2) )
+                P34 = P34 + self.rate*( (massaP34/aux1) / np.sqrt(veloP34/aux2) )
+       
+                Gd2 = - e2 
+                Gd3 = - e3 
+                Gd4 = - e4 
+
+                massaB2 = 0.9*massaB2 + (1-0.9)*Gd2
+                massaB3 = 0.9*massaB3 + (1-0.9)*Gd3
+                massaB4 = 0.9*massaB4 + (1-0.9)*Gd4
+
+                veloB2 = 0.999*veloB2 + (1-0.999)*(Gd2**2)
+                veloB3 = 0.999*veloB3 + (1-0.999)*(Gd3**2)
+                veloB4 = 0.999*veloB4 + (1-0.999)*(Gd4**2) 
+    
+                B2 = B2 + self.rate*( (massaB2/aux1) / np.sqrt(veloB2/aux2) )
+                B3 = B3 + self.rate*( (massaB3/aux1) / np.sqrt(veloB3/aux2) )
+                B4 = B4 + self.rate*( (massaB4/aux1) / np.sqrt(veloB4/aux2) )
+ 
+
+        print('100%')
+
+        P12 = P12m*1
+        P23 = P23m*1
+        P34 = P34m*1
+        B2 = B2m*1
+        B3 = B3m*1
+        B4 = B4m*1
+
+
+        #Salva os pesos e bias em arquivos txt----------------------------------------------------------
+        np.savetxt(nomepasta + "P12.txt", P12)
+        np.savetxt(nomepasta + "P23.txt", P23)
+        np.savetxt(nomepasta + "P34.txt", P34)
+        np.savetxt(nomepasta + "B2.txt", B2)
+        np.savetxt(nomepasta + "B3.txt", B3)
+        np.savetxt(nomepasta + "B4.txt", B4)
+        VetorErro[0] = itememo
+        np.savetxt(nomepasta + "Convergencia.txt", VetorErro)
+
+        tfim = time.time()
+        print('runtime(s) = ' , tfim-tinicio)
+
+
+
+
+
+
+
+
+
+
+
+
+
+
     #Plota a convergencia ----------------------------------------------------------
     def Plotconv(self):
 
+
+        #ajuste do local de salvamento, se especificado
+        if (self.namenet==''):
+            nomepasta=''
+        else:
+            nomepasta = self.namenet + '/'
+
+            
         #grafico da convergencia
-        Conve = np.loadtxt("Convergencia.txt")
+        Conve = np.loadtxt(nomepasta + "Convergencia.txt")
         tamanho = len(Conve)
+        
         MenorErro = np.min(Conve)
+        itemenorerro = Conve[0]
 
-        eixoX = np.zeros((tamanho)) 
-        eixoY = np.zeros((tamanho))
+        eixoX = np.zeros((tamanho-1)) 
+        eixoY = np.zeros((tamanho-1))
 
-        eixoX = np.arange(0, tamanho, dtype=int)
-        eixoY = Conve*1  
+        eixoX = np.arange(0, tamanho-1, dtype=int)
+        eixoY = Conve[1:tamanho]
     
         plt.figure(figsize=(12, 5))
-        plt.title('Mean squared error = ' + str(MenorErro))
+        plt.title('Mean squared error = ' + str(MenorErro) + ', iteration number = ' + str(itemenorerro))
         plt.xlabel('Study data')
         plt.ylabel('Error, mse')
         plt.plot(eixoX, eixoY, marker = '', color = 'darkblue')  
         plt.show()
```

### Comparing `tupa123-1.2.9/tupa123.egg-info/PKG-INFO` & `tupa123-1.3.0/tupa123.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,100 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.2.9
+Version: 1.3.0
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Fully connected four-layer neural network <br>
 Solves a huge number of cases, classification and regression <br>
 The following sequence explains how to use with the help of two example files. <br>
 The first file contains the learning process, where the neural network finds its weights <br>
 The second file demonstrates the network's ability to make predictions on new, unseen data that is not part of the training set <br>
 <br>
+<br>
+#Manual = https://www.mediafire.com/file/vtzpb8ne1g92mgz/Manual_Tupa123.pdf <br>
+<br>
+#Excel example data = https://www.mediafire.com/file/k8xkw4592tb9uab/ALETAS.xlsx <br>
+<br>
+<br>
 #<b>-----Files without comments:--------------------------------------- </b><br>
 <br>
 #-----FILE TO MACHINE LEARNING <br>
 <br>
 import tupa123 as tu <br>
 <br>
-X = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
-y = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
+X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300) <br>
+y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300) <br>
 <br>
 model = tu.nnet4(norma=5, coef=0, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0) <br>
 model.Fit_ADAM(X, y) <br>
 model.Plotconv() <br>
 <br>
 input('end') <br>
 <br>
 #-----FILE TO APPLICATION OF MACHINE LEARNING <br>
 <br>
 import tupa123 as tu <br>
 <br>
 model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, fa2c=5, fa3c=5, fa4c=0) <br>
-X_new = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
-y_resposta = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
+X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000) <br>
+y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) <br>
 y_pred = model.Predict(X_new) <br>
 <br>
 tu.Statistics(y_pred, y_resposta) <br>
 tu.PlotCorrelation(y_pred, y_resposta) <br>
 tu.PlotComparative(y_pred, y_resposta) <br>
 input('end') <br>
 <br>
 #<b>------Commented file:------------------------------------------</b> <br>
 <br>
 #-----MACHINE LEARNING <br>
 <br>
 <b>import tupa123 as tu</b> <br>
 #import the library <br>
 <br>
-<b>X = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300)</b> <br>
-<b>y = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300)</b> <br>
+<b>X = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=300)</b> <br>
+<b>y = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=300)</b> <br>
 #learning data <br>
 #The data can come from any source, but the ExcelMatrix function allows a practical interaction with Excel <br>
 #ExcelMatrix = collect data from excel, the spreadsheet needs to be in the same folder as the python file <br>
 #'ALETAS.xlsm' = example name of the excel file / 'Sheet1' = example name of the tab where the data are <br>
 #Lineini=2, Columini=1 = example initial row and column of data <br>
 #linesquantity = number of lines of learning data <br>
 #X = regression input data / y = data to be predicted <br>
 <br>
-<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0)</b> <br>
+<b>model = tu.nnet4(norma=5, coef=0, normout=1, nn1c=5, nn2c=7, nn3c=5, nn4c=2, rate=0.01, epochs=2000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='')</b> <br>
 #creates the Neural Network model <br>
+<br>
 #norma = type of data normalization: (default=2)<br>
 #=-1, standardization <br>
 #=0, do anything <br>
 #=1, between 0 and 1 <br>
 #=2, between -1 and 1 <br>
 #=3, log(x+coef) <br>
 #=4, log(x+coef)  between 0 and 1 <br>
 #=5, log(x+coef)  between -1 and 1 <br>
 #=6, log(x+coef)  and standardization <br>
 #coef = used to avoid zero in log normalizations, example 0.0012345 (default=0)<br>
-#normout = if 1 normalizes the output (default=1) <br>
+#normout = if 1 normalizes the output (default=1), 0 dont <br>
+<br>
 #nn1c=5, nn2c=7, nn3c=5, nn4c=2 = number of neurons from the first to the fourth layer (default=1,5,5,1) <br>
 #rate = learning rate (default=0.01) <br>
 #epochs = number of epochs (default=1000)<br>
 #fa2c=5, fa3c=5, fa4c=0 = second to fourth layer activation functions (default=5,5,0) <br>
 #for regression the fourth layer is recommended as linear = 0 <br>
+#cost=0, cost function, (default=0). 0 = MSE, mean squared error for regression and classification / 1 = BCE, binary cross entropy for classification <br>
+#regu= regularization, (default=0). Usual value for regression = 0.01 <br>
+#namenet= name of the folder where the weights are saved, default is the same directory as the .py file, necessary when working with more than one neural network <br>
+<br>
 #Activation functions: <br>
 #=0 linear <br> 
 #=1 Sigmoide <br>
 #=2 softpluss <br>
 #=3 gaussinana <br>
 #=4 ReLU <br>
 #=5 tanh <br>
@@ -97,14 +109,15 @@
 #=14 X**3 <br>
 #=15 Symmetric Rectified Linear <br>
 <br>
 <b>model.Fit_ADAM(X, y) </b><br>
 #machine learning <br>
 #model.Fit_ADAM(X, y) = single batch interpolation of all learning data, with ADAM accelerator <br>
 #model.Fit_STOC(X, y) = case-by-case interpolation, stochastic gradient descent <br>
+#model.Fit_STOC_ADAM(X, y) = case-by-case interpolation, stochastic with ADAM <br>
 <br>
 <b>model.Plotconv()</b> <br>
 #Plot the convergence process <br>
 <br>
 input('End') <br>
 <br>
 #-----APPLICATION OF MACHINE LEARNING <br>
@@ -112,18 +125,18 @@
 <b>import tupa123 as tu</b> <br>
 <br>
 <b>model = tu.nnet4(norma=5, coef=0, nn1c=5, nn2c=7, nn3c=5, nn4c=2, fa2c=5, fa3c=5, fa4c=0) </b><br>
 #application file must be in the same folder as the learning file <br>
 #where some .txt files were generated with the neural network settings <br>
 #neural network must have the same configuration that was used in the learning phase <br>
 <br>
-<b>X_new = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000)</b> <br>
+<b>X_new = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=1, columnquantity=5, linesquantity=1000)</b> <br>
 #variables to be predicted <br>
 <br>
-<b>y_resposta = tu.ExcelMatrix('ALETAS.xlsm', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) </b><br>
+<b>y_resposta = tu.ExcelMatrix('ALETAS.xlsx', 'Plan1', Lineini=2, Columini=6, columnquantity=2, linesquantity=1000) </b><br>
 #right answer to compare, to evaluate neural network performance <br>
 <br>
 <b>y_pred = model.Predict(X_new) </b><br>
 #prediction, neural network result <br>
 <br>
 <b>tu.Statistics(y_pred, y_resposta) </b><br>
 #Statistical evaluation of the results <br>
@@ -134,20 +147,23 @@
 <br>
 <b>tu.PlotCorrelation2(y_pred, y_resposta) </b><br>
 #Calculated and target correlation plot with standard deviation lines<br>
 <br>
 <b>tu.PlotComparative(y_pred, y_resposta) </b><br>
 #Calculated and target comparative plot <br>
 <br>
-<b>tu.PlotComparative2(y_pred, y_resposta) </b><br>
-#Calculated and target comparative plot <br>
+<b>tu.PlotComparative2(y_pred, y_resposta, window_size=1000) </b><br>
+#Error plot with movel average<br>
 <br>
 <b>tu.PlotComparative3(y_pred, y_resposta) </b><br>
 #Calculated and target comparative plot with standard deviation areas <br>
 <br>
+<b>tu.PlotComparative4(y_pred, y_resposta) </b><br>
+#Plot 2 sigma tandard deviation areas with target <br>
+<br>
 <b>tu.PlotDispe(y_pred, y_resposta) </b><br>
 #Error dispersion <br>
 <br>
 <b>tu.PlotDispe2(y_pred, y_resposta) </b><br>
 #Error dispersion with error proportion<br>
 <br>
 <b>tu.PlotHisto(y_pred, y_resposta) </b><br>
```

