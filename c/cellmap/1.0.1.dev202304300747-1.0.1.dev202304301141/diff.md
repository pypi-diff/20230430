# Comparing `tmp/cellmap-1.0.1.dev202304300747-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304301141-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 19238 bytes, number of entries: 5
+Zip file size: 19734 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx   108786 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300747.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300747.dist-info/WHEEL
-?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304300747.dist-info/RECORD
-5 files, 111200 bytes uncompressed, 18484 bytes compressed:  83.4%
+-rw-r--r--  2.0 unx   112821 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304301141.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304301141.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304301141.dist-info/RECORD
+5 files, 115235 bytes uncompressed, 18980 bytes compressed:  83.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304300747.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304301141.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304300747.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304301141.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304300747.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304301141.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -520,15 +520,16 @@
     color_key = 'potential',
     cluster_key = 'clusters',
     show_graph = True,
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
-    filename = 'CellMap_view',
+    save_dir = None,
+    save_filename = 'CellMap_view',
     figsize = None,
     fontsize_text = 16,
     cbar = True,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata, basis=basis)
@@ -558,15 +559,17 @@
                 txt = plt.text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=fontsize_text,ha='center', va='center',fontweight='bold',zorder=20)
                 txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
         else:
             print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
     ax.axis('off')
     ax.set_title(title,fontsize=18)
     if cbar: plt.colorbar(sc,aspect=20, pad=0.01, orientation='vertical').set_label(color_key,fontsize=20)
-    if save: fig.savefig(filename+'.png', bbox_inches='tight')
+    if save:
+        filename = '%s' % (save_filename) if save_dir == None else '%s/%s' % (save_dir,save_filename)
+        fig.savefig(filename+'.png', bbox_inches='tight')
 
 
 def view_cluster(
     adata,
     basis = 'umap',
     potential_key = 'potential',
     cluster_key = 'clusters',
@@ -694,15 +697,16 @@
     cluster_key = 'clusters',
     potential_key = 'potential',
     rotation_key = 'rotation',
     cutedge_vol  = None,
     cutedge_length = None,
     title = '',
     save = False,
-    filename = 'CellMap_stream_line',
+    save_dir = None,
+    save_filename = 'CellMap_stream_line',
     figsize = (24,6),
     fontsize = 18,
     cbar = False,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,basis = basis)
@@ -735,15 +739,17 @@
                 cluster = adata.obs[cluster_key]
                 for c in np.unique(cluster):
                     # plt.scatter(data_pos[cluster == c,0],data_pos[cluster == c,1],zorder=1,alpha=0.1,s=100)
                     txt = ax[i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=20,ha='center', va='center',fontweight='bold',zorder=20)
                     txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
         else:
             print('There is no cluster key \"%s\" in adata.obs' % cluster_key)
-    if save: fig.savefig(filename+'.png', bbox_inches='tight')
+    if save:
+        filename = '%s' % (save_filename) if save_dir == None else '%s/%s' % (save_dir,save_filename)
+        fig.savefig(filename+'.png', bbox_inches='tight')
 
 
 def view_quiver(
     adata,
     basis = 'umap',
     vkey = 'velocity',
     potential_vkey = 'potential_velocity',
@@ -866,15 +872,14 @@
     cutedge_length = None,
     show_cells = False,
     show_shadow = True,
     shadow_alpha = 0.2,
     title = 'Landscape',
     bgcolor = "white",
     gridcolor = "gray",
-    edges_color='lightgray',
     seed = None,
     n_points = 500,
     save = False,
     filename = 'CellMap_view_3D',
     **kwargs
     ):
     
@@ -1589,20 +1594,20 @@
         n_div = 100,
         fontsize_label = 14,
         fontsize_text = 12,
         fontsize_nDEG = 18,
         fontsize_legend = 10,
         DEG_min = 1.0,
         DEG_rate = 0.3,
-        save_type = 'gif',
         max_num_annotations = 10,
         max_num_legend = 40,
         save = False,
         save_dir = None,
         save_filename = 'DEG_dynamics',
+        save_type = 'gif',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     n_plot_ = int(len(target_clusters)*(len(target_clusters)-1)/2)
     cmap_ = plt.get_cmap("tab10")
@@ -1714,17 +1719,31 @@
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
             ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
             if save:
                 filename = '%s_%s_%s' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
                 if len(target_genes): filename += '_TG' + str(len(target_genes))
-                filename += '.gif'
-                print('\nSaving gif animation as %s' % filename)
-                ani.save(filename)
+                if save_type in ['gif','video','animetion']:
+                    filename += '.gif'
+                    print('\nSaving gif animation as %s...' % filename)
+                    ani.save(filename)
+                elif save_type in ['image','png','jpg','jpeg']:
+                    if save_type == 'image': save_type = 'png'
+                    print('\nSaving gif animation as %s' % filename)
+                    for t in range(n_div+1):
+                        fig = plt.figure(figsize=(14,10),tight_layout=True)
+                        grid = plt.GridSpec(10,14)
+                        ax1 = fig.add_subplot(grid[0:2,0:12])
+                        ax2 = fig.add_subplot(grid[2:10,0:8])
+                        ax3 = fig.add_subplot(grid[2:10,8:14])
+                        update(t,name_i_,name_j_,max_val_,lim,i,j,k)
+                        filename_ = '%s_%03d.%s' % (filename,t,save_type)
+                        fig.savefig(filename_, bbox_inches='tight')
+                        plt.close()
             plt.close()
 
 def DEG_dynamics_clusters(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
@@ -1735,20 +1754,20 @@
         n_div = 100,
         fontsize_label = 14,
         fontsize_text = 12,
         fontsize_nDEG = 18,
         fontsize_legend = 10,
         DEG_min = 1.0,
         DEG_rate = 0.3,
-        save_type = 'gif',
         max_num_annotations = 10,
         max_num_legend = 25,
         save = False,
         save_dir = None,
         save_filename = 'DEG_dynamics',
+        save_type = 'gif',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     n_plot_ = int(len(target_clusters)*(len(target_clusters)-1)/2)
     cmap_ = plt.get_cmap("tab10")
@@ -1860,24 +1879,40 @@
             grid = plt.GridSpec(10,14)
             ax1 = fig.add_subplot(grid[0:2,0:12])
             ax2 = fig.add_subplot(grid[2:10,0:8])
             ax3 = fig.add_subplot(grid[2:10,8:14])
             max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
-            n_clusters = max(np.max(adata.var['clusters_'+name_i_]),np.max(adata.var['clusters_'+name_j_]))+1
             ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
+            plt.close()
             if save:
                 filename = '%s_%s_%s' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
                 if len(target_genes): filename += '_TG' + str(len(target_genes))
-                filename += '.gif'
-                print('\nSaving gif animation as %s' % filename)
-                ani.save(filename)
-            plt.close()
+                if save_type in ['gif','video','animetion']:
+                    filename += '.gif'
+                    print('\nSaving gif animation as %s' % filename)
+                    ani.save(filename)
+                elif save_type in ['image','png','jpg','jpeg']:
+                    matplotlib.use('Agg')
+                    if save_type == 'image': save_type = 'png'
+                    print('\nSaving gif animation as %s' % filename)
+                    for t in range(n_div+1):
+                        fig = plt.figure(figsize=(14,10),tight_layout=True)
+                        grid = plt.GridSpec(10,14)
+                        ax1 = fig.add_subplot(grid[0:2,0:12])
+                        ax2 = fig.add_subplot(grid[2:10,0:8])
+                        ax3 = fig.add_subplot(grid[2:10,8:14])
+                        update(t,name_i_,name_j_,max_val_,lim,i,j,k)
+                        filename_ = '%s_%03d.%s' % (filename,t,save_type)
+                        fig.savefig(filename_, bbox_inches='tight')
+                        plt.close()
+                    matplotlib.use('TkAgg')
+                    
 
 def culc_bifurcation_diagram(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
         exp_key = None,
@@ -1913,14 +1948,17 @@
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
         bifurcation_diagram_key = 'bifurcation_diagram',
         n_div = 100,
         fontsize_label = 14,
         adjusttext =False,
         PC = 1,
+        save = False,
+        save_dir = None,
+        save_filename = 'bifurcation_diagram',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
         culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
     
     if bifurcation_diagram_key not in adata.uns.keys():
         culc_bifurcation_diagram(
@@ -1948,14 +1986,17 @@
     ax.spines['top'].set_visible(False)
     ax.spines['bottom'].set_visible(False)
     ax.xaxis.set_label_position('top')
     ax.xaxis.tick_top()
     ax.yaxis.set_visible(False)
     ax.set_xticks(vlines)
     ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
+    if save:
+        filename = '%s' % (save_filename) if save_dir == None else '%s/%s' % (save_dir,save_filename)
+        fig.savefig(filename+'.png', bbox_inches='tight')
 
 def culc_gene_atlas(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
         exp_key = None,
@@ -2038,14 +2079,15 @@
         threshold_min = 1,
         n_clusters = 20,
         n_components = 2,
         pt_size = 5,
         save = False,
         save_dir = None,
         save_filename = 'gene_atlas',
+        save_type = 'html',
     ):
     if gene_atlas_key not in adata.uns.keys():
         culc_gene_atlas(adata,source_cluster,target_clusters,gene_dynamics_key = gene_dynamics_key, gene_atlas_key=gene_atlas_key,
             n_div = n_div,n_neighbors = n_neighbors,min_dist = min_dist,seed = seed,threshold_min=threshold_min, 
             n_clusters = n_clusters,n_components = n_components,
         )
     elif n_clusters != len(np.unique(adata.uns[gene_atlas_key]['clusters'])):
@@ -2192,19 +2234,29 @@
             zeroline=False,
             showticklabels=False,
             layer='below traces',
         ),
         annotations=annotations
     )
 
-    fig = go.Figure(data=data_clusters_, layout=layout)
-    pio.show(fig)
+    fig1 = go.Figure(data=data_clusters_, layout=layout)
+    pio.show(fig1)
+
+    fig2 = go.Figure(data=data_celltypes_, layout=layout)
+    pio.show(fig2)
+
+    if save:
+        filename = '%s' % (save_filename) if save_dir == None else '%s/%s' % (save_dir,save_filename)
+        if save_type in ['png','pdf','svg','eps']:
+            pio.write_image(fig1, filename + '_cluster.' + save_type)
+            pio.write_image(fig2, filename + '_celltype.' + save_type)
+        if save_type in ['html']:
+            plotly.offline.plot(fig1, filename=filename + '_cluster.' + save_type)
+            plotly.offline.plot(fig2, filename=filename + '_celltype.' + save_type)
 
-    fig = go.Figure(data=data_celltypes_, layout=layout)
-    pio.show(fig)
 
 
 def gene_dynamics_clusters(
         adata,
         source_cluster,
         target_clusters,
         gene_dynamics_key = 'gene_dynamics',
@@ -2304,37 +2356,52 @@
 
     if gene_dynamics_key not in adata.uns.keys():
         culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     idx_t_n_ = np.arange(n_div+1)[(np.linspace(0,1,n_div+1) <= time)]
     idx_t_p_ = np.arange(n_div+1)[(np.linspace(0,1,n_div+1) >= time)]
 
-    i,j = 0,1
-    name_i_ = source_cluster + '_' + target_clusters[i]
-    name_j_ = source_cluster + '_' + target_clusters[j]
-    gene_dynamics_ = adata.uns[gene_dynamics_key]
-
-    max_i_,max_j_ = np.max(gene_dynamics_[name_i_],axis=0),np.max(gene_dynamics_[name_j_],axis=0)
-    idx_max_ = (max_i_ > threshold_min) & (max_j_ > threshold_min)
-
-    vol_p_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_p_]-gene_dynamics_[name_j_][idx_t_p_]),axis=0)
-    vol_n_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_n_]-gene_dynamics_[name_j_][idx_t_n_]),axis=0)
-    diff_ = vol_p_/(1e-5+vol_n_)
-    diff_order_ = np.argsort(diff_[idx_max_])[::-1]
+    columns_ = []
+    for i in range(len(target_clusters)):
+        for j in range(i+1,len(target_clusters)):
+            columns_ = np.append(columns_,target_clusters[i]+'_vs_'+target_clusters[j])
 
     cmap_ = plt.get_cmap("tab10")
     vlines = [0,0.2,0.4,0.6,0.8,1]
-    vline_labels = np.append(np.append('Source (0)\n%s' % source_cluster,np.array(vlines)[1:-1]),'Target (1)')
-    for i_ in range(n_genes):
-        fig,ax = plt.subplots(1,1,figsize=(8,2),tight_layout=True)
-        ax.plot(np.linspace(0,1,n_div+1),gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]],color=cmap_(i),zorder=2)
-        ax.text(1,gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]][-1],' '+target_clusters[i],fontsize=fontsize_label,va='center',ha='left')
-        ax.plot(np.linspace(0,1,n_div+1),gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]],color=cmap_(j),zorder=2)
-        ax.text(1,gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]][-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left')
-        ax.set_title(adata.var.index[idx_max_][diff_order_[i_]])
-        ax.axvline(time,color='r',zorder=1)
-        ax.text(time,0.95,str(time)+' ',color='r',zorder=1,va='top',ha='right',transform=ax.transAxes)
-        ax.set_xlim([0,1])
-        ax.set_xticks(vlines)
-        ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
-        ax.spines['top'].set_visible(False)
-        ax.spines['right'].set_visible(False)
+    sign_dict_ = {'1':'+','-1':'-'}
+    out_pd_ = pd.DataFrame(index=(np.arange(n_genes)+1),columns=pd.MultiIndex.from_product([list(columns_),[]]))
+    for i in range(len(target_clusters)):
+        for j in range(i+1,len(target_clusters)):
+            
+            name_i_ = source_cluster + '_' + target_clusters[i]
+            name_j_ = source_cluster + '_' + target_clusters[j]
+            gene_dynamics_ = adata.uns[gene_dynamics_key]
+
+            max_i_,max_j_ = np.max(gene_dynamics_[name_i_],axis=0),np.max(gene_dynamics_[name_j_],axis=0)
+            idx_max_ = (max_i_ > threshold_min) & (max_j_ > threshold_min)
+
+            vol_p_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_p_]-gene_dynamics_[name_j_][idx_t_p_]),axis=0)
+            vol_n_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_n_]-gene_dynamics_[name_j_][idx_t_n_]),axis=0)
+            diff_ = vol_p_/(1e-5+vol_n_)
+            diff_order_ = np.argsort(diff_[idx_max_])[::-1]
+
+            out_pd_[(target_clusters[i]+'_vs_'+target_clusters[j],'gene')] = adata.var.index[idx_max_][diff_order_[:n_genes]]
+            sign_ = [int(np.sign(np.sum(gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]][idx_t_p_]-gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]][idx_t_p_]))) for i_ in range(n_genes)]
+            out_pd_[(target_clusters[i]+'_vs_'+target_clusters[j],target_clusters[i])] = [sign_dict_[str(s_)] for s_ in sign_]
+            out_pd_[(target_clusters[i]+'_vs_'+target_clusters[j],target_clusters[j])] = [sign_dict_[str(-s_)] for s_ in sign_]
+
+            vline_labels = np.append(np.append('Source (0)\n%s' % source_cluster,np.array(vlines)[1:-1]),'Target (1)')
+            for i_ in range(n_genes):
+                fig,ax = plt.subplots(1,1,figsize=(8,2),tight_layout=True)
+                ax.plot(np.linspace(0,1,n_div+1),gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]],color=cmap_(i),zorder=2)
+                ax.text(1,gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]][-1],' '+target_clusters[i],fontsize=fontsize_label,va='center',ha='left')
+                ax.plot(np.linspace(0,1,n_div+1),gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]],color=cmap_(j),zorder=2)
+                ax.text(1,gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]][-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left')
+                ax.set_title(adata.var.index[idx_max_][diff_order_[i_]])
+                ax.axvline(time,color='r',zorder=1)
+                ax.text(time,0.95,str(time)+' ',color='r',zorder=1,va='top',ha='right',transform=ax.transAxes)
+                ax.set_xlim([0,1])
+                ax.set_xticks(vlines)
+                ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
+                ax.spines['top'].set_visible(False)
+                ax.spines['right'].set_visible(False)
+    display(out_pd_)
```

## Comparing `cellmap-1.0.1.dev202304300747.dist-info/METADATA` & `cellmap-1.0.1.dev202304301141.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304300747
+Version: 1.0.1.dev202304301141
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

