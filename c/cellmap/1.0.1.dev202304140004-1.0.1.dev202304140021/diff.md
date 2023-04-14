# Comparing `tmp/cellmap-1.0.1.dev202304140004-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304140021-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 9363 bytes, number of entries: 5
+Zip file size: 9558 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    45851 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140004.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140004.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140004.dist-info/RECORD
-5 files, 48147 bytes uncompressed, 8609 bytes compressed:  82.1%
+-rw-r--r--  2.0 unx    46524 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140021.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140021.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140021.dist-info/RECORD
+5 files, 48820 bytes uncompressed, 8804 bytes compressed:  82.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140004.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304140021.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140004.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304140021.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140004.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304140021.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -474,15 +474,15 @@
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[color_key])
     
     data_pos = adata.obsm[basis_key]
-    fig,ax = plt.subplots(figsize=(15,10))
+    fig,ax = plt.subplots(figsize=(8,6))
     sc = ax.scatter(data_pos[:,0],data_pos[:,1],c=adata.obs[color_key],zorder=10,**kwargs)
     if show_graph:
         tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
         ax.tripcolor(tri_,adata.obs[color_key],lw=0.5,zorder=0,alpha=0.3,cmap=kwargs['cmap'])
     if cluster_key != None:
         if cluster_key in adata.obs.keys():
             cluster = adata.obs[cluster_key]
@@ -521,15 +521,15 @@
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
 
     data_pos = adata.obsm[basis_key]
-    fig,ax = plt.subplots(figsize=(15,10))
+    fig,ax = plt.subplots(figsize=(8,6))
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     # sc = ax.tripcolor(tri_,adata.obs[potential_key],lw=0.5,zorder=0,alpha=0.75,cmap=kwargs['cmap'])
     sc = ax.tricontourf(tri_,adata.obs[potential_key],zorder=0,alpha=0.9,cmap=kwargs['cmap'],levels=100)
     if cluster_key in adata.obs.keys():
         cluster = adata.obs[cluster_key]
         idx_random = np.zeros(cluster.shape,dtype=bool)
         np.random.seed(seed)
@@ -568,15 +568,15 @@
     basis_key = 'X_%s' % basis
 
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[color_key])
     
     data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
-    fig,ax = plt.subplots(figsize=(15,10))
+    fig,ax = plt.subplots(figsize=(8,6))
     cntr = ax.tricontourf(tri_,adata.obs[color_key],cmap=kwargs['cmap'],levels=100,zorder=2)
     fig.colorbar(cntr, shrink=0.75, orientation='vertical').set_label(color_key,fontsize=20)
     if show_graph: ax.triplot(tri_,color='w',lw=0.5,zorder=10,alpha=1)
     ax.set_xlim(np.min(data_pos[:,0])-0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])),np.max(data_pos[:,0])+0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])))
     ax.set_ylim(np.min(data_pos[:,1])-0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])),np.max(data_pos[:,1])+0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])))
     ax.tick_params(labelbottom=False,labelleft=False,labelright=False,labeltop=False,bottom=False,left=False,right=False,top=False)
     ax.spines['right'].set_visible(False),ax.spines['top'].set_visible(False),ax.spines['bottom'].set_visible(False),ax.spines['left'].set_visible(False)
@@ -614,50 +614,64 @@
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
 
 def view_stream_line(
     adata,
     basis = 'umap',
-    contour_key = 'Stream_line',
+    contour_key = 'stream_line',
     cluster_key = 'clusters',
+    potential_key = 'potential',
+    rotation_key = 'rotation',
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
-    filename = 'CellMap_view',
+    filename = 'CellMap_stream_line',
+    figsize = (24,6),
+    fontsize = 18,
+    cbar = False,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,basis = basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
-    if 'cmap' not in kwargs:
-        kwargs['cmap'] = cmap_earth(adata.obs[contour_key])
+    key_ = '%s_%s' % (contour_key,basis)
+    pot_key_ = '%s_%s_%s' % (potential_key,contour_key,basis)
+    rot_key_ = '%s_%s_%s' % (rotation_key,contour_key,basis)
+    
     
     data_pos = adata.obsm[basis_key]
-    fig,ax = plt.subplots(figsize=(15,10))
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
-    sc = ax.tripcolor(tri_,adata.obs[contour_key],cmap=kwargs['cmap'])
-    ax.tricontour(tri_,adata.obs[contour_key],lw=1,alpha=1,levels=20,zorder=3,colors='k',cmap=None,ls='-')
-    if cluster_key != None:
-        if cluster_key in adata.obs.keys():
-            cluster = adata.obs[cluster_key]
-            for c in np.unique(cluster):
-                # plt.scatter(data_pos[cluster == c,0],data_pos[cluster == c,1],zorder=1,alpha=0.1,s=100)
-                txt = plt.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold',zorder=20)
-                txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
+    
+    contour_keys = [key_, pot_key_, rot_key_]
+    camps = [cmap_earth(adata.obs[key_]),'rainbow','coolwarm']
+    titles = ['RNA velocity','Potential flow','Rotational flow']
+    
+    fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
+    for i in range(3):
+        ax[i].axis('off')
+        ax[i].set_title(title,fontsize=18)
+        sc = ax[i].tripcolor(tri_,adata.obs[contour_keys[i]],cmap=camps[i])
+        ax[i].tricontour(tri_,adata.obs[contour_keys[i]],lw=0.2,alpha=0.2,levels=75,zorder=3,colors='k',cmap=None,ls='-')
+        ax[i].tricontour(tri_,adata.obs[contour_keys[i]],lw=1,alpha=1,levels=15,zorder=3,colors='k',cmap=None,ls='-')
+        if cbar: plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(contour_key,fontsize=20)
+        ax[i].set_title(titles[i],fontsize=fontsize)
+        if cluster_key != None:
+            if cluster_key in adata.obs.keys():
+                cluster = adata.obs[cluster_key]
+                for c in np.unique(cluster):
+                    # plt.scatter(data_pos[cluster == c,0],data_pos[cluster == c,1],zorder=1,alpha=0.1,s=100)
+                    txt = ax[i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold',zorder=20)
+                    txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
         else:
             print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
-    ax.axis('off')
-    ax.set_title(title,fontsize=18)
-    plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(contour_key,fontsize=20)
-    if save:
-        fig.savefig(filename+'.png', bbox_inches='tight')
+    if save: fig.savefig(filename+'.png', bbox_inches='tight')
 
 
 def view_quiver(
     adata,
     basis = 'umap',
     vkey = 'velocity',
     potential_vkey = 'potential_velocity',
@@ -678,15 +692,15 @@
     rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
     cluster_set = np.unique(adata.obs[cluster_key].values)
     cmap = plt.get_cmap("tab20")
     color = np.zeros(adata.shape[0],dtype=int)
     for j in range(len(cluster_set)):
         idx = adata.obs[cluster_key] == cluster_set[j]
         color[idx] = j
-    fig,ax = plt.subplots(1,3,figsize=(24,8),tight_layout=True)
+    fig,ax = plt.subplots(1,3,figsize=(24,6),tight_layout=True)
     for i in range(3):
         for j in range(len(cluster_set)):
             idx = adata.obs[cluster_key] == cluster_set[j]
             ax[i].scatter(adata.obsm[basis_key][idx,0],adata.obsm[basis_key][idx,1],s=200,alpha=alpha,label=cluster_set[j],color=cmap(j),zorder=0)
             ax[i].text(np.mean(adata.obsm[basis_key][idx,0]),np.mean(adata.obsm[basis_key][idx,1]),cluster_set[j],fontsize=fontsize,
                        ha='center',va='center',weight='bold')
     idx_qvr_ = np.random.choice(np.arange(adata.shape[0]),int(quiver_rate*adata.shape[0]),replace=False)
```

## Comparing `cellmap-1.0.1.dev202304140004.dist-info/METADATA` & `cellmap-1.0.1.dev202304140021.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304140004
+Version: 1.0.1.dev202304140021
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

