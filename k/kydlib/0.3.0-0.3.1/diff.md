# Comparing `tmp/kydlib-0.3.0.tar.gz` & `tmp/kydlib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kydlib-0.3.0.tar", last modified: Fri Feb  3 17:44:55 2023, max compression
+gzip compressed data, was "kydlib-0.3.1.tar", last modified: Thu Apr 13 17:32:29 2023, max compression
```

## Comparing `kydlib-0.3.0.tar` & `kydlib-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 afranio    (501) staff       (20)        0 2023-02-03 17:44:55.025880 kydlib-0.3.0/
--rw-r--r--   0 afranio    (501) staff       (20)     4654 2023-02-03 17:44:55.025428 kydlib-0.3.0/PKG-INFO
--rw-r--r--   0 afranio    (501) staff       (20)     3441 2023-01-27 00:52:10.000000 kydlib-0.3.0/README.md
-drwxr-xr-x   0 afranio    (501) staff       (20)        0 2023-02-03 17:44:55.021659 kydlib-0.3.0/kydlib/
--rw-rw-r--   0 afranio    (501) staff       (20)       46 2022-08-17 22:00:16.000000 kydlib-0.3.0/kydlib/__init__.py
--rwxr-xr-x   0 afranio    (501) staff       (20)    16819 2023-01-27 00:46:12.000000 kydlib-0.3.0/kydlib/kydlib.py
-drwxr-xr-x   0 afranio    (501) staff       (20)        0 2023-02-03 17:44:55.024695 kydlib-0.3.0/kydlib.egg-info/
--rw-r--r--   0 afranio    (501) staff       (20)     4654 2023-02-03 17:44:54.000000 kydlib-0.3.0/kydlib.egg-info/PKG-INFO
--rw-r--r--   0 afranio    (501) staff       (20)      203 2023-02-03 17:44:54.000000 kydlib-0.3.0/kydlib.egg-info/SOURCES.txt
--rw-r--r--   0 afranio    (501) staff       (20)        1 2023-02-03 17:44:54.000000 kydlib-0.3.0/kydlib.egg-info/dependency_links.txt
--rw-r--r--   0 afranio    (501) staff       (20)      144 2023-02-03 17:44:54.000000 kydlib-0.3.0/kydlib.egg-info/requires.txt
--rw-r--r--   0 afranio    (501) staff       (20)        7 2023-02-03 17:44:54.000000 kydlib-0.3.0/kydlib.egg-info/top_level.txt
--rw-r--r--   0 afranio    (501) staff       (20)       38 2023-02-03 17:44:55.026057 kydlib-0.3.0/setup.cfg
--rwxr-xr-x   0 afranio    (501) staff       (20)      861 2023-02-03 17:41:17.000000 kydlib-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:32:29.144123 kydlib-0.3.1/
+-rw-rw-rw-   0        0        0     1089 2023-02-02 15:50:21.000000 kydlib-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3876 2023-04-13 17:32:29.144123 kydlib-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3554 2023-02-02 15:50:21.000000 kydlib-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:32:29.111235 kydlib-0.3.1/kydlib/
+-rw-rw-rw-   0        0        0       48 2023-02-02 15:50:21.000000 kydlib-0.3.1/kydlib/__init__.py
+-rw-rw-rw-   0        0        0    17288 2023-04-13 17:03:25.000000 kydlib-0.3.1/kydlib/kydlib.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:32:29.139729 kydlib-0.3.1/kydlib.egg-info/
+-rw-rw-rw-   0        0        0     3876 2023-04-13 17:32:28.000000 kydlib-0.3.1/kydlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-13 17:32:28.000000 kydlib-0.3.1/kydlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:32:28.000000 kydlib-0.3.1/kydlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-04-13 17:32:28.000000 kydlib-0.3.1/kydlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-13 17:32:28.000000 kydlib-0.3.1/kydlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:32:29.145125 kydlib-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-04-13 17:04:07.000000 kydlib-0.3.1/setup.py
```

### Comparing `kydlib-0.3.0/README.md` & `kydlib-0.3.1/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-# KydLIB: Know Your Data Library
-
-KydLIB  is a Python module that provides tools for exploratory data analysis. It is specially designed to work with time series data typically obtained from process system engineering (PSE) applications, although it can also be useful for many types of data.
-
-There are methods for analyzing and visualizing:
-
-* linear and nonlinear pair correlations;
-* autocorrelations;
-* signal-to-noise ratios;
-* multivariate Gaussianity.
-
-For details on methodologies and application examples, see:
-
-* Melo et al. (2022): Open benchmarks for assessment of process monitoring and fault diagnosis techniques: A review and critical analysis. [doi:10.1016/j.compchemeng.2022.107964](https://doi.org/10.1016/j.compchemeng.2022.107964).
-* Laarne et al. (2021): ennemi: Non-linear correlation detection with mutual information. [doi:10.1016/j.softx.2021.100686](https://doi.org/10.1016/j.softx.2021.100686).
-* Zhang et al. (2016): A Novel Strategy of the Data Characteristics Test for Selecting a Process Monitoring Method Automatically. [doi:10.1021/acs.iecr.5b03525](https://doi.org/10.1021/acs.iecr.5b03525).
-* Feital and Pinto (2015): Use of variance spectra for in-line validation of process measurements in continuous processes. [doi:10.1002/cjce.22219](https://doi.org/10.1002/cjce.22219).
-
-## Installation
-
-### With pip
-
-```
-pip install kydlib
-```
-
-### With conda
-
-```
-conda install -c conda-forge kydlib
-```
-## Usage
-
-Let's download a dataset from the Tennessee Eastman Process benchmark to serve as an example:
-
-```python
-import pandas as pd
-
-url = 'https://raw.githubusercontent.com/camaramm/tennessee-eastman-profBraatz/master/d00_te.dat'
-df = pd.read_csv(url, delim_whitespace=True, header=None).iloc[:,:22]
-```
-To use KydLIB, we must instantiate a `Study` object providing the data to be analyzed:
-
-```python
-import kydlib
-
-s = kydlib.Study(df)
-```
-We are now ready to do the exploratory data analysis.
-
-#### Lineplots
-
-```python
-s.lineplot()
-```
-
-![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_lines.png)
-
-#### Scatterplots
-
-```python
-s.scatterplot()
-```
-
-![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_scatter.png)
-
-#### Linear and nonlinear correlations
-
-```python
-s.corr_coef()
-s.corr_coef_plot()
-```
-![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_correlation.png)
-
-#### Autocorrelation
-
-```python
-s.autocorrelation()
-s.autocorrelation_plot()
-```
-![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_autocorrelation.png)
-
-#### Signal-to-noise ratio
-
-```python
-s.signal_to_noise()
-s.signal_to_noise_plot()
-```
-![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_snr.png)
-
-#### Multivariate Gaussianity
-
-```python
-s.gaussianity()
-s.gaussianity_plot()
-```
-
-![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_gaussianity.png)
-
-## Citing
-
-If this package has helped you in your research, consider citing:
-
-```
-@article{melo_open_2022,
-  title = {Open benchmarks for assessment of process monitoring and fault diagnosis techniques: A review and critical analysis},
-  journal = {Computers \& Chemical Engineering},
-  volume = {165},  
-  pages = {107964},
-  year = {2022},
-  doi = {10.1016/j.compchemeng.2022.107964},
-  author = {Melo, Afrânio and Câmara, Maurício M. and Clavijo, Nayher and Pinto, José Carlos}
-}
+# KydLIB: Know Your Data Library
+
+KydLIB  is a Python module that provides tools for exploratory data analysis. It is specially designed to work with time series data typically obtained from process system engineering (PSE) applications, although it can also be useful for many types of data.
+
+There are methods for analyzing and visualizing:
+
+* linear and nonlinear pair correlations;
+* autocorrelations;
+* signal-to-noise ratios;
+* multivariate Gaussianity.
+
+For details on methodologies and application examples, see:
+
+* Melo et al. (2022): Open benchmarks for assessment of process monitoring and fault diagnosis techniques: A review and critical analysis. [doi:10.1016/j.compchemeng.2022.107964](https://doi.org/10.1016/j.compchemeng.2022.107964).
+* Laarne et al. (2021): ennemi: Non-linear correlation detection with mutual information. [doi:10.1016/j.softx.2021.100686](https://doi.org/10.1016/j.softx.2021.100686).
+* Zhang et al. (2016): A Novel Strategy of the Data Characteristics Test for Selecting a Process Monitoring Method Automatically. [doi:10.1021/acs.iecr.5b03525](https://doi.org/10.1021/acs.iecr.5b03525).
+* Feital and Pinto (2015): Use of variance spectra for in-line validation of process measurements in continuous processes. [doi:10.1002/cjce.22219](https://doi.org/10.1002/cjce.22219).
+
+## Installation
+
+### With pip
+
+```
+pip install kydlib
+```
+
+### With conda
+
+```
+conda install -c conda-forge kydlib
+```
+## Usage
+
+Let's download a dataset from the Tennessee Eastman Process benchmark to serve as an example:
+
+```python
+import pandas as pd
+
+url = 'https://raw.githubusercontent.com/camaramm/tennessee-eastman-profBraatz/master/d00_te.dat'
+df = pd.read_csv(url, delim_whitespace=True, header=None).iloc[:,:22]
+```
+To use KydLIB, we must instantiate a `Study` object providing the data to be analyzed:
+
+```python
+import kydlib
+
+s = kydlib.Study(df)
+```
+We are now ready to do the exploratory data analysis.
+
+#### Lineplots
+
+```python
+s.lineplot()
+```
+
+![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_lines.png)
+
+#### Scatterplots
+
+```python
+s.scatterplot()
+```
+
+![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_scatter.png)
+
+#### Linear and nonlinear correlations
+
+```python
+s.corr_coef()
+s.corr_coef_plot()
+```
+![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_correlation.png)
+
+#### Autocorrelation
+
+```python
+s.autocorrelation()
+s.autocorrelation_plot()
+```
+![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_autocorrelation.png)
+
+#### Signal-to-noise ratio
+
+```python
+s.signal_to_noise()
+s.signal_to_noise_plot()
+```
+![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_snr.png)
+
+#### Multivariate Gaussianity
+
+```python
+s.gaussianity()
+s.gaussianity_plot()
+```
+
+![](https://raw.githubusercontent.com/afraniomelo/KydLIB/main/examples/assets/tep_gaussianity.png)
+
+## Citing
+
+If this package has helped you in your research, consider citing:
+
+```
+@article{melo_open_2022,
+  title = {Open benchmarks for assessment of process monitoring and fault diagnosis techniques: A review and critical analysis},
+  journal = {Computers \& Chemical Engineering},
+  volume = {165},  
+  pages = {107964},
+  year = {2022},
+  doi = {10.1016/j.compchemeng.2022.107964},
+  author = {Melo, Afrânio and Câmara, Maurício M. and Clavijo, Nayher and Pinto, José Carlos}
+}
 ```
```

### Comparing `kydlib-0.3.0/kydlib/kydlib.py` & `kydlib-0.3.1/kydlib/kydlib.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,471 +1,471 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Aug 17 18:43:59 2022
-
-@author: afranio
-"""
-
-import numpy as np
-import pandas as pd
-
-import scipy.spatial
-import scipy.stats
-from statsmodels.graphics.tsaplots import acf
-from ennemi import pairwise_corr
-
-import matplotlib.pyplot as plt
-import seaborn as sns
-import datashader as ds
-import colorcet as cc
-
-class Study():
-    
-    def __init__ (self, data):
-        
-        """
-        Constructor.
-        
-        Parameters
-        ----------
-        data: pandas.DataFrame or numpy.array
-            Data that will serve as the basis for the study.
-        """
-        
-        self.data = data
-        self.n = data.shape[0]
-        self.m = data.shape[1]
-        
-    def lineplot (self, ylabels = None, lw = 0.7, figsize = (12,10),
-                  return_fig = False):
-        """
-        Lineplots of individual variables.
-        
-        Parameters
-        ----------    
-        ylabels: sequence, optional
-            Values to use for ylabels. If None, use 1 to n_variables.
-        lw: float, optional
-            Linewidths.
-        figsize: a tuple (width, height) in inches
-        return_fig: boolean, optional
-            Whether to return the matplotlib.figure.Figure object.          
-        """
-        
-        data = pd.DataFrame(self.data)
-        m = data.shape[1]
-        
-        if ylabels is None:
-            ylabels = range(1,m+1)
-        
-        n_graph = len(ylabels)
-        
-        fig, ax = plt.subplots(m, 1, figsize=figsize)
-        
-        for i in range(n_graph):
-            ax[i].plot(data.iloc[:,i].index, 
-                       data.iloc[:,i], c='k', linewidth=lw)
-            ax[i].set_ylabel(ylabels[i], rotation=0, fontsize=14)
-            ax[i].set_yticks([])
-            ax[i].spines["top"].set_visible(False)
-            ax[i].spines["right"].set_visible(False)
-            ax[i].spines["left"].set_visible(False)
-            if i<(n_graph-1):
-                        ax[i].set_xticks([])
-                        ax[i].spines["bottom"].set_visible(False)
-                        ax[i].xaxis.set_ticks_position('none')
-            else:
-                for label in ax[i].get_xticklabels():
-                    label.set_rotation(45)
-                    label.set_ha('right')
-                    
-        if return_fig:
-            return fig
-     
-    def scatterplot (self, cols = None, ticklabels = None, 
-                     figsize = (15,15), px = 5, cmap = cc.fire,
-                     return_fig = False):
-        
-        """
-        Scatterplot using the Datashader package.
-        
-        Parameters
-        ----------
-        cols: sequence of str, optional
-            Which data variables to plot. If None, all variables are plotted.
-        ticklabels: sequence, optional
-            Values to use for ticks. If None, use 1 to n_variables.
-        figsize: a tuple (width, height) in inches
-        px: int, optional
-            Datashader parameter. Number of pixels to spread on all sides.
-        cmap: list of colors or matplotlib.colors.Colormap, optional
-            Datashader parameter. The colormap to use for 2D agg arrays. 
-            Can be either a list of colors (specified either by name, 
-            RGBA hexcode, or as a tuple of (red, green, blue) values.), 
-            or a matplotlib colormap object. 
-        return_fig: boolean, optional
-            Whether to return the matplotlib.figure.Figure object.      
-        """
-
-        data = pd.DataFrame(self.data)
-        
-        data.columns = [str(c) for c in data.columns]
-        
-        if cols is None:
-            cols = data.columns
-        
-        if ticklabels is None:
-            ticklabels = range(1,len(cols)+1)
-        
-        n_graph = len(ticklabels)
-        
-        fig, ax = plt.subplots(n_graph, n_graph, figsize=figsize)
-        
-        for i in range(n_graph):
-            for j in range(n_graph):
-                if i <= j:
-                    ax[i,j].set_visible(False)
-                else:
-                    cvs = ds.Canvas()
-                    agg = cvs.points(data, cols[j], cols[i])
-                    img = ds.tf.set_background(ds.tf.shade(
-                                               ds.tf.spread(agg,px=5), 
-                                               cmap=cmap), "white").to_pil()
-                    ax[i,j].imshow(img)
-                    if j==0:
-                        ax[i,j].set_ylabel(ticklabels[i])
-                    if i==n_graph-1:
-                        ax[i,j].set_xlabel(ticklabels[j])
-                ax[i,j].xaxis.set_ticks([])
-                ax[i,j].yaxis.set_ticks([])
-                ax[i,j].spines['top'].set_visible(False)
-                ax[i,j].spines['right'].set_visible(False)
-                ax[i,j].spines['bottom'].set_visible(False)
-                ax[i,j].spines['left'].set_visible(False)
-                
-        if return_fig:
-            return fig
-        
-    def corr_coef (self, cols = None):
-        
-        """
-        Linear (Pearson) and nonlinear (mutual info) correlation coefficients. 
-        The mutual info coefficients are computed using the 
-        [ennemi package](https://github.com/polsys/ennemi).
-        Check [this](https://doi.org/10.1021/acs.iecr.5b03525) and 
-        [this](https://doi.org/10.1016/j.softx.2021.100686) papers for
-        details on the methodology.
-        
-        Parameters
-        ----------
-        cols: sequence, optional
-            Which data variables to consider in the calculation.
-            If None, all variables are plotted.
-        """        
-        
-        if cols is None:
-            data = np.array(self.data)
-        else:
-            data = np.array(pd.DataFrame(self.data[cols]))
-            
-        m = data.shape[1]
-                
-        self.vxy = pairwise_corr(data)
-        np.fill_diagonal(self.vxy,1)
-                
-        self.rho_xy = np.corrcoef(data,rowvar=False)
-        self.rxy = self.vxy*(1-np.abs(self.rho_xy))
-        
-        self.r = np.sqrt((self.rxy**2).sum()/(m**2-m))
-        self.rho = np.sqrt(((self.rho_xy**2).sum()-m)/(m**2-m))
-        
-    def corr_coef_plot (self, ax = None, labels = None, title = True,
-                        return_fig = False):
-
-        """
-        Plot heatmaps of results computed by the `corr_coef` method.
-        
-        Parameters
-        ----------
-        ax: matplotlib.axes._subplots.AxesSubplot, optional
-            Axes on which the graph will be plotted.
-            If None, a figure with axes will be generated.
-        labels: sequence, optional
-            Values to use for ticks. If None, use 1 to n_variables.  
-        title: boolean, optional
-            If True, the Figure will have a suptitle containing the values of
-            overall correlation coefficients.
-        return_fig: boolean, optional
-            Whether to return the matplotlib.figure.Figure object.      
-        """        
-        
-        if ax is None:
-            fig, ax = plt.subplots(1,3,figsize=(15,5))
-        if labels is None:
-            labels=range(1,self.m+1)
-            
-        mask = np.zeros_like(self.vxy)
-
-        mask[np.triu_indices_from(mask)] = True
-        
-        sns.heatmap(self.vxy,ax=ax[0],cmap='Reds', mask=mask,
-                    xticklabels=labels, yticklabels=labels, vmin=0, vmax=1)
-        sns.heatmap(self.rho_xy,ax=ax[1],cmap='coolwarm',
-                    xticklabels=labels, yticklabels=labels, mask=mask,
-                    vmin=-1, vmax=1)
-        sns.heatmap(self.rxy,ax=ax[2],cmap='Reds', mask=mask,
-                    xticklabels=labels, yticklabels=labels, vmin=0, vmax=1)
-        
-        ax[0].set_title('Mutual info coefficients')
-        ax[1].set_title('Pearson linearity coefficients')
-        ax[2].set_title('Nonlinearity coefficients')
-        
-        fig = ax[0].get_figure()
-        
-        if title:
-            fig.suptitle(f'Overall linearity coefficient: '
-                         f'{self.rho:.3f}\n'
-                         f'Overall nonlinearity coefficient: '
-                         f'{self.r:.3f}')
-        
-        #ax[0].set_xlabel('Variables')
-        #ax[1].set_xlabel('Variables')
-        #ax[2].set_xlabel('Variables')
-        
-        fig.tight_layout()
-        
-        if return_fig:
-            return fig
-        
-    def gaussianity (self):
-
-        """
-        Gaussianity test using Mahalanobis distance.
-        For more details on the methodology, check 
-        [this](https://doi.org/10.1021/acs.iecr.5b03525) paper.    
-        """     
-        
-        data = np.array(self.data)
-        
-        S = np.cov(data, rowvar=False, ddof=1)
-        
-        if np.linalg.matrix_rank(self.data)==self.m:
-            inv_cov = np.linalg.inv(S)
-        else:
-            inv_cov = np.linalg.pinv(S)
-            
-        mean = self.data.mean(axis=0)
-        D = np.array([scipy.spatial.distance.mahalanobis(data[i,:],
-                                                         mean,inv_cov)**2 
-                      for i in range(self.n)])
-        Dt = np.sort(D)
-        rt = [(t-0.5)/self.n for t in range(1,self.n+1)]
-        coef = self.m*(self.n**2-1)/(self.n*(self.n-self.m))
-        Ft = np.array([coef*scipy.stats.f.ppf(p, self.m, 
-                                              self.n-self.m) for p in rt])
-        F_mean = np.mean(Ft)
-        reg = scipy.stats.linregress(Dt,Ft)
-        a, b, r2 = reg[1], reg[0], reg[2]
-        s = np.sqrt(((Ft-(a+b*Dt))**2).sum()/(self.n-2))
-        significance = s/F_mean
-        if significance>0.15:
-            gaussian = False
-        else:
-            if np.abs(b-1) <0.2 and np.abs(a)<F_mean*0.05:
-                gaussian = True
-            else:
-                gaussian = False
-                
-        (self.a, self.b, self.significance, self.r2, 
-         self.Dt, self.Ft, self.gaussian) = (a, b, significance, 
-                                             r2, Dt, Ft, gaussian)
-
-    def gaussianity_plot (self, ax = None, return_fig = False):
-        
-        """
-        Plot results computed by the `gaussianity` method.
-        
-        Parameters
-        ----------
-        ax: matplotlib.axes._subplots.AxesSubplot, optional
-            Axis on which the graph will be plotted.
-            If None, the method will use the current axis.
-        return_fig: boolean, optional
-            Whether to return the matplotlib.figure.Figure object.      
-        """
-        
-        if ax is None:
-            ax = plt.gca()
-            
-        ax.plot(self.Dt, self.Ft,marker='o',ls='',color='k',ms=4)
-        x = np.linspace(self.Dt[0], self.Dt[-1])
-        y = self.b*x+self.a
-        ax.plot(x,y,c='r',ls='--',linewidth=4)
-        title = (f'a={self.a:.3f}, b={self.b:.3f}, ' 
-                 f'sig = {100*self.significance:.2f}%\nData Gaussianity '
-                 f'is {self.gaussian}.')
-        ax.set_title(title)
-        ax.grid('on')
-        ax.set_xlabel('Dt')
-        ax.set_ylabel('Ft')
-        
-        if return_fig:
-            return ax.get_figure()
-        
-    def autocorrelation (self, nlags = 50):
-
-        """
-        Autocorrelation function calculation using the statsmodel package.
-        
-        Parameters
-        ----------
-        nlags: int, optional
-            statsmodel parameter. 
-            Number of lags to return autocorrelation for.
-        """    
-        
-        data = pd.DataFrame(self.data)
-        
-        self.lags_y = []
-        self.lags_x = np.arange(1,nlags+1)
-        
-        for i in range(self.m):
-            
-            y = acf(data.iloc[:,i],nlags=nlags)[1:]
-            self.lags_y.append(y)
-            
-    def autocorrelation_plot (self, plot_acf = False, plot_bar = True,
-                              ax_acf = None, ax_bar = None, title_bar = True,
-                              critic_auto = 0.5,
-                              return_fig = False):
-
-        """
-        Plot results computed by the `autocorrelation` method.
-        
-        Two types of plots can be made:
-            
-            * autocorrelation function traditional plots;
-            * bar plots showing the time necessary to achieve a critic value
-            of autocorrelation (tipically 0.5) for each variable.
-        
-        Parameters
-        ----------
-        plot_acf: boolean, optional
-            If autocorrelation functions will be plotted.
-        plot_bar: boolean, optional
-            If the bar graph will be plotted.
-        ax_acf: matplotlib.axes._subplots.AxesSubplot, optional
-            Axes on which the autocorrelation functions will be plotted.
-            It must be provided if plot_acf is True.
-        ax_bar: matplotlib.axes._subplots.AxesSubplot, optional
-            Axes on which the bar graph will be plotted.
-            If None, and if plot_bar is True, 
-            a figure with an axis will be generated.
-        title_bar: boolean, optional
-            If True, the Figure will have a title describing what it means.
-        critic_auto: float, optional
-            Value to use as a critical threshold for the bar plot.
-        return_fig: boolean, optional
-            Whether to return the matplotlib.figure.Figure objects.
-        """    
-        
-        data = pd.DataFrame(self.data)
-
-        if plot_acf:
-
-            for i in range(self.m):
-                ax_acf.ravel()[i].plot(self.lags_x, self.lags_y[i],c='k')
-                ax_acf.ravel()[i].axhline(critic_auto,c='r',ls='--')
-                title = data.iloc[:,i].name
-                ax_acf.ravel()[i].set_title(title);
-                fig_acf = ax_acf[0].get_figure()
-        
-        else:
-            fig_acf = None
-            
-        if plot_bar:
-            
-            if ax_bar is None:
-                fig_bar, ax_bar = plt.subplots()
-                
-        else:
-            
-            fig_bar= None
-
-            self.critic_auto_x = [np.searchsorted(-self.lags_y[i],
-                                                  -critic_auto) 
-                                  for i in range(len(self.lags_y))]
-
-            ax_bar.bar(range(1,len(self.critic_auto_x)+1),
-                       np.array(self.critic_auto_x), color='k');
-            ax_bar.set_xlabel('Variable')
-            ax_bar.set_ylabel('Number of lags')
-            ax_bar.set_xlim([0,self.m+1]);
-            ax_bar.set_xticks(np.arange(1,self.m+1));
-            ax_bar.xaxis.set_tick_params(labelsize=12)
-            ax_bar.axhline(np.mean(self.critic_auto_x),
-                           ls='-',c='k',label='mean')
-            ax_bar.axhline(np.median(self.critic_auto_x),ls='-.',
-                           c='k',label='median')
-            ax_bar.legend();
-            if title_bar:
-                ax_bar.set_title(f'Number of lags necessary to achieve'
-                                 f' {critic_auto} autocorrelation')
-            
-        if return_fig:
-            return fig_acf, fig_bar
-
-    def signal_to_noise (self):
-
-        """
-        Signal-to-noise ratios using the variance spectra.
-        For more details on the methodology, check 
-        [this](https://doi.org/10.1002/cjce.22219) paper.    
-        """    
-                
-        self.snr = np.zeros(self.m)
-        
-        # https://stackoverflow.com/questions/39232790
-        idx = lambda WS,d: \
-        (d*np.arange((self.n-WS+1)/d)[:,None].astype(int) + \
-        np.arange(WS))
-            
-        data = np.array(self.data)
-        
-        for j in range(self.m):
-            WS = 2
-            win = data[idx(WS,1)]
-            self.var_noise = np.mean(np.var(win,ddof=1,axis=1),axis=0)
-            self.var_signal = np.var(data,ddof=1,axis=0)    
-            self.snr = self.var_signal/self.var_noise    
-            
-    def signal_to_noise_plot (self, ax = None, return_fig = False):
-
-        """
-        Plot results computed by the `signal_to_noise` method.
-        
-        Parameters
-        ----------
-        ax: matplotlib.axes._subplots.AxesSubplot, optional
-            Axis on which the graph will be plotted.
-            If None, the method will use the current axis.
-        return_fig: boolean, optional
-            Whether to return the matplotlib.figure.Figure object. 
-        """
-        
-        if ax is None: 
-            fig, ax = plt.subplots()
-            
-        ax.bar(np.arange(1,len(self.snr)+1),self.snr,color='k')
-        ax.set_xlabel('Variable')
-        ax.set_ylabel('Signal-to-noise ratio')
-        ax.axhline(1,ls='--',c='r',label='snr=1')
-        ax.axhline(np.mean(self.snr),ls='-',c='k',label='mean')
-        ax.axhline(np.median(self.snr),ls='-.',c='k',label='median')
-        ax.set_yscale('log')
-        ax.set_xlim([0,self.m+1]);
-        ax.set_xticks(np.arange(1,self.m+1));
-        ax.legend();
-        
-        if return_fig:
-            return ax.get_figure()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Aug 17 18:43:59 2022
+
+@author: afranio
+"""
+
+import numpy as np
+import pandas as pd
+
+import scipy.spatial
+import scipy.stats
+from statsmodels.graphics.tsaplots import acf
+from ennemi import pairwise_corr
+
+import matplotlib.pyplot as plt
+import seaborn as sns
+import datashader as ds
+import colorcet as cc
+
+class Study():
+    
+    def __init__ (self, data):
+        
+        """
+        Constructor.
+        
+        Parameters
+        ----------
+        data: pandas.DataFrame or numpy.array
+            Data that will serve as the basis for the study.
+        """
+        
+        self.data = data
+        self.n = data.shape[0]
+        self.m = data.shape[1]
+        
+    def lineplot (self, ylabels = None, lw = 0.7, figsize = (12,10),
+                  return_fig = False):
+        """
+        Lineplots of individual variables.
+        
+        Parameters
+        ----------    
+        ylabels: sequence, optional
+            Values to use for ylabels. If None, use 1 to n_variables.
+        lw: float, optional
+            Linewidths.
+        figsize: a tuple (width, height) in inches
+        return_fig: boolean, optional
+            Whether to return the matplotlib.figure.Figure object.          
+        """
+        
+        data = pd.DataFrame(self.data)
+        m = data.shape[1]
+        
+        if ylabels is None:
+            ylabels = range(1,m+1)
+        
+        n_graph = len(ylabels)
+        
+        fig, ax = plt.subplots(m, 1, figsize=figsize)
+        
+        for i in range(n_graph):
+            ax[i].plot(data.iloc[:,i].index, 
+                       data.iloc[:,i], c='k', linewidth=lw)
+            ax[i].set_ylabel(ylabels[i], rotation=0, fontsize=14)
+            ax[i].set_yticks([])
+            ax[i].spines["top"].set_visible(False)
+            ax[i].spines["right"].set_visible(False)
+            ax[i].spines["left"].set_visible(False)
+            if i<(n_graph-1):
+                        ax[i].set_xticks([])
+                        ax[i].spines["bottom"].set_visible(False)
+                        ax[i].xaxis.set_ticks_position('none')
+            else:
+                for label in ax[i].get_xticklabels():
+                    label.set_rotation(45)
+                    label.set_ha('right')
+                    
+        if return_fig:
+            return fig
+     
+    def scatterplot (self, cols = None, ticklabels = None, 
+                     figsize = (15,15), px = 5, cmap = cc.fire,
+                     return_fig = False):
+        
+        """
+        Scatterplot using the Datashader package.
+        
+        Parameters
+        ----------
+        cols: sequence of str, optional
+            Which data variables to plot. If None, all variables are plotted.
+        ticklabels: sequence, optional
+            Values to use for ticks. If None, use 1 to n_variables.
+        figsize: a tuple (width, height) in inches
+        px: int, optional
+            Datashader parameter. Number of pixels to spread on all sides.
+        cmap: list of colors or matplotlib.colors.Colormap, optional
+            Datashader parameter. The colormap to use for 2D agg arrays. 
+            Can be either a list of colors (specified either by name, 
+            RGBA hexcode, or as a tuple of (red, green, blue) values.), 
+            or a matplotlib colormap object. 
+        return_fig: boolean, optional
+            Whether to return the matplotlib.figure.Figure object.      
+        """
+
+        data = pd.DataFrame(self.data)
+        
+        data.columns = [str(c) for c in data.columns]
+        
+        if cols is None:
+            cols = data.columns
+        
+        if ticklabels is None:
+            ticklabels = range(1,len(cols)+1)
+        
+        n_graph = len(ticklabels)
+        
+        fig, ax = plt.subplots(n_graph, n_graph, figsize=figsize)
+        
+        for i in range(n_graph):
+            for j in range(n_graph):
+                if i <= j:
+                    ax[i,j].set_visible(False)
+                else:
+                    cvs = ds.Canvas()
+                    agg = cvs.points(data, cols[j], cols[i])
+                    img = ds.tf.set_background(ds.tf.shade(
+                                               ds.tf.spread(agg,px=5), 
+                                               cmap=cmap), "white").to_pil()
+                    ax[i,j].imshow(img)
+                    if j==0:
+                        ax[i,j].set_ylabel(ticklabels[i])
+                    if i==n_graph-1:
+                        ax[i,j].set_xlabel(ticklabels[j])
+                ax[i,j].xaxis.set_ticks([])
+                ax[i,j].yaxis.set_ticks([])
+                ax[i,j].spines['top'].set_visible(False)
+                ax[i,j].spines['right'].set_visible(False)
+                ax[i,j].spines['bottom'].set_visible(False)
+                ax[i,j].spines['left'].set_visible(False)
+                
+        if return_fig:
+            return fig
+        
+    def corr_coef (self, cols = None):
+        
+        """
+        Linear (Pearson) and nonlinear (mutual info) correlation coefficients. 
+        The mutual info coefficients are computed using the 
+        [ennemi package](https://github.com/polsys/ennemi).
+        Check [this](https://doi.org/10.1021/acs.iecr.5b03525) and 
+        [this](https://doi.org/10.1016/j.softx.2021.100686) papers for
+        details on the methodology.
+        
+        Parameters
+        ----------
+        cols: sequence, optional
+            Which data variables to consider in the calculation.
+            If None, all variables are plotted.
+        """        
+        
+        if cols is None:
+            data = np.array(self.data)
+        else:
+            data = np.array(pd.DataFrame(self.data[cols]))
+            
+        m = data.shape[1]
+                
+        self.vxy = pairwise_corr(data)
+        np.fill_diagonal(self.vxy,1)
+                
+        self.rho_xy = np.corrcoef(data,rowvar=False)
+        self.rxy = self.vxy*(1-np.abs(self.rho_xy))
+        
+        self.r = np.sqrt((self.rxy**2).sum()/(m**2-m))
+        self.rho = np.sqrt(((self.rho_xy**2).sum()-m)/(m**2-m))
+        
+    def corr_coef_plot (self, ax = None, labels = None, title = True,
+                        return_fig = False):
+
+        """
+        Plot heatmaps of results computed by the `corr_coef` method.
+        
+        Parameters
+        ----------
+        ax: matplotlib.axes._subplots.AxesSubplot, optional
+            Axes on which the graph will be plotted.
+            If None, a figure with axes will be generated.
+        labels: sequence, optional
+            Values to use for ticks. If None, use 1 to n_variables.  
+        title: boolean, optional
+            If True, the Figure will have a suptitle containing the values of
+            overall correlation coefficients.
+        return_fig: boolean, optional
+            Whether to return the matplotlib.figure.Figure object.      
+        """        
+        
+        if ax is None:
+            fig, ax = plt.subplots(1,3,figsize=(15,5))
+        if labels is None:
+            labels=range(1,self.m+1)
+            
+        mask = np.zeros_like(self.vxy)
+
+        mask[np.triu_indices_from(mask)] = True
+        
+        sns.heatmap(self.vxy,ax=ax[0],cmap='Reds', mask=mask,
+                    xticklabels=labels, yticklabels=labels, vmin=0, vmax=1)
+        sns.heatmap(self.rho_xy,ax=ax[1],cmap='coolwarm',
+                    xticklabels=labels, yticklabels=labels, mask=mask,
+                    vmin=-1, vmax=1)
+        sns.heatmap(self.rxy,ax=ax[2],cmap='Reds', mask=mask,
+                    xticklabels=labels, yticklabels=labels, vmin=0, vmax=1)
+        
+        ax[0].set_title('Mutual info coefficients')
+        ax[1].set_title('Pearson linearity coefficients')
+        ax[2].set_title('Nonlinearity coefficients')
+        
+        fig = ax[0].get_figure()
+        
+        if title:
+            fig.suptitle(f'Overall linearity coefficient: '
+                         f'{self.rho:.3f}\n'
+                         f'Overall nonlinearity coefficient: '
+                         f'{self.r:.3f}')
+        
+        #ax[0].set_xlabel('Variables')
+        #ax[1].set_xlabel('Variables')
+        #ax[2].set_xlabel('Variables')
+        
+        fig.tight_layout()
+        
+        if return_fig:
+            return fig
+        
+    def gaussianity (self):
+
+        """
+        Gaussianity test using Mahalanobis distance.
+        For more details on the methodology, check 
+        [this](https://doi.org/10.1021/acs.iecr.5b03525) paper.    
+        """     
+        
+        data = np.array(self.data)
+        
+        S = np.cov(data, rowvar=False, ddof=1)
+        
+        if np.linalg.matrix_rank(self.data)==self.m:
+            inv_cov = np.linalg.inv(S)
+        else:
+            inv_cov = np.linalg.pinv(S)
+            
+        mean = self.data.mean(axis=0)
+        D = np.array([scipy.spatial.distance.mahalanobis(data[i,:],
+                                                         mean,inv_cov)**2 
+                      for i in range(self.n)])
+        Dt = np.sort(D)
+        rt = [(t-0.5)/self.n for t in range(1,self.n+1)]
+        coef = self.m*(self.n**2-1)/(self.n*(self.n-self.m))
+        Ft = np.array([coef*scipy.stats.f.ppf(p, self.m, 
+                                              self.n-self.m) for p in rt])
+        F_mean = np.mean(Ft)
+        reg = scipy.stats.linregress(Dt,Ft)
+        a, b, r2 = reg[1], reg[0], reg[2]
+        s = np.sqrt(((Ft-(a+b*Dt))**2).sum()/(self.n-2))
+        significance = s/F_mean
+        if significance>0.15:
+            gaussian = False
+        else:
+            if np.abs(b-1) <0.2 and np.abs(a)<F_mean*0.05:
+                gaussian = True
+            else:
+                gaussian = False
+                
+        (self.a, self.b, self.significance, self.r2, 
+         self.Dt, self.Ft, self.gaussian) = (a, b, significance, 
+                                             r2, Dt, Ft, gaussian)
+
+    def gaussianity_plot (self, ax = None, return_fig = False):
+        
+        """
+        Plot results computed by the `gaussianity` method.
+        
+        Parameters
+        ----------
+        ax: matplotlib.axes._subplots.AxesSubplot, optional
+            Axis on which the graph will be plotted.
+            If None, the method will use the current axis.
+        return_fig: boolean, optional
+            Whether to return the matplotlib.figure.Figure object.      
+        """
+        
+        if ax is None:
+            ax = plt.gca()
+            
+        ax.plot(self.Dt, self.Ft,marker='o',ls='',color='k',ms=4)
+        x = np.linspace(self.Dt[0], self.Dt[-1])
+        y = self.b*x+self.a
+        ax.plot(x,y,c='r',ls='--',linewidth=4)
+        title = (f'a={self.a:.3f}, b={self.b:.3f}, ' 
+                 f'sig = {100*self.significance:.2f}%\nData Gaussianity '
+                 f'is {self.gaussian}.')
+        ax.set_title(title)
+        ax.grid('on')
+        ax.set_xlabel('Dt')
+        ax.set_ylabel('Ft')
+        
+        if return_fig:
+            return ax.get_figure()
+        
+    def autocorrelation (self, nlags = 50):
+
+        """
+        Autocorrelation function calculation using the statsmodel package.
+        
+        Parameters
+        ----------
+        nlags: int, optional
+            statsmodel parameter. 
+            Number of lags to return autocorrelation for.
+        """    
+        
+        data = pd.DataFrame(self.data)
+        
+        self.lags_y = []
+        self.lags_x = np.arange(1,nlags+1)
+        
+        for i in range(self.m):
+            
+            y = acf(data.iloc[:,i],nlags=nlags)[1:]
+            self.lags_y.append(y)
+            
+    def autocorrelation_plot (self, plot_acf = False, plot_bar = True,
+                              ax_acf = None, ax_bar = None, title_bar = True,
+                              critic_auto = 0.5,
+                              return_fig = False):
+
+        """
+        Plot results computed by the `autocorrelation` method.
+        
+        Two types of plots can be made:
+            
+            * autocorrelation function traditional plots;
+            * bar plots showing the time necessary to achieve a critic value
+            of autocorrelation (tipically 0.5) for each variable.
+        
+        Parameters
+        ----------
+        plot_acf: boolean, optional
+            If autocorrelation functions will be plotted.
+        plot_bar: boolean, optional
+            If the bar graph will be plotted.
+        ax_acf: matplotlib.axes._subplots.AxesSubplot, optional
+            Axes on which the autocorrelation functions will be plotted.
+            It must be provided if plot_acf is True.
+        ax_bar: matplotlib.axes._subplots.AxesSubplot, optional
+            Axes on which the bar graph will be plotted.
+            If None, and if plot_bar is True, 
+            a figure with an axis will be generated.
+        title_bar: boolean, optional
+            If True, the Figure will have a title describing what it means.
+        critic_auto: float, optional
+            Value to use as a critical threshold for the bar plot.
+        return_fig: boolean, optional
+            Whether to return the matplotlib.figure.Figure objects.
+        """    
+        
+        data = pd.DataFrame(self.data)
+
+        if plot_acf:
+
+            for i in range(self.m):
+                ax_acf.ravel()[i].plot(self.lags_x, self.lags_y[i],c='k')
+                ax_acf.ravel()[i].axhline(critic_auto,c='r',ls='--')
+                title = data.iloc[:,i].name
+                ax_acf.ravel()[i].set_title(title);
+                fig_acf = ax_acf[0].get_figure()
+        
+        else:
+            fig_acf = None
+            
+        if plot_bar:
+            
+            if ax_bar is None:
+                fig_bar, ax_bar = plt.subplots()
+
+            self.critic_auto_x = [np.searchsorted(-self.lags_y[i],
+                                                    -critic_auto) 
+                                    for i in range(len(self.lags_y))]
+
+            ax_bar.bar(range(1,len(self.critic_auto_x)+1),
+                        np.array(self.critic_auto_x), color='k');
+            ax_bar.set_xlabel('Variable')
+            ax_bar.set_ylabel('Number of lags')
+            ax_bar.set_xlim([0,self.m+1]);
+            ax_bar.set_xticks(np.arange(1,self.m+1));
+            ax_bar.xaxis.set_tick_params(labelsize=12)
+            ax_bar.axhline(np.mean(self.critic_auto_x),
+                            ls='-',c='k',label='mean')
+            ax_bar.axhline(np.median(self.critic_auto_x),ls='-.',
+                            c='k',label='median')
+            ax_bar.legend();
+            if title_bar:
+                ax_bar.set_title(f'Number of lags necessary to achieve'
+                                    f' {critic_auto} autocorrelation')
+                
+        else:
+            
+            fig_bar= None
+
+        if return_fig:
+            return fig_acf, fig_bar
+
+    def signal_to_noise (self):
+
+        """
+        Signal-to-noise ratios using the variance spectra.
+        For more details on the methodology, check 
+        [this](https://doi.org/10.1002/cjce.22219) paper.    
+        """    
+                
+        self.snr = np.zeros(self.m)
+        
+        # https://stackoverflow.com/questions/39232790
+        idx = lambda WS,d: \
+        (d*np.arange((self.n-WS+1)/d)[:,None].astype(int) + \
+        np.arange(WS))
+            
+        data = np.array(self.data)
+        
+        for j in range(self.m):
+            WS = 2
+            win = data[idx(WS,1)]
+            self.var_noise = np.mean(np.var(win,ddof=1,axis=1),axis=0)
+            self.var_signal = np.var(data,ddof=1,axis=0)    
+            self.snr = self.var_signal/self.var_noise    
+            
+    def signal_to_noise_plot (self, ax = None, return_fig = False):
+
+        """
+        Plot results computed by the `signal_to_noise` method.
+        
+        Parameters
+        ----------
+        ax: matplotlib.axes._subplots.AxesSubplot, optional
+            Axis on which the graph will be plotted.
+            If None, the method will use the current axis.
+        return_fig: boolean, optional
+            Whether to return the matplotlib.figure.Figure object. 
+        """
+        
+        if ax is None: 
+            fig, ax = plt.subplots()
+            
+        ax.bar(np.arange(1,len(self.snr)+1),self.snr,color='k')
+        ax.set_xlabel('Variable')
+        ax.set_ylabel('Signal-to-noise ratio')
+        ax.axhline(1,ls='--',c='r',label='snr=1')
+        ax.axhline(np.mean(self.snr),ls='-',c='k',label='mean')
+        ax.axhline(np.median(self.snr),ls='-.',c='k',label='median')
+        ax.set_yscale('log')
+        ax.set_xlim([0,self.m+1]);
+        ax.set_xticks(np.arange(1,self.m+1));
+        ax.legend();
+        
+        if return_fig:
+            return ax.get_figure()
```

### Comparing `kydlib-0.3.0/setup.py` & `kydlib-0.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Aug  17 20:03:43 2022
-
-@author: afranio
-"""
-
-import setuptools
-import os
-
-with open('README.md') as f:
-    README = f.read()
-    
-requirements = os.path.dirname(os.path.realpath(__file__))+'/requirements.txt'
-
-if os.path.isfile(requirements):
-    with open(requirements) as f:
-        install_requires = f.read().splitlines()
-
-setuptools.setup(
-    author="Afrânio Melo",
-    author_email="afraeq@gmail.com",
-    name='kydlib',
-    description='Routines for exploratory data analysis.',
-    license="MIT",
-    version='0.3.0',
-    long_description=README,
-    long_description_content_type='text/markdown',
-    url='https://github.com/afraniomelo/kydlib',
-    packages=setuptools.find_packages(include=['kydlib','kydlib.*']),
-    python_requires=">=3.7",
-    install_requires=install_requires
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Aug  17 20:03:43 2022
+
+@author: afranio
+"""
+
+import setuptools
+import os
+
+with open('README.md') as f:
+    README = f.read()
+    
+requirements = os.path.dirname(os.path.realpath(__file__))+'/requirements.txt'
+
+if os.path.isfile(requirements):
+    with open(requirements) as f:
+        install_requires = f.read().splitlines()
+
+setuptools.setup(
+    author="Afrânio Melo",
+    author_email="afraeq@gmail.com",
+    name='kydlib',
+    description='Routines for exploratory data analysis.',
+    license="MIT",
+    version='0.3.1',
+    long_description=README,
+    long_description_content_type='text/markdown',
+    url='https://github.com/afraniomelo/kydlib',
+    packages=setuptools.find_packages(include=['kydlib','kydlib.*']),
+    python_requires=">=3.7",
+    install_requires=install_requires
 )
```

