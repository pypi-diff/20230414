# Comparing `tmp/qufit-1.0.6.tar.gz` & `tmp/qufit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qufit-1.0.6.tar", last modified: Mon Dec 26 11:43:39 2022, max compression
+gzip compressed data, was "qufit-1.0.7.tar", last modified: Fri Apr 14 07:10:49 2023, max compression
```

## Comparing `qufit-1.0.6.tar` & `qufit-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-26 11:43:39.369455 qufit-1.0.6/
--rw-rw-rw-   0        0        0      820 2022-12-26 11:43:39.368456 qufit-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-26 11:43:39.340565 qufit-1.0.6/qufit/
--rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.0.6/qufit/__init__.py
--rw-rw-rw-   0        0        0    24217 2022-11-06 13:51:42.000000 qufit-1.0.6/qufit/dataTools.py
--rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.0.6/qufit/opt.py
--rw-rw-rw-   0        0        0    59840 2022-12-26 11:39:44.000000 qufit-1.0.6/qufit/optimize.py
-drwxrwxrwx   0        0        0        0 2022-12-26 11:43:39.365463 qufit-1.0.6/qufit.egg-info/
--rw-rw-rw-   0        0        0      820 2022-12-26 11:43:39.000000 qufit-1.0.6/qufit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2022-12-26 11:43:39.000000 qufit-1.0.6/qufit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-26 11:43:39.000000 qufit-1.0.6/qufit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-12-26 11:43:39.000000 qufit-1.0.6/qufit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-26 11:43:39.369455 qufit-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      707 2022-12-26 11:42:00.000000 qufit-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:10:49.946347 qufit-1.0.7/
+-rw-rw-rw-   0        0        0      820 2023-04-14 07:10:49.944353 qufit-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 07:10:49.922448 qufit-1.0.7/qufit/
+-rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.0.7/qufit/__init__.py
+-rw-rw-rw-   0        0        0    26204 2023-04-06 10:36:53.000000 qufit-1.0.7/qufit/dataTools.py
+-rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.0.7/qufit/opt.py
+-rw-rw-rw-   0        0        0    59935 2023-04-14 07:09:30.000000 qufit-1.0.7/qufit/optimize.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:10:49.942357 qufit-1.0.7/qufit.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 07:10:49.000000 qufit-1.0.7/qufit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 07:10:49.946347 qufit-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-14 07:10:03.000000 qufit-1.0.7/setup.py
```

### Comparing `qufit-1.0.6/PKG-INFO` & `qufit-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.0.6
+Version: 1.0.7
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.0.6/qufit/dataTools.py` & `qufit-1.0.7/qufit/dataTools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import sys
-import os
-sys.path.append(os.path.dirname(
-    os.path.dirname(os.path.abspath(__file__))))
-
 import numpy as np
 import scipy as sp 
-import sympy as sy
+import sympy as sy, imp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
-import qufit.optimize as op
+from home.skzhao.tools import optimize as op
+op = imp.reload(op)
 import math
 
 
 xvar = sy.Symbol('x',real=True)
 
 
 def nearest(y,target,x=None):
@@ -309,67 +305,113 @@
             ax = axes[i//2][i%2] if num>1 else axes[i]
             ax.scatter(np.real(ss),np.imag(ss),c=y,s=10)
             ax.set_title(f'|1>pop={round(percent_on*100,3)}%')
             ax.axis('equal')
         plt.savefig(r'D:\skzhao\fig\%s.png'%(name+'classify'))
         plt.close()
 
-async def find_circle(measure,s_st,target=0):
-    s_off, s_on, s_on2 = s_st[0,:,target], s_st[1,:,target], s_st[2,:,target]
-    S = list(s_off) + list(s_on)
-    x,z = np.real(S), np.imag(S)
-    d = list(zip(x,z))
-    kmeans = KMeans(n_clusters=2,max_iter=1000,tol=0.0001)
-    kmeans.fit(d)
-    c0, c1 = kmeans.cluster_centers_[0,:], kmeans.cluster_centers_[1,:]
-    center0 = np.array([np.real(np.mean(s_off)),np.imag(np.mean(s_off))]) 
-    center1 = np.array([np.real(np.mean(s_on)),np.imag(np.mean(s_on))])
-    center0, center1 = (c0,c1) if np.sum((center0-c0)**2)<np.sum((center0-c1)**2) else (c1,c0)
-    sdiff = np.complex(*(center1-center0))
-    s0 = s_off / (sdiff/np.abs(sdiff))
-    s1 = s_on / (sdiff/np.abs(sdiff))
-    s0 = np.real(s0)
-    s1 = np.real(s1)
-    bins = 120
-    mu = np.complex(*center1)/ (sdiff/np.abs(sdiff))
-    x0 = np.linspace(min(s0),max(s0),bins)
-    x1_old = np.linspace(min(s1),max(s1),bins)
-    lower, high = np.real(mu)-2*np.std(s1), np.real(mu)+2*np.std(s1)
-    x1 = x1_old[x1_old>lower]
-
-    fig, axes = plt.subplots(ncols=2,nrows=1,figsize=(9,3))
-    bin0 = axes[0].hist(s0,bins=bins)
-    bin1 = axes[0].hist(s1,bins=bins)
-    para0, func0 = op.Gaussian_Fit().fitGaussian(x0,bin0[0])
-    axes[0].plot(x0,func0(x0,para0.x))
-    b1 = bin1[0][x1_old>lower]
-    b1 = b1[x1<high]
-    x1 = x1[x1<high]
-    para1, func1 = op.Gaussian_Fit().fitGaussian(x1,b1)
-    axes[0].plot(x1,func1(x1,para1.x))
-#     axes[0].set_title(f'center={center0,center1}')
-
-    offstd, onstd = para0.x[2], para1.x[2]
-    theta = np.arange(0, 2*np.pi, 0.01)
-    roff = c0[0] + 2*offstd * np.cos(theta)
-    ioff = c0[1] + 2*offstd * np.sin(theta)
-    ron = c1[0] + 2*onstd * np.cos(theta)
-    ion = c1[1] + 2*onstd * np.sin(theta)
-    axes[1].plot(np.real(s_off),np.imag(s_off),'.')
-    axes[1].plot(np.real(s_on2),np.imag(s_on2),'.',alpha=0.4)
-    axes[1].plot(np.real(s_on),np.imag(s_on),'.')
-    axes[1].plot(*c1,'bo')
-    axes[1].plot(*c0,'ro')
-    axes[1].plot(roff,ioff)
-    axes[1].plot(ron,ion)
-    axes[1].axis('equal')
-#     axes[1].set_title(f'sigma={para0.x[2],para1.x[2]}')
-    plt.savefig(r'D:\skzhao\fig\%s.png'%(f'q{target+1}'+'postSle'))
-    measure.postSle[f'q{target+1}'] = [(center0,para0.x[2]), (center1,para1.x[2])]
-    return (center0,para0.x[2]), (center1,para1.x[2])
+def cutCircle(info_c0,info_c1,data):
+        # print(data.shape)
+        # data0, data1 = data[0,:], data[1,:]
+        c0, r0 = info_c0[0], info_c0[1]
+        c1, r1 = info_c1[0], info_c1[1]
+        s0 = (data.real-c0[0])**2+(data.imag-c0[1])**2
+        s1 = (data.real-c1[0])**2+(data.imag-c1[1])**2
+        # idx = ((np.abs(s0)<r0**2) +  (np.abs(s1)<r1**2))
+        s1_cut = (s1<r1**2)*1
+        s0_cut = (s0<r0**2)*1
+        num0 = np.count_nonzero(s0_cut)
+        num1 = np.count_nonzero(s1_cut)
+        print(num0)
+        num0 /= (num0+num1)
+        num1 /= (num0+num1)
+
+        return num0, num1
+
+def find_circle(s_st,target=0,stdnum=1,n_clusters=2):
+    from collections.abc import Iterable
+    dim = np.shape(s_st)[-1]
+    target = target if isinstance(target,Iterable) else [target]
+    fig, axes = plt.subplots(ncols=2,nrows=dim,figsize=(9,14))
+    cLst_m, num0Lst, num1Lst = [], [], []
+    cLst, pLst = [], []
+    for i,qi in enumerate(range(dim)):
+        ax0 = axes[i][0] if dim>1 else axes[0]
+        ax1 = axes[i][1] if dim>1 else axes[1]
+ 
+        x,z, predict,center,color,p=Classify_fit(s_st,qnum=i,nstate=n_clusters)
+        pLst.append(p)
+        center = np.array([center[i][0]+1j*center[i][1] for i in range(n_clusters)])
+        center0, center1 = center[:2]
+        if n_clusters < 3:
+            s_off, s_on = s_st[0,:,qi], s_st[1,:,qi]
+            sdiff = np.complex(*(center1-center0))
+            s0 = s_off / (sdiff/np.abs(sdiff))
+            s1 = s_on / (sdiff/np.abs(sdiff))
+            s0 = np.real(s0)
+            s1 = np.real(s1)
+            bins = 120
+            mu = np.complex(*center1)/ (sdiff/np.abs(sdiff))
+            x0 = np.linspace(min(s0),max(s0),bins)
+            x1_old = np.linspace(min(s1),max(s1),bins)
+            lower, high = np.real(mu)-2*np.std(s1), np.real(mu)+2*np.std(s1)
+            x1 = x1_old[x1_old>lower]
+
+            bin0 = ax1.hist(s0,bins=bins)
+            bin1 = ax1.hist(s1,bins=bins)
+            para0, func0 = op.Gaussian_Fit().fitGaussian(x0,bin0[0],fine=False)
+            ax1.plot(x0,func0(x0,para0.x))
+            b1 = bin1[0][x1_old>lower]
+            b1 = b1[x1<high]
+            x1 = x1[x1<high]
+            para1, func1 = op.Gaussian_Fit().fitGaussian(x1,b1,fine=False)
+            ax1.plot(x1,func1(x1,para1.x))
+        #     axes[0].set_title(f'center={center0,center1}')
+
+            offstd, onstd = stdnum*np.abs(para0.x[2]), stdnum*np.abs(para1.x[2])
+            theta = np.arange(0, 2*np.pi, 0.01)
+            roff = center0[0] + offstd * np.cos(theta)
+            ioff = center0[1] + offstd * np.sin(theta)
+            ron = center1[0] + onstd * np.cos(theta)
+            ion = center1[1] + onstd * np.sin(theta)
+            ax0.plot(np.real(s_off),np.imag(s_off),'.')
+            # ax0.plot(np.real(s_on2),np.imag(s_on2),'.',alpha=0.4)
+            ax0.plot(np.real(s_on),np.imag(s_on),'.')
+            ax0.plot(*center1,'bo')
+            ax0.plot(*center0,'ro')
+            ax0.plot(roff,ioff)
+            ax0.plot(ron,ion)
+            ax0.axis('equal')
+            cLst_m.append([(center0,offstd),(center1,onstd)])
+            # cLst.append([c0Lst,c1Lst])
+            num0, _ = cutCircle((center0,offstd),(center1,onstd),s_off)
+            _, num1 = cutCircle((center0,offstd),(center1,onstd),s_on)
+            num0Lst.append(num0)
+            num1Lst.append(num1)
+            plt.tight_layout()
+        else:
+            
+            cLst_m = [(center[i],stdnum*np.std(s_st[i,:,qi])) for i in range(n_clusters)]
+            num0Lst, num1Lst = p[:2]
+            for n_state in range(n_clusters):
+                s = s_st[n_state,:,qi]
+                ax0.plot(np.real(s),np.imag(s),'.')
+            color = ['ko','wo','bo']
+            for n_state in range(n_clusters):
+                s = s_st[n_state,:,qi]
+                theta = np.arange(0, 2*np.pi, 0.01)
+                roff = np.real(center[n_state]) + stdnum*np.std(s) * np.cos(theta)
+                ioff = np.imag(center[n_state]) + stdnum*np.std(s) * np.sin(theta)
+                ax0.plot(np.real(center[n_state]),np.imag(center[n_state]),color[n_state],label=str(n_state))
+                ax0.plot(roff,ioff)
+                ax0.axis('equal')
+            ax0.legend()
+        cLst.append(cLst_m)
+    return cLst, num0Lst, num1Lst, fig, axes, pLst
+    
 
 def post_selection(measure,s,sigma_num=2):
     center0,center1 = [], []
     radius0, radius1 = [], []
     for i in measure.postSle:
         center0.append(np.complex(*(measure.postSle[i][0][0])))
         radius0.append(measure.postSle[i][0][1])
```

### Comparing `qufit-1.0.6/qufit/opt.py` & `qufit-1.0.7/qufit/opt.py`

 * *Files identical despite different names*

### Comparing `qufit-1.0.6/qufit/optimize.py` & `qufit-1.0.7/qufit/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,18 +829,22 @@
         res, _ = self.fitExp(x[5:-5],y_new[5:-5])
         A, B, T1 = res
         T1 = 1 / T1
         if np.abs(self.T1-T1)>5000:
             T1 = self.T1
         Ag, Cg, Wg, phig = self.guessCos(x,y)
         return A, B, T1, Wg, phig
+    
+    def func_Rabi(self,x,paras):
+        A,B,T1,w,phi = paras
+        return A*np.exp(-x/T1)*np.cos(2*np.pi*w*x+phi) + B
 
-    def errRabi(self,para,x,y):
-        A,B,T1,w,phi = para
-        return np.sum((A*np.exp(-x/T1)*np.cos(2*np.pi*w*x+phi) + B - y)**2)
+    def errRabi(self,paras,x,y):
+        
+        return np.sum((self.func_Rabi(x,paras) - y)**2)
 
     def fitRabi(self,x,y):
         if self.envelopemethod == 'hilbert':
             out = self.envelope_Hilbert(y)
         else:
             out = self.envelope(y)
         A,B,T1,w,phi = self.guessRabi(x,out,y)
@@ -850,15 +854,15 @@
         B = B if np.abs(B-np.mean(y)) < 0.1*np.mean(y) else np.mean(y)
         p0 = A,B,T1,w,self.phi
         print(p0)
         # res = ls(self.errRabi, p0, args=(np.array(x), np.array(y)))   
         mybounds = MyBounds(xmin=[0,-np.inf,100,0,0],xmax=[np.inf,np.inf,100e3,1.5*w,2*np.pi])
         res = bh(self.errRabi,p0,niter=30,minimizer_kwargs={"method":"Nelder-Mead","args":(x, y)},accept_test=mybounds)      
         A,B,T1,w,phi = res.x
-        return A,B,T1,w,phi,env
+        return res, self.func_Rabi
 
 ################################################################################
 ### 拟合二维谱
 ################################################################################
 
 class Spec2d_Fit(Cos_Fit):
```

### Comparing `qufit-1.0.6/qufit.egg-info/PKG-INFO` & `qufit-1.0.7/qufit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.0.6
+Version: 1.0.7
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.0.6/setup.py` & `qufit-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qufit",
-    version="1.0.6",
+    version="1.0.7",
     author="赵寿宽(sk zhao)",
     author_email="2396776980@qq.com",
     description="本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/",
     packages=setuptools.find_packages(),
```

