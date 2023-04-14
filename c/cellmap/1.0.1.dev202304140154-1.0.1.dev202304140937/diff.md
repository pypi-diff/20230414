# Comparing `tmp/cellmap-1.0.1.dev202304140154-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304140937-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 9659 bytes, number of entries: 5
+Zip file size: 1388280 bytes, number of entries: 6
+-rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    47154 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140154.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140154.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140154.dist-info/RECORD
-5 files, 49450 bytes uncompressed, 8905 bytes compressed:  82.0%
+-rw-r--r--  2.0 unx    53291 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1783 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140937.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140937.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140937.dist-info/RECORD
+6 files, 4502653 bytes uncompressed, 1387394 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
+Filename: cellmap/CellMap_view_3D.html
+Comment: 
+
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140154.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304140937.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140154.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304140937.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140154.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304140937.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1,20 +1,23 @@
 import anndata
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
-from matplotlib import patheffects as PathEffects
+from matplotlib import patheffects as PathEffect
+import matplotlib.cm
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
 import matplotlib.colors
 import pandas as pd
 import logging
 import scanpy
 import scvelo as scv
+import plotly.graph_objects as go
+from plotly.offline import plot
 
 
 def create_graph(
     X,
     Y,
     cutedge_vol = None,
     cutedge_length = None,
@@ -159,20 +162,25 @@
                     logger.warning('The gene \"%s\" was not found. The gene \"%s\" is removed from \"%s\".' % (arg,arg,key))
                     kwargs[key].remove(arg)
         elif kwargs[key] != None:
             raise TypeError('The argument %s should be a list or None')
 
     return kwargs
 
+def pt(cv,k):
+    return np.percentile(cv,k)
 
 def cmap_earth(cv):
     #c_list  = np.array(['#0938BF','#50D9FB','#B7E5FA','#98D685','#36915c','#F9EFCD','#E0BB7D','#D3A62D','#997618','#705B10','#5F510D','#A56453','#5C1D09'])
     c_min,c_max = 5,95
-    c_list  = np.array(['#0938BF','#50D9FB','#B7E5FA','#98D685','#fff5d1','#997618','#705B10'])
+    c_list  = np.array(['#0938BF','#50D9FB','#B7E5FA','#98D685','#fff5d1','#997618','#705B10','#5C1D09'])
+    # c_list  = np.array(['#0938BF','#0938BF','#50D9FB','#B7E5FA','#98D685','#F9EFCD','#E0BB7D','#D3A62D','#997618','#705B10','#5F510D','#A56453','#5C1D09','#5C1D09'])
     c_level = np.array([np.percentile(cv,(c_max-c_min)*(i)/len(c_list)+c_min) for i in range(len(c_list))])
+    c_list  = ['#0938BF','#50D9FB','#B7E5FA','#98D685','#F9EFCD','#E0BB7D','#D3A62D','#997618','#705B10','#5F510D','#A56453','#5C1D09']
+    c_level = [pt(cv,0),pt(cv,5),pt(cv,20),pt(cv,40),pt(cv,60),pt(cv,75),pt(cv,80),pt(cv,85),pt(cv,90),pt(cv,95),pt(cv,99),pt(cv,100)]
     # c_level = np.array([np.percentile(cv,100*(i)/len(c_list)) for i in range(len(c_list))])
     # c_level = np.array([i*(np.max(cv)-np.min(cv))/len(c_list) + np.min(cv) for i in range(len(c_list))])
     color = np.vstack((c_level,c_list)).T
     hight = 1000*color[:,0].astype(np.float32)
     hightnorm = sklearn.preprocessing.minmax_scale(hight)
     colornorm = []
     for no, norm in enumerate(hightnorm):
@@ -509,53 +517,47 @@
     if save: fig.savefig(filename+'.png', bbox_inches='tight')
 
 
 def view_cluster(
     adata,
     basis = 'umap',
     potential_key = 'potential',
-    graph_key = 'CellMap_graph',
     cluster_key = 'clusters',
-    show_graph = True,
     cutedge_vol  = None,
     cutedge_length = None,
     n_points = 1000,
+    fontsize_text = 16,
     seed = None,
     title = '',
     **kwargs
     ):
     
-    kwargs_arg = check_arguments(adata,
-                             basis = basis,
-                             potential_key = potential_key,
-                             graph_key = graph_key,
-                            )
+    kwargs_arg = check_arguments(adata,basis = basis, potential_key=potential_key)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
 
     data_pos = adata.obsm[basis_key]
     fig,ax = plt.subplots(figsize=(8,6))
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
-    # sc = ax.tripcolor(tri_,adata.obs[potential_key],lw=0.5,zorder=0,alpha=0.75,cmap=kwargs['cmap'])
     sc = ax.tricontourf(tri_,adata.obs[potential_key],zorder=0,alpha=0.9,cmap=kwargs['cmap'],levels=100)
     if cluster_key in adata.obs.keys():
         cluster = adata.obs[cluster_key]
         idx_random = np.zeros(cluster.shape,dtype=bool)
         np.random.seed(seed)
         idx_random[np.random.choice(len(idx_random),min(n_points,len(idx_random)),replace=False)] = True
         cluster_set = np.unique(cluster)
         cmap_pt = plt.get_cmap("tab10") if len(cluster_set) <= 10 else plt.get_cmap("tab20")
         for i in range(len(cluster_set)):
             idx = (cluster == cluster_set[i]) & idx_random
             ax.scatter(data_pos[idx,0],data_pos[idx,1],zorder=10,alpha=0.8,edgecolor='w',color=cmap_pt(i),**kwargs)
             txt = plt.text(np.mean(data_pos[cluster == cluster_set[i]],axis=0)[0],np.mean(data_pos[cluster == cluster_set[i]],axis=0)[1],cluster_set[i]
-                           ,color=cmap_pt(i),fontsize=20,ha='center', va='center',fontweight='bold',zorder=20)
+                           ,color=cmap_pt(i),fontsize=fontsize_text,ha='center', va='center',fontweight='bold',zorder=20)
             txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
     else:
         print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
     ax.set_title(title,fontsize=18)
     plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(potential_key,fontsize=20)
     ax.axis('off')
 
@@ -655,15 +657,15 @@
     
     
     data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     
     contour_keys = [key_, pot_key_, rot_key_]
     camps = [cmap_earth(adata.obs[key_]),'rainbow','coolwarm']
-    titles = ['RNA velocity','Potential flow','Rotational flow']
+    titles = ['RNA velocity orbit','Development orbit','Periodic orbit']
     
     fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
     for i in range(3):
         ax[i].axis('off')
         ax[i].set_title(title,fontsize=18)
         sc = ax[i].tripcolor(tri_,adata.obs[contour_keys[i]],cmap=camps[i])
         ax[i].tricontour(tri_,adata.obs[contour_keys[i]],lw=0.2,alpha=0.2,levels=75,zorder=3,colors='k',cmap=None,ls='-')
@@ -711,14 +713,16 @@
     fig,ax = plt.subplots(1,3,figsize=(24,6),tight_layout=True)
     for i in range(3):
         for j in range(len(cluster_set)):
             idx = adata.obs[cluster_key] == cluster_set[j]
             ax[i].scatter(adata.obsm[basis_key][idx,0],adata.obsm[basis_key][idx,1],s=200,alpha=alpha,label=cluster_set[j],color=cmap(j),zorder=0)
             ax[i].text(np.mean(adata.obsm[basis_key][idx,0]),np.mean(adata.obsm[basis_key][idx,1]),cluster_set[j],fontsize=fontsize,
                        ha='center',va='center',weight='bold')
+            txt = ax[i].text(np.mean(adata.obsm[basis_key][idx,0]),np.mean(adata.obsm[basis_key][idx,1]),cluster_set[j],fontsize=20,ha='center', va='center',fontweight='bold',zorder=20)
+            txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
     idx_qvr_ = np.random.choice(np.arange(adata.shape[0]),int(quiver_rate*adata.shape[0]),replace=False)
     ax[0].quiver(adata.obsm[basis_key][idx_qvr_,0],adata.obsm[basis_key][idx_qvr_,1],adata.obsm[vkey_][idx_qvr_,0],adata.obsm[vkey_][idx_qvr_,1],scale=scale,zorder=1,**kwargs)
     ax[0].set_title('RNA velocity',fontsize=fontsize)
     ax[0].axis('off')
     ax[1].quiver(adata.obsm[basis_key][idx_qvr_,0],adata.obsm[basis_key][idx_qvr_,1],adata.obsm[pot_vkey_][idx_qvr_,0],adata.obsm[pot_vkey_][idx_qvr_,1],scale=scale,zorder=1,**kwargs)
     ax[1].set_title('Potential flow',fontsize=fontsize)
     ax[1].axis('off')
@@ -791,14 +795,176 @@
                 if cluster_key in adata.obs.keys():
                     cluster = adata.obs[cluster_key]
                     for c in np.unique(cluster):
                         txt = ax[ax_i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold')
                         txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
                         texts.append(txt)
 
+def view_3D(
+    adata,
+    basis = 'umap',
+    potential_key = 'potential',
+    cluster_key ='clusters',
+    cutedge_vol  = 1,
+    cutedge_length = 1,
+    show_cells = False,
+    show_shadow = True,
+    shadow_alpha = 0.2,
+    title = 'Landscape',
+    bgcolor = "white",
+    gridcolor = "gray",
+    edges_color='lightgray',
+    seed = None,
+    n_points = 500,
+    save = False,
+    filename = 'CellMap_view_3D',
+    **kwargs
+    ):
+    
+    kwargs_arg = check_arguments(adata, basis=basis, potential_key=potential_key)
+    basis = kwargs_arg['basis']
+    basis_key = 'X_%s' % basis
+    
+    if 'cmap' not in kwargs:
+        kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
+
+    x,y,z = adata.obsm[basis_key][:,0], adata.obsm[basis_key][:,1],adata.obs[potential_key]
+    
+    c_list  = ['#0938BF','#50D9FB','#B7E5FA','#98D685','#F9EFCD','#E0BB7D','#D3A62D','#997618','#705B10','#5F510D','#A56453','#5C1D09']
+    c_level = [0,5,20,40,60,75,80,85,90,95,99,100]
+    custom_cmap = [[0.01*c_level[i],c_list[i]] for i in range(len(c_list))]
+
+    tri_,idx_tri = create_graph(x,y,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
+    triangles = tri_.triangles[idx_tri]
+
+    camera = dict(eye=dict(x=1.8, y=-1.0, z=1.8))
+    idx = np.zeros(adata.shape[0],dtype=bool)
+    np.random.seed(seed)
+    idx[np.random.choice(adata.shape[0],min(n_points,adata.shape[0]),replace=False)] = True
+    shift = 0.01*(max(z)-min(z))
+    shadow = go.Mesh3d(
+        x=x,
+        y=y,
+        z=np.zeros(adata.shape[0]),
+        i=triangles[:, 0],
+        j=triangles[:, 1],
+        k=triangles[:, 2],
+        opacity=shadow_alpha,
+        color='black',
+    )
+
+    if cluster_key in adata.obs.keys():
+        clstr = adata.obs[cluster_key]
+        clstr_set = np.unique(clstr)
+        clstr_id = np.empty(adata.shape[0],dtype=int)
+        text = np.array([clstr[i]+'<br>Potential: '+str(np.round(z[i],decimals=2)) for i in range(adata.shape[0])])
+        for i in range(len(clstr_set)):
+            clstr_id[clstr == clstr_set[i]] = i
+        cmap = plt.get_cmap('tab10')
+        norm = plt.Normalize(vmin=0,vmax=10)
+        color_mapped = cmap(norm(clstr_id[idx]))
+        cells = go.Scatter3d(
+            x=x[idx],
+            y=y[idx],
+            z=z[idx]+shift,
+            mode='markers',
+            marker=dict(
+                size=2.5,
+                color=color_mapped,
+                opacity=1
+            ),
+            text=text[idx],
+            hovertemplate='X: %{x:.2f}<br>Y: %{y:.2f}<br>Z: %{z:.2f}<br>%{text}'
+        )
+
+        surf = go.Mesh3d(
+            x=x,
+            y=y,
+            z=z,
+            i=triangles[:, 0],
+            j=triangles[:, 1],
+            k=triangles[:, 2],
+            intensity=z,
+            colorscale=custom_cmap,
+            text=text,
+            opacity=1,
+            hovertemplate='X: %{x:.2f}<br>Y: %{y:.2f}<br>Z: %{z:.2f}<br>%{text}'
+        )
+        
+        annotations = [dict(
+            showarrow=False,
+            x=np.percentile(x[clstr == np.unique(clstr)[i]],50),
+            y=np.percentile(y[clstr == np.unique(clstr)[i]],50),
+            z=np.percentile(z[clstr == np.unique(clstr)[i]],50),
+            text="<b>%s<b>" % str(np.unique(clstr)[i]),
+            font=dict(size=14,color='rgba(0,0,0,1)'),bgcolor="rgba(255,255,255,0.7)") for i in range(len(np.unique(clstr)))]#,color="rgba%s" % str(tuple(np.array(cmap_clstr(i+1))*255))
+        layout = go.Layout(
+            title = title,
+            width=1500,
+            height=1000,
+            margin=dict(l=0,r=0, b=0,t=50),
+            scene_camera=camera,
+            scene=dict(annotations=annotations,xaxis_title=basis+"_1",yaxis_title=basis+"_2",zaxis_title=potential_key,
+                     xaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
+                     yaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
+                     zaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
+            ),
+            meta=dict(),
+            scene_aspectratio=dict(x=1.2, y=1.2, z=1.2),
+        )
+        data = [surf]
+        if show_cells: data.append(cells)
+        if show_shadow: data.append(shadow)
+        fig = go.Figure(data=data, layout=layout)
+        #                  )
+    else:
+        cells = go.Scatter3d(
+            x=x[idx],
+            y=y[idx],
+            z=z[idx]+shift,
+            mode='markers',
+            marker=dict(
+                size=2,
+                color='gray',
+            ),
+        )
+        surf = go.Mesh3d(
+            x=x,
+            y=y,
+            z=z,
+            i=triangles[:, 0],
+            j=triangles[:, 1],
+            k=triangles[:, 2],
+            intensity=z,
+            colorscale=custom_cmap,
+            opacity=1
+        )
+
+        layout = go.Layout(
+            title = title,
+            width=1500,
+            height=1000,
+            margin=dict(l=0,r=0, b=0,t=50),
+            scene_camera=camera,
+            scene=dict(xaxis_title=basis+"_1",yaxis_title=basis+"_2",zaxis_title=potential_key,
+                     xaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
+                     yaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
+                     zaxis = dict(backgroundcolor=bgcolor,gridcolor=gridcolor),
+            ),
+            meta=dict(),
+            scene_aspectratio=dict(x=1.2, y=1.2, z=1.2),
+        )
+        data = [surf]
+        if show_cells: data.append(cells)
+        if show_shadow: data.append(shadow)
+        fig = go.Figure(data=data, layout=layout)
+    fig.show()
+    
+    if save: plot(fig, filename=filename+'.html')
+
 def view_surface_3D(
     adata,
     basis = 'umap',
     potential_key = 'potential',
     graph_key = 'CellMap_graph',
     cluster_key = None,
     cutedge_vol  = 1,
@@ -873,19 +1039,17 @@
             kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
         fig = plt.figure(figsize=(15,15))
         ax = fig.add_subplot(111, projection='3d')
         cntr = ax.plot_trisurf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],zorder=2,alpha=0.9)#,cmap=cmap_CellMap,levels=100)
         ax.set_box_aspect(aspect = (1,1,0.8))
         ax.set_title(title,fontsize=18)
         fig.colorbar(cntr, shrink=0.5, orientation='vertical').set_label(potential_key,fontsize=20)
-        texts = []
         cluster = adata.obs[cluster_key]
         idx = np.zeros(cluster.shape,dtype=bool)
         np.random.seed(seed)
-        print(n_points,len(idx),min(n_points,len(idx)))
         idx[np.random.choice(len(idx),min(n_points,len(idx)),replace=False)] = True
         cluster_set = np.unique(cluster)
         z_shift = 0.05*np.abs( np.max(adata.obs[potential_key]) - np.min(adata.obs[potential_key]))
         if len(cluster_set) <= 10:
             cmap_pt = plt.get_cmap("tab10")
             vmin,vmax = 0,10
         else:
```

## Comparing `cellmap-1.0.1.dev202304140154.dist-info/METADATA` & `cellmap-1.0.1.dev202304140937.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304140154
+Version: 1.0.1.dev202304140937
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: anndata (>=0.8.0,<0.9.0)
 Requires-Dist: matplotlib (>=3.4.3)
 Requires-Dist: numpy (>=1.20)
+Requires-Dist: plotly (>=5.90)
 Requires-Dist: scikit-learn (>=0.24)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Project-URL: Documentation, https://github.com/yusuke-imoto-lab/CellMap/
 Project-URL: Repository, https://github.com/yusuke-imoto-lab/CellMap
 Description-Content-Type: text/markdown
 
 # CellMap - RNA landscape inference method
```

