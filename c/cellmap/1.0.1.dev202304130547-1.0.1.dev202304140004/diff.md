# Comparing `tmp/cellmap-1.0.1.dev202304130547-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304140004-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 9361 bytes, number of entries: 5
+Zip file size: 9363 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    46362 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304130547.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304130547.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304130547.dist-info/RECORD
-5 files, 48658 bytes uncompressed, 8607 bytes compressed:  82.3%
+-rw-r--r--  2.0 unx    45851 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1752 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140004.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304140004.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304140004.dist-info/RECORD
+5 files, 48147 bytes uncompressed, 8609 bytes compressed:  82.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304130547.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304140004.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304130547.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304140004.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304130547.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304140004.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -219,15 +219,15 @@
     exp_key = None,
     potential_key = 'potential',
     rotation_key = 'rotation',
     vorticity_key = 'vorticity',
     streamline_key = 'stream_line',
     graph_key = 'CellMap_graph',
     graph_method = 'Delauney',
-    HD_rate = 0.2,
+    HD_rate = 0.0,
     n_neighbors = 10,
     contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
     logscale_vel = True,
     ):
@@ -336,27 +336,27 @@
             vel_potential[i] = -2*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
         adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
     
     ## Solve vorticity & stream line
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((vel_LD[:,1],-vel_LD[:,0])).T,source,target))
     stream_line_ = -np.dot(lap_inv,vorticity_)
-    vorticity_ = -np.dot(lap_inv,stream_line_)
+    # vorticity_ = -np.dot(lap_inv,stream_line_)
     adata.obs[vor_key_] = vorticity_
     adata.obs[sl_key_]  = stream_line_-np.min(stream_line_)
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[pot_vkey_][:,1],-adata.obsm[pot_vkey_][:,0])).T,source,target))
     stream_line_ = -np.dot(lap_inv,vorticity_)
-    vorticity_ = -np.dot(lap_inv,stream_line_)
+    # vorticity_ = -np.dot(lap_inv,stream_line_)
     adata.obs[pot_vor_key_] = vorticity_
     adata.obs[pot_sl_key_] = stream_line_-np.min(stream_line_)
 
     vorticity_ = np.dot(div_mat,edge_velocity(exp_LD,np.vstack((adata.obsm[rot_vkey_][:,1],-adata.obsm[rot_vkey_][:,0])).T,source,target))
     stream_line_ = -np.dot(lap_inv,vorticity_)
-    vorticity_ = -np.dot(lap_inv,stream_line_)
+    # vorticity_ = -np.dot(lap_inv,stream_line_)
     adata.obs[rot_vor_key_] = vorticity_
     adata.obs[rot_sl_key_] = stream_line_-np.min(stream_line_)
 
     rot_flow = edge_vel - pot_flow
     adata.obs[rotation_key] = np.array([np.mean(np.vstack((rot_flow[source==i],-rot_flow[target==i]))) for i in range(adata.shape[0])])
 
     ## Contribution ratio
@@ -373,23 +373,20 @@
 
 def Hodge_decomposition_genes(
     adata,
     genes,
     basis = 'umap',
     vkey  = 'velocity',
     exp_key = None,
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     potential_vkey = 'potential_velocity',
-    rotation_key = 'Hodge_rotation',
+    rotation_key = 'rotation',
     rotation_vkey = 'rotation_velocity',
-    graph_key = 'CM_graph',
     graph_method = 'Delauney',
-    HD_rate = 0.2,
     n_neighbors = 10,
-    contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
     logscale_vel = True,
     ):
     """
     Hodge decomposition
@@ -456,29 +453,27 @@
         source_term = np.dot(div_mat,edge_vel)
         potential = np.dot(lap_inv,source_term)
         adata.obs[potential_key+'_Gene_%s' % gene] = potential - np.min(potential)
 
 def view(
     adata,
     basis = 'umap',
-    color_key = 'Hodge_potential',
-    graph_key = 'CM_graph',
+    color_key = 'potential',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
     filename = 'CellMap_view',
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
-                             graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[color_key])
     
@@ -502,15 +497,15 @@
     if save:
         fig.savefig(filename+'.png', bbox_inches='tight')
 
 
 def view_cluster(
     adata,
     basis = 'umap',
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     graph_key = 'CM_graph',
     cluster_key = 'clusters',
     show_graph = True,
     cutedge_vol  = None,
     cutedge_length = None,
     n_points = 1000,
     seed = None,
@@ -553,40 +548,37 @@
     plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(potential_key,fontsize=20)
     ax.axis('off')
 
 
 def view_surface(
     adata,
     basis = 'umap',
-    potential_key = 'Hodge_potential',
-    graph_key = 'CM_graph',
+    color_key = 'potential',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
-                             potential_key = potential_key,
-                             graph_key = graph_key,
                             )
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
 
     if 'cmap' not in kwargs:
-        kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
+        kwargs['cmap'] = cmap_earth(adata.obs[color_key])
     
     data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
     fig,ax = plt.subplots(figsize=(15,10))
-    cntr = ax.tricontourf(tri_,adata.obs[potential_key],cmap=kwargs['cmap'],levels=100,zorder=2)
-    fig.colorbar(cntr, shrink=0.75, orientation='vertical').set_label(potential_key,fontsize=20)
+    cntr = ax.tricontourf(tri_,adata.obs[color_key],cmap=kwargs['cmap'],levels=100,zorder=2)
+    fig.colorbar(cntr, shrink=0.75, orientation='vertical').set_label(color_key,fontsize=20)
     if show_graph: ax.triplot(tri_,color='w',lw=0.5,zorder=10,alpha=1)
     ax.set_xlim(np.min(data_pos[:,0])-0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])),np.max(data_pos[:,0])+0.02*(np.max(data_pos[:,0])-np.min(data_pos[:,0])))
     ax.set_ylim(np.min(data_pos[:,1])-0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])),np.max(data_pos[:,1])+0.02*(np.max(data_pos[:,1])-np.min(data_pos[:,1])))
     ax.tick_params(labelbottom=False,labelleft=False,labelright=False,labeltop=False,bottom=False,left=False,right=False,top=False)
     ax.spines['right'].set_visible(False),ax.spines['top'].set_visible(False),ax.spines['bottom'].set_visible(False),ax.spines['left'].set_visible(False)
     ax.set_title(title,fontsize=18)
     if cluster_key != None:
@@ -623,28 +615,24 @@
     scv.pl.velocity_embedding_stream(adata,basis=basis,vkey=rotation_vkey, title='Rotational flow',ax=ax[2],color=cluster_key,
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=legend_fontsize, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
 
 def view_stream_line(
     adata,
     basis = 'umap',
     contour_key = 'Stream_line',
-    graph_key = 'CM_graph',
     cluster_key = 'clusters',
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
     filename = 'CellMap_view',
     **kwargs
     ):
     
-    kwargs_arg = check_arguments(adata,
-                             basis = basis,
-                             graph_key = graph_key,
-                            )
+    kwargs_arg = check_arguments(adata,basis = basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[contour_key])
     
     data_pos = adata.obsm[basis_key]
@@ -714,15 +702,15 @@
 
 def view_surface_genes(
     adata,
     genes,
     exp_key = None,
     basis = 'umap',
     vkey  = 'velocity',
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     logscale_vel = True,
     **kwargs,
@@ -780,15 +768,15 @@
                         txt = ax[ax_i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold')
                         txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
                         texts.append(txt)
 
 def view_surface_3D(
     adata,
     basis = 'umap',
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     cutedge_vol  = 1,
     cutedge_length = 1,
     elev = 30,
     azim = -60,
     plot_rate = 0.3,
@@ -827,15 +815,15 @@
         # adjust_text(texts)
     ax.view_init(elev=elev, azim=azim)
 
 
 def view_surface_3D_cluster(
     adata,
     basis = 'umap',
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     graph_key = 'CM_graph',
     cluster_key = 'clusters',
     cutedge_vol  = 1,
     cutedge_length = 1,
     elev = 30,
     azim = -60,
     seed = None,
@@ -893,15 +881,15 @@
         print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
 
 
 def write(
     adata,
     filename = 'CellMap',
     basis = 'umap',
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     cluster_key = 'clusters',
     obs_key = None,
     genes = None,
     expression_key = None,
     use_HVG = True,
     n_HVG = 10,
 ):
@@ -946,15 +934,15 @@
     pd_out.to_csv('%s.csv' % filename)
 
 
 def create_dgraph_potential(
     adata,
     basis = 'umap',
     map_key = None,
-    potential_key = 'Hodge_potential',
+    potential_key = 'potential',
     graph_key = 'CM_graph',
     cutedge_vol  = None,
     cutedge_length = None,
     ):
     """
     Hodge decomposition
```

## Comparing `cellmap-1.0.1.dev202304130547.dist-info/METADATA` & `cellmap-1.0.1.dev202304140004.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304130547
+Version: 1.0.1.dev202304140004
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

