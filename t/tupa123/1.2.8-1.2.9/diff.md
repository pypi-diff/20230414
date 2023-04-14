# Comparing `tmp/tupa123-1.2.8.tar.gz` & `tmp/tupa123-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.2.8.tar", last modified: Tue Apr  4 17:44:37 2023, max compression
+gzip compressed data, was "tupa123-1.2.9.tar", last modified: Tue Apr  4 19:24:19 2023, max compression
```

## Comparing `tupa123-1.2.8.tar` & `tupa123-1.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 17:44:37.063140 tupa123-1.2.8/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0     6636 2023-04-04 17:44:37.063140 tupa123-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     6273 2023-04-04 17:40:49.000000 tupa123-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 17:44:37.063140 tupa123-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-04-04 17:34:48.000000 tupa123-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 17:44:37.047518 tupa123-1.2.8/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.2.8/tupa123/__init__.py
--rw-rw-rw-   0        0        0    38693 2023-04-04 17:20:20.000000 tupa123-1.2.8/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-04 17:44:37.063140 tupa123-1.2.8/tupa123.egg-info/
--rw-rw-rw-   0        0        0     6636 2023-04-04 17:44:36.000000 tupa123-1.2.8/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-04 17:44:36.000000 tupa123-1.2.8/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 17:44:36.000000 tupa123-1.2.8/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-04 17:44:36.000000 tupa123-1.2.8/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-04 17:44:36.000000 tupa123-1.2.8/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-04 19:24:19.590237 tupa123-1.2.9/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     6636 2023-04-04 19:24:19.590237 tupa123-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6273 2023-04-04 17:40:49.000000 tupa123-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-04 19:24:19.590237 tupa123-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      672 2023-04-04 19:24:09.000000 tupa123-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-04 19:24:19.580202 tupa123-1.2.9/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.2.9/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    38979 2023-04-04 19:20:04.000000 tupa123-1.2.9/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-04 19:24:19.590237 tupa123-1.2.9/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     6636 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-04 19:24:19.000000 tupa123-1.2.9/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.2.8/LICENSE.txt` & `tupa123-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.2.8/PKG-INFO` & `tupa123-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.2.8
+Version: 1.2.9
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.2.8/README.md` & `tupa123-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.2.8/setup.py` & `tupa123-1.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.2.8',
+    version='1.2.9',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy>=1.23.5','matplotlib>=3.6.3','pandas>=1.5.3'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.2.8/tupa123/tupa123.py` & `tupa123-1.2.9/tupa123/tupa123.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,17 @@
         eixoY1= Targeted[:,j]
         eixoY2= Calculated[:,j]
     
         plt.figure(figsize=(12, 5))
         plt.title('Comparison chart calculated variable vs targeted')
         plt.xlabel('Sequence of events')
         plt.ylabel('Target and predicted variable ' + str(j+1))
-        plt.plot(eixoX, eixoY1, marker = '', color = 'darkblue', label='Targeted')  
-        plt.plot(eixoX, eixoY2, marker = '', color = 'orangered', label='Calculated')
+        plt.plot(eixoX, eixoY1, marker = '', label='Targeted')  
+        plt.plot(eixoX, eixoY2, marker = '', label='Calculated')
+        #plt.plot(eixoX, eixoY2, c='black', marker = '.', label='Calculated', alpha=0.33)
         plt.legend(loc = "upper left")
         plt.show()
 
 
 
 
 
@@ -117,29 +118,33 @@
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
     
         plt.figure(figsize=(12, 5))
         plt.title('Comparison chart calculated variable vs targeted')
         plt.xlabel('Sequence of events')
         plt.ylabel('Target and predicted variable ' + str(j+1))
-        plt.plot(eixoX, eixoY1, marker = '', color = 'black', label='Targeted')  
-        plt.plot(eixoX, eixoY2, marker = '', color = 'orangered', label='Calculated')
-        plt.legend(loc = "upper left")
+        plt.plot(eixoX, eixoY1, marker = '',  label='Targeted')  
+        plt.plot(eixoX, eixoY2, linestyle='none', c='black', marker = '.', label='Calculated', alpha=0.33)
+        plt.legend(loc = "upper right")
 
         # Preenchendo a área entre as curvas
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - sigma, eixoY1 + erro_medio + sigma, color='gray', alpha=0.3)
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.2)
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 3*sigma, eixoY1 + erro_medio + 3*sigma, color='gray', alpha=0.1)
+
+        # Adicionando o valor do desvio padrão ao canto superior esquerdo do gráfico
+        plt.text(0.025, 0.95, "sigma = {:.2f}".format(sigma) + ", average = {:.2f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
         
         plt.show()
 
 
 
 
 
+
 #Plot correlation between calculated variables and objectives
 def PlotCorrelation(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
@@ -255,15 +260,15 @@
         
         eixoY3 = eixoY2 - eixoY1        
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
         eixoY4 = eixoY3/sigma
         
                         
-        plt.title('Targeted snipper, variable '+ str(j+1))
+        plt.title('Target vs sniper, variable '+ str(j+1))
         plt.scatter(eixoY4,razao,color='blue',s=15,edgecolor='red') #grafico de correlação entre as variaveis procuradas e alvo---
         plt.xlabel('Standard deviation sigma')
         plt.ylabel('Proportion = calculated/targeted')
 
         plt.plot([-1,1], [1,1], color='black', alpha=0.9, linestyle='dashed')
         plt.plot([0,0], [1-(np.max(razao)-1)*0.5,1+(np.max(razao)-1)*0.5], color='black', alpha=0.9, linestyle='dashed')
         
@@ -281,15 +286,16 @@
 def PlotHisto(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
 
     for j in range(0,numevar):    
         eixoY1= Targeted[:,j]
         eixoY2= Calculated[:,j]
-        eixoY3 = 100*(eixoY2 - eixoY1)/eixoY1 #erro percentual 0-100%
+        
+        eixoY3 = eixoY2 - eixoY1 #erro
 
         fig, ax = plt.subplots()
         
         desviopad = np.std(eixoY3) #devio padrão do erro
         erromedio = np.mean(eixoY3) #erro medio
         
         textstr = '\n'.join((r'$\mathrm{average}=%.2f$' % (erromedio, ),r'$\sigma=%.2f$' % (desviopad, )))
@@ -297,16 +303,16 @@
         ax.hist(eixoY3, bins=20, rwidth=0.9, color='blue', alpha=0.7, edgecolor='black')
         # these are matplotlib.patch.Patch properties
         props = dict(boxstyle='round', facecolor='wheat', alpha=0.5)
 
         # place a text box in upper left in axes coords
         ax.text(0.05, 0.95, textstr, transform=ax.transAxes, fontsize=14, verticalalignment='top', bbox=props)
 
-        plt.title('Percent error histogram', fontsize=15)
-        plt.xlabel('Variable ' + str(j+1) + ', %', fontsize=12)
+        plt.title('Error histogram', fontsize=15)
+        plt.xlabel('Variable ' + str(j+1) , fontsize=12)
         plt.ylabel('Frequency', fontsize=12)
 
         plt.show()
```

### Comparing `tupa123-1.2.8/tupa123.egg-info/PKG-INFO` & `tupa123-1.2.9/tupa123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.2.8
+Version: 1.2.9
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression classification tupa123
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

