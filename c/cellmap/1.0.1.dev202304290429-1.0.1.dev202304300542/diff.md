# Comparing `tmp/cellmap-1.0.1.dev202304290429-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304300542-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 17762 bytes, number of entries: 5
+Zip file size: 19251 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    91233 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304290429.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304290429.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304290429.dist-info/RECORD
-5 files, 93646 bytes uncompressed, 17008 bytes compressed:  81.8%
+-rw-r--r--  2.0 unx   108732 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1869 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300542.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304300542.dist-info/WHEEL
+?rw-r--r--  2.0 unx      405 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304300542.dist-info/RECORD
+5 files, 111146 bytes uncompressed, 18497 bytes compressed:  83.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304290429.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304300542.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304290429.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304300542.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304290429.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304300542.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1,8 +1,9 @@
-from adjustText import adjust_text
+# from adjustText import adjust_text
+import adjustText
 import anndata
 import IPython.display
 import logging
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.cm
@@ -12,16 +13,17 @@
 import networkx as nx
 import scanpy
 import scipy
 import scvelo as scv
 import sklearn.preprocessing
 import sklearn.mixture
 import sklearn.neighbors
-from sklearn.linear_model import LinearRegression
-from sklearn.preprocessing import PolynomialFeatures
+import sklearn.linear_model
+# from sklearn.linear_model import LinearRegression
+# from sklearn.preprocessing import PolynomialFeatures
 import pandas as pd
 import plotly.graph_objects as go
 import plotly.io as pio
 import plotly.offline
 import umap
 
 
@@ -484,15 +486,15 @@
     if graph_method == 'Delauney':
         source, target = create_graph(exp_LD,cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_type='edges')
         # source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
         exp_HD_pca = pca.fit_transform(exp_HD)
         n_pca = np.min(np.arange(len(pca.explained_variance_ratio_))[np.cumsum(pca.explained_variance_ratio_)>contribution_rate])
-        knn = NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
+        knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_HD_pca[:,:n_pca])
         distances, indices = knn.kneighbors(exp_HD_pca[:,:n_pca])
         distances, indices = distances[:,1:], indices[:,1:]
         source = np.ravel(np.repeat(np.arange(exp_HD.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
     n_edge_ = len(source)
@@ -679,15 +681,14 @@
                                      show=False,density=density,alpha=alpha,fontsize=fontsize,legend_fontsize=0, legend_loc=None,arrow_size=2,linewidth=2,**kwargs)
     for i in range(3):
         texts = []
         for c in np.unique(cluster):
             txt = ax[i].text(np.mean(data_pos[cluster == c],axis=0)[0],np.mean(data_pos[cluster == c],axis=0)[1],c,fontsize=legend_fontsize,ha='center', va='center',fontweight='bold',zorder=20)
             txt.set_path_effects([PathEffects.withStroke(linewidth=5, foreground='w')])
             texts.append(txt)
-        # adjust_text(texts)
 
 
 def view_stream_line(
     adata,
     basis = 'umap',
     contour_key = 'streamfunc',
     cluster_key = 'clusters',
@@ -1376,16 +1377,16 @@
         n_cells_ = np.min([n_cells,sum(adata.obs[cluster_key].values == source_cluster),sum(adata.obs[cluster_key].values == target_cluster)])
         data_trg_ = data_pos[adata.obs[cluster_key].values == target_cluster]
         center_trg_ = np.mean(data_trg_,axis=0)
         centrality_trg_ = np.linalg.norm(data_trg_-center_trg_,axis=1)
         n_trg_ = sum(adata.obs[cluster_key].values == target_cluster)
         idx_trg_ = np.arange(0,n_trg_,int(n_trg_/n_cells_))[:n_cells_]
         trg_set_ = np.arange(adata.shape[0])[adata.obs[cluster_key].values == target_cluster][np.argsort(centrality_trg_)][idx_trg_]
-        idx_src_= np.array([np.argmin(np.abs(streamfunc_[trg__] - streamfunc_[src_set_all_].values)) for trg__ in trg_set_])
-        # idx_src_ = np.arange(0,n_src_,int(n_src_/n_cells_))[:n_cells_]
+        # idx_src_= np.array([np.argmin(np.abs(streamfunc_[trg__] - streamfunc_[src_set_all_].values)) for trg__ in trg_set_])
+        idx_src_ = np.arange(0,n_src_,int(n_src_/n_cells_))[:n_cells_]
         src_set_ = src_set_all_[idx_src_]
 
         pathes,edges,weights,dists  = [],[],[],[]
         for src_,trg_ in np.vstack((src_set_,trg_set_)).T:
             # G.add_weighted_edges_from([(int(s),int(t),np.exp(-g*register)*np.linalg.norm(streamfunc_[trg_]-streamfunc_[int(t)])*np.exp(np.linalg.norm(data_pos[int(s)]-data_pos[int(t)])/dis_mean)) for s,t,g in np.vstack((source,target,grad_)).T])
             # G.add_weighted_edges_from([(int(t),int(s), np.exp(g*register)*np.linalg.norm(streamfunc_[trg_]-streamfunc_[int(t)])*np.exp(np.linalg.norm(data_pos[int(s)]-data_pos[int(t)])/dis_mean)) for s,t,g in np.vstack((source,target,grad_)).T])
             # weights_ = np.hstack((np.exp(-grad_*register)*np.abs(streamfunc_[trg_]-streamfunc_[target])*np.exp(np.linalg.norm(data_pos[source]-data_pos[target],axis=1)/dis_mean),np.exp(grad_*register)*np.abs(streamfunc_[trg_]-streamfunc_[target])*np.exp(np.linalg.norm(data_pos[source]-data_pos[target],axis=1)/dis_mean)))
@@ -1464,15 +1465,15 @@
     #     for i in range(n_cells_):
     #         ax.plot(data_pos[pathes[i],0],data_pos[pathes[i],1],color=cmap_(i_trg_),zorder=10,ls=':')
     # ax.scatter(data_pos[src_set_,0],data_pos[src_set_,1],color='gray',zorder=20,marker='D',s=30)
     # ax.axis('off')
     # adata.uns[path_key] = path_all
 
 
-def gene_dynamics(
+def culc_gene_dynamics(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
         n_div = 100,
@@ -1490,48 +1491,47 @@
         name_ = source_cluster+'_'+target_clusters[i]
         x_data,y_data = np.empty(0,dtype=float),np.empty([0,adata.shape[1]],dtype=float)
         for pi in path[name_]:
             x_data = np.append(x_data,np.linspace(0,1,len(pi)))
             y_data = np.vstack((y_data,data_exp[pi]))
 
         X = x_data[:, np.newaxis]
-        poly = PolynomialFeatures(degree=10)
+        poly = sklearn.preprocessing.PolynomialFeatures(degree=10)
         X_poly = poly.fit_transform(X)
-        model = LinearRegression()
+        model = sklearn.linear_model.LinearRegression()
         model.fit(X_poly, y_data)
         plot_x = np.linspace(0,1,n_div+1)
         gd_i_ = model.predict(poly.fit_transform(plot_x[:, np.newaxis]))
         gd_i_[gd_i_ <0] = 0
         gene_dynamics_[source_cluster+'_'+target_clusters[i]] = gd_i_
     adata.uns[gene_dynamics_key] = gene_dynamics_
     print('Done the computation of gene dynamics')
     
 
-
-
 def gene_dynamics_plot(
     adata,
     source_cluster,
     target_clusters,
     genes,
     path_key = 'path',
     exp_key = None,
     gene_dynamics_key = 'gene_dynamics',
+    n_div = 100,
     fontsize_title = 16,
     fontsize_label = 14,
     fontsize_legend = 12,
     save = False,
     save_dir = None,
     save_filename = 'gene_dynamics_plot',
 ):
     
     # kwargs_arg = check_arguments(adata, verbose=True)
 
     if gene_dynamics_key not in adata.uns.keys():
-        gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     if exp_key == None:
         if scipy.sparse.issparse(adata.X): data_exp = adata.X.toarray()
         else: data_exp = adata.X
     else:
         data_exp = adata.layers[exp_key]
     path = adata.uns[path_key]
@@ -1568,284 +1568,527 @@
                 fig.savefig(filename+'.png', bbox_inches='tight')
             plt.close()
         else:
             print('Gene \"%s\" was not found' % gene)
 
 
 
-def gene_dynamics_DEG(
+def DEG_dynamics(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
+        bifurcation_diagram_key = 'bifurcation_diagram',
         target_genes = [],
         n_div = 100,
         fontsize_label = 14,
         fontsize_text = 12,
         fontsize_nDEG = 18,
         fontsize_legend = 10,
         DEG_min = 1.0,
         DEG_rate = 0.3,
         save_type = 'gif',
         adjusttext = True,
         max_num_annotations = 10,
         max_num_legend = 40,
         save = False,
         save_dir = None,
-        save_filename = 'gene_dynamics_DEG',
+        save_filename = 'DEG_dynamics',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
-        gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     n_plot_ = int(len(target_clusters)*(len(target_clusters)-1)/2)
     cmap_ = plt.get_cmap("tab10")
     gene_dynamics_ = adata.uns[gene_dynamics_key]
     matplotlib.rcParams['animation.embed_limit'] = 2**128
-    # def update(t,name_i_,name_j_,max_val_,lim,i,j,k):
-    #     print('\rcomputing %s vs %s (%d/%d) %d/%d' % (target_clusters[i],target_clusters[j],k,n_plot_,t+1,n_div),end='')
-    #     idx_DEG_i_ = np.arange(adata.shape[1])[(gene_dynamics_[name_j_][t] < gene_dynamics_[name_i_][t] - DEG_rate) & (gene_dynamics_[name_i_][t] > DEG_min)]
-    #     idx_DEG_j_ = np.arange(adata.shape[1])[(gene_dynamics_[name_i_][t] < gene_dynamics_[name_j_][t] - DEG_rate) & (gene_dynamics_[name_j_][t] > DEG_min)]
-    #     if len(idx_DEG_i_) > max_num_annotations:
-    #         idx_DEG_top_i_ = idx_DEG_i_[np.argsort(gene_dynamics_[name_i_][t][idx_DEG_i_]- DEG_rate - gene_dynamics_[name_j_][t][idx_DEG_i_])[::-1][:max_num_annotations]]
-    #     else:
-    #         idx_DEG_top_i_  = idx_DEG_i_
-    #     if len(idx_DEG_j_) > max_num_annotations:
-    #         idx_DEG_top_j_ = idx_DEG_j_[np.argsort(gene_dynamics_[name_j_][t][idx_DEG_j_]- DEG_rate - gene_dynamics_[name_i_][t][idx_DEG_j_])[::-1][:max_num_annotations]]
-    #     else:
-    #         idx_DEG_top_j_  = idx_DEG_j_
-    #     plt.cla()
-    #     plt.title('Time = %.02f [s]' % (t/n_div))
-    #     plt.scatter(gene_dynamics_[name_i_][t],gene_dynamics_[name_j_][t],s=1,color="gray",zorder=1)
-    #     plt.scatter(gene_dynamics_[name_i_][t][idx_DEG_i_],gene_dynamics_[name_j_][t][idx_DEG_i_],color=cmap_(i),zorder=2,s=20)
-    #     plt.scatter(gene_dynamics_[name_i_][t][idx_DEG_j_],gene_dynamics_[name_j_][t][idx_DEG_j_],color=cmap_(j),zorder=2,s=20)
-    #     texts = []
-    #     for g in np.arange(adata.shape[1])[idx_DEG_top_i_]:
-    #         tx_ = plt.text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
-    #         texts = np.append(texts,tx_)
-    #     for g in np.arange(adata.shape[1])[idx_DEG_top_j_]:
-    #         tx_ = plt.text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
-    #         texts = np.append(texts,tx_)
-    #     if len(target_genes):
-    #         for gene_ in target_genes:
-    #             idx_gene_ = adata.var.index == gene_
-    #             plt.scatter(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],s=20,color="red",zorder=2)
-    #             tx_ = plt.text(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],gene_,color="r",zorder=2,fontsize=fontsize_text)
-    #             texts = np.append(texts,tx_)
-    #     if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'))
-    #     plt.text(0.9*(lim[1]-lim[0])+lim[0], 0.1*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_i_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(i), fontweight="bold",zorder=3)
-    #     plt.text(0.1*(lim[1]-lim[0])+lim[0], 0.9*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_j_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(j), fontweight="bold",zorder=3)
-    #     plt.fill_between(lim, lim-DEG_rate, lim+DEG_rate, facecolor='lightgray',  alpha=0.5,zorder=0)
-    #     plt.fill([-0.01*max_val_, DEG_min, DEG_min, -0.01*max_val_], [-0.01*max_val_, -0.01*max_val_, DEG_min, DEG_min], facecolor='lightgray', alpha=0.5,zorder=0)
-    #     plt.xlabel(target_clusters[i],fontsize=fontsize_label,color=cmap_(i), fontweight="bold")
-    #     plt.ylabel(target_clusters[j],fontsize=fontsize_label,color=cmap_(j), fontweight="bold")
-    #     plt.xlim(lim)
-    #     plt.ylim(lim)
-    #     plt.grid(ls='--')
+    vlines = [0,0.2,0.4,0.6,0.8,1]
+    vline_labels = np.append(np.append('Source (0)',np.array(vlines)[1:-1]),'Target (1)')
     def update(t,name_i_,name_j_,max_val_,lim,i,j,k):
         print('\rcomputing %s vs %s (%d/%d) %d/%d' % (target_clusters[i],target_clusters[j],k,n_plot_,t+1,n_div+1),end='')
         idx_DEG_i_ = np.arange(adata.shape[1])[(gene_dynamics_[name_j_][t] < gene_dynamics_[name_i_][t] - DEG_rate) & (gene_dynamics_[name_i_][t] > DEG_min)]
         idx_DEG_j_ = np.arange(adata.shape[1])[(gene_dynamics_[name_i_][t] < gene_dynamics_[name_j_][t] - DEG_rate) & (gene_dynamics_[name_j_][t] > DEG_min)]
         idx_DEG_i_ = idx_DEG_i_[np.argsort(gene_dynamics_[name_i_][t][idx_DEG_i_]- DEG_rate - gene_dynamics_[name_j_][t][idx_DEG_i_])[::-1]]
         idx_DEG_j_ = idx_DEG_j_[np.argsort(gene_dynamics_[name_j_][t][idx_DEG_j_]- DEG_rate - gene_dynamics_[name_i_][t][idx_DEG_j_])[::-1]]
         if len(idx_DEG_i_) > max_num_annotations:
             idx_DEG_ann_i_ = idx_DEG_i_[:max_num_annotations]
         else:
             idx_DEG_ann_i_  = idx_DEG_i_
         if len(idx_DEG_j_) > max_num_annotations:
             idx_DEG_ann_j_ = idx_DEG_j_[:max_num_annotations]
         else:
             idx_DEG_ann_j_  = idx_DEG_j_
-        
+
         if len(idx_DEG_i_) > max_num_legend:
             idx_DEG_leg_i_ = idx_DEG_i_[:max_num_legend]
         else:
             idx_DEG_leg_i_  = idx_DEG_i_
         if len(idx_DEG_j_) > max_num_legend:
             idx_DEG_leg_j_ = idx_DEG_j_[:max_num_legend]
         else:
             idx_DEG_leg_j_  = idx_DEG_j_
-        ax[0].cla()
-        ax[1].cla()
-        ax[0].set_title('Time = %.02f [s]' % (t/n_div))
-        ax[0].scatter(gene_dynamics_[name_i_][t],gene_dynamics_[name_j_][t],s=1,color="gray",zorder=1)
-        ax[0].scatter(gene_dynamics_[name_i_][t][idx_DEG_i_],gene_dynamics_[name_j_][t][idx_DEG_i_],color=cmap_(i),zorder=2,s=20)
-        ax[0].scatter(gene_dynamics_[name_i_][t][idx_DEG_j_],gene_dynamics_[name_j_][t][idx_DEG_j_],color=cmap_(j),zorder=2,s=20)
+        ax1.cla()
+        ax2.cla()
+        ax3.cla()
+        name_i__ = source_cluster + '_' + target_clusters[0]
+        ax1.text(0,adata.uns[bifurcation_diagram_key][name_i_][0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
+        for i_ in range(len(target_clusters)):
+            name_i__ = source_cluster + '_' + target_clusters[i_]
+            if name_i__ not in [name_i_,name_j_]:
+                y_ = adata.uns[bifurcation_diagram_key][name_i__]
+                ax1.plot(np.linspace(0,1,len(y_)),y_,lw=3,zorder=2,alpha=0.3,color=cmap_(i_))
+                ax1.text(1,y_[-1],' '+target_clusters[i_],fontsize=fontsize_label,va='center',ha='left',alpha=0.3)
+        y_ = adata.uns[bifurcation_diagram_key][name_i_]
+        ax1.plot(np.linspace(0,1,len(y_)),y_,lw=5,zorder=3,color=cmap_(i))
+        ax1.text(1,y_[-1],' '+target_clusters[i],fontsize=fontsize_label,va='center',ha='left')
+        y_ = adata.uns[bifurcation_diagram_key][name_j_]
+        ax1.plot(np.linspace(0,1,len(y_)),y_,lw=5,zorder=3,color=cmap_(j))
+        ax1.text(1,y_[-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left')
+        for vl in vlines:
+            ax1.axvline(vl,color='k',ls='--',lw=1,zorder=0)
+        ax1.axvline(t/n_div,color='r',ls='-',lw=2,zorder=3)
+        ax1.tick_params(axis='x', which='both', top=True)
+        ax1.spines['right'].set_visible(False)
+        ax1.spines['left'].set_visible(False)
+        ax1.spines['top'].set_visible(False)
+        ax1.spines['bottom'].set_visible(False)
+        ax1.xaxis.set_label_position('top')
+        ax1.xaxis.tick_top()
+        ax1.yaxis.set_visible(False)
+        ax1.set_xticks(vlines)
+        ax1.set_xticklabels(vline_labels,fontsize=fontsize_label)
+        ax2.set_title('Time = %.02f [s]' % (t/n_div))
+        ax2.scatter(gene_dynamics_[name_i_][t],gene_dynamics_[name_j_][t],s=1,color="gray",zorder=1)
+        ax2.scatter(gene_dynamics_[name_i_][t][idx_DEG_i_],gene_dynamics_[name_j_][t][idx_DEG_i_],color=cmap_(i),zorder=2,s=20)
+        ax2.scatter(gene_dynamics_[name_i_][t][idx_DEG_j_],gene_dynamics_[name_j_][t][idx_DEG_j_],color=cmap_(j),zorder=2,s=20)
         texts = []
         for g in np.arange(adata.shape[1])[idx_DEG_ann_i_]:
-            tx_ = ax[0].text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
+            tx_ = ax2.text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],'_'+adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
             texts = np.append(texts,tx_)
         for g in np.arange(adata.shape[1])[idx_DEG_ann_j_]:
-            tx_ = ax[0].text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
+            tx_ = ax2.text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],'_'+adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
             texts = np.append(texts,tx_)
         if len(target_genes):
             for gene_ in target_genes:
                 idx_gene_ = adata.var.index == gene_
-                ax[0].scatter(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],s=20,color="red",zorder=2)
-                tx_ = ax[0].text(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],gene_,color="r",zorder=2,fontsize=fontsize_text)
+                ax2.scatter(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],s=20,color="red",zorder=2)
+                tx_ = ax2.text(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],'_'+gene_,color="r",zorder=2,fontsize=fontsize_text)
                 texts = np.append(texts,tx_)
         legend_i_ = ''
         for g in np.arange(adata.shape[1])[idx_DEG_leg_i_]: legend_i_ += '(%.02f, %.02f)  %s\n' % (gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g])
         legend_j_ = ''
         for g in np.arange(adata.shape[1])[idx_DEG_leg_j_]: legend_j_ += '(%.02f, %.02f)  %s\n' % (gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g])
-        if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'),ax=ax[0])
-        ax[0].text(0.9*(lim[1]-lim[0])+lim[0], 0.1*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_i_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(i), fontweight="bold",zorder=3)
-        ax[0].text(0.1*(lim[1]-lim[0])+lim[0], 0.9*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_j_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(j), fontweight="bold",zorder=3)
-        ax[0].fill_between(lim, lim-DEG_rate, lim+DEG_rate, facecolor='lightgray',  alpha=0.5,zorder=0)
-        ax[0].fill([-0.01*max_val_, DEG_min, DEG_min, -0.01*max_val_], [-0.01*max_val_, -0.01*max_val_, DEG_min, DEG_min], facecolor='lightgray', alpha=0.5,zorder=0)
-        ax[0].set_xlabel(target_clusters[i],fontsize=fontsize_label,color=cmap_(i), fontweight="bold")
-        ax[0].set_ylabel(target_clusters[j],fontsize=fontsize_label,color=cmap_(j), fontweight="bold")
-        ax[0].set_xlim(lim)
-        ax[0].set_ylim(lim)
-        ax[0].grid(ls='--')
-        ax[1].text(0.0,1,target_clusters[i], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3, fontweight="bold")
-        ax[1].text(0.0,0.97,legend_i_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3)
-        ax[1].text(0.5,1,target_clusters[j], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3, fontweight="bold")
-        ax[1].text(0.5,0.97,legend_j_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3)
-        ax[1].axis('off')
+        # if adjusttext: adjustText.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'),ax=ax2)
+        ax2.text(0.9*(lim[1]-lim[0])+lim[0], 0.1*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_i_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(i), fontweight="bold",zorder=3)
+        ax2.text(0.1*(lim[1]-lim[0])+lim[0], 0.9*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_j_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(j), fontweight="bold",zorder=3)
+        ax2.fill_between(lim, lim-DEG_rate, lim+DEG_rate, facecolor='lightgray',  alpha=0.5,zorder=0)
+        ax2.fill([-0.01*max_val_, DEG_min, DEG_min, -0.01*max_val_], [-0.01*max_val_, -0.01*max_val_, DEG_min, DEG_min], facecolor='lightgray', alpha=0.5,zorder=0)
+        ax2.set_xlabel(target_clusters[i],fontsize=fontsize_label,color=cmap_(i), fontweight="bold")
+        ax2.set_ylabel(target_clusters[j],fontsize=fontsize_label,color=cmap_(j), fontweight="bold")
+        ax2.set_xlim(lim)
+        ax2.set_ylim(lim)
+        ax2.grid(ls='--')
+        ax3.text(0.0,1,target_clusters[i], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3, fontweight="bold")
+        ax3.text(0.0,0.97,legend_i_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3)
+        ax3.text(0.5,1,target_clusters[j], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3, fontweight="bold")
+        ax3.text(0.5,0.97,legend_j_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3)
+        ax3.axis('off')
+        
     k = 0
     for i in range(len(target_clusters)):
         for j in range(i+1,len(target_clusters)):
             name_i_ = source_cluster+'_'+target_clusters[i]
             name_j_ = source_cluster+'_'+target_clusters[j]
-            fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
+            # fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
+            fig = plt.figure(figsize=(14,10),tight_layout=True)
+            grid = plt.GridSpec(10,14)
+            ax1 = fig.add_subplot(grid[0:2,0:12])
+            ax2 = fig.add_subplot(grid[2:10,0:8])
+            ax3 = fig.add_subplot(grid[2:10,8:14])
             max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
             lim = np.array([-0.01*max_val_,1.01*max_val_])
             k = k+1
             ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
             IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
             if save:
                 filename = '%s_%s_%s' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
                 if len(target_genes): filename += '_TG' + str(len(target_genes))
                 filename += '.gif'
                 print('\nSaving gif animation as %s' % filename)
                 ani.save(filename)
             plt.close()
 
-def bifurcation_diagram(
+def DEG_dynamics_clusters(
         adata,
         source_cluster,
         target_clusters,
         path_key = 'path',
         exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
+        bifurcation_diagram_key = 'bifurcation_diagram',
+        target_genes = [],
         n_div = 100,
         fontsize_label = 14,
-        adjusttext =False,
-        PC = 1,
+        fontsize_text = 12,
+        fontsize_nDEG = 18,
+        fontsize_legend = 10,
+        DEG_min = 1.0,
+        DEG_rate = 0.3,
+        save_type = 'gif',
+        max_num_annotations = 10,
+        max_num_legend = 25,
+        save = False,
+        save_dir = None,
+        save_filename = 'DEG_dynamics',
     ):
 
     if gene_dynamics_key not in adata.uns.keys():
-        gene_dynamics(adata, source_cluster,target_clusters,path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=100)
-
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
+    n_plot_ = int(len(target_clusters)*(len(target_clusters)-1)/2)
+    cmap_ = plt.get_cmap("tab10")
+    cmap20_ = plt.get_cmap("tab20")
+    gene_dynamics_ = adata.uns[gene_dynamics_key]
+    matplotlib.rcParams['animation.embed_limit'] = 2**128
     vlines = [0,0.2,0.4,0.6,0.8,1]
     vline_labels = np.append(np.append('Source (0)',np.array(vlines)[1:-1]),'Target (1)')
+    def update(t,name_i_,name_j_,max_val_,lim,i,j,k):
+        print('\rcomputing %s vs %s (%d/%d) %d/%d' % (target_clusters[i],target_clusters[j],k,n_plot_,t+1,n_div+1),end='')
+        idx_DEG_i_ = np.arange(adata.shape[1])[(gene_dynamics_[name_j_][t] < gene_dynamics_[name_i_][t] - DEG_rate) & (gene_dynamics_[name_i_][t] > DEG_min)]
+        idx_DEG_j_ = np.arange(adata.shape[1])[(gene_dynamics_[name_i_][t] < gene_dynamics_[name_j_][t] - DEG_rate) & (gene_dynamics_[name_j_][t] > DEG_min)]
+        idx_DEG_i_ = idx_DEG_i_[np.argsort(gene_dynamics_[name_i_][t][idx_DEG_i_]- DEG_rate - gene_dynamics_[name_j_][t][idx_DEG_i_])[::-1]]
+        idx_DEG_j_ = idx_DEG_j_[np.argsort(gene_dynamics_[name_j_][t][idx_DEG_j_]- DEG_rate - gene_dynamics_[name_i_][t][idx_DEG_j_])[::-1]]
+        if len(idx_DEG_i_) > max_num_annotations:
+            idx_DEG_ann_i_ = idx_DEG_i_[:max_num_annotations]
+        else:
+            idx_DEG_ann_i_  = idx_DEG_i_
+        if len(idx_DEG_j_) > max_num_annotations:
+            idx_DEG_ann_j_ = idx_DEG_j_[:max_num_annotations]
+        else:
+            idx_DEG_ann_j_  = idx_DEG_j_
+
+        if len(idx_DEG_i_) > max_num_legend:
+            idx_DEG_leg_i_ = idx_DEG_i_[:max_num_legend]
+        else:
+            idx_DEG_leg_i_  = idx_DEG_i_
+        if len(idx_DEG_j_) > max_num_legend:
+            idx_DEG_leg_j_ = idx_DEG_j_[:max_num_legend]
+        else:
+            idx_DEG_leg_j_  = idx_DEG_j_
+        ax1.cla()
+        ax2.cla()
+        ax3.cla()
+        name_i__ = source_cluster + '_' + target_clusters[0]
+        ax1.text(0,adata.uns[bifurcation_diagram_key][name_i_][0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
+        for i_ in range(len(target_clusters)):
+            name_i__ = source_cluster + '_' + target_clusters[i_]
+            if name_i__ not in [name_i_,name_j_]:
+                y_ = adata.uns[bifurcation_diagram_key][name_i__]
+                ax1.plot(np.linspace(0,1,len(y_)),y_,lw=3,zorder=2,alpha=0.3)
+                ax1.text(1,y_[-1],' '+target_clusters[i_],fontsize=fontsize_label,va='center',ha='left',alpha=0.3)
+        y_ = adata.uns[bifurcation_diagram_key][name_i_]
+        ax1.plot(np.linspace(0,1,len(y_)),y_,lw=5,zorder=3)
+        ax1.text(1,y_[-1],' '+target_clusters[i],fontsize=fontsize_label,va='center',ha='left')
+        y_ = adata.uns[bifurcation_diagram_key][name_j_]
+        ax1.plot(np.linspace(0,1,len(y_)),y_,lw=5,zorder=3)
+        ax1.text(1,y_[-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left')
+        for vl in vlines:
+            ax1.axvline(vl,color='k',ls='--',lw=1,zorder=0)
+        ax1.axvline(t/n_div,color='r',ls='-',lw=2,zorder=3)
+        ax1.tick_params(axis='x', which='both', top=True)
+        ax1.spines['right'].set_visible(False)
+        ax1.spines['left'].set_visible(False)
+        ax1.spines['top'].set_visible(False)
+        ax1.spines['bottom'].set_visible(False)
+        ax1.xaxis.set_label_position('top')
+        ax1.xaxis.tick_top()
+        ax1.yaxis.set_visible(False)
+        ax1.set_xticks(vlines)
+        ax1.set_xticklabels(vline_labels,fontsize=fontsize_label)
+        ax2.set_title('Time = %.02f [s]' % (t/n_div))
+        ax2.scatter(gene_dynamics_[name_i_][t],gene_dynamics_[name_j_][t],s=1,color="gray",zorder=1)
+        for c_ in range(n_clusters):
+            idx_ = (adata.var['clusters_'+name_i_] == c_) & (gene_dynamics_[name_i_][t] > gene_dynamics_[name_j_][t])
+            ax2.scatter(gene_dynamics_[name_i_][t][idx_],gene_dynamics_[name_j_][t][idx_],color=cmap20_(c_),zorder=2,s=20,label=str(c_+1),marker='o')
+            idx_ = (adata.var['clusters_'+name_j_] == c_) & (gene_dynamics_[name_i_][t] < gene_dynamics_[name_j_][t])
+            ax2.scatter(gene_dynamics_[name_i_][t][idx_],gene_dynamics_[name_j_][t][idx_],color=cmap20_(c_),zorder=2,s=20,marker='o')
+        ax2.legend(loc='lower left', bbox_to_anchor=(1.05, 0.0), ncol=5,  title = "Clusters", columnspacing=0.5)
+        texts = []
+        for g in np.arange(adata.shape[1])[idx_DEG_ann_i_]:
+            tx_ = ax2.text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],'_'+adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
+            texts = np.append(texts,tx_)
+        for g in np.arange(adata.shape[1])[idx_DEG_ann_j_]:
+            tx_ = ax2.text(gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],'_'+adata.var.index[g],color="k",zorder=2,fontsize=fontsize_text)
+            texts = np.append(texts,tx_)
+        if len(target_genes):
+            for gene_ in target_genes:
+                idx_gene_ = adata.var.index == gene_
+                ax2.scatter(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],s=20,color="red",zorder=2)
+                tx_ = ax2.text(gene_dynamics_[name_i_][t][idx_gene_],gene_dynamics_[name_j_][t][idx_gene_],'_'+gene_,color="r",zorder=2,fontsize=fontsize_text)
+                texts = np.append(texts,tx_)
+        legend_i_ = ''
+        for g in np.arange(adata.shape[1])[idx_DEG_leg_i_]: legend_i_ += '(%.02f, %.02f)  %s\n' % (gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g])
+        legend_j_ = ''
+        for g in np.arange(adata.shape[1])[idx_DEG_leg_j_]: legend_j_ += '(%.02f, %.02f)  %s\n' % (gene_dynamics_[name_i_][t][g],gene_dynamics_[name_j_][t][g],adata.var.index[g])
+        ax2.text(0.9*(lim[1]-lim[0])+lim[0], 0.1*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_i_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(i), fontweight="bold",zorder=3)
+        ax2.text(0.1*(lim[1]-lim[0])+lim[0], 0.9*(lim[1]-lim[0])+lim[0], str(len(idx_DEG_j_)) , ha='center', va='center', fontsize=fontsize_nDEG,color=cmap_(j), fontweight="bold",zorder=3)
+        ax2.fill_between(lim, lim-DEG_rate, lim+DEG_rate, facecolor='lightgray',  alpha=0.5,zorder=0)
+        ax2.fill([-0.01*max_val_, DEG_min, DEG_min, -0.01*max_val_], [-0.01*max_val_, -0.01*max_val_, DEG_min, DEG_min], facecolor='lightgray', alpha=0.5,zorder=0)
+        ax2.set_xlabel(target_clusters[i],fontsize=fontsize_label,color=cmap_(i), fontweight="bold")
+        ax2.set_ylabel(target_clusters[j],fontsize=fontsize_label,color=cmap_(j), fontweight="bold")
+        ax2.set_xlim(lim)
+        ax2.set_ylim(lim)
+        ax2.grid(ls='--')
+        ax3.text(0.0,1,target_clusters[i], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3, fontweight="bold")
+        ax3.text(0.0,0.97,legend_i_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(i),zorder=3)
+        ax3.text(0.5,1,target_clusters[j], ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3, fontweight="bold")
+        ax3.text(0.5,0.97,legend_j_, ha='left', va='top', fontsize=fontsize_legend,color=cmap_(j),zorder=3)
+        ax3.axis('off')
+        
+    k = 0
+    for i in range(len(target_clusters)):
+        for j in range(i+1,len(target_clusters)):
+            name_i_ = source_cluster+'_'+target_clusters[i]
+            name_j_ = source_cluster+'_'+target_clusters[j]
+            # fig,ax = plt.subplots(1,2,figsize=(14,8),gridspec_kw={'width_ratios': [4,3]},tight_layout=True)
+            fig = plt.figure(figsize=(14,10),tight_layout=True)
+            grid = plt.GridSpec(10,14)
+            ax1 = fig.add_subplot(grid[0:2,0:12])
+            ax2 = fig.add_subplot(grid[2:10,0:8])
+            ax3 = fig.add_subplot(grid[2:10,8:14])
+            max_val_ = max(np.max(gene_dynamics_[name_i_]),np.max(gene_dynamics_[name_j_]))
+            lim = np.array([-0.01*max_val_,1.01*max_val_])
+            k = k+1
+            n_clusters = max(np.max(adata.var['clusters_'+name_i_]),np.max(adata.var['clusters_'+name_j_]))+1
+            ani = anm.FuncAnimation(fig,update,interval=200,fargs=(name_i_,name_j_,max_val_,lim,i,j,k,),frames=n_div+1)
+            IPython.display.display(IPython.display.HTML(ani.to_jshtml()))
+            if save:
+                filename = '%s_%s_%s' % (save_filename,target_clusters[i],target_clusters[j]) if save_dir == None else '%s/%s_%s_%s' % (save_dir,save_filename,target_clusters[i],target_clusters[j])
+                if len(target_genes): filename += '_TG' + str(len(target_genes))
+                filename += '.gif'
+                print('\nSaving gif animation as %s' % filename)
+                ani.save(filename)
+            plt.close()
+
+def culc_bifurcation_diagram(
+        adata,
+        source_cluster,
+        target_clusters,
+        path_key = 'path',
+        exp_key = None,
+        gene_dynamics_key = 'gene_dynamics',
+        bifurcation_diagram_key = 'bifurcation_diagram',
+        n_div = 100,
+        PC = 1,
+    ):
+
+    if gene_dynamics_key not in adata.uns.keys():
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
 
     name_i_ = source_cluster + '_' + target_clusters[0]
     samples_ = np.empty([len(target_clusters),adata.uns['gene_dynamics'][name_i_].shape[0],adata.uns['gene_dynamics'][name_i_].shape[1]],dtype=float)
     for i in range(len(target_clusters)):
         name_i_ = source_cluster + '_' + target_clusters[i]
         samples_[i] = adata.uns['gene_dynamics'][name_i_]
-    # samples_pca_ = sklearn.decomposition.PCA(n_components=2).fit_transform(np.concatenate(samples_))
     pca_ = sklearn.decomposition.PCA().fit(samples_[:,-1])
     samples_pca_ = pca_.transform(np.concatenate(samples_))
-    # for i in range(n_div):
-    #     idx_ = np.arange(i,len(target_clusters)*n_div,n_div)
-    #     samples_pca_[idx_] = samples_pca_[idx_] - samples_pca_[i]
 
-    fig,ax = plt.subplots(figsize=(12,4))
-    ax.text(0,samples_pca_[0,0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
+    bd_ = {}
+    for i in range(len(target_clusters)):
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        bd_[name_i_] = samples_pca_[i*(n_div+1):(i+1)*(n_div+1),PC-1]
+    
+    adata.uns[bifurcation_diagram_key] = bd_
+
+def bifurcation_diagram(
+        adata,
+        source_cluster,
+        target_clusters,
+        path_key = 'path',
+        exp_key = None,
+        gene_dynamics_key = 'gene_dynamics',
+        bifurcation_diagram_key = 'bifurcation_diagram',
+        n_div = 100,
+        fontsize_label = 14,
+        adjusttext =False,
+        PC = 1,
+    ):
+
+    if gene_dynamics_key not in adata.uns.keys():
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
+    
+    if bifurcation_diagram_key not in adata.uns.keys():
+        culc_bifurcation_diagram(
+        adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, 
+            bifurcation_diagram_key=bifurcation_diagram_key, n_div=n_div, PC=PC)
+
+    vlines = [0,0.2,0.4,0.6,0.8,1]
+    vline_labels = np.append(np.append('Source (0)',np.array(vlines)[1:-1]),'Target (1)')
+
+    fig,ax = plt.subplots(figsize=(12,3))
+    name_i_ = source_cluster + '_' + target_clusters[0]
+    ax.text(0,adata.uns[bifurcation_diagram_key][name_i_][0],source_cluster+' ',fontsize=fontsize_label,va='center',ha='right')
     texts = []
-    for j in range(len(target_clusters)):
-        y_ = samples_pca_[j*(n_div+1):(j+1)*(n_div+1),PC-1]
+    for i in range(len(target_clusters)):
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        y_ = adata.uns[bifurcation_diagram_key][name_i_]
         ax.plot(np.linspace(0,1,n_div+1),y_,lw=5,zorder=2)
-        texts = np.append(texts,ax.text(1,y_[-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left'))
-    if adjusttext: adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'))
+        texts = np.append(texts,ax.text(1,y_[-1],' '+target_clusters[i],fontsize=fontsize_label,va='center',ha='left'))
+    if adjusttext: adjustText.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='k'))
     for vl in vlines:
         ax.axvline(vl,color='k',ls='--',lw=1,zorder=0)
     ax.tick_params(axis='x', which='both', top=True)
     ax.spines['right'].set_visible(False)
     ax.spines['left'].set_visible(False)
     ax.spines['top'].set_visible(False)
     ax.spines['bottom'].set_visible(False)
     ax.xaxis.set_label_position('top')
     ax.xaxis.tick_top()
     ax.yaxis.set_visible(False)
     ax.set_xticks(vlines)
     ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
 
-def gene_atlas(
+def culc_gene_atlas(
         adata,
         source_cluster,
         target_clusters,
-        target_genes = [],
+        path_key = 'path',
+        exp_key = None,
         gene_dynamics_key = 'gene_dynamics',
+        gene_atlas_key = 'gene_atlas',
         n_div = 100,
         n_neighbors = 15,
         min_dist = 0.3,
         seed = 0,
         threshold_min = 1,
         n_clusters = 20,
         n_components = 2,
-        pt_size = 5,
     ):
-    gene_dynamics_ = adata.uns[gene_dynamics_key]
 
+    if gene_dynamics_key not in adata.uns.keys():
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
+
+    gene_dynamics_ = adata.uns[gene_dynamics_key]
     gene_dynamics_all_ = np.empty([0,n_div+1],dtype=float)
+    gene_dynamics_all_norm_ = np.empty([0,n_div+1],dtype=float)
     idx_gene_dynamics_ = [0]
     for i in range(len(target_clusters)):
         name_i_ = source_cluster + '_' + target_clusters[i]
         max_ = np.max(gene_dynamics_[name_i_],axis=0)
         idx_ = max_ > threshold_min
-        adata.var[name_i_+'_'+'expressed'] = idx_
+        adata.var['expressed_'+name_i_] = idx_
         idx_gene_dynamics_ = np.append(idx_gene_dynamics_,idx_gene_dynamics_[i]+sum(idx_))
-        gene_dynamics_all_ = np.vstack((gene_dynamics_all_,(gene_dynamics_[name_i_][:,idx_]/max_[idx_]).T))
+        gene_dynamics_all_ = np.vstack((gene_dynamics_all_,gene_dynamics_[name_i_][:,idx_].T))
+        gene_dynamics_all_norm_ = np.vstack((gene_dynamics_all_norm_,(gene_dynamics_[name_i_][:,idx_]/max_[idx_]).T))
 
 
     umap_ = umap.UMAP(n_components=n_components,random_state=seed,n_neighbors=n_neighbors,min_dist=min_dist)
     gene_dynamics_all_umap_ = umap_.fit_transform(gene_dynamics_all_)
 
     data_ = gene_dynamics_all_umap_
     gm = sklearn.mixture.GaussianMixture(n_components=n_clusters,random_state=0).fit(data_)
     clusters_tmp_ = gm.predict(data_)
-    pc1_ = sklearn.decomposition.PCA(n_components=1).fit_transform(data_)
+    pc1_ = sklearn.decomposition.PCA(n_components=1).fit_transform(data_)[:,0]
+    pc1_ = np.sign(np.dot(pc1_,gene_dynamics_all_umap_[:,0]))*pc1_
     pc1_order_ = np.argsort([np.mean(pc1_[clusters_tmp_==i]) for i in range(n_clusters)])
     dict_sort_ = dict(zip(pc1_order_,np.unique(clusters_tmp_)))
     clusters_ = np.array([dict_sort_[c] for c in clusters_tmp_])
+
+    texts_ = []
+    index_ = []
+    s_,e_ = 0,0
+    for i in range(len(target_clusters)):
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        idx_ = adata.var['expressed_'+name_i_]
+        gene_list_ = adata.var.index[idx_].values
+        e_ += sum(idx_)
+        txt_ = gene_list_ + '<br>' + target_clusters[i]+'<br>cluster '+ np.array(clusters_[s_:e_]+1,dtype=str)#+ '<br><img src="'+image_+'" width="200">'
+        texts_= np.append(texts_,txt_)
+        index_ = np.append(index_,source_cluster + '_' + target_clusters[i] + '_' + gene_list_)
+        adata.var['clusters_'+name_i_] = -np.ones(adata.shape[1],dtype=int)
+        adata.var['clusters_'+name_i_][idx_] = adata.uns['gene_atlas']['clusters'][s_:e_]
+        s_ += sum(idx_)
+
+    adata.uns[gene_atlas_key] = {
+        'index':index_,
+        'texts':texts_,
+        'dynamics':gene_dynamics_all_,
+        'dynamics_norm':gene_dynamics_all_norm_,
+        'gene_atlas':gene_dynamics_all_umap_,
+        'clusters': clusters_,
+    }
+
+def gene_atlas(
+        adata,
+        source_cluster,
+        target_clusters,
+        target_genes = [],
+        gene_dynamics_key = 'gene_dynamics',
+        gene_atlas_key = 'gene_atlas',
+        normalization = False,
+        n_div = 100,
+        n_neighbors = 15,
+        min_dist = 0.3,
+        seed = 0,
+        threshold_min = 1,
+        n_clusters = 20,
+        n_components = 2,
+        pt_size = 5,
+        save = False,
+        save_dir = None,
+        save_filename = 'gene_atlas',
+    ):
+    if gene_atlas_key not in adata.uns.keys():
+        culc_gene_atlas(adata,source_cluster,target_clusters,gene_dynamics_key = gene_dynamics_key, gene_atlas_key=gene_atlas_key,
+            n_div = n_div,n_neighbors = n_neighbors,min_dist = min_dist,seed = seed,threshold_min=threshold_min, 
+            n_clusters = n_clusters,n_components = n_components,
+        )
+    elif n_clusters != len(np.unique(adata.uns[gene_atlas_key]['clusters'])):
+        culc_gene_atlas(adata,source_cluster,target_clusters,gene_dynamics_key = gene_dynamics_key, gene_atlas_key = gene_atlas_key,
+            n_div=n_div,n_neighbors = n_neighbors,min_dist = min_dist,seed = seed,threshold_min=threshold_min, 
+            n_clusters = n_clusters,n_components = n_components,
+        )
+    
+    texts_ = adata.uns[gene_atlas_key]['texts']
+    if normalization:
+        gene_dynamics_all_ = adata.uns[gene_atlas_key]['dynamics_norm']
+    else:
+        gene_dynamics_all_ = adata.uns[gene_atlas_key]['dynamics']
+    gene_dynamics_all_umap_ = adata.uns[gene_atlas_key]['gene_atlas']
+    clusters_ = adata.uns[gene_atlas_key]['clusters']
     cluster_set_ = np.unique(clusters_)
 
     x_data = gene_dynamics_all_umap_[:,0]
     y_data = gene_dynamics_all_umap_[:,1]
 
-    color_clusters_ = np.array(['rgb'+str(tuple(int(i *255) for i in plt.get_cmap("tab20")(c))) for c in clusters_])
+    color_clusters_ = np.array(['rgb'+str(tuple(int(i*255) for i in plt.get_cmap("tab20")(c%20))) for c in clusters_])
     color_celltypes_ = np.empty(len(gene_dynamics_all_),dtype=object)
 
-    texts_ = []
-    s_,e_ = 0,0
+    
     annotations = [
         go.layout.Annotation(
             xref='paper',
             yref='paper',
             x=0.01,
             y=0.99,
             text='<b>Gene Atlas<b>',
             font=dict(size=18,color='white'),
             showarrow=False,
         )
     ]
+    s_,e_ = 0,0
     for i in range(len(target_clusters)):
-        idx_ = adata.var[source_cluster + '_' + target_clusters[i]+'_'+'expressed']
-        gene_list_ = adata.var.index[idx_].values
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        idx_ = adata.var['expressed_'+name_i_]
         e_ += sum(idx_)
-        color_celltypes_[s_:e_] = 'rgba'+str(plt.get_cmap("tab10")(i))
-        txt_ = gene_list_ + '<br>' + target_clusters[i]+'<br>cluster '+ np.array(clusters_[s_:e_]+1,dtype=str)#+ '<br><img src="'+image_+'" width="200">'
-        texts_= np.append(texts_,txt_)
+        gene_list_ = adata.var.index[idx_].values
+        color_celltypes_[s_:e_] = 'rgba'+str(plt.get_cmap("tab10")(i%10))
         for gene in target_genes:
             if gene in gene_list_:
                 x_pos = x_data[np.arange(sum(idx_))[gene_list_==gene][0]+s_]
                 y_pos = y_data[np.arange(sum(idx_))[gene_list_==gene][0]+s_]
                 annotations.append(
                     go.layout.Annotation(
                         x=x_pos,
@@ -1881,29 +2124,30 @@
             go.Scatter(
                 x=x_data[idx_],
                 y=y_data[idx_],
                 text = texts_[idx_],
                 mode='markers',
                 name='cluster '+str(c+1),
                 marker=dict(
-                    color='rgb'+str(tuple(int(i*255) for i in plt.get_cmap("tab20")(c))),
+                    color='rgb'+str(tuple(int(i*255) for i in plt.get_cmap("tab20")(c%20))),
                     size=pt_size,
                     opacity=1,
                     line=dict(
                         color='white',
                         width=0.5,
                     ),
                 ),
             )
         )
 
     s_,e_ = 0,0
     data_celltypes_ = []
     for i in range(len(target_clusters)):
-        idx_ = adata.var[source_cluster + '_' + target_clusters[i]+'_'+'expressed']
+        name_i_ = source_cluster + '_' + target_clusters[i]
+        idx_ = adata.var['expressed_'+name_i_]
         gene_list_ = adata.var.index[idx_].values
         e_ += sum(idx_)
         data_celltypes_.append(
             go.Scatter(
                 x=x_data[s_:e_],
                 y=y_data[s_:e_],
                 text = texts_[s_:e_],
@@ -1949,8 +2193,145 @@
         annotations=annotations
     )
 
     fig = go.Figure(data=data_clusters_, layout=layout)
     pio.show(fig)
 
     fig = go.Figure(data=data_celltypes_, layout=layout)
-    pio.show(fig)
+    pio.show(fig)
+
+
+def gene_dynamics_clusters(
+        adata,
+        source_cluster,
+        target_clusters,
+        gene_dynamics_key = 'gene_dynamics',
+        gene_atlas_key = 'gene_atlas',
+        normalization = False,
+        n_div = 100,
+        n_neighbors = 15,
+        min_dist = 0.3,
+        seed = 0,
+        threshold_min = 1,
+        n_clusters = 20,
+        n_components = 2,
+    ):
+    
+    if gene_atlas_key not in adata.uns.keys():
+        culc_gene_atlas(adata,source_cluster,target_clusters,gene_dynamics_key = gene_dynamics_key,ene_atlas_key = gene_atlas_key,
+            n_div = n_div,n_neighbors = n_neighbors,min_dist = min_dist,seed = seed,threshold_min=threshold_min, 
+            n_clusters = n_clusters,n_components = n_components,
+        )
+    
+    if normalization:
+        gene_dynamics_all_ = adata.uns[gene_atlas_key]['dynamics_norm']
+        ylabel_ = 'normalized gene expression'
+    else:
+        gene_dynamics_all_ = adata.uns[gene_atlas_key]['dynamics']
+        ylabel_ = 'gene expression'
+    
+    n_clusters = len(np.unique(adata.uns[gene_atlas_key]['clusters']))
+    for i in range(n_clusters):
+        x_ = np.linspace(0,1,n_div+1)
+        y_ = gene_dynamics_all_[adata.uns[gene_atlas_key]['clusters']==i].T
+
+        data_ = []
+        for j in range(y_.shape[1]):
+            data_.append(
+                go.Scatter(
+                    x=x_,
+                    y=y_[:,j],
+                    mode = "lines",
+                    text = adata.uns[gene_atlas_key]['texts'][adata.uns[gene_atlas_key]['clusters']==i][j],
+                    name = '',
+                    # hoverinfo='skip',
+                    showlegend=False,
+                    opacity=0.8,
+                    line=dict(
+                        width=1,
+                    ),
+                )
+            )
+        layout = go.Layout(
+            width=1200,
+            height=400,
+            plot_bgcolor='rgba(1,1,1,1)',
+            paper_bgcolor='rgba(0,0,0,0)',
+            xaxis=dict(
+                range=[0, 1],
+                # showgrid=False,
+                title = 'Time',
+                gridcolor='gray',
+                gridwidth=1,
+                griddash='dot',
+                zeroline=False,
+                # showticklabels=False,
+                layer='below traces',
+            ),
+            yaxis=dict(
+                # range=[0, 1],
+                # showgrid=False,
+                title = '<b>Cluster %s</b><br>%s' % (str(i+1),ylabel_),
+                gridcolor='gray',
+                gridwidth=1,
+                griddash='dot',
+                zeroline=False,
+                # showticklabels=False,
+                layer='below traces',
+            ),
+            # annotations=annotations
+        )
+
+        fig = go.Figure(data=data_, layout=layout)
+        pio.show(fig)
+
+
+def find_DEG_time(
+        adata,
+        source_cluster,
+        target_clusters,
+        time,
+        n_genes = 10,
+        threshold_min = 1,
+        path_key = 'path',
+        exp_key = None,
+        gene_dynamics_key = 'gene_dynamics',
+        n_div = 100,
+        fontsize_label = 10,
+    ):
+
+    if gene_dynamics_key not in adata.uns.keys():
+        culc_gene_dynamics(adata, source_cluster, target_clusters, path_key=path_key, exp_key=exp_key, gene_dynamics_key=gene_dynamics_key, n_div=n_div)
+
+    idx_t_n_ = np.arange(n_div+1)[(np.linspace(0,1,n_div+1) <= time)]
+    idx_t_p_ = np.arange(n_div+1)[(np.linspace(0,1,n_div+1) >= time)]
+
+    i,j = 0,1
+    name_i_ = source_cluster + '_' + target_clusters[i]
+    name_j_ = source_cluster + '_' + target_clusters[j]
+    gene_dynamics_ = adata.uns[gene_dynamics_key]
+
+    max_i_,max_j_ = np.max(gene_dynamics_[name_i_],axis=0),np.max(gene_dynamics_[name_j_],axis=0)
+    idx_max_ = (max_i_ > threshold_min) & (max_j_ > threshold_min)
+
+    vol_p_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_p_]-gene_dynamics_[name_j_][idx_t_p_]),axis=0)
+    vol_n_ = np.sum(np.abs(gene_dynamics_[name_i_][idx_t_n_]-gene_dynamics_[name_j_][idx_t_n_]),axis=0)
+    diff_ = vol_p_/(1e-5+vol_n_)
+    diff_order_ = np.argsort(diff_[idx_max_])[::-1]
+
+    cmap_ = plt.get_cmap("tab10")
+    vlines = [0,0.2,0.4,0.6,0.8,1]
+    vline_labels = np.append(np.append('Source (0)\n%s' % source_cluster,np.array(vlines)[1:-1]),'Target (1)')
+    for i_ in range(n_genes):
+        fig,ax = plt.subplots(1,1,figsize=(8,2),tight_layout=True)
+        ax.plot(np.linspace(0,1,n_div+1),gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]],color=cmap_(i),zorder=2)
+        ax.text(1,gene_dynamics_[name_i_][:,idx_max_][:,diff_order_[i_]][-1],' '+target_clusters[i],fontsize=fontsize_label,va='center',ha='left')
+        ax.plot(np.linspace(0,1,n_div+1),gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]],color=cmap_(j),zorder=2)
+        ax.text(1,gene_dynamics_[name_j_][:,idx_max_][:,diff_order_[i_]][-1],' '+target_clusters[j],fontsize=fontsize_label,va='center',ha='left')
+        ax.set_title(adata.var.index[idx_max_][diff_order_[i_]])
+        ax.axvline(time,color='r',zorder=1)
+        ax.text(time,0.95,str(time)+' ',color='r',zorder=1,va='top',ha='right',transform=ax.transAxes)
+        ax.set_xlim([0,1])
+        ax.set_xticks(vlines)
+        ax.set_xticklabels(vline_labels,fontsize=fontsize_label)
+        ax.spines['top'].set_visible(False)
+        ax.spines['right'].set_visible(False)
```

## Comparing `cellmap-1.0.1.dev202304290429.dist-info/METADATA` & `cellmap-1.0.1.dev202304300542.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304290429
+Version: 1.0.1.dev202304300542
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

