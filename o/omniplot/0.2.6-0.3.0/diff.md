# Comparing `tmp/omniplot-0.2.6.tar.gz` & `tmp/omniplot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplot-0.2.6.tar", last modified: Mon Apr  3 02:49:12 2023, max compression
+gzip compressed data, was "omniplot-0.3.0.tar", last modified: Fri Apr 14 03:24:53 2023, max compression
```

## Comparing `omniplot-0.2.6.tar` & `omniplot-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-03 02:49:12.830483 omniplot-0.2.6/
--rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-03-02 01:40:14.000000 omniplot-0.2.6/LICENSE
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-03 02:49:12.826483 omniplot-0.2.6/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-03-31 07:39:48.000000 omniplot-0.2.6/README.md
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-03 02:49:12.826483 omniplot-0.2.6/omniplot/
--rw-rw-r--   0 koh       (1000) koh       (1000)      299 2023-03-29 01:49:18.000000 omniplot-0.2.6/omniplot/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-03 02:27:14.000000 omniplot-0.2.6/omniplot/_version.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-03-31 09:32:32.000000 omniplot-0.2.6/omniplot/chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-03-02 01:40:14.000000 omniplot-0.2.6/omniplot/chipseq_utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-03 02:49:12.826483 omniplot-0.2.6/omniplot/cython_utils/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-03-02 01:40:14.000000 omniplot-0.2.6/omniplot/cython_utils/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-03-02 01:40:14.000000 omniplot-0.2.6/omniplot/data.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    12847 2023-03-02 01:40:14.000000 omniplot-0.2.6/omniplot/igraph_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    31933 2023-03-09 08:59:09.000000 omniplot-0.2.6/omniplot/networkplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    50036 2023-03-30 07:06:19.000000 omniplot-0.2.6/omniplot/plot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-03-31 09:12:42.000000 omniplot-0.2.6/omniplot/plot_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    60834 2023-03-31 09:01:37.000000 omniplot-0.2.6/omniplot/proportion.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-03-13 07:42:01.000000 omniplot-0.2.6/omniplot/regressionplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   117295 2023-04-03 02:23:43.000000 omniplot-0.2.6/omniplot/scatter.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-03 02:49:12.826483 omniplot-0.2.6/omniplot/scripts/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-03-02 01:40:14.000000 omniplot-0.2.6/omniplot/scripts/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-03-02 01:40:14.000000 omniplot-0.2.6/omniplot/scripts/gff2tss.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-03-15 05:07:07.000000 omniplot-0.2.6/omniplot/statistics.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    41510 2023-04-02 06:03:10.000000 omniplot-0.2.6/omniplot/utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-03 02:49:12.826483 omniplot-0.2.6/omniplot.egg-info/
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-03 02:49:12.000000 omniplot-0.2.6/omniplot.egg-info/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)      644 2023-04-03 02:49:12.000000 omniplot-0.2.6/omniplot.egg-info/SOURCES.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-03 02:49:12.000000 omniplot-0.2.6/omniplot.egg-info/dependency_links.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)      200 2023-04-03 02:49:12.000000 omniplot-0.2.6/omniplot.egg-info/requires.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-03 02:49:12.000000 omniplot-0.2.6/omniplot.egg-info/top_level.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-03 02:49:12.830483 omniplot-0.2.6/setup.cfg
--rw-rw-r--   0 koh       (1000) koh       (1000)     2747 2023-03-29 03:09:46.000000 omniplot-0.2.6/setup.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-03 02:49:12.826483 omniplot-0.2.6/tests/
--rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.2.6/tests/test_chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3029 2023-03-09 08:54:57.000000 omniplot-0.2.6/tests/test_network.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    11869 2023-04-03 01:48:18.000000 omniplot-0.2.6/tests/tests.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-14 03:24:53.566883 omniplot-0.3.0/
+-rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-03-02 01:40:14.000000 omniplot-0.3.0/LICENSE
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-14 03:24:53.566883 omniplot-0.3.0/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-03-31 07:39:48.000000 omniplot-0.3.0/README.md
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-14 03:24:53.566883 omniplot-0.3.0/omniplot/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      299 2023-03-29 01:49:18.000000 omniplot-0.3.0/omniplot/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-14 02:52:11.000000 omniplot-0.3.0/omniplot/_adjustText.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-14 03:05:59.000000 omniplot-0.3.0/omniplot/_version.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-03-31 09:32:32.000000 omniplot-0.3.0/omniplot/chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-03-02 01:40:14.000000 omniplot-0.3.0/omniplot/chipseq_utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-14 03:24:53.566883 omniplot-0.3.0/omniplot/cython_utils/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-03-02 01:40:14.000000 omniplot-0.3.0/omniplot/cython_utils/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-03-02 01:40:14.000000 omniplot-0.3.0/omniplot/data.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    12847 2023-03-02 01:40:14.000000 omniplot-0.3.0/omniplot/igraph_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    31933 2023-03-09 08:59:09.000000 omniplot-0.3.0/omniplot/networkplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    50009 2023-04-13 05:07:27.000000 omniplot-0.3.0/omniplot/plot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-03-31 09:12:42.000000 omniplot-0.3.0/omniplot/plot_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    73071 2023-04-05 07:46:21.000000 omniplot-0.3.0/omniplot/proportion.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-03-13 07:42:01.000000 omniplot-0.3.0/omniplot/regressionplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   132637 2023-04-14 03:05:35.000000 omniplot-0.3.0/omniplot/scatter.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-14 03:24:53.566883 omniplot-0.3.0/omniplot/scripts/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-03-02 01:40:14.000000 omniplot-0.3.0/omniplot/scripts/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-03-02 01:40:14.000000 omniplot-0.3.0/omniplot/scripts/gff2tss.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-03-15 05:07:07.000000 omniplot-0.3.0/omniplot/statistics.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    41917 2023-04-14 02:47:28.000000 omniplot-0.3.0/omniplot/utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-14 03:24:53.566883 omniplot-0.3.0/omniplot.egg-info/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-14 03:24:53.000000 omniplot-0.3.0/omniplot.egg-info/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)      668 2023-04-14 03:24:53.000000 omniplot-0.3.0/omniplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-14 03:24:53.000000 omniplot-0.3.0/omniplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-04-14 03:24:53.000000 omniplot-0.3.0/omniplot.egg-info/requires.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-14 03:24:53.000000 omniplot-0.3.0/omniplot.egg-info/top_level.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-14 03:24:53.566883 omniplot-0.3.0/setup.cfg
+-rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-14 03:01:51.000000 omniplot-0.3.0/setup.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-14 03:24:53.566883 omniplot-0.3.0/tests/
+-rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.3.0/tests/test_chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3033 2023-04-12 09:33:24.000000 omniplot-0.3.0/tests/test_network.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    13490 2023-04-14 02:53:22.000000 omniplot-0.3.0/tests/tests.py
```

### Comparing `omniplot-0.2.6/LICENSE` & `omniplot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/PKG-INFO` & `omniplot-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.2.6
+Version: 0.3.0
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.2.6/README.md` & `omniplot-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/chipseq.py` & `omniplot-0.3.0/omniplot/chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/chipseq_utils.py` & `omniplot-0.3.0/omniplot/chipseq_utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/igraph_classes.py` & `omniplot-0.3.0/omniplot/igraph_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/networkplot.py` & `omniplot-0.3.0/omniplot/networkplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/plot.py` & `omniplot-0.3.0/omniplot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1342,13 +1342,12 @@
         
     _save(save, "violin")
     
     return {"p values":newpvals,"axes":ax}
 
 
 
-def volcanoplot():
-    pass
+
 
 
 if __name__=="__main__":
     pass
```

### Comparing `omniplot-0.2.6/omniplot/plot_classes.py` & `omniplot-0.3.0/omniplot/plot_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/proportion.py` & `omniplot-0.3.0/omniplot/proportion.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 maker_list: list=['.', '_' , '+','|', 'x', 'v', '^', '<', '>', 's', 'p', '*', 'h', 'D', 'd', 'P', 'X','o', '1', '2', '3', '4','|', '_']
 
 plt.rcParams['font.family']= 'sans-serif'
 plt.rcParams['font.sans-serif'] = ['Arial']
 plt.rcParams['svg.fonttype'] = 'none'
 sns.set_theme(font="Arial")
 
-__all__=["stacked_barplot","nice_piechart","nice_piechart_num","stackedlines","nested_piechart","_nested_piechart"]
+__all__=["stacked_barplot","nice_piechart","nice_piechart_num","stackedlines","nested_piechart","_nested_piechart","stacked_barplot_num"]
 
 def _stacked_barplot(df: pd.DataFrame,
                     x: Union[str, list],
                     hue: Union[str, list],
                     scale: str="fraction",
                     order: list=[],
                     hue_order: list=[],
@@ -321,28 +321,29 @@
                     hue: Union[str, list],
                     scale: str="fraction",
                     order: Optional[list]=None,
                     hue_order: Optional[list]=None,
                     test_pairs: List[List[str]]=[],
                     palette: Union[str,dict]="tab20c",
                     show_values: bool=True,
+                    show_values_intact: bool=False,
                     show: bool=False,
                     figsize: List[int]=[],
                     xunit: str="",
                     yunit: str="",
                     title: str="",
                     hatch: bool=False,
                     rotation: int=90,
                     ax: Optional[plt.Axes]=None,
                     show_legend:bool=True,
                     bin_num: Union[dict, int]=10,
                     ylim: Optional[int]=None)-> Dict:
     
     """
-    Drawing a stacked barplot with or without the fisher's exact test 
+    Drawing a stacked barplot by counting observations with or without the fisher's exact test. 
     
     Parameters
     ----------
     df : pandas DataFrame
     
     x: str or list
         The category to place in x axis. Multiple categories can be passed by a list. 
@@ -361,15 +362,18 @@
                     ["Gentoo","Chinstrap" ],
                     ["Adelie","Gentoo" ]]
     palette : str or dict, optional (default: "tab20c")
         A matplotlib colormap name or dictionary in which keys are values of the hue category and values are RGB array.
         e.g.) palette={""}
     show_values: bool, optional
         Wheter to exhibit the values of fractions/counts/percentages.
-    
+
+    show_values_intact: bool, optional
+        Wheter to exhibit non-scaled counts.
+
     show : bool, optional
         Whether or not to show the figure.
     
     figsize : List[int], optional
         The figure size, e.g., [4, 6].
     title: str optional, (default:"")
         The title of the figure.
@@ -383,15 +387,15 @@
         Whether to show legends.
     bin_num: dict, int, optional (default: 10)
         A histogram bin number when columns with float values are selected. 
         You can specify the bin number of each column by using dictionary (e.g., bin_num={"A":10,"B",5}).
 
     Returns
     -------
-    dict {"pval":pvals,"axes":ax}
+    {"pval":pvals,"axes":ax,"data":data} : dict
     
     Raises
     ------
     Notes
     -----
     References
     ----------
@@ -645,28 +649,347 @@
     else:
         plt.tight_layout(w_pad=2)
     
     if title !="" and fig !=None:
         fig.suptitle(title)
     if show:
         plt.show()
-    return {"pval":pvals,"axes":ax}
+    return {"pval":pvals,"axes":ax,"data":data}
+
+def stacked_barplot_num(df: pd.DataFrame,
+                    x: str="",
+                    scale: str="fraction",
+                    test_pairs: List[List[str]]=[],
+                    palette: Union[str,dict]="tab20c",
+                    show_values: bool=True,
+                    show_values_intact: bool=False,
+                    show: bool=False,
+                    figsize: List[int]=[],
+                    xlabel: str="",
+                    ylabel: str="",
+                    unit: Union[str, List, Dict]="",
+                    title: str="",
+                    hatch: bool=False,
+                    rotation: Optional[int]=None,
+                    ax: Optional[plt.Axes]=None,
+                    show_legend:bool=True,
+                    ylim: Optional[int]=None,
+                    horizontal: bool=False,
+                    margins: dict={},
+                    gridspec_kw: dict={},
+                    legend_row_num: int=2,
+                    bar_width: float=0.75
+                    )-> Dict:
+    
+    """
+    Drawing a stacked barplot by taking values as an input with or without the fisher's exact test. 
+    
+    Parameters
+    ----------
+    df : pandas DataFrame
+        A wide-form data format.
+        e.g., 
+                  Bournemouth    Brighton
+        Possession         36          64
+        Shots              14          16
+        Shots on Target     3           6
+        Corners             5           5
+        Fouls              11           5
+    
+    x: str
+        The category to place in x axis. If not set, it will use the index of the input dataframe.
+    scale: str, optional
+        Scaling method. Available options are: fraction, percentage, absolute
+    test_pairs : list, optional
+        pairs of categorical values related to x. It will calculate -log10 (p value) (mlp) of the fisher exact test.
+        Examples: [["Adelie","Chinstrap" ],
+                    ["Gentoo","Chinstrap" ],
+                    ["Adelie","Gentoo" ]]
+    palette : str or dict, optional (default: "tab20c")
+        A matplotlib colormap name or dictionary in which keys are values of the hue category and values are RGB array.
+        e.g.) palette={""}
+    show_values: bool, optional
+        Wheter to exhibit the values of fractions/counts/percentages.
+
+    show_values_intact: bool, optional
+        Wheter to exhibit non-scaled values.
+
+    show : bool, optional
+        Whether or not to show the figure.
+    
+    figsize : List[int], optional
+        The figure size, e.g., [4, 6].
+    title: str optional, (default:"")
+        The title of the figure.
+    hatch: bool, optional (default: False)
+        Adding hatches to the bars
+    rotation: int, optional (default:90)
+        The orientation of the x axis labels.
+    ax: plt.Axes, optional (default: None)
+        The ax object to be plotted.
+    show_legend: bool, optional (default: True)
+        Whether to show legends.
+    bin_num: dict, int, optional (default: 10)
+        A histogram bin number when columns with float values are selected. 
+        You can specify the bin number of each column by using dictionary (e.g., bin_num={"A":10,"B",5}).
+
+    Returns
+    -------
+    {"pval":pvals,"axes":ax,"data":data} : dict
+    
+    Raises
+    ------
+    Notes
+    -----
+    References
+    ----------
+    See Also
+    --------
+    Examples
+    --------
+    """
+    if type(df)==Dict:
+        df=pd.DataFrame(df)
+   
+    pvals={}
+    # if len(test_pairs) >0:
+    #     print("mlp stands for -log10(p value)")
+    #     for _hue in hue:
+            
+    #         for i, h in enumerate(huekeys[_hue]):
+                
+    #     for p1,p2 in test_pairs:
+    #         yes_total=np.sum(data[_x][_hue][keys[idx1]])
+    #         no_total=np.sum(data[_x][_hue][keys[idx2]])
+    #         yes_and_hue=data[_x][_hue][keys[idx1]][i]
+    #         no_and_hue=data[_x][_hue][keys[idx2]][i]
+    #         table=[[yes_and_hue, no_and_hue],
+    #                 [yes_total-yes_and_hue, no_total-no_and_hue]]
+
+    #         odd, pval=fisher_exact(table)
+    #         pvals[_x][_hue][h].append([idx1, idx2, pval])
+    
+    
+    if len(gridspec_kw)==0:
+        if horizontal==True:
+            gridspec_kw=dict(top=0.75,left=0.25,right=0.9, bottom=0.17)
+        else:
+            gridspec_kw=dict(top=0.93,left=0.1,right=0.7, bottom=0.17)
+
+    if len(margins)==0:
+        if horizontal==True and scale!="absolute":
+            margins=dict(x=0)
+        else:
+            margins=dict(x=0.1)
+
+
+    if len(figsize)==0:
+        if horizontal==True:
+            figsize=[6, len(df.index)/2]
+        else:
+            figsize=[len(df.columns)+1, 6]
+    if ax!=None:
+        fig=None
+    else:
+        fig, ax=plt.subplots(figsize=figsize,gridspec_kw=gridspec_kw)
+        plt.margins(**margins)
+    if unit=="":
+        if scale=="absolute":
+            unit=""
+        elif scale=="fraction":
+            unit=""
+        elif scale=="percentage":
+            unit="%"
+
+    pos={}
+    if x=="":
+        keys=list(df.index)
+        _df=df
+    else:
+        keys=list(df[x])
+        _df=df.drop(columns=[x])
+
+    if scale=="fraction":
+        _df=_df.div(_df.sum(axis=1),axis = 'rows',)
+    elif scale=="percentage":
+        _df=100*_df.div(_df.sum(axis=1),axis = 'rows',)
 
 
+    if type(palette)==str:
+        cmap=plt.get_cmap(palette, len(_df.columns)) 
+    pos={}
+    bottom=np.zeros([len(keys)])
+    
+    for i, col in enumerate(_df.columns):
+        # print(col)
+        heights=_df[col].values
+        # print(heights,bottom)
+        originalval=df[col].values
+        if horizontal==True:
+            if type(palette)==dict:
+                if hatch==True:
+                    ax.barh(keys, width=heights,height=bar_width, left=bottom, color=palette[col], label=col, hatch=hatch_list[i])
+                else:
+                    ax.barh(keys, width=heights,height=bar_width, left=bottom, color=palette[col], label=col)
+            else:
+                if hatch==True:
+                    ax.barh(keys, width=heights,height=bar_width, left=bottom, color=cmap(i), label=col, hatch=hatch_list[i])
+                else:
+                    ax.barh(keys, width=heights,height=bar_width, left=bottom, color=cmap(i), label=col)
+
+        else:
+            if type(palette)==dict:
+                if hatch==True:
+                    ax.bar(keys, heights,width=bar_width, bottom=bottom, color=palette[col], label=col, hatch=hatch_list[i])
+                else:
+                    ax.bar(keys, heights,width=bar_width, bottom=bottom, color=palette[col], label=col)
+            else:
+                if hatch==True:
+                    ax.bar(keys, heights,width=bar_width, bottom=bottom, color=cmap(i), label=col, hatch=hatch_list[i])
+                else:
+                    ax.bar(keys, heights,width=bar_width, bottom=bottom, color=cmap(i), label=col)
+        if show_values==True:
+            
+            for j, k in enumerate(keys):
+                
+                if type(unit)==dict:
+                    if k in unit:
+                        u=unit[k]
+                    else:
+                        u=""
+                elif type(unit)==list:
+                    u=unit[j]
+                else:
+                    u=unit
+                if horizontal==True:
+                    if show_values_intact==True:
+                        ax.text(bottom[j]+heights[j]/2, j,"{}{}".format(originalval[j],u), va="center",ha="center",
+                                bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
+                    else:
+                        ax.text(bottom[j]+heights[j]/2,j,"{:.2f}{}".format(heights[j],u), va="center",ha="center",
+                                bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
+                else:
+                    if show_values_intact==True:
+                        ax.text(j,bottom[j]+heights[j]/2,"{}{}".format(originalval[j],u), ha="center",
+                                bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
+                    else:
+                        ax.text(j,bottom[j]+heights[j]/2,"{:.2f}{}".format(heights[j],u), ha="center",
+                                bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="y", lw=1, alpha=0.8))
+                    
+            
+        pos[col]={key: [he, bo] for key, he, bo in zip(keys, heights, bottom)}
+        bottom+=heights
+    
+    #ax.set_xticklabels(ax.get_xticklabels(), rotation=90)
+    if show_legend==True:
+        if horizontal==True:
+            ax.legend(loc=[0,1.01], ncols=len(_df.columns)//legend_row_num+int(len(_df.columns)%legend_row_num!=0))
+        else:
+            ax.legend(loc=[1.01,0])
+    if horizontal==True:
+        if rotation==None:
+            rotation=0
+
+        if len(keys)==1:
+            ax.set_yticks(ax.get_yticks(), labels=keys, rotation=rotation)
+            ax.margins(x=1)
+        else:
+            ax.set_yticks(ax.get_yticks(), labels=keys, rotation=rotation)
+        ax.set_ylabel(ylabel)
+        if xlabel =="":
+            if show_values_intact==False:
+                if scale=="absolute":
+                    xlabel="Counts"
+                elif scale=="fraction":
+                    xlabel="Fraction"
+                elif scale=="percentage":
+                    xlabel="Percentage"
+        
+        ax.set_xlabel(xlabel)
+    else:
+        if rotation==None:
+            rotation=90
+        if len(keys)==1:
+            ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
+            ax.margins(x=1)
+        else:
+            ax.set_xticks(ax.get_xticks(), labels=keys, rotation=rotation)
+        ax.set_xlabel(xlabel)
+        if ylabel =="":
+            if show_values_intact==False:
+                if scale=="absolute":
+                    ylabel="Counts"
+                elif scale=="fraction":
+                    ylabel="Fraction"
+                elif scale=="percentage":
+                    ylabel="Percentage"
+        ax.set_ylabel(ylabel)
+
+    # if len(pvals)>0:
+        
+    #     for _hue in hue:
+    #         if _x==_hue:
+    #             continue
+    #         if not _hue in pos[_x]:
+    #             continue
+    #         hues=huekeys[_hue]
+    #         for i, h in enumerate(hues):
+    #             #print(pos)
+    #             #print(pos[_x])
+    #             _pos=pos[_x][_hue][h]
+    #             for idx1, idx2, pval in pvals[_x][_hue][h]:
+                    
+    #                 he1, bot1=_pos[keys[idx1]]
+    #                 he2, bot2=_pos[keys[idx2]]
+    #                 line, =ax.plot([idx1,idx2],[he1/2+bot1,he2/2+bot2],color="gray")
+    #                 # r1=ax.transData.transform([idx1, he1/2+bot1])
+    #                 # r2=ax.transData.transform([idx2, he2/2+bot2])
+    #                 r1=np.array([idx1, he1/2+bot1])
+    #                 r2=np.array([idx2, he2/2+bot2])
+    #                 r=r2-r1
+    #                 #print(ax.get_xlim(),ax.get_ylim())
+    #                 r=np.array([1,3])*r/np.array([ax.get_xlim()[1]-ax.get_xlim()[0],ax.get_ylim()[1]-ax.get_ylim()[0]])
+    #                 #r=ax.transData.transform(r)
+    #                 if idx2<idx1:
+    #                     r=-r
+    #                 #print(r)
+    #                 r=r*(r @ r)**(-0.5)
+    #                 #print(h,r)
+    #                 angle=np.arccos(r[0])
+    #                 if r[1]<0:
+    #                     angle= -angle
+    #                 #print(angle)
+    #                 if pval < 0.05:
+    #                     pval_str=str(np.round(-np.log10(pval), decimals=1))
+    #                 else:
+    #                     pval_str="ns"
+    #                 _line_annotate( "mlp="+pval_str, line, (idx1+idx2)/2, color="magenta")
+    if scale=="absolute" and ylim !=None:
+        ax.set_ylim(0, ylim)
+    if horizontal==True:
+        ax.invert_yaxis()
+
+    if title !="" and fig !=None:
+        fig.suptitle(title)
+    if show:
+        plt.show()
+    return {"pval":pvals,"axes":ax}
+
 def nice_piechart(df: pd.DataFrame, 
                   category: Union[str, List[str]],
                   palette: str="tab20c",
                   order: str="largest",
                   ncols: int=2,
                   ignore: float=0.05,
                   show_values: bool=True,
                   title: str="",
                   hatch: bool=False,
                   figsize: list=[],
-                  show_legend:bool=False,bbox_to_anchor: list=[1.1, 1],
+                  show_legend:bool=False,
+                  bbox_to_anchor: list=[1.1, 1],
                   right: float=0.7,bottom=0.1) ->Dict:
     """
     Drawing a nice pichart by counting the occurrence of values from pandas dataframe. if you want to draw a pie chart from numerical values, try nice_piechart_num.
     
     Parameters
     ----------
     df : pandas DataFrame
```

### Comparing `omniplot-0.2.6/omniplot/regressionplot.py` & `omniplot-0.3.0/omniplot/regressionplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/scatter.py` & `omniplot-0.3.0/omniplot/scatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,28 +29,31 @@
 #sys.path.append( script_dir )
 from omniplot.utils import _create_color_markerlut, _separate_data, _line_annotate, _dendrogram_threshold, _radialtree2,_get_cluster_classes,_calc_curveture, _draw_ci_pi,_calc_r2,_ci_pi, _save, _baumkuchen_xy, _get_embedding
 import scipy.stats as stats
 from joblib import Parallel, delayed
 from omniplot.chipseq_utils import _calc_pearson
 import itertools as it
 from matplotlib.ticker import StrMethodFormatter
-
-
+import statsmodels.api as sm
+from sklearn.linear_model import RANSACRegressor
+from matplotlib import colors
+from omniplot._adjustText import adjust_text
+import copy
 colormap_list: list=["nipy_spectral", "terrain","tab20b","tab20c","gist_rainbow","hsv","CMRmap","coolwarm","gnuplot","gist_stern","brg","rainbow","jet"]
 hatch_list: list = ['//', '\\\\', '||', '--', '++', 'xx', 'oo', 'OO', '..', '**','/o', '\\|', '|*', '-\\', '+o', 'x*', 'o-', 'O|', 'O.', '*-']
 marker_list: list=[ "o",'_' , '+','|', 'x', 'v', '^', '<', '>', 's', 'p', '*', 'h', 'D', 'd', 'P', 'X','.', '1', '2', '3', '4','|', '_']
 
 
 
 plt.rcParams['font.family']= 'sans-serif'
 plt.rcParams['font.sans-serif'] = ['Arial']
 plt.rcParams['svg.fonttype'] = 'none'
 sns.set_theme(font="Arial")
 
-__all__=["clusterplot", "decomplot", "pie_scatter","manifoldplot", "regression_single","scatterplot"]
+__all__=["clusterplot", "decomplot", "pie_scatter","manifoldplot", "regression_single","scatterplot","volcanoplot"]
 def _scatter(_df, 
              x,
              y, 
              cat, 
              ax, 
              lut, 
              barrierfree, 
@@ -193,33 +196,38 @@
                     alpha=0.5)
     _ax.set_yticks([])
 
 
 def scatterplot(df: pd.DataFrame,
                 x: str,
                 y: str,
-
                 ax: Optional[plt.Axes]= None,
                 fig : Optional[mpl.figure.Figure] =None,
 
                 colors: Union[str, List[str]]="",
                 category: Union[str, List[str]]="",
                 sizes: str="",
                 marginal_dist: bool=False,
                 kde: bool=False,
+                kde_kw: dict={},
+
                 kmeans: bool=False,
                 n_clusters: int=3,
                 cluster_center: bool=True,
                 kmeans_kw: dict={},
 
+                regression: bool=False,
+                robust_param: dict={},
+                regression_color: str="lightgreen",
+
                 c: Union[List, np.ndarray] =[],
                 cname: str="",
                 size_scale: float=100,
                 palette: str="",
-                palette_cat: str="tab20c",
+                palette_cat: Union[str, Dict]="tab20c",
                 palette_val: str="coolwarm",
                 size_legend_num: int=4,
                 markers: bool=False,
                 size: float=30.0,
                 show_labels: dict={},
                 alpha: float=1,
                 edgecolors: str="w",
@@ -237,15 +245,17 @@
                 axlabel: str="single",
                 title: str="",
                 show_legend: bool=True,
                 logscalex: bool=False,
                 logscaley: bool=False,
                 figsize: list=[],
                 rows_cols: list=[],
-                save: str="",kde_kw: dict={}
+                save: str="",
+                gridspec_kw: dict={},
+
                 )-> Dict:
     """
     Simple scatter plot. almost same function with seaborn.scatterplot.  
     
     Parameters
     ----------
     df : pandas DataFrame
@@ -322,98 +332,142 @@
         The scale of the point sizes, only effective when "sizes" option is set. If the sizes of points are too small or too large, adjust the sizes with this option.
     edgecolors: str="w", optional
         The point edge color.
     linewidths: float=1, optional
         The point edge width.
     cbar_format, size_format, xformat, yformat: str 
         e.g., "{x:.2f}", '{x:.3E}'
-    
+
+    gridspec_kw: dict, optional
+        Parameters for matplotlib gridspec. (https://matplotlib.org/stable/api/_as_gen/matplotlib.gridspec.GridSpec.html)
+        e.g., {"wspace":0.75,"hspace":0.5}
+    adjust_kw: dict, optional
+
     Return
     ------
-    {"axes":axes, "fig":fig} : dict
+    {"axes":axes, "fig":fig, 
+    "regression_models":regression_models, "regression_results":regression_results, 
+    "kmeans_result":_kmeans, "df":df} : dict
 
     """
+    # functions to scale and rescale the size of each point
     def _scale_size(x, size_scale, smin, smax):
         return size_scale*(0.01+(x-smin)/(smax-smin))
     def _reverse_size(x, size_scale, smin, smax):
         return (x/size_scale-0.01)*(smax-smin)+smin
     
     if len(kde_kw)==0:
         kde_kw=dict(alpha=0.5, levels=4)
     
     if palette !="":
         palette_cat=palette 
         palette_val=palette
     
     original_index=df.index
     
-    X, category=_separate_data(df, variables=[x, y], category=category)
+    X, category=_separate_data(df, 
+                               variables=[x, y], 
+                               category=category)
     if len(colors)!=0:
         if type(colors)==str:
             colors=[colors]
     else: 
         colors=[]
     c=np.array(c)
     if len(c) !=0:
         if cname =="":
             cname="c"
         if len(c.shape)==1:
             df[cname]=c
             colors.append(cname)
 
+    # Calculating clusters and add cluster labels to dataframe
+    _kmeans=None
+    if kmeans==True:
+        _kmeans = KMeans(n_clusters=n_clusters, random_state=0, n_init="auto").fit(X, *kmeans_kw)
+        df["kmeans"]=_kmeans.labels_
+        _kmeanlabels=np.unique(_kmeans.labels_)
+        category.append("kmeans")
+
 
+    totalnum=len(category)+len(colors)+int(len(c.shape)==2)
+    if totalnum<=1:
+        totalnum=1
+        axlabel="each"
     # determining the figure size and the number of rows and columns.
-
+    if len(gridspec_kw)==0:
+        _right=0
+        if show_legend==False:
+            _right+=0.16
+        if totalnum==1:
+            if regression==True:
+                gridspec_kw={"right":0.67+_right, "bottom":0.3}
+            else:
+                gridspec_kw={"right":0.67+_right, "bottom":0.15}
+        elif totalnum==2:
+            if regression==True:
+                gridspec_kw={"wspace":0.75,"hspace":0.5,"right":0.85, "bottom":0.35, "top":0.95}
+            else:
+                gridspec_kw={"wspace":0.75,"right":0.85, "top":0.95}
+        else:
+            if regression==True:
+                gridspec_kw={"wspace":0.75,"hspace":0.5,"right":0.85, "bottom":0.2, "top":0.95}
+            else:
+                gridspec_kw={"wspace":0.75,"right":0.85, "top":0.95}
     if ax !=None:
-        axes=[ax]
+        if totalnum==1 and type(ax)==plt.Axes:
+
+            axes=[ax]
+        elif totalnum>1 and type(ax)==np.ndarray:
+            axes=ax.flatten()
+        elif totalnum>1 and  type(ax)==list:
+            axes=ax
+        elif totalnum>1 and ax==plt.Axes:
+            raise Exception("If you provide the ax option, the number of plots and axes must be equal. \
+                            The total number of plots will be the sum of category and colors plus whether or not c and kmeans options provided")
+        plt.subplots_adjust(**gridspec_kw)
         totalnum=1
         if marginal_dist==True and fig==None:
             raise Exception("if you pass an axis opject and want to draw marginal distribution, you also need to give a figure object")
 
     elif len(rows_cols)==0:
-        totalnum=len(category)+len(colors)+int(len(c.shape)==2)+int(kmeans)
+        
         if totalnum<=1:
-            totalnum=1
             if len(figsize)==0:
-                figsize=[7,5]
-            fig, ax=plt.subplots(figsize=figsize)
+                figsize=[6,4]
+            fig, ax=plt.subplots(figsize=figsize,gridspec_kw=gridspec_kw)
             axes=[ax]
         else:
             if len(figsize)==0:
-                figsize=[10,4*totalnum//2+int(totalnum%2!=0)]
+                if regression==True:
+                    figsize=[9,5*totalnum//2+int(totalnum%2!=0)]
+                else:
+                    figsize=[9,4*totalnum//2+int(totalnum%2!=0)]
+            
             fig, axes=plt.subplots(nrows=totalnum//2+int(totalnum%2!=0),
-                                 ncols=2,figsize=figsize,gridspec_kw={"wspace":0.75})
+                                    ncols=2,figsize=figsize,gridspec_kw=gridspec_kw)
             axes=axes.flatten()
     else:
         if len(figsize)==0:
             figsize=[10,4*totalnum//2+int(totalnum%2!=0)]
         fig, axes=plt.subplots(nrows=rows_cols[0],
                                  ncols=rows_cols[1],
                                  figsize=figsize,
-                                 gridspec_kw={"wspace":0.75})
+                                 gridspec_kw=gridspec_kw)
         axes=axes.flatten()
-    if len(category)+len(colors)==0:
-        plt.subplots_adjust(right=0.67)
-    
-    else:
-        plt.subplots_adjust(right=0.85)
-    
+
 
     if axlabel=="single":
         _axlabeleach=False
     elif axlabel=="non":
         _axlabeleach=False
     elif axlabel=="each":
         _axlabeleach=True
 
-    if kmeans==True:
-        _kmeans = KMeans(n_clusters=n_clusters, random_state=0, n_init="auto").fit(df[[x, y]].values, *kmeans_kw)
-        df["kmeans"]=_kmeans.labels_
-        _kmeanlabels=np.unique(_kmeans.labels_)
-        category.append("kmeans")
+
     # Creating point size array protional to values in the column specified by "sizes" option. 
     # Point sizes are scaled maximum to be size_scale (in order to avoid too small/large points). 
     # And creating a size legend of which size labels correspond to the original values 
     if sizes !="":
 
         size=df[sizes]
         size=np.nan_to_num(size)
@@ -432,15 +486,14 @@
         for _i in range(size_legend_num):
             s=vmin+_i*vinterval
             _s=_reverse_size(s, size_scale, smin, smax)
             size_legend_elements.append(Line2D([0], [0], marker='o', linewidth=0, markeredgecolor="white",markersize=s**(0.5),
                                 label=size_format.format(x=_s),
                                 markerfacecolor="black"))
 
-    
 
     legendx=1.01
     legendy=1
     
     # Preparing x and y ranges for marginal distribution.
     margins=0.1
     if marginal_dist==True:
@@ -454,88 +507,110 @@
         marginal_proportion=0.8
         legendx=legendx/marginal_proportion
     
     
     i=0
     # Drawing scatter plots 
     lut={}
+    regression_models={}
+    regression_results={}
     if len(category) !=0:
         
         for cat in category:
             ax=axes[i]
             ax.margins(margins)
             ax.set_zorder(1)
             i+=1
 
             _clut, _mlut=_create_color_markerlut(df, cat,palette_cat,marker_list)
             
             
             
             lut[cat]={"colorlut":_clut, "markerlut":_mlut}
 
-
-            if cat=="kmeans" and cluster_center==True:
+            # Plotting KMeans results
+            if cat=="kmeans" and cluster_center==True and regression==False:
                 for ul, center in zip(_kmeanlabels, _kmeans.cluster_centers_):
                     _df=df.loc[df["kmeans"]==ul]
                     for _x, _y in zip(_df[x], _df[y]):
-                        ax.plot([center[0], _x], [center[1], _y], color=_clut[ul], alpha=0.5)
-
+                        ax.plot([center[0], _x], [center[1], _y], color=_clut[ul], alpha=0.25)
+            
+            # Plotting regression results
+            if regression==True:
+                fitted_models, reg_results=_regression(df, x, y, ax, cat=cat, _clut=_clut, robust_param=robust_param)
+                regression_models.update(fitted_models)
+                regression_results.update(reg_results)
+            
+            #Plotting a scatter plot
             sc=_scatter(df, x, y, cat, ax, lut, markers, size,
                         axlabel=_axlabeleach,
                         alpha=alpha,
                         edgecolors=edgecolors,
                         linewidths=linewidths,
                         outside=True,legendx=legendx, legendy=legendy, legend=show_legend)
             
-            
-
+            # Plotting a KDE plot
             if kde==True:
-                sns.kdeplot(data=df, x=x, y=y,hue=cat, ax=ax, palette=_clut, **kde_kw)
+                sns.kdeplot(data=df, x=x, y=y,hue=cat, ax=ax, palette=_clut, legend=False, **kde_kw)
+                ax.set(xlabel=None)
+                ax.set(ylabel=None)
+
+            # Plotting marginal distribution
             if marginal_dist==True:
                 _marginal_plot(fig, ax,df, x,y, cat, lut,_xrange,_yrange , marginal_proportion)
 
-            
+            # Setting the format of axes
             _set_axis_format(ax, xformat, yformat, xunit, yunit, logscalex,logscaley)
            
-
+            # Drawing the legend of point sizes
             if sizes !="" and show_legend==True:
 
                 if size_unit!="":
                     sizes=sizes+"("+size_unit+")"
-                ax.add_artist(ax.legend(handles=size_legend_elements, title=sizes,bbox_to_anchor=(legendx,0.5)))
+                ax.add_artist(ax.legend(handles=size_legend_elements, title=sizes,bbox_to_anchor=(legendx,0.6)))
+
+            # Drawing point labels
             if len(show_labels)!=0:
                 _add_labels(ax, df, x, y, show_labels["val"], show_labels["topn"])
+    
+    # Plotting scatter plots with color values specified by "colors"
     if len(colors) !=0:
         if type(color_unit)==str:
             color_unit=[color_unit]
 
         for _c, _unit in zip(colors, color_unit):
             ax=axes[i]
             ax.margins(margins)
             ax.set_zorder(1)
             i+=1
             _df=df.sort_values(by=[_c], ascending=True)
             if type(size)==float or type(size)==int:
                 _size=size
             else:
                 _size=size[np.argsort(df[_c])]
+
+            if regression==True:
+                fitted_models, reg_results=_regression(df, x, y, ax, robust_param=robust_param, newkey="total", color=regression_color)
+                regression_models.update(fitted_models)
+                regression_results.update(reg_results)
+           
             sc=ax.scatter(_df[x], _df[y], c=_df[_c], 
                           cmap=palette_val,
                           s=_size,
                           alpha=alpha,
                           edgecolors=edgecolors,
                           linewidths=linewidths)
             if kde==True:
-                sns.kdeplot(data=df, x=x, y=y, ax=ax, color=color, **kde_kw)
-            # cax = plt.axes([0.86, 0.1, 0.075, 0.5])
-            # plt.colorbar(cax=cax)
+                sns.kdeplot(data=df, x=x, y=y, ax=ax, color=color, legend=False, **kde_kw)
+                ax.set(xlabel=None)
+                ax.set(ylabel=None)
+
             if marginal_dist==True:
                 _marginal_plot(fig, ax,df, x,y, "", lut,_xrange,_yrange , marginal_proportion)
 
-
             bb=ax.get_position()
             axx , axy, axw, axh=bb.bounds
             _xcax=axx+axw*1.005
             if marginal_dist==True:
                 _xcax=axx+axw*1.005/marginal_proportion
             cax = plt.axes([_xcax, axy, 0.02, 0.1])
             if _unit!="":
@@ -544,90 +619,117 @@
             if cbar_format!="":
                 ax.xaxis.set_major_formatter(StrMethodFormatter(cbar_format))
 
             #ax.set_title(_c)
             if _axlabeleach==True:
                 ax.set_xlabel(x)
                 ax.set_ylabel(y)
+
             _set_axis_format(ax, xformat, yformat, xunit, yunit, logscalex,logscaley)
 
             if sizes !="" and show_legend==True:
-
                 if size_unit!="":
                     sizes=sizes+"("+size_unit+")"
                 ax.add_artist(ax.legend(handles=size_legend_elements, title=sizes,bbox_to_anchor=(legendx,1)))
+
             if len(show_labels)!=0:
                 _add_labels(ax, df, x, y, show_labels["val"], show_labels["topn"])
 
 
     if int(len(c.shape)>1):
         ax=axes[i]
         i+=1
         if type(color_unit)==str:
             color_unit=[color_unit]
         _unit=color_unit[-1]
         ax.margins(margins)
         ax.set_zorder(1)
+
+        if regression==True:
+            fitted_models, reg_results=_regression(df, x, y, ax, robust_param=robust_param, newkey="total", color=regression_color)
+            regression_models.update(fitted_models)
+            regression_results.update(reg_results)
+
         sc=ax.scatter(df[x], df[y], c=c, 
                         s=size,
                         edgecolors=edgecolors,
                         linewidths=linewidths)
-        if kde==True:
-            sns.kdeplot(data=df, x=x, y=y, ax=ax, color=color, **kde_kw)
         ax.text(0.1,0.8, cname, bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="gray", lw=1, alpha=0.8))
+
+
+        if kde==True:
+            sns.kdeplot(data=df, x=x, y=y, ax=ax, color=color, legend=False, **kde_kw)
+            ax.set(xlabel=None)
+            ax.set(ylabel=None)
+
         if marginal_dist==True:
             _marginal_plot(fig, ax,df, x,y, "", lut,_xrange,_yrange , marginal_proportion)
         
         if _axlabeleach==True:
             ax.set_xlabel(x)
             ax.set_ylabel(y)
+
         _set_axis_format(ax, xformat, yformat, xunit, yunit, logscalex,logscaley)
 
         if sizes !="" and show_legend==True:
             if size_unit!="":
                 sizes=sizes+"("+size_unit+")"
             ax.add_artist(ax.legend(handles=size_legend_elements, title=sizes,bbox_to_anchor=(legendx,1)))
+
         if len(show_labels)!=0:
             _add_labels(ax, df, x, y, show_labels["val"], show_labels["topn"])
 
     
     if len(category)+len(colors)==0 and int(len(c.shape)!=2):
+
         ax=axes[i]
+        if regression==True:
+            fitted_models, reg_results=_regression(df, x, y, ax, robust_param=robust_param, newkey="total", color=regression_color)
+            regression_models.update(fitted_models)
+            regression_results.update(reg_results)
+
         sc=ax.scatter(df[x], df[y], c=color,s=size,alpha=alpha,edgecolors=edgecolors,linewidths=linewidths)
         if kde==True:
             sns.kdeplot(data=df, x=x, y=y, ax=ax, color=color, **kde_kw)
-        if axlabel=="each":
-            ax.set_xlabel(x)
-            ax.set_ylabel(y)
+            ax.set(xlabel=None)
+            ax.set(ylabel=None)
+
+        ax.set_xlabel(x)
+        ax.set_ylabel(y)
         
         _set_axis_format(ax, xformat, yformat, xunit, yunit, logscalex,logscaley)
+
         if sizes !="" and show_legend==True:
             if size_unit!="":
                 sizes=sizes+"("+size_unit+")"
             ax.add_artist(ax.legend(handles=size_legend_elements, 
                                     title=sizes,
                                     bbox_to_anchor=(1.01,1)))
             
     if title!="":
         if fig !=None:
             fig.suptitle(title)
         else:
             plt.title(title)
+
     if axlabel=="single" and fig !=None:
         bbox=axes[0].get_position()
-        fig.text(0.5, 0.01, x, ha='center')
-        fig.text(bbox.bounds[0]*0.5, 0.5, y, va='center', rotation='vertical')
+        fig.text(0.5, 0.05, x, ha='center',fontsize="large")
+        fig.text(bbox.bounds[0]*0.5, 0.5, y, va='center', rotation='vertical',fontsize="large")
+
     if len(axes) != totalnum:
         for i in range(len(axes)-totalnum):
             axes[-(i+1)].set_axis_off()
     
     _save(save, "scatter")
     #  plt.tight_layout()
 
-    return {"axes":axes, "fig":fig}
+    return {"axes":axes, "fig":fig, 
+            "regression_models":regression_models, "regression_results":regression_results, 
+            "kmeans_result":_kmeans, "df":df}
 
 def clusterplot(df: pd.DataFrame,
                 variables: List=[],
                 category: Union[List[str], str]="", 
                 method: str="kmeans",
                 n_clusters: Union[str , int]=3,
                 x: str="",
@@ -2841,56 +2943,38 @@
     
     Y=df[y]
     _X=np.array(df[x]).reshape([-1,1])
     X=np.array(df[x])
     plotline_X = np.arange(X.min(), X.max()).reshape(-1, 1)
     n = X.shape[0]
     plt.rcParams.update({'font.size': 14})
-    fig, ax = plt.subplots(figsize=figsize)
-    fig.suptitle(title)
+    if ax==None:
+        fig, ax = plt.subplots(figsize=figsize)
+        fig.suptitle(title)
+    else:
+        fig=None
+        # plt.title(title)
     plt.subplots_adjust(left=0.15)
     if method=="ransac":
         _title="RANSAC regression, r2: {:.2f}, MSE: {:.2f}\ny = {:.2f} + {:.2f}x, coefficient p-value: {:.2E}"
-        from sklearn.linear_model import RANSACRegressor
-        fit_df=pd.DataFrame()
-        fitted_model = RANSACRegressor(random_state=random_state,**ransac_param).fit(_X,Y)
-        fit_df["ransac_regression"] = fitted_model.predict(plotline_X)
-        coef = fitted_model.estimator_.coef_[0]
-        intercept=fitted_model.estimator_.intercept_
-        inlier_mask = fitted_model.inlier_mask_
-        outlier_mask = ~inlier_mask
-        
-                                # number of samples
-        y_model=fitted_model.predict(_X)
-
-        r2 = _calc_r2(X,Y)
-        # mean squared error
-        MSE = 1/n * np.sum( (Y - y_model)**2 )
-        
-        # to plot the adjusted model
-        x_line = plotline_X.flatten()
-        y_line = fit_df["ransac_regression"]
-         
-        ci, pi, std_error=_ci_pi(X,Y,plotline_X.flatten(),y_model)
-        q=((X-X.mean()).transpose() @ (X-X.mean()))
-        sigma=std_error*(q**-1)**(0.5)
-        coef_p=stats.t.sf(abs(fitted_model.estimator_.coef_[0]/sigma), df=X.shape[0]-2)
+        fitted_model, coef, coef_p, intercept, r2, x_line, y_line, ci, pi,std_error, MSE, inlier_mask, outlier_mask=_ransac(X,Y,plotline_X,random_state, ransac_param)
+        
         ############### Ploting
 
         _draw_ci_pi(ax, ci, pi,x_line, y_line)
         sns.scatterplot(x=X[inlier_mask], y=Y[inlier_mask], color="blue", label="Inliers")
         sns.scatterplot(x=X[outlier_mask], y=Y[outlier_mask], color="red", label="Outliers")
         plt.xlabel(x)
         plt.ylabel(y)
         #print(r2, MSE,ransac_coef,ransac.estimator_.intercept_)
         plt.title(_title.format(
             r2, MSE,coef,intercept,coef_p
             )
         )
-        plt.plot(plotline_X.flatten(),fit_df["ransac_regression"])
+        plt.plot(plotline_X.flatten(),y_line)
         
         _save(save, method)
         if len(category)!=0:
             fig, ax1=plt.subplots(figsize=figsize)
             plt.subplots_adjust(left=0.15)
             _draw_ci_pi(ax1, ci, pi,x_line, y_line)
             sns.scatterplot(data=df,x=x, y=y, hue=category, ax=ax1)
@@ -2898,35 +2982,20 @@
             plt.xlabel(x)
             plt.ylabel(y)
             #print(r2, MSE,ransac_coef,ransac.estimator_.intercept_)
             plt.title(_title.format(
                 r2, MSE,coef,intercept,coef_p
                 )
             )
-            plt.plot(plotline_X.flatten(),fit_df["ransac_regression"])
+            plt.plot(plotline_X.flatten(),y_line)
             _save(save, method+"_"+category)
     elif method=="robust":
         _title="Robust linear regression, r2: {:.2f}, MSE: {:.2f}\ny = {:.2f} + {:.2f}x , p-values: coefficient {:.2f}, \
         intercept {:.2f}"
-        import statsmodels.api as sm
-        rlm_model = sm.RLM(Y, sm.add_constant(X),
-        M=sm.robust.norms.HuberT(),**robust_param)
-        fitted_model = rlm_model.fit()
-        summary=fitted_model.summary()
-        coef=fitted_model.params[1]
-        intercept=fitted_model.params[0]
-        intercept_p=fitted_model.pvalues[0]
-        coef_p=fitted_model.pvalues[1]
-        y_model=fitted_model.predict(sm.add_constant(X))
-        r2 = _calc_r2(X,Y)
-        x_line = plotline_X.flatten()
-        y_line = fitted_model.predict(sm.add_constant(x_line))
-        
-        ci, pi,std_error=_ci_pi(X,Y,plotline_X.flatten(),y_model)
-        MSE = 1/n * np.sum( (Y - y_model)**2 )
+        fitted_model, summary, coef, coef_p, intercept, intercept_p, r2, x_line, y_line, ci, pi,std_error, MSE=_robust_regression(X, Y, plotline_X, robust_param)
 
         _draw_ci_pi(ax, ci, pi,x_line, y_line)
         sns.scatterplot(data=df,x=x, y=y, color="blue")
         #print(r2, MSE,ransac_coef,ransac.estimator_.intercept_)
         plt.title(_title.format(
             r2, MSE,coef,intercept,coef_p,intercept_p
             )
@@ -2943,34 +3012,17 @@
                 r2, MSE,coef,intercept,coef_p,intercept_p
                 )
             )
             plt.plot(plotline_X.flatten(),y_line)
             _save(save, method+"_"+category)
     elif method=="lasso" or method=="elastic_net" or method=="ols":
         _title="OLS ({}), r2: {:.2f}, MSE: {:.2f}\ny = {:.2f} + {:.2f}x, coefficient p-value: {:.2E}"
-        if method=="lasso":
-            method="sqrt_lasso"
-        import statsmodels.api as sm
-        rlm_model = sm.OLS(Y, sm.add_constant(X))
-        if method=="ols":
-            fitted_model = rlm_model.fit()
-        else:
-            fitted_model = rlm_model.fit_regularized(method)
-        coef=fitted_model.params[1]
-        intercept=fitted_model.params[0]
-        y_model=fitted_model.predict(sm.add_constant(X))
-        r2 = _calc_r2(X,Y)
-        x_line = plotline_X.flatten()
-        y_line = fitted_model.predict(sm.add_constant(x_line))
-        ci, pi, std_error=_ci_pi(X,Y,plotline_X.flatten(),y_model)
-        q=((X-X.mean()).transpose() @ (X-X.mean()))
-        sigma=std_error*(q**-1)**(0.5)
-        print(sigma,coef )
-        coef_p=stats.t.sf(abs(coef/sigma), df=X.shape[0]-2)
-        MSE = 1/n * np.sum( (Y - y_model)**2 )
+
+        fitted_model, coef, coef_p, intercept, r2, x_line, y_line, ci, pi,std_error, MSE=_ols(X, Y, plotline_X, method)
+
 
         _draw_ci_pi(ax, ci, pi,x_line, y_line)   
         sns.scatterplot(data=df,x=x, y=y, color="blue")
         #print(r2, MSE,ransac_coef,ransac.estimator_.intercept_)
         plt.title(_title.format(method,
             r2, MSE,coef,intercept,coef_p
             )
@@ -2992,8 +3044,332 @@
     if yunit!="":
         ax.text(0, 1, "({})".format(yunit), transform=ax.transAxes, ha="right")
         ax1.text(0, 1, "({})".format(yunit), transform=ax.transAxes, ha="right")
     if xunit!="":
         ax.text(1, 0, "({})".format(xunit), transform=ax.transAxes, ha="left",va="top")
         ax1.text(1, 0, "({})".format(xunit), transform=ax.transAxes, ha="left",va="top")
     
-    return {"axes":ax, "coefficient":coef,"intercept":intercept,"coefficient_pval":coef_p, "r2":r2, "fitted_model":fitted_model}
+    return {"axes":ax, "coefficient":coef,"intercept":intercept,"coefficient_pval":coef_p, "r2":r2, "fitted_model":fitted_model}
+
+
+def _robust_regression(X, Y, plotline_X, robust_param):
+    n = X.shape[0]
+    rlm_model = sm.RLM(Y, sm.add_constant(X),
+    M=sm.robust.norms.HuberT(),**robust_param)
+    fitted_model = rlm_model.fit()
+    summary=fitted_model.summary()
+    coef=fitted_model.params[1]
+    intercept=fitted_model.params[0]
+    intercept_p=fitted_model.pvalues[0]
+    coef_p=fitted_model.pvalues[1]
+    y_model=fitted_model.predict(sm.add_constant(X))
+    r2 = _calc_r2(X,Y)
+    x_line = plotline_X.flatten()
+    y_line = fitted_model.predict(sm.add_constant(x_line))
+    
+    ci, pi,std_error=_ci_pi(X,Y,plotline_X.flatten(),y_model)
+    MSE = 1/n * np.sum( (Y - y_model)**2 )
+    return fitted_model, summary, coef, coef_p, intercept, intercept_p, r2, x_line, y_line, ci, pi,std_error, MSE
+
+def _ols(X, Y, plotline_X, method):
+    n = X.shape[0]
+    if method=="lasso":
+        method="sqrt_lasso"
+    rlm_model = sm.OLS(Y, sm.add_constant(X))
+    if method=="ols":
+        fitted_model = rlm_model.fit()
+    else:
+        fitted_model = rlm_model.fit_regularized(method)
+    coef=fitted_model.params[1]
+    intercept=fitted_model.params[0]
+    y_model=fitted_model.predict(sm.add_constant(X))
+    r2 = _calc_r2(X,Y)
+    x_line = plotline_X.flatten()
+    y_line = fitted_model.predict(sm.add_constant(x_line))
+    ci, pi, std_error=_ci_pi(X,Y,plotline_X.flatten(),y_model)
+    q=((X-X.mean()).transpose() @ (X-X.mean()))
+    sigma=std_error*(q**-1)**(0.5)
+    # print(sigma,coef )
+    coef_p=stats.t.sf(abs(coef/sigma), df=X.shape[0]-2)
+    MSE = 1/n * np.sum( (Y - y_model)**2 )
+    return fitted_model, coef, coef_p, intercept, r2, x_line, y_line, ci, pi,std_error, MSE
+
+def _ransac(X,Y,plotline_X,random_state, ransac_param):
+    n = X.shape[0]
+    _X=np.array(X).reshape([-1,1])
+    fitted_model = RANSACRegressor(random_state=random_state,**ransac_param).fit(_X,Y)
+    y_line= fitted_model.predict(plotline_X)
+    coef = fitted_model.estimator_.coef_[0]
+    intercept=fitted_model.estimator_.intercept_
+    inlier_mask = fitted_model.inlier_mask_
+    outlier_mask = ~inlier_mask
+    
+                            # number of samples
+    y_model=fitted_model.predict(_X)
+
+    r2 = _calc_r2(X,Y)
+    # mean squared error
+    MSE = 1/n * np.sum( (Y - y_model)**2 )
+    
+    # to plot the adjusted model
+    x_line = plotline_X.flatten()
+        
+    ci, pi, std_error=_ci_pi(X,Y,plotline_X.flatten(),y_model)
+    q=((X-X.mean()).transpose() @ (X-X.mean()))
+    sigma=std_error*(q**-1)**(0.5)
+    coef_p=stats.t.sf(abs(fitted_model.estimator_.coef_[0]/sigma), df=X.shape[0]-2)
+
+    return fitted_model, coef, coef_p, intercept, r2, x_line, y_line, ci, pi,std_error, MSE, inlier_mask, outlier_mask
+
+
+def _regression(df, x, y, ax, cat="", _clut={}, robust_param={}, newkey="", color=""):
+    reg_legend_elements=[]
+    fitted_models={}
+    reg_res={}
+    if cat !="":
+        
+        for key in _clut.keys():
+            key_filt=df[cat]==key
+            rdf=df.loc[key_filt]
+            rX, rY=rdf[x], rdf[y]
+            plotline_X = np.arange(rX.min(), rX.max()).reshape(-1, 1)
+            fitted_model, summary, coef, coef_p, intercept, intercept_p, r2, x_line, y_line, ci, pi,std_error, MSE=_robust_regression(rX, rY, plotline_X, robust_param)
+            _tmpcolor=np.array(_clut[key])
+            _draw_ci_pi(ax, ci, pi,x_line, y_line, pi_color=_tmpcolor, ci_color=_tmpcolor+(1-_tmpcolor)*0.5, alpha=0.75)
+            ax.plot(x_line, y_line, c=_tmpcolor)   
+            reg_legend_elements.append(Line2D([0], [0], marker="", linewidth=3,color=_tmpcolor,
+                                label="\u03B21: {x:.2f}\np: {p:.1E}\nr2: {y:.2f}".format(x=coef,y=r2, p=coef_p),
+                                ))
+            fitted_models[cat+"_"+key]=fitted_model
+            reg_res[cat+"_"+key]={"coefficient":coef,
+                                  "coefficient_pvalue":coef_p,
+                                  "intercept":intercept,
+                                  "intercept_pvalue":intercept_p,
+                                  "r2": r2,
+                                  "mse":MSE}
+    else:
+
+        rX, rY=df[x], df[y]
+        plotline_X = np.arange(rX.min(), rX.max()).reshape(-1, 1)
+        (fitted_model, summary, coef, coef_p, 
+         intercept, intercept_p, r2, 
+         x_line, y_line, ci, pi,std_error, MSE)=_robust_regression(rX, rY, plotline_X, robust_param)
+        if color !="":
+            _tmpcolor=np.array(colors.to_rgb(color))
+        else:
+            _tmpcolor=np.array([0,0.75,0])
+        _draw_ci_pi(ax, ci, pi,x_line, y_line, pi_color=_tmpcolor, ci_color=_tmpcolor+(1-_tmpcolor)*0.5, alpha=0.75)
+        ax.plot(x_line, y_line, c=_tmpcolor)   
+        reg_legend_elements.append(Line2D([0], [0], marker="", linewidth=3,color=_tmpcolor,
+                            label="\u03B21: {x:.2f}\np: {p:.1E}\nr2: {y:.2f}".format(x=coef,y=r2, p=coef_p),
+                            ))
+        if newkey=="":
+            newkey="regression"
+        fitted_models[newkey]=fitted_model
+        reg_res[newkey]={"coefficient":coef,
+                                "coefficient_pvalue":coef_p,
+                                "intercept":intercept,
+                                "intercept_pvalue":intercept_p,
+                                "r2": r2,
+                                "mse":MSE}
+    ax.add_artist(ax.legend(handles=reg_legend_elements, 
+                            title="Regression",
+                            loc="upper left", bbox_to_anchor=(0.0, -0.1), ncol=3))
+    return fitted_models,reg_res
+
+def volcanoplot(df: pd.DataFrame,
+                x: str,
+                y: str,
+                label: str="",
+                logscalex: bool=False,
+                logscaley: bool=True,
+                sizes: str="",
+                xthreshold: float=1,
+                ythreshold: float=0.05,
+                
+                topn_labels: int=5,
+                rankby: str="both",
+                topn_labels_left: int=0,
+                topn_labels_right: int=0,
+
+                base_color: str="gray",
+                highlight_color: str="red",
+                
+                save: str="",
+                write_csv: Union[bool, str]=False,
+
+                ax: Optional[plt.Axes]= None,
+                fig : Optional[mpl.figure.Figure] =None,
+                
+                markers: bool=False,
+                size: float=5.0,
+                size_scale: float=100,
+                plotline: bool=True,
+                linestyle="-",
+                linecolor="darkcyan",
+                alpha: float=1,
+                edgecolors: str="w",
+                size_format: str="",
+                xformat: str="",
+                yformat: str="",
+                xunit: str="",
+                yunit:str="",
+                size_unit: str="",
+                title: str="",
+                figsize: list=[],
+                
+                gridspec_kw: dict={},):
+    
+    if topn_labels_left==0 and topn_labels_right==0:
+        topn_labels_left=topn_labels
+        topn_labels_right=topn_labels
+
+    df=copy.deepcopy(df)
+    if len(figsize)==0:
+        figsize=[5,5]
+    if ax==None:
+        
+
+        fig, ax=plt.subplots(figsize=figsize)
+    
+    if np.amax(df[y]) <=1:
+
+        if logscaley!=False:
+            print("Transforming {} to -log10 values. if you do not want it, set 'logscaley=False'.".format(y))
+            df[y]=-np.log10(df[y])
+    elif logscaley==True:
+        df[y]=-np.log10(df[y])
+    if logscalex==True:
+        df[x]=np.log2(df[x])
+    if ythreshold <1:
+        ythreshold=-np.log10(ythreshold)
+    updown=[]
+    for _x, _y in zip(list(df[x]), list(df[y])):
+        if (_y <=ythreshold) or (np.abs(_x)<xthreshold):
+            updown.append("ns")
+        elif _y>ythreshold and _x>=xthreshold:
+            updown.append("up")
+        elif _y>ythreshold and _x<=-xthreshold:
+            updown.append("down")
+    df["updown"]=updown
+    
+    sig=df.loc[df["updown"]=="up"]
+    sig=sig.reset_index()
+    sigm=df.loc[df["updown"]=="down"]
+    sigm=sigm.reset_index()
+    palette={"ns": colors.to_rgb(base_color),
+             "up": colors.to_rgb(highlight_color),
+             "down": colors.to_rgb(highlight_color)}
+    
+    if sizes!="":
+        
+        scatterplot(df=df, x=x, y=y, category="updown", ax=ax,sizes=sizes, color=base_color, alpha=alpha, edgecolors=None, show_legend=False)
+        #ax.scatter(nonsig[x], nonsig[y], c=base_color, s=nonsig[sizes], alpha=alpha,)
+        # scatterplot(df=sig, x=x, y=y, ax=ax,sizes=sizes, color=highlight_color, alpha=alpha, edgecolors=None, show_legend=False)
+        # scatterplot(df=sigm, x=x, y=y, ax=ax,sizes=sizes, color=highlight_color, alpha=alpha, edgecolors=None, show_legend=False, xunit=xunit, yunit=yunit, title=title)
+        # # ax.scatter(sig[x], sig[y], c=highlight_color, s=sig[sizes])
+        # ax.scatter(sigm[x], sigm[y], c=highlight_color, s=sigm[sizes])
+    else:
+        scatterplot(df=df, x=x, y=y, category="updown",palette=palette, ax=ax,size=size, color=base_color, alpha=alpha, edgecolors=None, show_legend=False)
+        # scatterplot(df=nonsig, x=x, y=y, ax=ax,size=size, color=base_color, alpha=alpha, edgecolors=None, show_legend=False)
+        # scatterplot(df=sig, x=x, y=y, ax=ax,size=size, color=highlight_color, alpha=alpha, edgecolors=None, show_legend=False)
+        # scatterplot(df=sigm, x=x, y=y, ax=ax,size=size, color=highlight_color, alpha=alpha, edgecolors=None, show_legend=False, xunit=xunit, yunit=yunit, title=title)
+        # ax.scatter(nonsig[x], nonsig[y], c=base_color, s=size)
+        # ax.scatter(sig[x], sig[y], c=highlight_color, s=size)
+        # ax.scatter(sigm[x], sigm[y], c=highlight_color, s=size)
+    
+    # ax.set_xlabel(x)
+    # ax.set_xlabel(y)
+
+    xsrt=np.argsort(sig[x])[::-1]
+    xrank=np.argsort(xsrt)
+    xsrtm=np.argsort(np.abs(sigm[x]))[::-1]
+    xrankm=np.argsort(xsrtm)
+
+    ysrt=np.argsort(sig[y])[::-1]
+    yrank=np.argsort(ysrt)
+    ysrtm=np.argsort(sigm[y])[::-1]
+    yrankm=np.argsort(ysrtm)
+    if rankby=="both":
+        rank=(xrank+yrank)/2
+        rankm=(xrankm+yrankm)/2
+    elif rankby=="x" or rankby==x:
+        rank=xrank
+        rankm=xrankm
+    elif rankby=="y" or rankby==y:
+        rank=yrank
+        rankm=yrankm
+    labeled_genes=[]
+    texts=[]
+    for _rank, _sig, _topn_labels in zip([rank, rankm], [sig, sigm], [topn_labels_right, topn_labels_left]):
+        if len(_rank)!=0:
+            top_index=np.argsort(_rank)[:_topn_labels]
+            topsig=_sig.iloc[top_index]
+            if label=="":
+                labels=topsig.index
+            else:
+                labels=topsig[label]
+            
+            for _x, _y, _l in zip(topsig[x],topsig[y], labels):
+                #ax.text(_x, _y, _l)
+                texts.append( ax.text(_x, _y, _l, va="bottom"))
+
+            labeled_genes.append(topsig)
+    adjust_text(texts,
+            arrowprops=dict(arrowstyle="-", color='black', lw=0.5),force_text=(0.2,0.4))
+    ymin, ymax=np.amin(df[y]),np.amax(df[y])
+    xmin, xmax=np.amin(df[x]),np.amax(df[x])
+
+    if plotline==True:
+        ax.plot([xthreshold,xthreshold], [ythreshold, ymax],linestyle, color=linecolor, alpha=0.5)
+        ax.plot([-xthreshold,-xthreshold], [ythreshold, ymax],linestyle, color=linecolor, alpha=0.5)
+        ax.plot([xthreshold, xmax], [ythreshold, ythreshold],linestyle, color=linecolor, alpha=0.5)
+        ax.plot([xmin, -xthreshold], [ythreshold, ythreshold],linestyle, color=linecolor, alpha=0.5)
+        # ax.plot([xmin, xmax], [ythreshold, ythreshold],linestyle)
+    _save(save, "volcano")
+    res={"upgenes":sig, "downgenes":sigm,"labeledgenes":pd.concat(labeled_genes)}
+    if type(write_csv)==bool and write_csv==True:
+        for k, v in res.items():
+            v.to_csv(k+".csv")
+    elif type(write_csv)==str and write_csv!="":
+        for k, v in res.items():
+            v.to_csv(write_csv+"_"+k+".csv")
+    return  res
+    
+def manhattanplot(df: pd.DataFrame,
+                  x: str="BP",
+                  p: str="P",
+                  chrom: str="CHR",
+                  snp: str="SNP",
+                  zscore: str="",
+                  effectsize: str="",
+                  gene: str="",
+                  distance: str="",
+                  logtransform: bool=True,
+                  threshold: float=4,
+                  thresholdcolor: str="red"
+                  ):
+    df=df.reset_index()
+    gb = df.groupby(chrom)
+    if logtransform==True:
+
+        df[p]=-np.log10(df[p])
+    if threshold <1:
+        threshold=-np.log10(threshold)
+    colors=["gray", "black"]
+
+    fig, ax=plt.subplots()
+
+    for i, x in enumerate(gb.groups):
+
+        _df=gb.get_group(x)
+        ax.scatter(_df.index, _df[p], c=colors[i%2], s=5)
+        ax.text((np.max(_df.index)+np.min(_df.index))/2, -0.5, x)
+    _df=df.loc[df[p]>threshold]
+    ax.scatter(_df.index, _df[p], c=thresholdcolor, s=4)
+    maxindex=np.argmax(df[p])
+    ax.text(df.index[maxindex],df[p][maxindex], df[snp][maxindex]) #+"\n"+str(df[chrom][maxindex])+":"+str(df[x][maxindex]))
+    ax.spines['top'].set_visible(False)
+    ax.spines['right'].set_visible(False)
+    ax.spines['bottom'].set_visible(False)
+    #ax.spines['left'].set_visible(False)
+    ax.set_xticks([])
```

### Comparing `omniplot-0.2.6/omniplot/scripts/gff2tss.py` & `omniplot-0.3.0/omniplot/scripts/gff2tss.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/statistics.py` & `omniplot-0.3.0/omniplot/statistics.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/omniplot/utils.py` & `omniplot-0.3.0/omniplot/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 colormap_list=["nipy_spectral", "terrain","tab20b","gist_rainbow","tab20c","CMRmap","coolwarm","gnuplot","gist_stern","brg","rainbow"]
 plt.rcParams['font.family']= 'sans-serif'
 plt.rcParams['font.sans-serif'] = ['Arial']
 plt.rcParams['svg.fonttype'] = 'none'
 sns.set_theme()
 from matplotlib.text import Annotation
 from matplotlib.transforms import Affine2D
-import os 
+import os
+import copy
 
 __all__=["_create_color_markerlut", 
          "_separate_data", "_line_annotate", "_dendrogram_threshold", "_radialtree2",
          "_get_cluster_classes","_calc_curveture", "_draw_ci_pi","_calc_r2",
          "_ci_pi", "_save","_baumkuchen", "_baumkuchen_xy", "_get_embedding"]
 
 
@@ -845,28 +846,28 @@
     # predicting interval
     pi = t * std_error * (1 + 1/n + (x_line - x_mean)**2 / np.sum((X - x_mean)**2))**.5
     return ci, pi,std_error
 def _draw_ci_pi(ax: plt.Axes, 
                ci: np.ndarray, 
                pi: np.ndarray,
                x_line: np.ndarray, 
-               y_line: np.ndarray):
+               y_line: np.ndarray, pi_color: str='lightcyan',ci_color: str='skyblue', alpha: float=0.5):
     """
     Drawing a confidence interval and a prediction interval 
     """
-    
+    ax.fill_between(x_line, y_line + ci, 
+                    y_line - ci, color = ci_color, 
+                    label = '95% confidence interval',
+                    alpha=alpha)
     
     ax.fill_between(x_line, y_line + pi, y_line - pi, 
-                color = 'lightcyan', 
+                color = pi_color, 
                 label = '95% prediction interval',
-                alpha=0.5)
-    ax.fill_between(x_line, y_line + ci, 
-                    y_line - ci, color = 'skyblue', 
-                    label = '95% confidence interval',
-                    alpha=0.5)
+                alpha=alpha*0.5)
+    
     
 from sklearn.cluster import KMeans
 def _optimal_kmeans(X: Union[np.ndarray, list], testrange: list, topn: int=2)-> List[int]:
     Sum_of_squared_distances = []
     K = list(range(*testrange))
     for k in K:
         km = KMeans(n_clusters=k,n_init=10)
@@ -1030,24 +1031,31 @@
         if x.dtype!=float: 
             raise TypeError(f"data must contain only float values. \
         or you can specify the numeric variables with the option 'variables'.")
         
     return x, category
 
 def _create_color_markerlut(df, cat, palette, markers=[]):
+    # print(type(palette))
     color_lut={}
     marker_lut={}
     if df[cat].isnull().values.any():
         df[cat]=df[cat].fillna("NA")
     uniq_labels=sorted(list(set(df[cat])))
-    _cmap=plt.get_cmap(palette, len(uniq_labels))
-    
-    color_lut={u: _cmap(i) for i, u in enumerate(uniq_labels)}
-    
-    if len(markers)!=0:
-        if len(markers) < len(uniq_labels):
-            while len(markers) < len(uniq_labels):
-                markers.extend(markers)
-        marker_lut={u: markers[i] for i, u in enumerate(uniq_labels)}
+    if type(palette)==str:
+        _cmap=plt.get_cmap(palette, len(uniq_labels))
+        
+        color_lut={u: _cmap(i) for i, u in enumerate(uniq_labels)}
+        
+        if len(markers)!=0:
+            if len(markers) < len(uniq_labels):
+                while len(markers) < len(uniq_labels):
+                    markers.extend(markers)
+            marker_lut={u: markers[i] for i, u in enumerate(uniq_labels)}
+    elif type(palette)==dict:
+        color_lut=copy.deepcopy(palette)
+    else:
+        raise TypeError("Unexpected type of the palette option. It must be either a matplot colormap name or the dictionary of a color look up table")
+
 
     return color_lut, marker_lut
```

### Comparing `omniplot-0.2.6/omniplot.egg-info/PKG-INFO` & `omniplot-0.3.0/omniplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.2.6
+Version: 0.3.0
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.2.6/omniplot.egg-info/SOURCES.txt` & `omniplot-0.3.0/omniplot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 omniplot/__init__.py
+omniplot/_adjustText.py
 omniplot/_version.py
 omniplot/chipseq.py
 omniplot/chipseq_utils.py
 omniplot/data.py
 omniplot/igraph_classes.py
 omniplot/networkplot.py
 omniplot/plot.py
```

### Comparing `omniplot-0.2.6/setup.py` & `omniplot-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,11 +77,11 @@
                       "umap-learn",
                       "tensorflow",
                       "fastcluster","cvxopt",
                       "statsmodels",
                       "natsort",
                       "joblib","pyranges",
                       "ray",
-                      "intervaltree","networkx","datashader","python-louvain", "scikit-fuzzy","scikit-image",
+                      "intervaltree","networkx","datashader","python-louvain", "scikit-fuzzy","scikit-image","adjustText","bioframe"
                       ],
     long_description=long_description,
 )
```

### Comparing `omniplot-0.2.6/tests/test_chipseq.py` & `omniplot-0.3.0/tests/test_chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.2.6/tests/test_network.py` & `omniplot-0.3.0/tests/test_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from scipy.stats import zscore
 from joblib import Parallel, delayed
 from scipy.spatial.distance import pdist, squareform
 import itertools as it
 from datashader.bundling import hammer_bundle
 test="pienode"
 test="correlation"
-test="correlation"
+test="sankey_category"
 if test=="correlation":
     df=sns.load_dataset("penguins")
     df=df.dropna(axis=0)
     df=df.reset_index()
     onp.correlation(df, category=["species", "island","sex"], 
                 method="pearson", 
                 ztransform=True,
```

### Comparing `omniplot-0.2.6/tests/tests.py` & `omniplot-0.3.0/tests/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 test="decomp"
 test="manifold"
 test="triangle_heatmap"
 test="radialtree"
 test="violinplot"
 test="cluster"
 test="regression"
-test="complex_clustermap"
+
 test="dotplot"
 test="regression"
 test="nice_piechart_num"
 test="pie_scatter"
 test="correlation"
 test="manifold"
 test="stacked"
 test="stackedlines"
 test="correlation"
 test="cluster"
 test="nested_piechart"
 test="radialtree"
 test="scatterplot"
-
-
+test="stacked_num"
+test="complex_clustermap"
+test="volcanoplot"
 if test=="stackedlines":
     f="/media/koh/grasnas/home/data/omniplot/energy/owid-energy-data.csv"
     df=pd.read_csv(f)
     _df=df.loc[df["country"]=="Japan"]
     cols=['biofuel_consumption',
             'coal_consumption',
             'gas_consumption',
@@ -108,15 +109,40 @@
     # op.stacked_barplot(df, x="species",
     #                     hue="sex", scale="percentage", hatch=True)
 
     df=sns.load_dataset("titanic")
     op.stacked_barplot(df=df,x=["sex"],hue=["age","alone"], bin_num=10)
 
     plt.show()
-
+elif test=="stacked_num": 
+    """          　Bournemouth    Brighton
+        Possession         36          64
+        Shots              14          16
+        Shots on Target     3           6
+        Corners             5           5
+        Fouls              11           5
+    """
+    df=pd.DataFrame({"Bournemouth":[36,14,3,5,11],"Brighton":[64,16,6,5,5]}, index=["Possession","Shots","Shots on Target","Corners","Fouls"])
+    op.stacked_barplot_num(df=df,show_values_intact=True, 
+                           unit={"Possession":"%"}, 
+                           horizontal=True)
+    df=pd.read_csv("/media/koh/grasnas/home/data/omniplot/energy/owid-energy-data_curated_with_continents.csv")
+    df=df.loc[df["year"]==2021]
+    cols=["country","coal_consumption","gas_consumption","hydro_consumption","oil_consumption",
+          "nuclear_consumption","biofuel_consumption","solar_consumption","wind_consumption"]
+    df=df[cols]
+    df=df.reindex()
+    
+    srt=np.argsort(np.array(df.sum(axis=1)))[::-1]
+    df=df.iloc[srt[:10]]
+    print(df)
+    op.stacked_barplot_num(df=df,x="country",show_values=False,# show_values_intact=True, 
+                           #unit={"Possession":"%"}, 
+                           horizontal=True,scale="absolute",xlabel="kwh",legend_row_num=4)
+    plt.show()
 
 elif test=="nice_piechart_num":
     f="/home/koh/ews/omniplot/data/energy_vs_gdp.csv"
     df=pd.read_csv(f, comment='#')
     df=df.set_index("country")
     op.nice_piechart_num(df, hue=['biofuel_electricity',
                                                     'coal_electricity',
@@ -137,15 +163,15 @@
         
     op.correlation(df, category=["species", "island","sex"], method="pearson", ztransform=True)
     plt.show()
 
 elif test=="regression":
     df=sns.load_dataset("penguins")
     df=df.dropna(axis=0)
-    op.regression_single(df, x="bill_length_mm",y="body_mass_g", method="robust",category="species")
+    op.regression_single(df, x="bill_length_mm",y="body_mass_g", method="ransac",category="species")
     plt.show()
 elif test=="dotplot":
     df=pd.DataFrame({"Experiments":["exp1","exp1","exp1","exp1","exp2","exp2","exp3"],
                         "GO":["nucleus","cytoplasm","chromosome","DNA binding","chromosome","RNA binding","RNA binding"],
                         "FDR":[10,1,5,3,1,2,0.5],
                         "odds":[3.3,1.1,2.5,2.1,0.8,2.3,0.9]})
     op.dotplot(df, row="GO",col="Experiments", size_val="FDR",color_val="odds", highlight="FDR",
@@ -255,21 +281,25 @@
 
 elif test=="scatterplot":
     df=sns.load_dataset("penguins")
     df=df.dropna(axis=0)
     #features=["species","sex","bill_length_mm","bill_depth_mm","flipper_length_mm","body_mass_g"]
     #df=df[features]
     print(df.shape)
-    op.scatterplot(df, x="bill_length_mm",y="bill_depth_mm",xunit="mm", yunit="mm", 
-                   category=['species',"sex","island"],
-                   colors=["flipper_length_mm"],
-                   sizes="body_mass_g",
-                   show_labels={"val": "body_mass_g", "topn":5},
-                   marginal_dist=True,
-                   kmeans=True,
-                                                )
-    fig, ax=plt.subplots()
-    op.scatterplot(df, ax=ax,
+    # op.scatterplot(df, x="bill_length_mm",y="bill_depth_mm", # xunit="mm", yunit="mm", 
+    #                category=['species',"sex","island"],
+    #                colors=["flipper_length_mm"],
+    #                sizes="body_mass_g",#size_scale=1000,
+    #                #show_labels={"val": "body_mass_g", "topn":5},
+    #                marginal_dist=True,
+    #                kmeans=True,
+    #                                             )
+    # fig, ax=plt.subplots()
+    op.scatterplot(df,
+                category=['species'],
                x="bill_length_mm",
-               y="bill_depth_mm", 
-                sizes="flipper_length_mm")
+               y="bill_depth_mm", save="/home/koh/data/omniplot/kde_kmeans")
+    plt.show()
+elif test=="volcanoplot":
+    df=pd.read_csv("/home/koh/vscode/omniplot/data/volcano.csv")
+    op.volcanoplot(df=df, x="log2FC", y="p-value", label="GeneNames", rankby="both", topn_labels_right=3)
     plt.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

