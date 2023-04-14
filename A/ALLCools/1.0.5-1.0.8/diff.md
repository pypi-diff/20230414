# Comparing `tmp/ALLCools-1.0.5.tar.gz` & `tmp/ALLCools-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALLCools-1.0.5.tar", last modified: Sat Aug 27 18:16:28 2022, max compression
+gzip compressed data, was "ALLCools-1.0.8.tar", last modified: Fri Sep 23 06:50:55 2022, max compression
```

## Comparing `ALLCools-1.0.5.tar` & `ALLCools-1.0.8.tar`

### file list

```diff
@@ -1,100 +1,104 @@
--rw-r--r--   0        0        0      154 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/__init__.py
--rw-r--r--   0        0        0    27909 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/__main__.py
--rw-r--r--   0        0        0     8723 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_allc_to_bigwig.py
--rw-r--r--   0        0        0    14129 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_allc_to_region_count.py
--rw-r--r--   0        0        0    18951 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_bam_to_allc.py
--rw-r--r--   0        0        0     9228 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_doc.py
--rw-r--r--   0        0        0    14869 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_extract_allc.py
--rw-r--r--   0        0        0    19061 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_merge_allc.py
--rw-r--r--   0        0        0    15305 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/_open.py
--rw-r--r--   0        0        0       32 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/abc/__init__.py
--rw-r--r--   0        0        0    13031 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/abc/abc_score.py
--rw-r--r--   0        0        0      624 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/api.py
--rw-r--r--   0        0        0     5835 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/ClusterMerging.py
--rw-r--r--   0        0        0    29849 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/ConsensusClustering.py
--rw-r--r--   0        0        0      638 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/__init__.py
--rw-r--r--   0        0        0     6057 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/art_of_tsne.py
--rw-r--r--   0        0        0    12658 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/balanced_pca.py
--rw-r--r--   0        0        0      910 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/chromatin_conformation.py
--rw-r--r--   0        0        0    17669 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/dmg.py
--rw-r--r--   0        0        0       86 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/doublets/__init__.py
--rw-r--r--   0        0        0     6700 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/doublets/coverage_doublets.py
--rw-r--r--   0        0        0    10214 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/doublets/scrublet.py
--rw-r--r--   0        0        0      113 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/feature_selection/__init__.py
--rw-r--r--   0        0        0    10574 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/feature_selection/feature_enrichment.py
--rw-r--r--   0        0        0     3393 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/feature_selection/gene_panel_design.py
--rw-r--r--   0        0        0     7821 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/incremental_pca.py
--rw-r--r--   0        0        0     5944 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/lsi.py
--rw-r--r--   0        0        0     3696 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/mcad.py
--rw-r--r--   0        0        0     5578 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/pvclust.py
--rw-r--r--   0        0        0      643 2022-08-27 18:15:56.726531 ALLCools-1.0.5/ALLCools/clustering/rutilities.py
--rw-r--r--   0        0        0       66 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/__init__.py
--rw-r--r--   0        0        0      114 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/atac.py
--rw-r--r--   0        0        0    23016 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/base_ds.py
--rw-r--r--   0        0        0    14453 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/dataset.py
--rw-r--r--   0        0        0    10291 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/h5ad.py
--rw-r--r--   0        0        0     5839 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/mcad.py
--rw-r--r--   0        0        0    18533 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/mcds.py
--rw-r--r--   0        0        0     4562 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/snap.py
--rw-r--r--   0        0        0     1873 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/count_matrix/zarr.py
--rw-r--r--   0        0        0       41 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dataset/__init__.py
--rw-r--r--   0        0        0      168 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dataset/dataset.yaml
--rw-r--r--   0        0        0     2041 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dataset/directory_structure.py
--rw-r--r--   0        0        0      181 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dataset/entry_point.py
--rw-r--r--   0        0        0      133 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dmr/__init__.py
--rw-r--r--   0        0        0     8795 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dmr/call_dmr.py
--rw-r--r--   0        0        0     7476 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dmr/call_dms.py
--rw-r--r--   0        0        0     2461 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dmr/parse_methylpy.py
--rw-r--r--   0        0        0     2337 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/dmr/rms_test.py
--rw-r--r--   0        0        0     5639 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/gtf/Gtf.py
--rw-r--r--   0        0        0       80 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/gtf/__init__.py
--rw-r--r--   0        0        0     1164 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/gtf/utilities.py
--rw-r--r--   0        0        0      195 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/integration/__init__.py
--rw-r--r--   0        0        0    12276 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/integration/cca.py
--rw-r--r--   0        0        0     6554 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/integration/confusion.py
--rw-r--r--   0        0        0     9912 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/integration/metric.py
--rw-r--r--   0        0        0    31922 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/integration/seurat_class.py
--rw-r--r--   0        0        0       83 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/mcds/__init__.py
--rw-r--r--   0        0        0    11906 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/mcds/base_ds.py
--rw-r--r--   0        0        0    11587 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/mcds/correlation.py
--rw-r--r--   0        0        0    57597 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/mcds/mcds.py
--rw-r--r--   0        0        0    39343 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/mcds/region_ds.py
--rw-r--r--   0        0        0    18370 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/mcds/utilities.py
--rw-r--r--   0        0        0       75 2022-08-27 18:15:56.730532 ALLCools-1.0.5/ALLCools/motif/__init__.py
--rw-r--r--   0        0        0  1614001 2022-08-27 18:15:56.738532 ALLCools-1.0.5/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme
--rw-r--r--   0        0        0   172054 2022-08-27 18:15:56.738532 ALLCools-1.0.5/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv
--rw-r--r--   0        0        0    77918 2022-08-27 18:15:56.738532 ALLCools-1.0.5/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv
--rw-r--r--   0        0        0        0 2022-08-27 18:15:56.738532 ALLCools-1.0.5/ALLCools/motif/default_motif_set/__init__.py
--rw-r--r--   0        0        0     8709 2022-08-27 18:15:56.738532 ALLCools-1.0.5/ALLCools/motif/motifs.py
--rw-r--r--   0        0        0     4260 2022-08-27 18:15:56.738532 ALLCools-1.0.5/ALLCools/motif/parse_meme.py
--rw-r--r--   0        0        0     4864 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/motif/snakemake.py
--rw-r--r--   0        0        0      306 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/__init__.py
--rw-r--r--   0        0        0     9026 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/categorical_scatter.py
--rw-r--r--   0        0        0     4512 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/color.py
--rw-r--r--   0        0        0     7704 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/continuous_scatter.py
--rw-r--r--   0        0        0     1429 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/contour.py
--rw-r--r--   0        0        0     2645 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/decomposition.py
--rw-r--r--   0        0        0     7940 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/dendro.py
--rw-r--r--   0        0        0    12573 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/genome_track/GtfTrack.py
--rw-r--r--   0        0        0    10256 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py
--rw-r--r--   0        0        0       55 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/genome_track/__init__.py
--rw-r--r--   0        0        0    37598 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/genome_track/_pygenometrack.py
--rw-r--r--   0        0        0     1026 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/interactive_scatter.py
--rw-r--r--   0        0        0     7382 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/qc_plots.py
--rw-r--r--   0        0        0      833 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/size.py
--rw-r--r--   0        0        0     7469 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/sunburst.py
--rw-r--r--   0        0        0     2083 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/text_anno_scatter.py
--rw-r--r--   0        0        0     7410 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/plot/utilities.py
--rw-r--r--   0        0        0      166 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/pseudo_cell/__init__.py
--rw-r--r--   0        0        0     6211 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/pseudo_cell/pseudo_cell_kmeans.py
--rw-r--r--   0        0        0    10950 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/pseudo_cell/pseudo_cell_knn.py
--rw-r--r--   0        0        0       29 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/reptile/__init__.py
--rw-r--r--   0        0        0    31804 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/reptile/reptile.py
--rw-r--r--   0        0        0        0 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/schema/__init__.py
--rw-r--r--   0        0        0      894 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/schema/mcds_schema.py
--rw-r--r--   0        0        0    11318 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/table_to_allc.py
--rw-r--r--   0        0        0    18046 2022-08-27 18:15:56.742532 ALLCools-1.0.5/ALLCools/utilities.py
--rw-r--r--   0        0        0     1073 2022-08-27 18:15:56.742532 ALLCools-1.0.5/LICENSE
--rw-r--r--   0        0        0      339 2022-08-27 18:15:56.742532 ALLCools-1.0.5/README.md
--rw-r--r--   0        0        0     2018 2022-08-27 18:15:57.038536 ALLCools-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2127 1970-01-01 00:00:00.000000 ALLCools-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/__init__.py
+-rw-r--r--   0        0        0    27909 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/__main__.py
+-rw-r--r--   0        0        0     8723 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_allc_to_bigwig.py
+-rw-r--r--   0        0        0    14129 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_allc_to_region_count.py
+-rw-r--r--   0        0        0    18951 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_bam_to_allc.py
+-rw-r--r--   0        0        0     9228 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_doc.py
+-rw-r--r--   0        0        0    14869 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_extract_allc.py
+-rw-r--r--   0        0        0    19061 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_merge_allc.py
+-rw-r--r--   0        0        0    15305 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/_open.py
+-rw-r--r--   0        0        0       32 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/abc/__init__.py
+-rw-r--r--   0        0        0    13031 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/abc/abc_score.py
+-rw-r--r--   0        0        0      624 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/api.py
+-rw-r--r--   0        0        0     5835 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/ClusterMerging.py
+-rw-r--r--   0        0        0    29849 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/ConsensusClustering.py
+-rw-r--r--   0        0        0      638 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/__init__.py
+-rw-r--r--   0        0        0     6057 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/art_of_tsne.py
+-rw-r--r--   0        0        0    12785 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/balanced_pca.py
+-rw-r--r--   0        0        0      910 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/chromatin_conformation.py
+-rw-r--r--   0        0        0    17669 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/dmg.py
+-rw-r--r--   0        0        0       86 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/doublets/__init__.py
+-rw-r--r--   0        0        0     6700 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/doublets/coverage_doublets.py
+-rw-r--r--   0        0        0    10214 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/doublets/scrublet.py
+-rw-r--r--   0        0        0      113 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/feature_selection/__init__.py
+-rw-r--r--   0        0        0    10574 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/feature_selection/feature_enrichment.py
+-rw-r--r--   0        0        0     3393 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/feature_selection/gene_panel_design.py
+-rw-r--r--   0        0        0     7821 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/incremental_pca.py
+-rw-r--r--   0        0        0     5944 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/lsi.py
+-rw-r--r--   0        0        0     3696 2022-09-23 06:50:34.755006 ALLCools-1.0.8/ALLCools/clustering/mcad.py
+-rw-r--r--   0        0        0     5578 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/clustering/pvclust.py
+-rw-r--r--   0        0        0      643 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/clustering/rutilities.py
+-rw-r--r--   0        0        0       66 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/__init__.py
+-rw-r--r--   0        0        0      114 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/atac.py
+-rw-r--r--   0        0        0    23961 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/base_ds.py
+-rw-r--r--   0        0        0    14453 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/dataset.py
+-rw-r--r--   0        0        0    10291 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/h5ad.py
+-rw-r--r--   0        0        0     5839 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/mcad.py
+-rw-r--r--   0        0        0    18533 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/mcds.py
+-rw-r--r--   0        0        0     4562 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/snap.py
+-rw-r--r--   0        0        0     1873 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/count_matrix/zarr.py
+-rw-r--r--   0        0        0       41 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/__init__.py
+-rw-r--r--   0        0        0      168 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/dataset.yaml
+-rw-r--r--   0        0        0     2041 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/directory_structure.py
+-rw-r--r--   0        0        0      181 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dataset/entry_point.py
+-rw-r--r--   0        0        0      133 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/__init__.py
+-rw-r--r--   0        0        0     8795 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dmr.py
+-rw-r--r--   0        0        0     6644 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dmr_baseds.py
+-rw-r--r--   0        0        0     7321 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dms.py
+-rw-r--r--   0        0        0     8561 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/call_dms_baseds.py
+-rw-r--r--   0        0        0     2461 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/parse_methylpy.py
+-rw-r--r--   0        0        0     4503 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/dmr/rms_test.py
+-rw-r--r--   0        0        0        0 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/genomic/__init__.py
+-rw-r--r--   0        0        0     5639 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/gtf/Gtf.py
+-rw-r--r--   0        0        0       80 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/gtf/__init__.py
+-rw-r--r--   0        0        0     1164 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/gtf/utilities.py
+-rw-r--r--   0        0        0      195 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/__init__.py
+-rw-r--r--   0        0        0    12276 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/cca.py
+-rw-r--r--   0        0        0     6554 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/confusion.py
+-rw-r--r--   0        0        0     9912 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/metric.py
+-rw-r--r--   0        0        0    32816 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/integration/seurat_class.py
+-rw-r--r--   0        0        0     4794 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/jbrowse/__init__.py
+-rw-r--r--   0        0        0      124 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/__init__.py
+-rw-r--r--   0        0        0    25737 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/base_ds.py
+-rw-r--r--   0        0        0    11587 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/correlation.py
+-rw-r--r--   0        0        0    57790 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/mcds.py
+-rw-r--r--   0        0        0    39343 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/region_ds.py
+-rw-r--r--   0        0        0    19345 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/mcds/utilities.py
+-rw-r--r--   0        0        0       75 2022-09-23 06:50:34.759006 ALLCools-1.0.8/ALLCools/motif/__init__.py
+-rw-r--r--   0        0        0  1614001 2022-09-23 06:50:34.767006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme
+-rw-r--r--   0        0        0   172054 2022-09-23 06:50:34.767006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv
+-rw-r--r--   0        0        0    77918 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv
+-rw-r--r--   0        0        0        0 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/default_motif_set/__init__.py
+-rw-r--r--   0        0        0     8709 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/motifs.py
+-rw-r--r--   0        0        0     4260 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/parse_meme.py
+-rw-r--r--   0        0        0     4864 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/motif/snakemake.py
+-rw-r--r--   0        0        0      306 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/__init__.py
+-rw-r--r--   0        0        0     9026 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/categorical_scatter.py
+-rw-r--r--   0        0        0     4512 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/color.py
+-rw-r--r--   0        0        0     7704 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/continuous_scatter.py
+-rw-r--r--   0        0        0     1429 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/contour.py
+-rw-r--r--   0        0        0     2645 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/decomposition.py
+-rw-r--r--   0        0        0     7940 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/dendro.py
+-rw-r--r--   0        0        0    12573 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/GtfTrack.py
+-rw-r--r--   0        0        0    10256 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py
+-rw-r--r--   0        0        0       55 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/__init__.py
+-rw-r--r--   0        0        0    37598 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/genome_track/_pygenometrack.py
+-rw-r--r--   0        0        0     1026 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/interactive_scatter.py
+-rw-r--r--   0        0        0     7382 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/qc_plots.py
+-rw-r--r--   0        0        0      833 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/size.py
+-rw-r--r--   0        0        0     7469 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/sunburst.py
+-rw-r--r--   0        0        0     2083 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/text_anno_scatter.py
+-rw-r--r--   0        0        0     7410 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/plot/utilities.py
+-rw-r--r--   0        0        0      166 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/pseudo_cell/__init__.py
+-rw-r--r--   0        0        0     6211 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_kmeans.py
+-rw-r--r--   0        0        0    10950 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_knn.py
+-rw-r--r--   0        0        0       29 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/reptile/__init__.py
+-rw-r--r--   0        0        0    31804 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/reptile/reptile.py
+-rw-r--r--   0        0        0        0 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/schema/__init__.py
+-rw-r--r--   0        0        0      894 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/schema/mcds_schema.py
+-rw-r--r--   0        0        0    11318 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/table_to_allc.py
+-rw-r--r--   0        0        0    18046 2022-09-23 06:50:34.771006 ALLCools-1.0.8/ALLCools/utilities.py
+-rw-r--r--   0        0        0     1073 2022-09-23 06:50:34.771006 ALLCools-1.0.8/LICENSE
+-rw-r--r--   0        0        0      339 2022-09-23 06:50:34.771006 ALLCools-1.0.8/README.md
+-rw-r--r--   0        0        0     2018 2022-09-23 06:50:35.059016 ALLCools-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2127 1970-01-01 00:00:00.000000 ALLCools-1.0.8/PKG-INFO
```

### Comparing `ALLCools-1.0.5/ALLCools/__main__.py` & `ALLCools-1.0.8/ALLCools/__main__.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_allc_to_bigwig.py` & `ALLCools-1.0.8/ALLCools/_allc_to_bigwig.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_allc_to_region_count.py` & `ALLCools-1.0.8/ALLCools/_allc_to_region_count.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_bam_to_allc.py` & `ALLCools-1.0.8/ALLCools/_bam_to_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_doc.py` & `ALLCools-1.0.8/ALLCools/_doc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_extract_allc.py` & `ALLCools-1.0.8/ALLCools/_extract_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_merge_allc.py` & `ALLCools-1.0.8/ALLCools/_merge_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/_open.py` & `ALLCools-1.0.8/ALLCools/_open.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/abc/abc_score.py` & `ALLCools-1.0.8/ALLCools/abc/abc_score.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/api.py` & `ALLCools-1.0.8/ALLCools/api.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/ClusterMerging.py` & `ALLCools-1.0.8/ALLCools/clustering/ClusterMerging.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/ConsensusClustering.py` & `ALLCools-1.0.8/ALLCools/clustering/ConsensusClustering.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/__init__.py` & `ALLCools-1.0.8/ALLCools/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/art_of_tsne.py` & `ALLCools-1.0.8/ALLCools/clustering/art_of_tsne.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/balanced_pca.py` & `ALLCools-1.0.8/ALLCools/clustering/balanced_pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,34 +104,42 @@
     """
     pcs = adata.obsm[obsm]
     if pcs.shape[0] > downsample:
         print(f"Downsample PC matrix to {downsample} cells to calculate significant PC components")
         use_pcs = pd.DataFrame(pcs).sample(downsample).values
     else:
         use_pcs = pcs
+
+    n_components = pc_ks_test(use_pcs, p_cutoff=p_cutoff, min_pc=4)
+
+    if update:
+        adata.obsm[obsm] = pcs[:, :n_components]
+        print(f"Changing adata.obsm['X_pca'] from shape {pcs.shape} to {adata.obsm[obsm].shape}")
+    return n_components
+
+
+def pc_ks_test(pcs, p_cutoff=0.1, min_pc=4):
     i = 0
-    for i in range(use_pcs.shape[1] - 1):
-        cur_pc = use_pcs[:, i]
-        next_pc = use_pcs[:, i + 1]
+    for i in range(pcs.shape[1] - 1):
+        cur_pc = pcs[:, i]
+        next_pc = pcs[:, i + 1]
         _, p = ks_2samp(cur_pc, next_pc)
         if p > p_cutoff:
             break
-    n_components = min(i + 1, use_pcs.shape[1])
-    min_pc = min(4, use_pcs.shape[1])
+    n_components = min(i + 1, pcs.shape[1])
+    min_pc = min(min_pc, pcs.shape[1])
+
     if n_components < min_pc:
         print(
             f"only {n_components} passed the P cutoff, "
             f"in order to proceed following analysis, will use first {min_pc} PCs"
         )
         n_components = min_pc
     else:
         print(f"{n_components} components passed P cutoff of {p_cutoff}.")
-    if update:
-        adata.obsm[obsm] = pcs[:, :n_components]
-        print(f"Changing adata.obsm['X_pca'] from shape {pcs.shape} to {adata.obsm[obsm].shape}")
     return n_components
 
 
 def balanced_pca(adata: anndata.AnnData, groups: str = "pre_clusters", max_cell_prop=0.1, n_comps=100, scale=False):
     """
     Perform Balanced PCA on the data.
```

### Comparing `ALLCools-1.0.5/ALLCools/clustering/chromatin_conformation.py` & `ALLCools-1.0.8/ALLCools/clustering/chromatin_conformation.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/dmg.py` & `ALLCools-1.0.8/ALLCools/clustering/dmg.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/doublets/coverage_doublets.py` & `ALLCools-1.0.8/ALLCools/clustering/doublets/coverage_doublets.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/doublets/scrublet.py` & `ALLCools-1.0.8/ALLCools/clustering/doublets/scrublet.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/feature_selection/feature_enrichment.py` & `ALLCools-1.0.8/ALLCools/clustering/feature_selection/feature_enrichment.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/feature_selection/gene_panel_design.py` & `ALLCools-1.0.8/ALLCools/clustering/feature_selection/gene_panel_design.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/incremental_pca.py` & `ALLCools-1.0.8/ALLCools/clustering/incremental_pca.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/lsi.py` & `ALLCools-1.0.8/ALLCools/clustering/lsi.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/mcad.py` & `ALLCools-1.0.8/ALLCools/clustering/mcad.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/pvclust.py` & `ALLCools-1.0.8/ALLCools/clustering/pvclust.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/clustering/rutilities.py` & `ALLCools-1.0.8/ALLCools/clustering/rutilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/base_ds.py` & `ALLCools-1.0.8/ALLCools/count_matrix/base_ds.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     def fetch_df(self, *args, **kwargs) -> pd.DataFrame:
         """
         Fetch ALLC files by position and return a pandas dataframe.
 
         Parameters
         ----------
         args :
-            positional arguments for TabixFile.fetch
+            positional arguments for `TabixFile.fetch`
         kwargs :
-            keyword arguments for TabixFile.fetch
+            keyword arguments for `TabixFile.fetch`
 
         Returns
         -------
         df :
             a pandas dataframe with shape (n_rows, 7).
         """
         df = pd.DataFrame(
@@ -80,27 +80,31 @@
         If pos_base is 0, the position is converted to 0-base.Original ALLC files are 1-base.
         the second column is the mc count.
         the third column is the cov count.
 
         Parameters
         ----------
         args :
-            positional arguments for TabixFile.fetch
+            positional arguments for `TabixFile.fetch`
         pos_base :
             the position base for the array, default is 0, which means the array pos column is 0-based.
             ALLC file is 1-based.
         kwargs :
             keyword arguments for TabixFile.fetch
 
         Returns
         -------
         records :
             a numpy array with shape (n_rows, 3).
         """
-        records = np.array([(pos, mc, cov) for _, pos, _, _, mc, cov, _ in self.fetch(*args, **kwargs)])
+        try:
+            records = np.array([(pos, mc, cov) for _, pos, _, _, mc, cov, _ in self.fetch(*args, **kwargs)])
+        except ValueError as e:
+            print(f"{self.filename} fetch causing ValueError")
+            raise e
         if records.shape[0] == 0:
             # no records in allc
             # this records is still empty, but shape is correct
             records = np.zeros(shape=(0, 3))
 
         if pos_base == 0:
             # ALLC pos is 1-based,
@@ -116,15 +120,15 @@
         Fetch ALLC files by position and return a full-base numpy array with shape (pos_max, 2).
 
         The first column is the mc count. The second column is cov count.
 
         Parameters
         ----------
         args :
-            positional arguments for TabixFile.fetch
+            positional arguments for `TabixFile.fetch`
         pos_min :
             the minimum position fetched from ALLC or the minimum position in the query region provided by user.
             Use this number as the offset for the array position.
         pos_max :
             the relative maximum position (compare to pos_min) fetched from ALLC
             or the maximum position in the query region provided by user.
         sparse :
@@ -264,29 +268,36 @@
     with pysam.FastaFile(genome_fasta_path, filepath_index=f"{genome_fasta_path}.fai") as fa:
         sequence = fa.fetch(chrom).upper()
 
     # make sure chrom size consistent
     assert len(sequence) == chrom_size, f"chrom {chrom} size {len(sequence)} is not consistent with {chrom_size}"
 
     context_codebook = zarr_root.require_dataset(
-        "codebook", shape=(chrom_size, len(contexts)), chunks=chunk_size, dtype="bool"
+        "codebook", shape=(chrom_size, len(contexts)), chunks=chunk_size, dtype="int8"
     )
     context_codebook.attrs["_ARRAY_DIMENSIONS"] = ["pos", "mc_type"]
 
     for i, context in enumerate(contexts):
         print(context, end=", ")
         # positive strand
-        pos_pattern = re.compile(context)
-        context_pos = [match.start() for match in pos_pattern.finditer(sequence)]
+        # in order to count overlapping contexts, this regex pattern is necessary
+        # see https://stackoverflow.com/questions/5616822/how-to-use-regex-to-find-all-overlapping-matches
+        pos_context_str = f"(?=({context}))"
+        pos_pattern = re.compile(pos_context_str)
+        pos_pos = [match.start() for match in pos_pattern.finditer(sequence)]
         # negative strand
-        neg_pattern = re.compile(reverse_complement(context))
-        context_pos += [match.end() for match in neg_pattern.finditer(sequence)]
-
-        context_pos = sorted(set(context_pos))
-        context_codebook[context_pos, i] = True
+        neg_context_str = f"(?=({reverse_complement(context)}))"
+        neg_pattern = re.compile(neg_context_str)
+        neg_dodge = len(context) - 1
+        neg_pos = [match.end() + neg_dodge for match in neg_pattern.finditer(sequence)]
+
+        pos_value = pd.Series({i: 1 for i in pos_pos})
+        neg_value = pd.Series({i: -1 for i in neg_pos})
+        value = pd.concat([pos_value, neg_value]).sort_index()
+        context_codebook[value.index, i] = value.values
 
     context_codebook.attrs["contexts"] = list(contexts)
     print()
     return
 
 
 def _create_mc_type_zarr(root, contexts, c_pos, include_n, context_size):
@@ -560,26 +571,35 @@
     mode="a",
     n_cpu=1,
 ):
     """Create a BaseDS zarr dataset."""
     output_dir_path = pathlib.Path(output_dir_path)
     output_dir_path.mkdir(exist_ok=True, parents=True)
 
-    chroms = pd.read_csv(chrom_size_path, header=None, sep="\t", index_col=0, names=["chrom", "size"]).squeeze()
+    chroms = pd.read_csv(chrom_size_path, header=None, sep="\t", index_col=0, names=["chrom", "size"])["size"]
     # save chroms to output_dir_path
     chroms.to_csv(f"{output_dir_path}/chrom_sizes.csv", index=True, header=False)
 
     allc_table_path = pathlib.Path(allc_table_path)
     sample_path_series = pd.read_csv(
         allc_table_path,
         header=None,
         index_col=0,
         sep="\t" if allc_table_path.name.endswith("tsv") else ",",
     ).squeeze()
 
+    # check if all the allc paths in sample_path_series exist
+    flag = False
+    for p in sample_path_series.to_list():
+        if not pathlib.Path(p).exists():
+            flag = True
+            print(f"{p} does not exist.")
+    if flag:
+        raise FileNotFoundError(f"Some of the allc files in {allc_table_path} do not exist.")
+
     if generate_codebook:
         fasta_path = pathlib.Path(genome_fasta_path)
         fai_path = pathlib.Path(f"{fasta_path}.fai")
         if not fai_path.exists():
             print(f"{fai_path} not found. Try generating...")
             import subprocess
```

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/dataset.py` & `ALLCools-1.0.8/ALLCools/count_matrix/dataset.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/h5ad.py` & `ALLCools-1.0.8/ALLCools/count_matrix/h5ad.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/mcad.py` & `ALLCools-1.0.8/ALLCools/count_matrix/mcad.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/mcds.py` & `ALLCools-1.0.8/ALLCools/count_matrix/mcds.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/snap.py` & `ALLCools-1.0.8/ALLCools/count_matrix/snap.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/count_matrix/zarr.py` & `ALLCools-1.0.8/ALLCools/count_matrix/zarr.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/dataset/directory_structure.py` & `ALLCools-1.0.8/ALLCools/dataset/directory_structure.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/dmr/call_dmr.py` & `ALLCools-1.0.8/ALLCools/dmr/call_dmr.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/dmr/call_dms.py` & `ALLCools-1.0.8/ALLCools/dmr/call_dms.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from ALLCools.mcds.utilities import write_ordered_chunks
 from ALLCools.utilities import genome_region_chunks
 
 from .rms_test import (
     calculate_residual,
     downsample_table,
+    init_rms_functions,
     permute_root_mean_square_test,
 )
 
 
 def _read_single_allc(path, region):
     grange = region.split(":")[1]
     start, _ = grange.split("-")
@@ -184,19 +185,16 @@
             cpu = 1
 
     # temp dir
     dms_chunk_dir = pathlib.Path(f"{output_dir}/.dms_chunks")
     dms_chunk_dir.mkdir(exist_ok=True, parents=True)
     dms_dir = f"{output_dir}/dms"
 
-    # trigger the numba JIT compilation before multiprocessing
-    table = np.array([[0, 1], [0, 1]])
-    permute_root_mean_square_test(table)
-    calculate_residual(table)
-    downsample_table(table, max_row_count=max_row_count)
+    # init numba function
+    init_rms_functions()
 
     # parallel each chunk
     with ProcessPoolExecutor(cpu) as exe:
         futures = {}
         for chunk_id, region in enumerate(regions):
             future = exe.submit(
                 _perform_rms_batch,
```

### Comparing `ALLCools-1.0.5/ALLCools/dmr/parse_methylpy.py` & `ALLCools-1.0.8/ALLCools/dmr/parse_methylpy.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/dmr/rms_test.py` & `ALLCools-1.0.8/ALLCools/dmr/rms_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from numba import njit
+from scipy.stats import norm
 
 
 @njit
 def _get_e(table, n, m):
     row_sum = table.sum(axis=0).astype(np.float64)
     col_sum = table.sum(axis=1).astype(np.float64)
     e = np.dot(col_sum.reshape(n, 1), row_sum.reshape(1, 2)) / m
@@ -39,15 +40,26 @@
         )
     )
     return residual
 
 
 @njit
 def permute_root_mean_square_test(table, n_permute=3000, min_pvalue=0.034):
-    """Permute root-mean-square test."""
+    """
+    Permute root-mean-square test.
+
+    Parameters
+    ----------
+    table :
+        N-by-2 table of methylated and unmethylated counts.
+    n_permute :
+        Number of permutations.
+    min_pvalue :
+        Minimum p-value to perform the test.
+    """
     # calculate real goodness-of-fit s
     n = table.shape[0]
     m = table.sum()
     e = _get_e(table, n, m)
     real_s = _calculate_goodness_of_fit(table, n, m)
 
     # permutation
@@ -65,22 +77,84 @@
             return greater_than_real / (i + 2)
 
     p_value = greater_than_real / n_permute
     return p_value
 
 
 @njit
+def _get_read_s_and_permute_s(table, n_permute=10000, min_pvalue=0.034):
+    # calculate real goodness-of-fit s
+    n = table.shape[0]
+    m = table.sum()
+    e = _get_e(table, n, m)
+    real_s = _calculate_goodness_of_fit(table, n, m)
+
+    # permutation
+    p = e.flatten() / m
+    greater_than_real = 1
+    max_greater_value = n_permute * min_pvalue
+    ss = np.zeros(n_permute + 1, dtype=np.float64)
+    ss[0] = real_s
+    for i in range(n_permute):
+        p_table = _make_permutation_table(p, n, m)
+        # calculate permuted goodness of fit s'
+        s = _calculate_goodness_of_fit(p_table, n, m)
+        ss[i + 1] = s
+
+        greater_than_real += int(s >= real_s)
+        # break in advance if p-value can be significant
+        if greater_than_real > max_greater_value:
+            # return current p value
+            return ss[: i + 1].copy()
+    return ss
+
+
+def permute_root_mean_square_test_and_estimate_p(table, n_permute=10000, min_pvalue=0.034):
+    """
+    Permute root-mean-square test
+
+    Report estimated p-value by approximate null distribution as normal distribution.
+    """
+    ss = _get_read_s_and_permute_s(table=table, n_permute=n_permute, min_pvalue=min_pvalue)
+    real_s = ss[0]
+    ss = ss[1:]
+
+    e, std = norm.fit(ss)
+    if std == 0:
+        p_value = 1
+    else:
+        p_value = 1 - norm(e, std).cdf(real_s)
+
+    if p_value < 1e-14:  # np.finfo(np.float64).resolution: 1e-15
+        p_value = 1e-14
+    return p_value
+
+
+@njit
 def _downsample_sample_count(a, max_count):
     a = a.astype(np.float64)
     total = a.sum()
     p = a / total
     if total > max_count:
         b = max_count * p
     else:
         b = a
     b = b.astype(np.int64)
     return b
 
 
-def downsample_table(table, max_row_count):
+def downsample_table(table, max_row_count=50, max_total_count=3000):
     """Downsample high count rows to max_row_count."""
+    n_sample = table.shape[0]
+    max_row_count = min(max_total_count / n_sample, max_row_count)
+    max_row_count = max(10, max_row_count)
+
     return np.apply_along_axis(_downsample_sample_count, axis=1, arr=table, max_count=max_row_count)
+
+
+def init_rms_functions():
+    """Initialize the numba JIT compilation before multiprocessing RMS functions."""
+    table = np.array([[0, 1], [0, 1]])
+    permute_root_mean_square_test(table)
+    calculate_residual(table)
+    downsample_table(table, max_row_count=10)
+    return
```

### Comparing `ALLCools-1.0.5/ALLCools/gtf/Gtf.py` & `ALLCools-1.0.8/ALLCools/gtf/Gtf.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/gtf/utilities.py` & `ALLCools-1.0.8/ALLCools/gtf/utilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/integration/cca.py` & `ALLCools-1.0.8/ALLCools/integration/cca.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/integration/confusion.py` & `ALLCools-1.0.8/ALLCools/integration/confusion.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/integration/metric.py` & `ALLCools-1.0.8/ALLCools/integration/metric.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/integration/seurat_class.py` & `ALLCools-1.0.8/ALLCools/integration/seurat_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,16 +151,16 @@
         metric="euclidean",
         n_neighbors=k_filter,
         random_state=random_state,
         parallel_batch_queries=True,
         n_jobs=n_jobs,
     )
     G = index.query(qry_data, k=k_filter)[0]
-    anchor = np.array([xx for xx in anchor if (xx[0] in G[xx[1]])])
     input_anchors = anchor.shape[0]
+    anchor = np.array([xx for xx in anchor if (xx[0] in G[xx[1]])])
     print(f"Anchor selected with high CC feature graph: {anchor.shape[0]} / {input_anchors}")
     return anchor
 
 
 def score_anchor(anchor, G11, G12, G21, G22, k_score=30, Gp1=None, Gp2=None, k_local=50):
     """
     Score the anchor by the number of shared neighbors.
@@ -426,15 +426,15 @@
                         random_state=self.random_state,
                         n_jobs=self.n_jobs,
                     )[:, ::-1]
         elif dim_red in ("rpca", "rlsi"):
             from .cca import LSI, SVD, downsample
 
             adata1, adata2 = adata1.X, adata2.X
-            k = max([k_anchor, k_local, k_score, 50])
+            k = max(i for i in [k_anchor, k_local, k_score, 50] if i is not None)
             if dim_red == "rpca":
                 print("Run rPCA")
                 model = SVD(n_components=ncc, random_state=random_state)
             elif dim_red == "rlsi":
                 print("Run rLSI")
                 model = LSI(n_components=ncc, random_state=random_state)
             else:
@@ -500,14 +500,15 @@
         k_local=None,
         key_local="X_pca",
         key_anchor="X",
         dim_red="pca",
         svd_algorithm="randomized",
         scale1=False,
         scale2=False,
+        scale_list=None,
         k_filter=None,
         n_features=200,
         n_components=None,
         max_cc_cells=50000,
         chunk_size=50000,
         k_anchor=5,
         k_score=30,
@@ -540,14 +541,21 @@
         # alignments and all_pairs
         self.alignments = alignments
         self._get_all_pairs()
 
         print("Find anchors across datasets.")
         for i in range(self.n_dataset - 1):
             for j in range(i + 1, self.n_dataset):
+                if scale_list is not None:
+                    scale1 = scale_list[i]
+                    scale2 = scale_list[j]
+                    print("Get scale1 and scale2 from scale_list")
+                    print(f"dataset {i} scale: {scale1}")
+                    print(f"dataset {j} scale: {scale2}")
+
                 if key_match is None:
                     anchor_df = self._pairwise_find_anchor(
                         i=i,
                         i_sel=None,
                         j=j,
                         j_sel=None,
                         dim_red=dim_red,
@@ -836,27 +844,36 @@
         all_column_variables = np.repeat(categorical_key + continuous_key, cat_counts)
         label_qry = pd.DataFrame(label_qry, index=data_qry_index, columns=all_column_names)
         result = {}
         for key in categorical_key + continuous_key:
             result[key] = label_qry.iloc[:, all_column_variables == key]
         return result
 
-    def save(self, output_path, save_local_knn=False, save_raw_anchor=False, save_mutual_knn=False):
+    def save(self, output_path, save_local_knn=False, save_raw_anchor=False, save_mutual_knn=False, save_adata=False):
         """Save the model and results to disk."""
         # save each adata in a separate dir
         output_path = pathlib.Path(output_path)
         output_path.mkdir(exist_ok=True, parents=True)
 
-        # save adata and clear the self.adata_dict
-        adata_dir = output_path / "adata"
-        adata_dir.mkdir(exist_ok=True)
-        with open(f"{adata_dir}/order.txt", "w") as f:
-            for k, v in self.adata_dict.items():
-                v.write_h5ad(f"{adata_dir}/{k}.h5ad")
-                f.write(f"{k}\n")
+        if save_adata:
+            # save adata and clear the self.adata_dict
+            adata_dir = output_path / "adata"
+            adata_dir.mkdir(exist_ok=True)
+            with open(f"{adata_dir}/order.txt", "w") as f:
+                for k, v in self.adata_dict.items():
+                    for col, val in v.obs.items():
+                        if val.dtype == "O":
+                            v.obs[col] = val.fillna("nan").astype(str)
+                        elif val.dtype == "category":
+                            v.obs[col] = val.fillna("nan").astype(str)
+                        else:
+                            pass
+                    v.write_h5ad(f"{adata_dir}/{k}.h5ad")
+                    f.write(f"{k}\n")
+
         # clear the adata in integrator
         self.adata_dict = {}
 
         if not save_local_knn:
             self.local_knn = []
         if not save_raw_anchor:
             self.raw_anchor = {}
@@ -873,15 +890,17 @@
         model_path = f"{input_path}/model.lib"
 
         obj = joblib.load(model_path)
 
         orders = pd.read_csv(f"{adata_dir}/order.txt", header=None, index_col=0).index
         adata_dict = OrderedDict()
         for k in orders:
-            adata_dict[k] = anndata.read_h5ad(f"{adata_dir}/{k}.h5ad")
+            adata_path = f"{adata_dir}/{k}.h5ad"
+            if pathlib.Path(adata_path).exists():
+                adata_dict[k] = anndata.read_h5ad(f"{adata_dir}/{k}.h5ad")
         obj.adata_dict = adata_dict
         return obj
 
     @classmethod
     def save_transfer_results_to_adata(cls, adata, transfer_results, new_label_suffix="_transfer"):
         """Save transfer results to adata."""
         for key, df in transfer_results.items():
```

### Comparing `ALLCools-1.0.5/ALLCools/mcds/correlation.py` & `ALLCools-1.0.8/ALLCools/mcds/correlation.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/mcds/mcds.py` & `ALLCools-1.0.8/ALLCools/mcds/mcds.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,18 +426,22 @@
         alpha :
             alpha value for the transformation regularization
         normalize_per_cell :
             if True, will normalize the mC rate data array per cell
         da_suffix :
             name suffix appended to the calculated mC rate data array
         """
+        var_dim = self._verify_dim(var_dim, mode="var")
+
         if da is None:
+            if var_dim is None:
+                raise ValueError("Both da and var_dim are not specified")
             da = f"{var_dim}_da"
         if da not in self.data_vars:
-            raise KeyError(f"{da} is not in this dataset")
+            raise KeyError(f"{da} is not in this dataset, please specify da or var_dim")
         if var_dim not in self[da].dims:
             raise KeyError(f"{var_dim} is not a dimension of {da}")
 
         frac = self._calculate_frac(var_dim=var_dim, da=da, normalize_per_cell=False, clip_norm_value=None)
 
         m_value = np.log2((frac + alpha) / (1 - frac + alpha))
```

### Comparing `ALLCools-1.0.5/ALLCools/mcds/region_ds.py` & `ALLCools-1.0.8/ALLCools/mcds/region_ds.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/mcds/utilities.py` & `ALLCools-1.0.8/ALLCools/mcds/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -493,7 +493,41 @@
     # save the changes
     with open(old_zmetadata_path, "w") as f:
         json.dump(zmeta_tmp, f)
 
     # delete temp zarr
     subprocess.run(["rm", "-rf", temp_zarr_path], check=True)
     return
+
+
+def binnify(chromsizes, binsize):
+    """
+    Divide a genome into evenly sized bins.
+
+    Parameters
+    ----------
+    chromsizes : Series
+        pandas Series indexed by chromosome name with chromosome lengths in bp.
+    binsize : int
+        size of bins in bp
+
+    Returns
+    -------
+    bins : :py:class:`pandas.DataFrame`
+        Dataframe with columns: ``chrom``, ``start``, ``end``.
+    """
+
+    def _each(chrom):
+        clen = chromsizes[chrom]
+        n_bins = int(np.ceil(clen / binsize))
+        binedges = np.arange(0, (n_bins + 1)) * binsize
+        binedges[-1] = clen
+        return pd.DataFrame(
+            {"chrom": [chrom] * n_bins, "start": binedges[:-1], "end": binedges[1:]},
+            columns=["chrom", "start", "end"],
+        )
+
+    bintable = pd.concat(map(_each, chromsizes.keys()), axis=0, ignore_index=True)
+
+    bintable["chrom"] = pd.Categorical(bintable["chrom"], categories=list(chromsizes.index), ordered=True)
+
+    return bintable
```

### Comparing `ALLCools-1.0.5/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme` & `ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.meme`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv` & `ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.metadata.csv`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv` & `ALLCools-1.0.8/ALLCools/motif/default_motif_set/JASPAR2018HOCOMOCOv11Jolma2013.thresholds.csv`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/motif/motifs.py` & `ALLCools-1.0.8/ALLCools/motif/motifs.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/motif/parse_meme.py` & `ALLCools-1.0.8/ALLCools/motif/parse_meme.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/motif/snakemake.py` & `ALLCools-1.0.8/ALLCools/motif/snakemake.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/categorical_scatter.py` & `ALLCools-1.0.8/ALLCools/plot/categorical_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/color.py` & `ALLCools-1.0.8/ALLCools/plot/color.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/continuous_scatter.py` & `ALLCools-1.0.8/ALLCools/plot/continuous_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/contour.py` & `ALLCools-1.0.8/ALLCools/plot/contour.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/decomposition.py` & `ALLCools-1.0.8/ALLCools/plot/decomposition.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/dendro.py` & `ALLCools-1.0.8/ALLCools/plot/dendro.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/genome_track/GtfTrack.py` & `ALLCools-1.0.8/ALLCools/plot/genome_track/GtfTrack.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py` & `ALLCools-1.0.8/ALLCools/plot/genome_track/HiCMatrixCoolTrack.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/genome_track/_pygenometrack.py` & `ALLCools-1.0.8/ALLCools/plot/genome_track/_pygenometrack.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/interactive_scatter.py` & `ALLCools-1.0.8/ALLCools/plot/interactive_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/qc_plots.py` & `ALLCools-1.0.8/ALLCools/plot/qc_plots.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/size.py` & `ALLCools-1.0.8/ALLCools/plot/size.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/sunburst.py` & `ALLCools-1.0.8/ALLCools/plot/sunburst.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/text_anno_scatter.py` & `ALLCools-1.0.8/ALLCools/plot/text_anno_scatter.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/plot/utilities.py` & `ALLCools-1.0.8/ALLCools/plot/utilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/pseudo_cell/pseudo_cell_kmeans.py` & `ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_kmeans.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/pseudo_cell/pseudo_cell_knn.py` & `ALLCools-1.0.8/ALLCools/pseudo_cell/pseudo_cell_knn.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/reptile/reptile.py` & `ALLCools-1.0.8/ALLCools/reptile/reptile.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/schema/mcds_schema.py` & `ALLCools-1.0.8/ALLCools/schema/mcds_schema.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/table_to_allc.py` & `ALLCools-1.0.8/ALLCools/table_to_allc.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/ALLCools/utilities.py` & `ALLCools-1.0.8/ALLCools/utilities.py`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/LICENSE` & `ALLCools-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ALLCools-1.0.5/pyproject.toml` & `ALLCools-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     { name = "Hanqing Liu", email = "hanliu@salk.edu" },
     { name = "Jingtian Zhou", email = "jzhou@salk.edu" },
     { name = "Wei Tian", email = "wtian@salk.edu" }
 ]
 urls.Documentation = "https://lhqing.github.io/ALLCools/intro.html"
 urls.Source = "https://github.com/lhqing/ALLCools"
 urls.Home-page = "https://github.com/lhqing/ALLCools"
-version = "1.0.5"
+version = "1.0.8"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 readme = "README.md"
 dependencies = [
     "anndata",
     "numpy",
     'matplotlib',
```

### Comparing `ALLCools-1.0.5/PKG-INFO` & `ALLCools-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLCools
-Version: 1.0.5
+Version: 1.0.8
 Summary: Toolkit for single-cell DNA methylome and multiomic data analysis.
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanliu@salk.edu>, Jingtian Zhou <jzhou@salk.edu>, Wei Tian <wtian@salk.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: anndata
 Requires-Dist: numpy
```

