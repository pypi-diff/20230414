# Comparing `tmp/cellmap-1.0.1.dev202304140021-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304140154-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 9558 bytes, number of entries: 5
+Zip file size: 9659 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    46524 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140021.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140021.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140021.dist-info/RECORD
-5 files, 48820 bytes uncompressed, 8804 bytes compressed:  82.0%
+-rw-r--r--  2.0 unx    47154 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140154.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140154.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140154.dist-info/RECORD
+5 files, 49450 bytes uncompressed, 8905 bytes compressed:  82.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140021.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304140154.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140021.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304140154.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304140021.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304140154.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -310,26 +310,30 @@
     potential = np.dot(lap_inv,source_term)
     pot_flow = -np.dot(grad_mat,potential)
     adata.obs[potential_key] = potential - np.min(potential)
 
 
     ## Compute potential & rotational flow
     vel_potential = np.zeros([adata.shape[0],2],dtype=float)
+    # vel_rotation = np.zeros([adata.shape[0],2],dtype=float)
     if graph_method == 'Delauney':
         tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
         source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
         for i in range(adata.shape[0]):
             idx_s = source == i
             idx_t = target == i
             ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
             ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
             vel_potential[i] = 2*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
                                 np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
+            # vel_rotation[i] = 2*(np.sum((adata.obs[rotation_key][source[idx_s]].values-adata.obs[rotation_key][target[idx_s]].values)*ex_s.T,axis=1) + \
+            #                     np.sum((adata.obs[rotation_key][target[idx_t]].values-adata.obs[rotation_key][source[idx_t]].values)*ex_t.T,axis=1))
         adata.obsm[pot_vkey_] = vel_potential
         adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
+        # adata.obsm[rot_vkey_] = vel_rotation
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
@@ -454,59 +458,66 @@
         potential = np.dot(lap_inv,source_term)
         adata.obs[potential_key+'_Gene_%s' % gene] = potential - np.min(potential)
 
 def view(
     adata,
     basis = 'umap',
     color_key = 'potential',
-    cluster_key = None,
-    show_graph = False,
+    cluster_key = 'clusters',
+    show_graph = True,
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
     filename = 'CellMap_view',
+    figsize = None,
+    fontsize_text = 16,
+    cbar = True,
     **kwargs
     ):
     
-    kwargs_arg = check_arguments(adata,
-                             basis = basis,
-                            )
+    kwargs_arg = check_arguments(adata, basis=basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[color_key])
+
+    if cluster_key not in adata.obs.keys():
+        cluster_key = None
     
+    if figsize == None:
+        figsize = (10,6) if cbar else (8,6)
+        
+
     data_pos = adata.obsm[basis_key]
-    fig,ax = plt.subplots(figsize=(8,6))
+    fig,ax = plt.subplots(figsize=figsize)
     sc = ax.scatter(data_pos[:,0],data_pos[:,1],c=adata.obs[color_key],zorder=10,**kwargs)
     if show_graph:
         tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
         ax.tripcolor(tri_,adata.obs[color_key],lw=0.5,zorder=0,alpha=0.3,cmap=kwargs['cmap'])
     if cluster_key != None:
         if cluster_key in adata.obs.keys():
             cluster = adata.obs[cluster_key]
             for c in np.unique(cluster):
-                txt = plt.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold',zorder=20)
+                txt = plt.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=fontsize_text,ha='center', va='center',fontweight='bold',zorder=20)
                 txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
         else:
             print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
     ax.axis('off')
     ax.set_title(title,fontsize=18)
-    plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(color_key,fontsize=20)
-    if save:
-        fig.savefig(filename+'.png', bbox_inches='tight')
+    if cbar: plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(color_key,fontsize=20)
+    if save: fig.savefig(filename+'.png', bbox_inches='tight')
 
 
 def view_cluster(
     adata,
     basis = 'umap',
     potential_key = 'potential',
-    graph_key = 'CM_graph',
+    graph_key = 'CellMap_graph',
     cluster_key = 'clusters',
     show_graph = True,
     cutedge_vol  = None,
     cutedge_length = None,
     n_points = 1000,
     seed = None,
     title = '',
@@ -593,25 +604,26 @@
 def view_stream(
     adata,
     basis = 'umap',
     vkey = 'velocity',
     potential_vkey = 'potential_velocity',
     rotation_vkey = 'rotation_velocity',
     cluster_key = 'clusters',
+    figsize=(24,6),
     density = 4,
     alpha = 0.3,
     fontsize = 18,
     legend_fontsize = 18,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata, basis = basis)
     basis = kwargs_arg['basis']
     
-    fig,ax = plt.subplots(1,3,figsize=(24,8),tight_layout=True)
+    fig,ax = plt.subplots(1,3,figsize=figsize,tight_layout=True)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=vkey, title='RNA velocity',ax=ax[0],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=potential_vkey, title='Potential flow',ax=ax[1],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
 
@@ -717,15 +729,15 @@
 def view_surface_genes(
     adata,
     genes,
     exp_key = None,
     basis = 'umap',
     vkey  = 'velocity',
     potential_key = 'potential',
-    graph_key = 'CM_graph',
+    graph_key = 'CellMap_graph',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     logscale_vel = True,
     **kwargs,
     ):
@@ -783,15 +795,15 @@
                         txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
                         texts.append(txt)
 
 def view_surface_3D(
     adata,
     basis = 'umap',
     potential_key = 'potential',
-    graph_key = 'CM_graph',
+    graph_key = 'CellMap_graph',
     cluster_key = None,
     cutedge_vol  = 1,
     cutedge_length = 1,
     elev = 30,
     azim = -60,
     plot_rate = 0.3,
     title = '',
@@ -830,15 +842,15 @@
     ax.view_init(elev=elev, azim=azim)
 
 
 def view_surface_3D_cluster(
     adata,
     basis = 'umap',
     potential_key = 'potential',
-    graph_key = 'CM_graph',
+    graph_key = 'CellMap_graph',
     cluster_key = 'clusters',
     cutedge_vol  = 1,
     cutedge_length = 1,
     elev = 30,
     azim = -60,
     seed = None,
     n_points = 500,
@@ -949,15 +961,15 @@
 
 
 def create_dgraph_potential(
     adata,
     basis = 'umap',
     map_key = None,
     potential_key = 'potential',
-    graph_key = 'CM_graph',
+    graph_key = 'CellMap_graph',
     cutedge_vol  = None,
     cutedge_length = None,
     ):
     """
     Hodge decomposition
 
     Parameters
```

## Comparing `cellmap-1.0.1.dev202304140021.dist-info/METADATA` & `cellmap-1.0.1.dev202304140154.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304140021
+Version: 1.0.1.dev202304140154
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

