# Comparing `tmp/damona-0.8.2.tar.gz` & `tmp/damona-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/damona-0.8.2.tar", last modified: Wed Feb 22 02:39:19 2023, max compression
+gzip compressed data, was "damona-0.8.3.tar", last modified: Fri Apr 14 09:55:16 2023, max compression
```

## Comparing `damona-0.8.2.tar` & `damona-0.8.3.tar`

### file list

```diff
@@ -1,196 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2023-02-22 02:39:16.000000 damona-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1532 2023-02-22 02:39:16.000000 damona-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      244 2023-02-22 02:39:16.000000 damona-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    20390 2023-02-22 02:39:19.000000 damona-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15718 2023-02-22 02:39:16.000000 damona-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2023-02-22 02:39:16.000000 damona-0.8.2/damona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3114 2023-02-22 02:39:16.000000 damona-0.8.2/damona/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/biocontainers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:16.000000 damona-0.8.2/damona/biocontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)  3790743 2023-02-22 02:39:16.000000 damona-0.8.2/damona/biocontainers/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     6105 2023-02-22 02:39:16.000000 damona-0.8.2/damona/builders.py
--rw-r--r--   0 runner    (1001) docker     (116)    13000 2023-02-22 02:39:16.000000 damona-0.8.2/damona/common.py
--rw-r--r--   0 runner    (1001) docker     (116)     5315 2023-02-22 02:39:16.000000 damona-0.8.2/damona/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    15657 2023-02-22 02:39:16.000000 damona-0.8.2/damona/environ.py
--rw-r--r--   0 runner    (1001) docker     (116)    22582 2023-02-22 02:39:16.000000 damona-0.8.2/damona/install.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/library/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/library/R/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1588 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/R/Singularity.R_3.6.3
--rwxr-xr-x   0 runner    (1001) docker     (116)     1589 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/R/Singularity.R_4.0.2
--rw-r--r--   0 runner    (1001) docker     (116)      144 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/R/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/library/conda/
--rw-r--r--   0 runner    (1001) docker     (116)     3358 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/conda/Singularity.conda_4.7.12
--rw-r--r--   0 runner    (1001) docker     (116)     2621 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/conda/Singularity.conda_4.9.2
--rw-r--r--   0 runner    (1001) docker     (116)      212 2023-02-22 02:39:16.000000 damona-0.8.2/damona/library/conda/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/papers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:16.000000 damona-0.8.2/damona/papers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16088 2023-02-22 02:39:16.000000 damona-0.8.2/damona/registry.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    26465 2023-02-22 02:39:16.000000 damona-0.8.2/damona/script.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/shell/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:16.000000 damona-0.8.2/damona/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/shell/bash/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:16.000000 damona-0.8.2/damona/shell/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5636 2023-02-22 02:39:16.000000 damona-0.8.2/damona/shell/bash/damona.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/shell/fish/
--rw-r--r--   0 runner    (1001) docker     (116)     3320 2023-02-22 02:39:16.000000 damona-0.8.2/damona/shell/fish/damona.fish
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/art/
--rwxr-xr-x   0 runner    (1001) docker     (116)      296 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/art/Singularity.art_2.5.8
--rwxr-xr-x   0 runner    (1001) docker     (116)      293 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/art/Singularity.art_3.11.14
--rw-r--r--   0 runner    (1001) docker     (116)      530 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/art/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bamtools/
--rw-r--r--   0 runner    (1001) docker     (116)      977 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bamtools/Singularity.bamtools_2.5.2
--rw-r--r--   0 runner    (1001) docker     (116)      286 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bamtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bbtools/
--rw-r--r--   0 runner    (1001) docker     (116)      439 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bbtools/Singularity.bbtools_38.94.0
--rw-r--r--   0 runner    (1001) docker     (116)     3102 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bbtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bcl2fastq/
--rw-r--r--   0 runner    (1001) docker     (116)      289 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bcl2fastq/Singularity.bcl2fastq_2.20.0
--rw-r--r--   0 runner    (1001) docker     (116)      298 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bcl2fastq/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bedtools/
--rw-r--r--   0 runner    (1001) docker     (116)      955 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bedtools/Singularity.bedtools_2.30.0
--rw-r--r--   0 runner    (1001) docker     (116)      289 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bedtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bioconvert/
--rw-r--r--   0 runner    (1001) docker     (116)     1858 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bioconvert/Singularity.bioconvert_0.6.1
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bioconvert/Singularity.bioconvert_0.6.2
--rw-r--r--   0 runner    (1001) docker     (116)     1769 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bioconvert/Singularity.bioconvert_0.6.3
--rw-r--r--   0 runner    (1001) docker     (116)      685 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bioconvert/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bowtie/
--rwxr-xr-x   0 runner    (1001) docker     (116)      956 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bowtie/Singularity.bowtie_1.3.1
--rw-r--r--   0 runner    (1001) docker     (116)      402 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bowtie/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/bowtie2/
--rw-r--r--   0 runner    (1001) docker     (116)      918 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bowtie2/Singularity.bowtie2_2.3.4
--rw-r--r--   0 runner    (1001) docker     (116)      912 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bowtie2/Singularity.bowtie2_2.4.2
--rw-r--r--   0 runner    (1001) docker     (116)      606 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/bowtie2/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/canu/
--rwxr-xr-x   0 runner    (1001) docker     (116)      322 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/canu/Singularity.canu_1.6.0
--rwxr-xr-x   0 runner    (1001) docker     (116)      322 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/canu/Singularity.canu_1.8.0
--rw-r--r--   0 runner    (1001) docker     (116)      464 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/canu/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/falco/
--rw-r--r--   0 runner    (1001) docker     (116)      531 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/falco/Singularity.falco_0.2.1
--rw-r--r--   0 runner    (1001) docker     (116)      778 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/falco/Singularity.falco_1.0.0
--rw-r--r--   0 runner    (1001) docker     (116)      497 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/falco/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/fastp/
--rw-r--r--   0 runner    (1001) docker     (116)      445 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/fastp/Singularity.fastp_0.23.2
--rw-r--r--   0 runner    (1001) docker     (116)      462 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/fastp/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/fastqc/
--rw-r--r--   0 runner    (1001) docker     (116)      522 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/fastqc/Singularity.fastqc_0.11.8
--rw-r--r--   0 runner    (1001) docker     (116)      492 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/fastqc/Singularity.fastqc_0.11.9
--rw-r--r--   0 runner    (1001) docker     (116)      705 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/fastqc/Singularity.fastqc_0.11.9_py3
--rw-r--r--   0 runner    (1001) docker     (116)      658 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/fastqc/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/flye/
--rwxr-xr-x   0 runner    (1001) docker     (116)      388 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/flye/Singularity.flye_2.9.0
--rw-r--r--   0 runner    (1001) docker     (116)      258 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/flye/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/gffread/
--rwxr-xr-x   0 runner    (1001) docker     (116)      601 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/gffread/Singularity.gffread_0.12.1
--rw-r--r--   0 runner    (1001) docker     (116)      266 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/gffread/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/graphviz/
--rwxr-xr-x   0 runner    (1001) docker     (116)      295 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/graphviz/Singularity.graphviz_2.43.0
--rw-r--r--   0 runner    (1001) docker     (116)      289 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/graphviz/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/gzip/
--rwxr-xr-x   0 runner    (1001) docker     (116)      180 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/gzip/Singularity.gzip_1.9.0
--rw-r--r--   0 runner    (1001) docker     (116)      280 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/gzip/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/hisat2/
--rw-r--r--   0 runner    (1001) docker     (116)      188 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/hisat2/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/homer/
--rwxr-xr-x   0 runner    (1001) docker     (116)      482 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/homer/Singularity.homer_4.11.0
--rw-r--r--   0 runner    (1001) docker     (116)      297 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/homer/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/idr/
--rwxr-xr-x   0 runner    (1001) docker     (116)      699 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/idr/Singularity.idr_2.0.3
--rw-r--r--   0 runner    (1001) docker     (116)      272 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/idr/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/igvtools/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1367 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/igvtools/Singularity.igvtools_2.12.0
--rw-r--r--   0 runner    (1001) docker     (116)      293 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/igvtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/kraken/
--rwxr-xr-x   0 runner    (1001) docker     (116)      638 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/kraken/Singularity.kraken_1.1.0
--rwxr-xr-x   0 runner    (1001) docker     (116)      904 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/kraken/Singularity.kraken_2.0.9
--rw-r--r--   0 runner    (1001) docker     (116)      604 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/kraken/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/minimap2/
--rw-r--r--   0 runner    (1001) docker     (116)      681 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/minimap2/Singularity.minimap2_2.17.0
--rw-r--r--   0 runner    (1001) docker     (116)      590 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/minimap2/Singularity.minimap2_2.23.0
--rw-r--r--   0 runner    (1001) docker     (116)      482 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/minimap2/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/phantompeakqualtools/
--rwxr-xr-x   0 runner    (1001) docker     (116)      942 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2
--rw-r--r--   0 runner    (1001) docker     (116)      522 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/phantompeakqualtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/pigz/
--rwxr-xr-x   0 runner    (1001) docker     (116)      185 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/pigz/Singularity.pigz_2.4.0
--rw-r--r--   0 runner    (1001) docker     (116)      280 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/pigz/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/prokka/
--rwxr-xr-x   0 runner    (1001) docker     (116)      617 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/prokka/Singularity.prokka_1.14.5
--rw-r--r--   0 runner    (1001) docker     (116)      238 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/prokka/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/quast/
--rwxr-xr-x   0 runner    (1001) docker     (116)      638 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/quast/Singularity.quast_5.0.2
--rw-r--r--   0 runner    (1001) docker     (116)      261 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/quast/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/rnadiff/
--rwxr-xr-x   0 runner    (1001) docker     (116)      930 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rnadiff/Singularity.rnadiff_1.7.1
--rw-r--r--   0 runner    (1001) docker     (116)      264 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rnadiff/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/rnaseqc/
--rwxr-xr-x   0 runner    (1001) docker     (116)      531 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0
--rw-r--r--   0 runner    (1001) docker     (116)      266 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rnaseqc/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/rtools/
--rwxr-xr-x   0 runner    (1001) docker     (116)      406 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rtools/Singularity.rtools_1.0.0
--rwxr-xr-x   0 runner    (1001) docker     (116)      509 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rtools/Singularity.rtools_1.1.0
--rwxr-xr-x   0 runner    (1001) docker     (116)      791 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rtools/Singularity.rtools_1.2.0
--rw-r--r--   0 runner    (1001) docker     (116)      668 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/rtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/salmon/
--rwxr-xr-x   0 runner    (1001) docker     (116)      594 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/salmon/Singularity.salmon_1.3.0
--rw-r--r--   0 runner    (1001) docker     (116)      281 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/salmon/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/samtools/
--rwxr-xr-x   0 runner    (1001) docker     (116)      805 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/samtools/Singularity.samtools_1.15.0
--rw-r--r--   0 runner    (1001) docker     (116)      482 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/samtools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/seqkit/
--rwxr-xr-x   0 runner    (1001) docker     (116)      548 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/seqkit/Singularity.seqkit_2.1.0
--rw-r--r--   0 runner    (1001) docker     (116)      261 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/seqkit/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/seqtk/
--rwxr-xr-x   0 runner    (1001) docker     (116)      498 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/seqtk/Singularity.seqtk_1.3.0
--rw-r--r--   0 runner    (1001) docker     (116)      259 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/seqtk/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/sequana/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1022 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana/Singularity.sequana_0.12.6
--rw-r--r--   0 runner    (1001) docker     (116)      320 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/sequana_denovo/
--rw-r--r--   0 runner    (1001) docker     (116)     5201 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2
--rw-r--r--   0 runner    (1001) docker     (116)      342 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_denovo/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/sequana_perl_tools/
--rwxr-xr-x   0 runner    (1001) docker     (116)      637 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0
--rwxr-xr-x   0 runner    (1001) docker     (116)      644 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0
--rw-r--r--   0 runner    (1001) docker     (116)      689 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_perl_tools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/sequana_ribofinder/
--rwxr-xr-x   0 runner    (1001) docker     (116)     1484 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0
--rw-r--r--   0 runner    (1001) docker     (116)      288 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_ribofinder/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/sequana_tools/
--rwxr-xr-x   0 runner    (1001) docker     (116)     2156 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0
--rwxr-xr-x   0 runner    (1001) docker     (116)     2242 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0
--rwxr-xr-x   0 runner    (1001) docker     (116)     2241 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0
--rwxr-xr-x   0 runner    (1001) docker     (116)     2338 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1
--rwxr-xr-x   0 runner    (1001) docker     (116)      695 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2
--rwxr-xr-x   0 runner    (1001) docker     (116)      640 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3
--rwxr-xr-x   0 runner    (1001) docker     (116)      366 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.5
--rwxr-xr-x   0 runner    (1001) docker     (116)     2641 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0
--rw-r--r--   0 runner    (1001) docker     (116)     5990 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/sequana_tools/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/shustring/
--rw-r--r--   0 runner    (1001) docker     (116)      463 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/shustring/Singularity.shustring_2.6.0
--rw-r--r--   0 runner    (1001) docker     (116)      289 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/shustring/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/snpeff/
--rw-r--r--   0 runner    (1001) docker     (116)     1185 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/snpeff/Singularity.snpeff_5.1.0
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/trf/
--rwxr-xr-x   0 runner    (1001) docker     (116)      891 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/trf/Singularity.trf_4.10.0
--rw-r--r--   0 runner    (1001) docker     (116)      198 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/trf/registry.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona/software/ucsc/
--rwxr-xr-x   0 runner    (1001) docker     (116)      521 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/ucsc/Singularity.ucsc_3.7.7
--rw-r--r--   0 runner    (1001) docker     (116)      356 2023-02-22 02:39:16.000000 damona-0.8.2/damona/software/ucsc/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    13630 2023-02-22 02:39:16.000000 damona-0.8.2/damona/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    20390 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5745 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      222 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2023-02-22 02:39:19.000000 damona-0.8.2/damona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2023-02-22 02:39:16.000000 damona-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      312 2023-02-22 02:39:19.000000 damona-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4822 2023-02-22 02:39:16.000000 damona-0.8.2/setup.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.297055 damona-0.8.3/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.245055 damona-0.8.3/.github/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.251055 damona-0.8.3/.github/workflows/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1748 2023-02-21 22:05:28.000000 damona-0.8.3/.github/workflows/bash_test.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1875 2023-02-21 22:06:16.000000 damona-0.8.3/.github/workflows/fish_test.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1594 2023-02-21 22:03:27.000000 damona-0.8.3/.github/workflows/main.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      961 2023-01-10 21:16:10.000000 damona-0.8.3/.github/workflows/pypi.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      976 2021-12-30 10:11:24.000000 damona-0.8.3/.gitignore
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      340 2023-04-11 13:45:36.000000 damona-0.8.3/.readthedocs.yml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1574 2020-08-25 18:37:15.000000 damona-0.8.3/CONTRIBUTING.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1532 2020-08-10 11:26:10.000000 damona-0.8.3/LICENSE
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      244 2022-01-19 17:14:01.000000 damona-0.8.3/MANIFEST.in
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17299 2023-04-14 09:55:16.297055 damona-0.8.3/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16010 2023-04-12 15:49:38.000000 damona-0.8.3/README.rst
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.254055 damona-0.8.3/damona/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1481 2022-01-19 10:34:27.000000 damona-0.8.3/damona/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3114 2022-01-19 11:46:01.000000 damona-0.8.3/damona/admin.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.255055 damona-0.8.3/damona/biocontainers/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-18 11:56:04.000000 damona-0.8.3/damona/biocontainers/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)  3790743 2022-01-19 12:13:06.000000 damona-0.8.3/damona/biocontainers/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6105 2021-12-31 09:42:03.000000 damona-0.8.3/damona/builders.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13000 2022-01-19 11:00:41.000000 damona-0.8.3/damona/common.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5315 2021-12-31 10:56:58.000000 damona-0.8.3/damona/config.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    15657 2021-12-31 15:14:31.000000 damona-0.8.3/damona/environ.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    22582 2022-01-19 12:09:57.000000 damona-0.8.3/damona/install.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.259055 damona-0.8.3/damona/library/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.260055 damona-0.8.3/damona/library/R/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      119 2020-08-04 13:32:55.000000 damona-0.8.3/damona/library/R/Makefile
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1588 2020-08-11 20:17:37.000000 damona-0.8.3/damona/library/R/Singularity.R_3.6.3
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1589 2021-03-19 12:22:16.000000 damona-0.8.3/damona/library/R/Singularity.R_4.0.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      144 2021-03-19 12:18:31.000000 damona-0.8.3/damona/library/R/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-12-29 10:11:19.000000 damona-0.8.3/damona/library/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.261055 damona-0.8.3/damona/library/conda/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      521 2021-12-22 14:56:38.000000 damona-0.8.3/damona/library/conda/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3358 2021-02-22 19:31:08.000000 damona-0.8.3/damona/library/conda/Singularity.conda_4.7.12
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2621 2022-11-08 16:04:03.000000 damona-0.8.3/damona/library/conda/Singularity.conda_4.9.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      212 2021-12-22 14:55:56.000000 damona-0.8.3/damona/library/conda/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.261055 damona-0.8.3/damona/library/rust/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      272 2022-08-26 07:32:05.000000 damona-0.8.3/damona/library/rust/Singularity.rust
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.262055 damona-0.8.3/damona/library/ubuntu/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      724 2021-09-02 15:44:16.000000 damona-0.8.3/damona/library/ubuntu/Singularity.ubuntu_16.04
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3391 2021-09-02 15:44:16.000000 damona-0.8.3/damona/library/ubuntu/Singularity.ubuntu_18.04
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      166 2021-09-02 15:44:16.000000 damona-0.8.3/damona/library/ubuntu/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.262055 damona-0.8.3/damona/papers/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-19 11:53:53.000000 damona-0.8.3/damona/papers/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    16088 2023-04-10 17:45:28.000000 damona-0.8.3/damona/registry.py
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)    26465 2023-02-21 11:15:46.000000 damona-0.8.3/damona/script.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.262055 damona-0.8.3/damona/shell/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-09-01 19:41:28.000000 damona-0.8.3/damona/shell/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/shell/bash/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2021-12-30 11:40:38.000000 damona-0.8.3/damona/shell/bash/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5636 2021-12-30 10:08:08.000000 damona-0.8.3/damona/shell/bash/damona.sh
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      809 2021-09-02 15:44:17.000000 damona-0.8.3/damona/shell/damona_comp.sh
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/shell/fish/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3320 2021-12-30 10:03:26.000000 damona-0.8.3/damona/shell/fish/damona.fish
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/software/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.263055 damona-0.8.3/damona/software/RIPseeker/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      983 2023-03-27 15:34:19.000000 damona-0.8.3/damona/software/RIPseeker/Singularity.RIPseeker_1.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      668 2023-03-22 09:02:18.000000 damona-0.8.3/damona/software/RIPseeker/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-08-04 13:32:55.000000 damona-0.8.3/damona/software/__init__.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.264055 damona-0.8.3/damona/software/art/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      296 2021-11-13 18:22:59.000000 damona-0.8.3/damona/software/art/Singularity.art_2.5.8
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      293 2021-11-13 18:23:34.000000 damona-0.8.3/damona/software/art/Singularity.art_3.11.14
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      530 2022-02-22 14:07:33.000000 damona-0.8.3/damona/software/art/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.265055 damona-0.8.3/damona/software/bamtools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      977 2023-02-17 16:03:17.000000 damona-0.8.3/damona/software/bamtools/Singularity.bamtools_2.5.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      286 2022-11-22 08:10:42.000000 damona-0.8.3/damona/software/bamtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.265055 damona-0.8.3/damona/software/bbtools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      439 2021-12-31 14:51:14.000000 damona-0.8.3/damona/software/bbtools/Singularity.bbtools_38.94.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3102 2021-12-31 14:58:24.000000 damona-0.8.3/damona/software/bbtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.266055 damona-0.8.3/damona/software/bcl2fastq/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      160 2020-08-12 08:05:20.000000 damona-0.8.3/damona/software/bcl2fastq/Makefile
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1140 2021-12-08 13:09:00.000000 damona-0.8.3/damona/software/bcl2fastq/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2020-08-11 20:07:37.000000 damona-0.8.3/damona/software/bcl2fastq/Singularity.bcl2fastq_2.20.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      298 2021-09-02 16:37:43.000000 damona-0.8.3/damona/software/bcl2fastq/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.267055 damona-0.8.3/damona/software/bedtools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      955 2022-11-22 09:58:55.000000 damona-0.8.3/damona/software/bedtools/Singularity.bedtools_2.30.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2022-11-22 09:54:23.000000 damona-0.8.3/damona/software/bedtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.268055 damona-0.8.3/damona/software/bioconvert/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1858 2022-08-30 12:01:29.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1753 2022-12-21 19:41:04.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1769 2023-03-07 09:19:34.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1770 2023-03-07 09:58:04.000000 damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_1.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      880 2023-03-07 11:48:52.000000 damona-0.8.3/damona/software/bioconvert/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.268055 damona-0.8.3/damona/software/bowtie/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      956 2022-11-22 15:10:01.000000 damona-0.8.3/damona/software/bowtie/Singularity.bowtie_1.3.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      402 2021-12-30 14:16:40.000000 damona-0.8.3/damona/software/bowtie/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.269055 damona-0.8.3/damona/software/bowtie2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      918 2021-12-07 22:46:55.000000 damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.3.4
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      912 2021-12-22 18:04:18.000000 damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.4.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      606 2021-12-08 13:33:41.000000 damona-0.8.3/damona/software/bowtie2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.269055 damona-0.8.3/damona/software/busco/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2706 2023-04-06 14:03:40.000000 damona-0.8.3/damona/software/busco/Singularity.busco_5.4.6
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      279 2023-04-06 14:03:40.000000 damona-0.8.3/damona/software/busco/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.270055 damona-0.8.3/damona/software/bwa/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1162 2023-03-15 10:44:53.000000 damona-0.8.3/damona/software/bwa/Singularity.bwa_0.7.17
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      256 2023-03-15 10:45:44.000000 damona-0.8.3/damona/software/bwa/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.271055 damona-0.8.3/damona/software/canu/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      322 2023-04-06 14:05:13.000000 damona-0.8.3/damona/software/canu/Singularity.canu_1.6.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      322 2021-12-07 22:29:23.000000 damona-0.8.3/damona/software/canu/Singularity.canu_1.8.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      753 2023-04-07 10:00:30.000000 damona-0.8.3/damona/software/canu/Singularity.canu_2.1.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      652 2023-04-07 10:04:55.000000 damona-0.8.3/damona/software/canu/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.271055 damona-0.8.3/damona/software/ccs/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      334 2023-04-11 10:33:31.000000 damona-0.8.3/damona/software/ccs/Singularity.ccs_6.4.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      271 2023-04-11 10:35:40.000000 damona-0.8.3/damona/software/ccs/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.272055 damona-0.8.3/damona/software/circlator/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2779 2023-04-12 13:41:45.000000 damona-0.8.3/damona/software/circlator/Singularity.circlator_1.5.5
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      268 2023-04-12 13:48:17.000000 damona-0.8.3/damona/software/circlator/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.272055 damona-0.8.3/damona/software/falco/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      531 2022-08-22 09:04:26.000000 damona-0.8.3/damona/software/falco/Singularity.falco_0.2.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      778 2022-08-22 10:14:18.000000 damona-0.8.3/damona/software/falco/Singularity.falco_1.0.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      497 2022-08-22 14:26:58.000000 damona-0.8.3/damona/software/falco/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.273055 damona-0.8.3/damona/software/fastp/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      445 2022-11-14 16:32:09.000000 damona-0.8.3/damona/software/fastp/Singularity.fastp_0.23.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      462 2022-11-16 13:29:53.000000 damona-0.8.3/damona/software/fastp/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.274055 damona-0.8.3/damona/software/fastqc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      522 2020-08-11 20:13:30.000000 damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.8
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      492 2021-02-12 14:59:23.000000 damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.9
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      705 2022-11-22 13:28:06.000000 damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.9_py3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      658 2022-12-16 09:49:55.000000 damona-0.8.3/damona/software/fastqc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.274055 damona-0.8.3/damona/software/flye/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      388 2021-11-26 14:49:41.000000 damona-0.8.3/damona/software/flye/Singularity.flye_2.9.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      357 2023-03-14 16:03:34.000000 damona-0.8.3/damona/software/flye/Singularity.flye_2.9.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      464 2023-03-15 08:43:07.000000 damona-0.8.3/damona/software/flye/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.275055 damona-0.8.3/damona/software/gffread/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      601 2020-08-11 20:15:32.000000 damona-0.8.3/damona/software/gffread/Singularity.gffread_0.12.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      266 2021-12-22 17:57:32.000000 damona-0.8.3/damona/software/gffread/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.276055 damona-0.8.3/damona/software/graphviz/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      279 2023-04-11 20:29:23.000000 damona-0.8.3/damona/software/graphviz/Singularity.graphviz_2.43.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2021-12-08 13:44:16.000000 damona-0.8.3/damona/software/graphviz/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      183 2021-12-08 13:41:34.000000 damona-0.8.3/damona/software/graphviz/test.dot
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      192 2021-12-22 20:51:22.000000 damona-0.8.3/damona/software/graphviz/test.sh
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.276055 damona-0.8.3/damona/software/gzip/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      180 2022-08-30 09:44:02.000000 damona-0.8.3/damona/software/gzip/Singularity.gzip_1.9.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-08-30 09:51:19.000000 damona-0.8.3/damona/software/gzip/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.277055 damona-0.8.3/damona/software/hifiasm/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      695 2023-03-15 11:04:46.000000 damona-0.8.3/damona/software/hifiasm/Singularity.hifiasm_0.19.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      265 2023-03-15 13:49:27.000000 damona-0.8.3/damona/software/hifiasm/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.277055 damona-0.8.3/damona/software/hisat2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2021-12-22 15:20:09.000000 damona-0.8.3/damona/software/hisat2/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      188 2022-01-14 16:44:28.000000 damona-0.8.3/damona/software/hisat2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.278055 damona-0.8.3/damona/software/homer/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      482 2022-11-08 20:13:27.000000 damona-0.8.3/damona/software/homer/Singularity.homer_4.11.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      297 2022-11-08 20:26:09.000000 damona-0.8.3/damona/software/homer/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.278055 damona-0.8.3/damona/software/idr/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      699 2022-12-07 21:29:04.000000 damona-0.8.3/damona/software/idr/Singularity.idr_2.0.3
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      272 2022-11-08 19:56:00.000000 damona-0.8.3/damona/software/idr/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.278055 damona-0.8.3/damona/software/igvtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1367 2022-08-25 09:41:44.000000 damona-0.8.3/damona/software/igvtools/Singularity.igvtools_2.12.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      293 2022-08-25 15:40:00.000000 damona-0.8.3/damona/software/igvtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.279055 damona-0.8.3/damona/software/kraken/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      140 2020-08-04 13:32:55.000000 damona-0.8.3/damona/software/kraken/Makefile
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      638 2020-08-11 20:16:50.000000 damona-0.8.3/damona/software/kraken/Singularity.kraken_1.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      904 2020-08-11 20:16:44.000000 damona-0.8.3/damona/software/kraken/Singularity.kraken_2.0.9
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      604 2021-12-23 10:47:17.000000 damona-0.8.3/damona/software/kraken/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.280055 damona-0.8.3/damona/software/mergegi/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      448 2022-12-09 10:41:16.000000 damona-0.8.3/damona/software/mergegi/Singularity.mergegi_0.0.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      291 2022-12-09 10:43:14.000000 damona-0.8.3/damona/software/mergegi/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.281055 damona-0.8.3/damona/software/minimap2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      681 2021-12-22 17:36:12.000000 damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.17.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      589 2023-04-07 15:31:23.000000 damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.23.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      478 2023-04-11 20:17:17.000000 damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.24.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      675 2023-04-11 13:46:34.000000 damona-0.8.3/damona/software/minimap2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.281055 damona-0.8.3/damona/software/pbbam/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1062 2023-04-11 10:14:40.000000 damona-0.8.3/damona/software/pbbam/Singularity.pbbam_2.1.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1297 2023-04-11 10:14:58.000000 damona-0.8.3/damona/software/pbbam/Singularity.pbbam_2.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      495 2023-04-11 10:35:46.000000 damona-0.8.3/damona/software/pbbam/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.282055 damona-0.8.3/damona/software/phantompeakqualtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      942 2022-11-07 19:50:54.000000 damona-0.8.3/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      522 2022-11-10 20:11:13.000000 damona-0.8.3/damona/software/phantompeakqualtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.282055 damona-0.8.3/damona/software/picard/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      523 2022-09-20 21:09:49.000000 damona-0.8.3/damona/software/picard/Singularity.picard_2.26
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.282055 damona-0.8.3/damona/software/pigz/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      185 2022-11-22 10:01:11.000000 damona-0.8.3/damona/software/pigz/Singularity.pigz_2.4.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-11-22 10:03:15.000000 damona-0.8.3/damona/software/pigz/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.283055 damona-0.8.3/damona/software/polypolish/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      630 2023-03-07 09:07:51.000000 damona-0.8.3/damona/software/polypolish/Singularity.polypolish_0.5.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      269 2023-03-07 09:14:59.000000 damona-0.8.3/damona/software/polypolish/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.283055 damona-0.8.3/damona/software/prokka/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      617 2021-05-05 09:12:20.000000 damona-0.8.3/damona/software/prokka/Singularity.prokka_1.14.5
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      238 2021-11-21 15:26:58.000000 damona-0.8.3/damona/software/prokka/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.284055 damona-0.8.3/damona/software/pycoqc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      103 2023-03-17 16:01:16.000000 damona-0.8.3/damona/software/pycoqc/Singularity.pycoqc_2.5.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      281 2023-03-17 21:36:36.000000 damona-0.8.3/damona/software/pycoqc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.284055 damona-0.8.3/damona/software/quast/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      638 2021-11-17 23:21:58.000000 damona-0.8.3/damona/software/quast/Singularity.quast_5.0.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      261 2021-12-22 18:38:46.000000 damona-0.8.3/damona/software/quast/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.285055 damona-0.8.3/damona/software/rnadiff/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      930 2022-12-20 12:52:53.000000 damona-0.8.3/damona/software/rnadiff/Singularity.rnadiff_1.7.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      264 2022-12-20 12:53:05.000000 damona-0.8.3/damona/software/rnadiff/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.285055 damona-0.8.3/damona/software/rnaseqc/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      531 2020-08-25 09:13:07.000000 damona-0.8.3/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      266 2021-12-22 18:39:26.000000 damona-0.8.3/damona/software/rnaseqc/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.286055 damona-0.8.3/damona/software/rtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      406 2021-03-19 14:03:02.000000 damona-0.8.3/damona/software/rtools/Singularity.rtools_1.0.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      509 2023-02-17 14:08:13.000000 damona-0.8.3/damona/software/rtools/Singularity.rtools_1.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      791 2023-02-20 09:57:39.000000 damona-0.8.3/damona/software/rtools/Singularity.rtools_1.2.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      668 2023-02-21 22:55:12.000000 damona-0.8.3/damona/software/rtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.287055 damona-0.8.3/damona/software/salmon/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      179 2020-08-04 13:32:55.000000 damona-0.8.3/damona/software/salmon/Makefile
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      594 2022-08-30 09:55:04.000000 damona-0.8.3/damona/software/salmon/Singularity.salmon_1.3.0
+-rw-rw----   0 cokelaer  (1000) cokelaer  (1000)      281 2022-08-25 15:43:58.000000 damona-0.8.3/damona/software/salmon/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.288055 damona-0.8.3/damona/software/samtools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      805 2022-12-14 13:49:36.000000 damona-0.8.3/damona/software/samtools/Singularity.samtools_1.15.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      818 2023-04-08 20:18:25.000000 damona-0.8.3/damona/software/samtools/Singularity.samtools_1.16.1
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      482 2022-12-14 14:46:18.000000 damona-0.8.3/damona/software/samtools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.288055 damona-0.8.3/damona/software/samtools_minimap2/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      906 2023-04-11 13:29:17.000000 damona-0.8.3/damona/software/samtools_minimap2/Singularity.samtools_1.17_minimap2_2.24.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      296 2023-04-12 15:46:15.000000 damona-0.8.3/damona/software/samtools_minimap2/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.289055 damona-0.8.3/damona/software/seqkit/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      548 2023-04-12 13:51:51.000000 damona-0.8.3/damona/software/seqkit/Singularity.seqkit_2.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      389 2023-04-12 13:51:58.000000 damona-0.8.3/damona/software/seqkit/Singularity.seqkit_2.4.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      451 2023-04-12 13:55:18.000000 damona-0.8.3/damona/software/seqkit/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.289055 damona-0.8.3/damona/software/seqtk/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      498 2021-11-26 14:19:46.000000 damona-0.8.3/damona/software/seqtk/Singularity.seqtk_1.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      259 2021-11-26 14:07:18.000000 damona-0.8.3/damona/software/seqtk/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.290055 damona-0.8.3/damona/software/sequana/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1022 2023-04-06 14:09:18.000000 damona-0.8.3/damona/software/sequana/Singularity.sequana_0.12.6
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1037 2023-03-14 19:53:08.000000 damona-0.8.3/damona/software/sequana/Singularity.sequana_0.14.6
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      514 2023-03-15 08:42:48.000000 damona-0.8.3/damona/software/sequana/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.291055 damona-0.8.3/damona/software/sequana_denovo/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5201 2023-04-12 14:04:40.000000 damona-0.8.3/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      342 2022-11-18 20:00:11.000000 damona-0.8.3/damona/software/sequana_denovo/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.292055 damona-0.8.3/damona/software/sequana_perl_tools/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      637 2021-05-05 09:13:25.000000 damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      644 2022-11-18 15:12:46.000000 damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5197 2022-11-18 15:39:03.000000 damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      689 2022-11-08 20:04:09.000000 damona-0.8.3/damona/software/sequana_perl_tools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.292055 damona-0.8.3/damona/software/sequana_ribofinder/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     1484 2022-11-22 16:28:40.000000 damona-0.8.3/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      288 2022-11-22 16:27:58.000000 damona-0.8.3/damona/software/sequana_ribofinder/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.294055 damona-0.8.3/damona/software/sequana_tools/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      427 2022-11-14 15:42:49.000000 damona-0.8.3/damona/software/sequana_tools/README.txt
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2156 2021-03-29 14:32:32.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2242 2021-07-24 20:18:11.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2241 2022-08-30 09:52:49.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2338 2022-12-20 15:01:03.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      695 2022-09-21 07:48:13.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      640 2022-09-21 07:45:54.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      366 2023-02-06 10:24:17.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.5
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      391 2023-02-06 10:23:27.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.6
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     2641 2021-03-19 12:11:02.000000 damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5990 2023-04-11 14:46:53.000000 damona-0.8.3/damona/software/sequana_tools/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.295055 damona-0.8.3/damona/software/shustring/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      463 2023-02-21 11:04:27.000000 damona-0.8.3/damona/software/shustring/Singularity.shustring_2.6.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      289 2023-02-21 11:44:36.000000 damona-0.8.3/damona/software/shustring/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.295055 damona-0.8.3/damona/software/snpeff/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1185 2022-11-18 20:58:56.000000 damona-0.8.3/damona/software/snpeff/Singularity.snpeff_5.1.0
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.296055 damona-0.8.3/damona/software/trf/
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      891 2021-03-08 19:58:50.000000 damona-0.8.3/damona/software/trf/Singularity.trf_4.10.0
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      198 2021-11-17 22:03:28.000000 damona-0.8.3/damona/software/trf/registry.yaml
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.296055 damona-0.8.3/damona/software/ucsc/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       88 2021-12-23 14:08:59.000000 damona-0.8.3/damona/software/ucsc/README.rst
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      521 2022-12-13 15:40:07.000000 damona-0.8.3/damona/software/ucsc/Singularity.ucsc_3.7.7
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      356 2022-12-13 15:23:14.000000 damona-0.8.3/damona/software/ucsc/registry.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    13985 2023-04-10 20:57:40.000000 damona-0.8.3/damona/zenodo.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-04-14 09:55:16.254055 damona-0.8.3/damona.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    17299 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8019 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/dependency_links.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       46 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2021-09-02 15:44:05.000000 damona-0.8.3/damona.egg-info/not-zip-safe
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      222 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/requires.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        7 2023-04-14 09:55:16.000000 damona-0.8.3/damona.egg-info/top_level.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       78 2021-12-23 15:50:31.000000 damona-0.8.3/requirements.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      312 2023-04-14 09:55:16.297055 damona-0.8.3/setup.cfg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4822 2023-04-11 13:45:20.000000 damona-0.8.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `damona-0.8.2/CONTRIBUTING.rst` & `damona-0.8.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/LICENSE` & `damona-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/PKG-INFO` & `damona-0.8.3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,455 +1,431 @@
-Metadata-Version: 2.1
-Name: damona
-Version: 0.8.2
-Summary: A set of NGS singularity recipes, built for you and easily downlable
-Home-page: http://github.com/sequana/sequana
-Author: Thomas Cokelaer
-Author-email: thomas.cokelaer@pasteur.fr
-Maintainer: Thomas Cokelaer
-Maintainer-email: thomas.cokelaer@pasteur.fr
-License: new BSD
-Download-URL: https://github.com/sequana/sequana/archive/0.8.2.tar.gz
-Description: DAMONA
-        ######
-        
-        
-        .. image:: https://badge.fury.io/py/damona.svg
-            :target: https://pypi.python.org/pypi/damona
-        
-        
-        .. image:: https://github.com/cokelaer/damona/actions/workflows/main.yml/badge.svg
-           :target: https://github.com/cokelaer/damona/actions/workflows/main.yml
-        
-        .. image:: https://coveralls.io/repos/github/cokelaer/damona/badge.svg?branch=master
-            :target: https://coveralls.io/github/cokelaer/damona?branch=master
-        
-        .. image:: http://readthedocs.org/projects/damona/badge/?version=latest
-            :target: http://damona.readthedocs.org/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://zenodo.org/badge/282275608.svg
-           :target: https://zenodo.org/badge/latestdoi/282275608
-        
-        
-        :Python version: Python 3.7, 3.8, 3.9
-        :Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
-        :Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
-        :Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
-        
-        Overview
-        ========
-        
-        Damona is a singularity environment manager.
-        
-        Damona started as a small collections of singularity recipes to help installing third-party tools for
-        `Sequana NGS pipelines <https://sequana.readthedocs.io>`_.
-        
-        Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
-        
-        In a nutshell, Damona combines the logic of Conda environments with the
-        reproducibility of singularity containers. We believe that it could be useful for
-        other projects and therefore decided to release it as an independent tool.
-        
-        As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
-        
-        Installation
-        ============
-        
-        If you are in a hurry, just type::
-        
-            pip install damona --upgrade
-        
-        You must install `Singularity <https://sylabs.io/docs>`_ to make use of **Damona**. 
-        
-        If you are familiar with conda, I believe you can do::
-        
-            conda install singularity
-        
-        Type **damona** in a shell. This will initiate the tool with a config file in your HOME/.config/damona directory for bash shell and `fish shell <https://fishshell.com/>`_ users.
-        
-        Bash users should add this code in their ~/.bashrc file::
-        
-            source ~/.config/damona/damona.sh
-        
-        and fishshell users should add the following code in their ~/.config/fish/config.fish file::
-        
-            source ~/.config/damona/damona.fish
-        
-        Open a new shell and you are ready to go. Please see the `Installation in details`_ section for more information.
-        
-        Quick Start
-        ===========
-        
-        **Damona** needs environments to work with.
-        First, let us *create* one, which is called TEST::
-        
-            damona env --create TEST
-        
-        Second, we need to *activate* it. Subsequent insallation will happen in this environment::
-        
-            damona activate TEST
-        
-        From there, we can install some binaries/images::
-        
-            damona install fastqc:0.11.9
-        
-        That's it. Time to test. Type **fastqc**.
-        
-        To rename this TEST example::
-        
-            damona env --rename TEST --new-name prod
-        
-        or delete it::
-        
-            damona env --delete prod
-        
-        See more examples hereafter or in the user guide on https://damona.readthedocs.io
-        
-        Motivation
-        ==========
-        
-        As stated on their website, `Conda <https:/docs.conda.io/en/latest>`_ is
-        an open source **package** management system
-        and **environment** management system.
-        Conda provides pre-compiled releases of software; they can be installed in
-        different local environments that do not interfer with your system. This has
-        great advantages for developers. For example, you can install a pre-compiled
-        libraries in a minute instead of trying to compile it yourself including all
-        dependencies. Different communities have emerged using this
-        framework. One of them is `Bioconda <https://bioconda.github.io>`_, which is dedicated to bioinformatics.
-        
-        Another great tool that emerged in the last years is
-        `Singularity <https://sylabs.io/docs>`_. Singularity containers can be used
-        to package entire scientific workflows,
-        software and libraries, and even data. It is a simple file that can be shared
-        between environments and guarantee exectution and reproducibility.
-        
-        Originally, Conda provided pre-compiled version of a software. Nowadays, it also provides
-        a docker and a singularity image of the tool. On the other side, Singularity can include an
-        entire conda environment. As you can see everything is there to build reproducible tools and
-        environment.
-        
-        Now, what about a software in development that depends on third-party packages ? 
-        You would create a conda environment and starts installing the required packages.
-        Quickly, you will install another package that will break your environment due
-        to unresolved conlicts; this is not common but it happens. In the worst case
-        scenario, the environment is broken. In facilities where users depends on you,
-        it can be quite stresful and time-consuming to maintain several such
-        environments. This is why we have moved little by little to a very light conda
-        environment where known-to-cause-problem packages have been shipped into
-        singularity containers. This means we have to create aliases to those
-        singularities. The singularities can be simple executable containers or full
-        environment containers with many executables inside. In both cases, one need to
-        manage those containers for different users, pipelines, versions etc. This
-        started to be cumbersome to have containers in different places and update
-        script that generate the aliases to those executables.
-        
-        
-        That's where **damona** started: we wanted to combine the conda-like environment 
-        framework to manage our singularity containers more easily.
-        
-        Although **Damona** was started with the `Sequana projet <https://sequana.readthedocs.io>`_,
-        **Damona** may be useful for others developers who wish to have a quick and easy
-        solution for their users when they need to install third-party libraries.
-        
-        Before showing real-case examples, let us install the software itself and 
-        understand the details.
-        
-        
-        
-        Installation in details
-        =======================
-        
-        The is the egg and chicken paradox. To get reproducible container with
-        singularity, at some point you need to install singularity itself. That the first
-        of the two software that you will need to install. Instructions
-        are on `singularity web site <https://sylabs.io/guides/3.6/user-guide/>`_. This
-        is not obvious to be honest. You need the GO language to be installed as well. I
-        personally installed from source and it worked like a charm.
-        
-        Second, you need **Damona**. This is a pure Python sotfware with only a few
-        dependencies. Install it with the **pip** software provided with your Python
-        installation (Python 3.X)::
-        
-            pip install damona --upgrade
-        
-        Type **damona** to create the Damona tree structure. Images and binaries 
-        will be saved in your home directory within the
-        ~/.config/damona directory. There, special files should be available:
-        **damona.sh**, **damona.fish**  and **damona.cfg**. Check that those files are present.
-        
-        Finally, you need to tell your system where to find damona. For bashrc users,
-        please add this line to you bashrc file::
-        
-            source ~/.config/damona/damona.sh
-        
-        open a new shell and type **damona** and you should be ready to go.
-        
-        For fishshell users, please add this line in **~/.config/fish/config.fish***::
-        
-            source ~/.config/damona/damona.fish
-        
-        Tutorial
-        ============
-        
-        The **Damona** standalone is called **damona**. It has a documentation that should suffice for most users.
-        
-        The main documentation is obtained using::
-        
-            damona --help
-        
-        where you will see the list of **Damona** commands (may be different with time) (may be::
-        
-            activate
-            clean
-            deactivate
-            env
-            export
-            info
-            install
-            list
-            remove
-            search
-            stats
-        
-        To get help for the *install* command, type::
-        
-            damona install --help
-        
-        
-        1. *list* available environments
-        --------------------------------
-        
-        By default you have an environment called **base**. Unlike the **base** environment found in **conda**, it is not
-        essential and may be altered. However, it cannot be removed or created. You can check the list of environments using::
-        
-            damona env
-        
-        2. *create* environments
-        ------------------------
-        All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
-        
-            damona env --create TEST
-        
-        There, you have a *bin* directory where binaries are going to be installed.
-        
-        You can check that it has been created::
-        
-            damona env
-        
-        Note the last line telling you that::
-        
-            Your current env is 'TEST'.
-        
-        3. activate and deactivate environments
-        ----------------------------------------
-        
-        In order to install new binaries or software package, you must activate an environment. You may activate several but the last one is the *active* one. Let us activate the *TEST* environment::
-        
-            damona activate TEST
-        
-        Check that it is active using::
-        
-            damona env
-        
-        and look at the last line. It should look like::
-        
-            Your current env is 'TEST'.
-        
-        What is going on when you activate an environment called TEST ? Simple: we append the directory ~/.config/damona/envs/TEST/bin to your PATH where binaries are searched for. This directory is removed when you use the *deactivate* command.
-        
-        ::
-        
-            damona deactivate TEST
-            damona env 
-        
-        should remove the TEST environment from your PATH. You may activate several and deactivate them. In such case, the
-        environments behave as a Last In First Out principle::
-        
-            damona activate base
-            damona activate TEST
-            damona deactivate 
-        
-        Removes the last activated environments. While this set of commands is more specific::
-        
-            damona activate base
-            damona activate TEST
-            damona deactivate base
-        
-        and keep the TEST environment only in your PATH.
-        
-        4. **install** a software
-        --------------------------
-        
-        Let us now consider that the TEST environment is active.
-        
-        Damona provides software that may have several releases. Each software/release comes with binaries that will be
-        installed together with the underlying singularity image.::
-        
-            damona install fastqc:0.11.9
-        
-        Here, the singularity image corresponding to the release 0.11.9 of the **fastqc** software is downloaded. Then, binaries registered in this release are installed (here the **fastqc** binary only).
-        
-        All images are stored in *~/.config/damona/images* and are shared between environments. 
-        
-        
-        5. Get **info** about installed images and binaries
-        ----------------------------------------------------
-        
-        You can get the binaries installed in an environment (and the images used by
-        them) using the **info** command::
-        
-            damona info TEST
-        
-        
-        6. Search the registry
-        ------------------------
-        
-        By default, we provide recipes (26 in Dec 2021 ; 38 releases) available in **Damona**. 
-        They can be searched for using::
-        
-            damona search PATTERN
-        
-        External registry can be set-up. For instance, a damona registry is accessible
-        as follows (for demonstration)::
-        
-            damona search fastqc --url damona
-        
-        Where *damona* is an alias defined in the .config/damona/damona.cfg that
-        is set to https://biomics.pasteur.fr/drylab/damona/registry.txt
-        
-        You may retrieve images from a website where a registry exists (see the developer
-        guide to create a registry yourself).
-        
-        
-        7. combine two different environments
-        --------------------------------------
-        
-        In damona, you can have sereral environments in parallel and later activate the
-        one you wish to use. Let us create a new one::
-        
-            damone env --create test1
-        
-        and check that you now have one more environment::
-        
-            damona env
-        
-        We want to create an alias to the previously downloaded image of fastqc tool but
-        in the *test1* environment. First we activate the newly create environment::
-        
-            damona activate test1
-        
-        then, we install the container::
-        
-            damona install fastqc:0.11.9
-        
-        This will not download the image again. It will just create a binary in the
-        ~/.config/damona/envs/test1/bin directory.
-        
-        you can combine this new environemnt with the base one::
-        
-            damona activate base
-        
-        If you are interested to know more, please see the User Guide and Developer
-        guide here below.
-        
-        Changelog
-        =========
-        
-        ========= ========================================================================
-        Version   Description
-        ========= ========================================================================
-        0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
-                  * add seqkit recipe and container
-                  * add shustring
-        0.8.1     * Include ability to interact with biocontainers by allowing retrieval
-                    of all biocontainers docker images using this syntax:
-                    'damona install biocontainers/xx:1.2.3' Note that although 9000 
-                    containers are available, in practice, only about 1000 dockers are 
-                    on dockerhub, which is already nice :-)
-                  * 
-        0.8.0     * Fix regression to install a software with its version
-        0.7.1     * Implement the fish shell 
-                  * add command "damona list"
-                  * rename recipes/ directory into software/ and created a new library/ 
-                    directory for images used as library, that are not installed.
-        0.7.0     * Check that singularity is installed
-                  * implement the remove command 
-                    https://github.com/cokelaer/damona/issues/15
-                  * more recipes cleanup (https://github.com/cokelaer/damona/issues/12)
-                  * removed damona recipes (pure python package)
-                  * cleanup all recipes
-                  * add zenodo stats (for admin)
-        0.6.0     * add ability to upload images on zenodo. No need for external 
-                    repositories.
-                  * ability to add/delete a software from different images
-                  * implement --help for the activate/deactivate (non trivial)
-                  * add --rename option in 'damona env'
-                  * 'base' environment is now at the same level as other environments
-                  * better bash script; no need for DAMONA_EXE variable anymore.
-        0.5.3     * Fixing config/shell 
-        0.5.2     * add missing shell package
-        0.5.1     * add DAMONA_SINGULARITY_OPTIONS env variable in the binary
-                  * Fix the way binaries are found in the releases.
-                  * new recipes: rtools
-                  * new releases: sequana_tools_0.10.0
-                  * Fix shell script to handle DAMONA_EXE variable 
-        0.5.0     * Major refactoring. 
-        
-                    - Simplification of the registries (dropping notion of exe/set 
-                      class
-                    - Main script should now be fully functional with functional
-                      activation/deactivation. 
-                    - New command to build images from local recipes or dockerhub 
-                      entries.
-                    - Install command can now install local container. 
-                    - DAMONA_PATH can be set to install damona images/binaries 
-                      anywhere, not just in local home. 
-                    - check md5 of images to not download/copy again
-        0.4.3     * Implement damona activate/deactivate
-        0.4.2     * Fix typo in the creation of aliases for 'set' containers
-        0.4.1     * implemented aliases for the --from-url option stored in a
-                    damona.cfg file
-        0.4.0     * implemented the 'env' and 'activate' command
-                  * ability to setup an external registry on any https and retrieve
-                    registry from there to download external images
-        0.3.X     * add gffread, rnadiff recipes
-        0.3.0     * A stable version with documentation and >95% coverage read-yto-use
-        0.2.3     * add new recipes (rnadiff)
-        0.2.2     * Download latest if no version provided
-                  * include *build* command to build image locally
-        0.2.1     fixed manifest
-        0.2.0     first working version of damona to pull image locally with binaries
-        0.1.1     small update to fix RTD, travis, coveralls
-        0.1       first release to test feasibility of the project
-        ========= ========================================================================
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-Keywords: NGS,singularity
-Platform: Linux
-Platform: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Provides-Extra: testing
-Provides-Extra: doc
+DAMONA
+######
+
+
+.. image:: https://badge.fury.io/py/damona.svg
+    :target: https://pypi.python.org/pypi/damona
+
+
+.. image:: https://github.com/cokelaer/damona/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/cokelaer/damona/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/cokelaer/damona/badge.svg?branch=master
+    :target: https://coveralls.io/github/cokelaer/damona?branch=master
+
+.. image:: http://readthedocs.org/projects/damona/badge/?version=latest
+    :target: http://damona.readthedocs.org/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://zenodo.org/badge/282275608.svg
+   :target: https://zenodo.org/badge/latestdoi/282275608
+
+
+:Python version: Python 3.7, 3.8, 3.9
+:Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
+:Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
+:Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
+
+Overview
+========
+
+Damona is a singularity environment manager.
+
+Damona started as a small collections of singularity recipes to help installing third-party tools for
+`Sequana NGS pipelines <https://sequana.readthedocs.io>`_.
+
+Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
+
+In a nutshell, Damona combines the logic of Conda environments with the
+reproducibility of singularity containers. We believe that it could be useful for
+other projects and therefore decided to release it as an independent tool.
+
+As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
+
+Installation
+============
+
+If you are in a hurry, just type::
+
+    pip install damona --upgrade
+
+You must install `Singularity <https://sylabs.io/docs>`_ to make use of **Damona**. 
+
+If you are familiar with conda, I believe you can do::
+
+    conda install singularity
+
+Type **damona** in a shell. This will initiate the tool with a config file in your HOME/.config/damona directory for bash shell and `fish shell <https://fishshell.com/>`_ users.
+
+Bash users should add this code in their ~/.bashrc file::
+
+    source ~/.config/damona/damona.sh
+
+and fishshell users should add the following code in their ~/.config/fish/config.fish file::
+
+    source ~/.config/damona/damona.fish
+
+Open a new shell and you are ready to go. Please see the `Installation in details`_ section for more information.
+
+Quick Start
+===========
+
+**Damona** needs environments to work with.
+First, let us *create* one, which is called TEST::
+
+    damona env --create TEST
+
+Second, we need to *activate* it. Subsequent insallation will happen in this environment::
+
+    damona activate TEST
+
+From there, we can install some binaries/images::
+
+    damona install fastqc:0.11.9
+
+That's it. Time to test. Type **fastqc**.
+
+To rename this TEST example::
+
+    damona env --rename TEST --new-name prod
+
+or delete it::
+
+    damona env --delete prod
+
+See more examples hereafter or in the user guide on https://damona.readthedocs.io
+
+Motivation
+==========
+
+As stated on their website, `Conda <https:/docs.conda.io/en/latest>`_ is
+an open source **package** management system
+and **environment** management system.
+Conda provides pre-compiled releases of software; they can be installed in
+different local environments that do not interfer with your system. This has
+great advantages for developers. For example, you can install a pre-compiled
+libraries in a minute instead of trying to compile it yourself including all
+dependencies. Different communities have emerged using this
+framework. One of them is `Bioconda <https://bioconda.github.io>`_, which is dedicated to bioinformatics.
+
+Another great tool that emerged in the last years is
+`Singularity <https://sylabs.io/docs>`_. Singularity containers can be used
+to package entire scientific workflows,
+software and libraries, and even data. It is a simple file that can be shared
+between environments and guarantee exectution and reproducibility.
+
+Originally, Conda provided pre-compiled version of a software. Nowadays, it also provides
+a docker and a singularity image of the tool. On the other side, Singularity can include an
+entire conda environment. As you can see everything is there to build reproducible tools and
+environment.
+
+Now, what about a software in development that depends on third-party packages ? 
+You would create a conda environment and starts installing the required packages.
+Quickly, you will install another package that will break your environment due
+to unresolved conlicts; this is not common but it happens. In the worst case
+scenario, the environment is broken. In facilities where users depends on you,
+it can be quite stresful and time-consuming to maintain several such
+environments. This is why we have moved little by little to a very light conda
+environment where known-to-cause-problem packages have been shipped into
+singularity containers. This means we have to create aliases to those
+singularities. The singularities can be simple executable containers or full
+environment containers with many executables inside. In both cases, one need to
+manage those containers for different users, pipelines, versions etc. This
+started to be cumbersome to have containers in different places and update
+script that generate the aliases to those executables.
+
+
+That's where **damona** started: we wanted to combine the conda-like environment 
+framework to manage our singularity containers more easily.
+
+Although **Damona** was started with the `Sequana projet <https://sequana.readthedocs.io>`_,
+**Damona** may be useful for others developers who wish to have a quick and easy
+solution for their users when they need to install third-party libraries.
+
+Before showing real-case examples, let us install the software itself and 
+understand the details.
+
+
+
+Installation in details
+=======================
+
+The is the egg and chicken paradox. To get reproducible container with
+singularity, at some point you need to install singularity itself. That the first
+of the two software that you will need to install. Instructions
+are on `singularity web site <https://sylabs.io/guides/3.6/user-guide/>`_. This
+is not obvious to be honest. You need the GO language to be installed as well. I
+personally installed from source and it worked like a charm.
+
+Second, you need **Damona**. This is a pure Python sotfware with only a few
+dependencies. Install it with the **pip** software provided with your Python
+installation (Python 3.X)::
+
+    pip install damona --upgrade
+
+Type **damona** to create the Damona tree structure. Images and binaries 
+will be saved in your home directory within the
+~/.config/damona directory. There, special files should be available:
+**damona.sh**, **damona.fish**  and **damona.cfg**. Check that those files are present.
+
+Finally, you need to tell your system where to find damona. For bashrc users,
+please add this line to you bashrc file::
+
+    source ~/.config/damona/damona.sh
+
+open a new shell and type **damona** and you should be ready to go.
+
+For fishshell users, please add this line in **~/.config/fish/config.fish***::
+
+    source ~/.config/damona/damona.fish
+
+Tutorial
+============
+
+The **Damona** standalone is called **damona**. It has a documentation that should suffice for most users.
+
+The main documentation is obtained using::
+
+    damona --help
+
+where you will see the list of **Damona** commands (may be different with time) (may be::
+
+    activate
+    clean
+    deactivate
+    env
+    export
+    info
+    install
+    list
+    remove
+    search
+    stats
+
+To get help for the *install* command, type::
+
+    damona install --help
+
+
+1. *list* available environments
+--------------------------------
+
+By default you have an environment called **base**. Unlike the **base** environment found in **conda**, it is not
+essential and may be altered. However, it cannot be removed or created. You can check the list of environments using::
+
+    damona env
+
+2. *create* environments
+------------------------
+All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
+
+    damona env --create TEST
+
+There, you have a *bin* directory where binaries are going to be installed.
+
+You can check that it has been created::
+
+    damona env
+
+Note the last line telling you that::
+
+    Your current env is 'TEST'.
+
+3. activate and deactivate environments
+----------------------------------------
+
+In order to install new binaries or software package, you must activate an environment. You may activate several but the last one is the *active* one. Let us activate the *TEST* environment::
+
+    damona activate TEST
+
+Check that it is active using::
+
+    damona env
+
+and look at the last line. It should look like::
+
+    Your current env is 'TEST'.
+
+What is going on when you activate an environment called TEST ? Simple: we append the directory ~/.config/damona/envs/TEST/bin to your PATH where binaries are searched for. This directory is removed when you use the *deactivate* command.
+
+::
+
+    damona deactivate TEST
+    damona env 
+
+should remove the TEST environment from your PATH. You may activate several and deactivate them. In such case, the
+environments behave as a Last In First Out principle::
+
+    damona activate base
+    damona activate TEST
+    damona deactivate 
+
+Removes the last activated environments. While this set of commands is more specific::
+
+    damona activate base
+    damona activate TEST
+    damona deactivate base
+
+and keep the TEST environment only in your PATH.
+
+4. **install** a software
+--------------------------
+
+Let us now consider that the TEST environment is active.
+
+Damona provides software that may have several releases. Each software/release comes with binaries that will be
+installed together with the underlying singularity image.::
+
+    damona install fastqc:0.11.9
+
+Here, the singularity image corresponding to the release 0.11.9 of the **fastqc** software is downloaded. Then, binaries registered in this release are installed (here the **fastqc** binary only).
+
+All images are stored in *~/.config/damona/images* and are shared between environments. 
+
+
+5. Get **info** about installed images and binaries
+----------------------------------------------------
+
+You can get the binaries installed in an environment (and the images used by
+them) using the **info** command::
+
+    damona info TEST
+
+
+6. Search the registry
+------------------------
+
+By default, we provide recipes (26 in Dec 2021 ; 38 releases) available in **Damona**. 
+They can be searched for using::
+
+    damona search PATTERN
+
+External registry can be set-up. For instance, a damona registry is accessible
+as follows (for demonstration)::
+
+    damona search fastqc --url damona
+
+Where *damona* is an alias defined in the .config/damona/damona.cfg that
+is set to https://biomics.pasteur.fr/drylab/damona/registry.txt
+
+You may retrieve images from a website where a registry exists (see the developer
+guide to create a registry yourself).
+
+
+7. combine two different environments
+--------------------------------------
+
+In damona, you can have sereral environments in parallel and later activate the
+one you wish to use. Let us create a new one::
+
+    damone env --create test1
+
+and check that you now have one more environment::
+
+    damona env
+
+We want to create an alias to the previously downloaded image of fastqc tool but
+in the *test1* environment. First we activate the newly create environment::
+
+    damona activate test1
+
+then, we install the container::
+
+    damona install fastqc:0.11.9
+
+This will not download the image again. It will just create a binary in the
+~/.config/damona/envs/test1/bin directory.
+
+you can combine this new environemnt with the base one::
+
+    damona activate base
+
+If you are interested to know more, please see the User Guide and Developer
+guide here below.
+
+
+
+Changelog
+=========
+
+========= ========================================================================
+Version   Description
+========= ========================================================================
+0.8.3     * create registry specifically for the sandbox (for testing)
+          * add damona community in the uploads
+          * add pbbam, bioconvert, busco, canu, ccs
+          * add polypolish, samtools 1.16.1, sequana 0.14.6, flye 2.9, canu 2.1.1
+            circlator 1.5.5, hifiasm
+0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
+          * add seqkit recipe and container
+          * add shustring
+0.8.1     * Include ability to interact with biocontainers by allowing retrieval
+            of all biocontainers docker images using this syntax:
+            'damona install biocontainers/xx:1.2.3' Note that although 9000 
+            containers are available, in practice, only about 1000 dockers are 
+            on dockerhub, which is already nice :-)
+          * 
+0.8.0     * Fix regression to install a software with its version
+0.7.1     * Implement the fish shell 
+          * add command "damona list"
+          * rename recipes/ directory into software/ and created a new library/ 
+            directory for images used as library, that are not installed.
+0.7.0     * Check that singularity is installed
+          * implement the remove command 
+            https://github.com/cokelaer/damona/issues/15
+          * more recipes cleanup (https://github.com/cokelaer/damona/issues/12)
+          * removed damona recipes (pure python package)
+          * cleanup all recipes
+          * add zenodo stats (for admin)
+0.6.0     * add ability to upload images on zenodo. No need for external 
+            repositories.
+          * ability to add/delete a software from different images
+          * implement --help for the activate/deactivate (non trivial)
+          * add --rename option in 'damona env'
+          * 'base' environment is now at the same level as other environments
+          * better bash script; no need for DAMONA_EXE variable anymore.
+0.5.3     * Fixing config/shell 
+0.5.2     * add missing shell package
+0.5.1     * add DAMONA_SINGULARITY_OPTIONS env variable in the binary
+          * Fix the way binaries are found in the releases.
+          * new recipes: rtools
+          * new releases: sequana_tools_0.10.0
+          * Fix shell script to handle DAMONA_EXE variable 
+0.5.0     * Major refactoring. 
+
+            - Simplification of the registries (dropping notion of exe/set 
+              class
+            - Main script should now be fully functional with functional
+              activation/deactivation. 
+            - New command to build images from local recipes or dockerhub 
+              entries.
+            - Install command can now install local container. 
+            - DAMONA_PATH can be set to install damona images/binaries 
+              anywhere, not just in local home. 
+            - check md5 of images to not download/copy again
+0.4.3     * Implement damona activate/deactivate
+0.4.2     * Fix typo in the creation of aliases for 'set' containers
+0.4.1     * implemented aliases for the --from-url option stored in a
+            damona.cfg file
+0.4.0     * implemented the 'env' and 'activate' command
+          * ability to setup an external registry on any https and retrieve
+            registry from there to download external images
+0.3.X     * add gffread, rnadiff recipes
+0.3.0     * A stable version with documentation and >95% coverage read-yto-use
+0.2.3     * add new recipes (rnadiff)
+0.2.2     * Download latest if no version provided
+          * include *build* command to build image locally
+0.2.1     fixed manifest
+0.2.0     first working version of damona to pull image locally with binaries
+0.1.1     small update to fix RTD, travis, coveralls
+0.1       first release to test feasibility of the project
+========= ========================================================================
+
+
+
+
+
+
+
+
+
+
```

### Comparing `damona-0.8.2/README.rst` & `damona-0.8.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: damona
+Version: 0.8.3
+Summary: A set of NGS singularity recipes, built for you and easily downlable
+Home-page: http://github.com/sequana/sequana
+Download-URL: https://github.com/sequana/sequana/archive/0.8.3.tar.gz
+Author: Thomas Cokelaer
+Author-email: thomas.cokelaer@pasteur.fr
+Maintainer: Thomas Cokelaer
+Maintainer-email: thomas.cokelaer@pasteur.fr
+License: new BSD
+Keywords: NGS,singularity
+Platform: Linux
+Platform: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: testing
+Provides-Extra: doc
+License-File: LICENSE
+
 DAMONA
 ######
 
 
 .. image:: https://badge.fury.io/py/damona.svg
     :target: https://pypi.python.org/pypi/damona
 
@@ -338,20 +370,27 @@
 you can combine this new environemnt with the base one::
 
     damona activate base
 
 If you are interested to know more, please see the User Guide and Developer
 guide here below.
 
+
+
 Changelog
 =========
 
 ========= ========================================================================
 Version   Description
 ========= ========================================================================
+0.8.3     * create registry specifically for the sandbox (for testing)
+          * add damona community in the uploads
+          * add pbbam, bioconvert, busco, canu, ccs
+          * add polypolish, samtools 1.16.1, sequana 0.14.6, flye 2.9, canu 2.1.1
+            circlator 1.5.5, hifiasm
 0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
           * add seqkit recipe and container
           * add shustring
 0.8.1     * Include ability to interact with biocontainers by allowing retrieval
             of all biocontainers docker images using this syntax:
             'damona install biocontainers/xx:1.2.3' Note that although 9000 
             containers are available, in practice, only about 1000 dockers are
```

### Comparing `damona-0.8.2/damona/__init__.py` & `damona-0.8.3/damona/__init__.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/admin.py` & `damona-0.8.3/damona/admin.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/biocontainers/registry.yaml` & `damona-0.8.3/damona/biocontainers/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/builders.py` & `damona-0.8.3/damona/builders.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/common.py` & `damona-0.8.3/damona/common.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/config.py` & `damona-0.8.3/damona/config.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/environ.py` & `damona-0.8.3/damona/environ.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/install.py` & `damona-0.8.3/damona/install.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/library/R/Singularity.R_3.6.3` & `damona-0.8.3/damona/library/R/Singularity.R_3.6.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/library/R/Singularity.R_4.0.2` & `damona-0.8.3/damona/library/R/Singularity.R_4.0.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/library/conda/Singularity.conda_4.7.12` & `damona-0.8.3/damona/library/conda/Singularity.conda_4.7.12`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/library/conda/Singularity.conda_4.9.2` & `damona-0.8.3/damona/library/conda/Singularity.conda_4.9.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/registry.py` & `damona-0.8.3/damona/registry.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/script.py` & `damona-0.8.3/damona/script.py`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/shell/bash/damona.sh` & `damona-0.8.3/damona/shell/bash/damona.sh`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/shell/fish/damona.fish` & `damona-0.8.3/damona/shell/fish/damona.fish`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/art/registry.yaml` & `damona-0.8.3/damona/software/art/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bamtools/Singularity.bamtools_2.5.2` & `damona-0.8.3/damona/software/bamtools/Singularity.bamtools_2.5.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bbtools/registry.yaml` & `damona-0.8.3/damona/software/bbtools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bedtools/Singularity.bedtools_2.30.0` & `damona-0.8.3/damona/software/bedtools/Singularity.bedtools_2.30.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bioconvert/Singularity.bioconvert_0.6.1` & `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bioconvert/Singularity.bioconvert_0.6.2` & `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bioconvert/Singularity.bioconvert_0.6.3` & `damona-0.8.3/damona/software/bioconvert/Singularity.bioconvert_0.6.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bioconvert/registry.yaml` & `damona-0.8.3/damona/software/bioconvert/registry.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -14,7 +14,12 @@
       doi: 10.5281/zenodo.7470179
       filesize: 1014280192
     0.6.3:
       download: https://zenodo.org/record/7603984/files/bioconvert_0.6.3.img
       md5sum: c2a2e44c4dc2e9af11a661fa39367c81
       doi: 10.5281/zenodo.7603984
       filesize: 1365348352
+    1.0.0:
+      download: https://zenodo.org/record/7704649/files/bioconvert_1.0.0.img
+      md5sum: 45827ef4d866aac9076b3924d2594776
+      doi: 10.5281/zenodo.7704649
+      filesize: 1369206784
```

### Comparing `damona-0.8.2/damona/software/bowtie/Singularity.bowtie_1.3.1` & `damona-0.8.3/damona/software/bowtie/Singularity.bowtie_1.3.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bowtie2/Singularity.bowtie2_2.3.4` & `damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.3.4`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bowtie2/Singularity.bowtie2_2.4.2` & `damona-0.8.3/damona/software/bowtie2/Singularity.bowtie2_2.4.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/bowtie2/registry.yaml` & `damona-0.8.3/damona/software/bowtie2/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/falco/Singularity.falco_0.2.1` & `damona-0.8.3/damona/software/falco/Singularity.falco_0.2.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/falco/Singularity.falco_1.0.0` & `damona-0.8.3/damona/software/falco/Singularity.falco_1.0.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/fastqc/Singularity.fastqc_0.11.8` & `damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.8`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/fastqc/Singularity.fastqc_0.11.9_py3` & `damona-0.8.3/damona/software/fastqc/Singularity.fastqc_0.11.9_py3`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/fastqc/registry.yaml` & `damona-0.8.3/damona/software/fastqc/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/gffread/Singularity.gffread_0.12.1` & `damona-0.8.3/damona/software/gffread/Singularity.gffread_0.12.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/idr/Singularity.idr_2.0.3` & `damona-0.8.3/damona/software/idr/Singularity.idr_2.0.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/igvtools/Singularity.igvtools_2.12.0` & `damona-0.8.3/damona/software/igvtools/Singularity.igvtools_2.12.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/kraken/Singularity.kraken_1.1.0` & `damona-0.8.3/damona/software/kraken/Singularity.kraken_1.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/kraken/Singularity.kraken_2.0.9` & `damona-0.8.3/damona/software/kraken/Singularity.kraken_2.0.9`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/kraken/registry.yaml` & `damona-0.8.3/damona/software/kraken/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/minimap2/Singularity.minimap2_2.17.0` & `damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.17.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/minimap2/Singularity.minimap2_2.23.0` & `damona-0.8.3/damona/software/minimap2/Singularity.minimap2_2.23.0`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     tar xvzf /install_tmp/v2.23.tar.gz
     rm /install_tmp/v2.23.tar.gz
     mv /install_tmp/minimap2-2.23 /minimap2
     cd /minimap2
     make
     ln -s /minimap2/minimap2 /usr/local/bin/minimap2
 
-    apk del wget make libc-dev zlib-dev xz-dev 
+    apk del wget make libc-dev zlib-dev xz-dev
 
 
 
 %runscript
      exec minimap2 "$@"
```

### Comparing `damona-0.8.2/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2` & `damona-0.8.3/damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/phantompeakqualtools/registry.yaml` & `damona-0.8.3/damona/software/phantompeakqualtools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/prokka/Singularity.prokka_1.14.5` & `damona-0.8.3/damona/software/prokka/Singularity.prokka_1.14.5`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/quast/Singularity.quast_5.0.2` & `damona-0.8.3/damona/software/quast/Singularity.quast_5.0.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/rnadiff/Singularity.rnadiff_1.7.1` & `damona-0.8.3/damona/software/rnadiff/Singularity.rnadiff_1.7.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0` & `damona-0.8.3/damona/software/rnaseqc/Singularity.rnaseqc_2.35.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/rtools/Singularity.rtools_1.2.0` & `damona-0.8.3/damona/software/rtools/Singularity.rtools_1.2.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/rtools/registry.yaml` & `damona-0.8.3/damona/software/RIPseeker/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/salmon/Singularity.salmon_1.3.0` & `damona-0.8.3/damona/software/salmon/Singularity.salmon_1.3.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/samtools/Singularity.samtools_1.15.0` & `damona-0.8.3/damona/software/samtools/Singularity.samtools_1.15.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/seqkit/Singularity.seqkit_2.1.0` & `damona-0.8.3/damona/software/seqkit/Singularity.seqkit_2.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana/Singularity.sequana_0.12.6` & `damona-0.8.3/damona/software/sequana/Singularity.sequana_0.12.6`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2` & `damona-0.8.3/damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0` & `damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0` & `damona-0.8.3/damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_perl_tools/registry.yaml` & `damona-0.8.3/damona/software/sequana_perl_tools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0` & `damona-0.8.3/damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.10.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.11.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.12.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.1`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.2`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.14.3`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0` & `damona-0.8.3/damona/software/sequana_tools/Singularity.sequana_tools_0.9.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/sequana_tools/registry.yaml` & `damona-0.8.3/damona/software/sequana_tools/registry.yaml`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/snpeff/Singularity.snpeff_5.1.0` & `damona-0.8.3/damona/software/snpeff/Singularity.snpeff_5.1.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/trf/Singularity.trf_4.10.0` & `damona-0.8.3/damona/software/trf/Singularity.trf_4.10.0`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/software/ucsc/Singularity.ucsc_3.7.7` & `damona-0.8.3/damona/software/ucsc/Singularity.ucsc_3.7.7`

 * *Files identical despite different names*

### Comparing `damona-0.8.2/damona/zenodo.py` & `damona-0.8.3/damona/zenodo.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     ::
 
         z = Zenodo(mode="sandbox.zenodo")
 
     You can retrieve an existing deposit (read-only) given its ID::
 
         deposit = z.get_deposition(959590)
+            oeturn "registry.yaml"
 
     Or start with a new one::
 
         deposit = z.create_new_deposition()
 
 
     If you want to create a new file deposition and publish it, follow those 4 commands:
@@ -208,14 +209,15 @@
                 "title": f"Damona singularity image of {software} software",
                 "upload_type": "physicalobject",
                 "description": f"""Singularity image(s) of {software} software to be used and installed with damona
 (<a href="https://damona.readthedocs.org">See https://damona.readthedocs.org</a>) for reproducible bioinformatics
 analysis.""",
                 "keywords": ["apptainer", "singularity", "damona", "bioinformatics", "reproducibility", "container"],
                 "version": f"{version}",
+                "communities": [{"identifier": "damona"}]
             }
         }
 
         if self.orcid:
             data["metadata"]["creators"] = [{"orcid": self.orcid, "name": self.author, "affiliation": self.affiliation}]
         else:
             data["metadata"]["creators"] = [{"name": self.author, "affiliation": self.affiliation}]
@@ -264,27 +266,36 @@
             return data.json()["id"]
         except:
             try:
                 return data["id"]
             except:
                 return data
 
+    def _get_registry(self):
+        print(self.mode)
+
+        if self.mode == "zenodo":
+            return "registry.yaml"
+        elif self.mode == "sandbox.zenodo":
+            return "registry_sandbox.yaml"
+    registry_name = property(_get_registry)
+
     def _upload(self, filename):
         data = ImageName(filename)
         software = Software(data.name)
 
         if software.name:
             msg = self.create_new_version_with_file_and_publish(filename)
             print(msg)
-            with open("registry.yaml", "a+") as fout:
+            with open(self.registry_name, "a+") as fout:
                 fout.write(msg)
         else:
             msg = self.create_new_deposit_with_file_and_publish(filename)
             print(msg)
-            with open("registry.yaml", "w") as fout:
+            with open(self.registry_name, "w") as fout:
                 fout.write(msg)
 
     def create_new_deposit_with_file_and_publish(self, filename):  # pragma: no cover
         """ """
         data = ImageName(filename)
 
         logger.info(f"Creating and Publising new deposit for {data.name}_{data.version}")
```

### Comparing `damona-0.8.2/damona.egg-info/PKG-INFO` & `damona-0.8.3/damona.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,443 +1,18 @@
 Metadata-Version: 2.1
 Name: damona
-Version: 0.8.2
+Version: 0.8.3
 Summary: A set of NGS singularity recipes, built for you and easily downlable
 Home-page: http://github.com/sequana/sequana
+Download-URL: https://github.com/sequana/sequana/archive/0.8.3.tar.gz
 Author: Thomas Cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: Thomas Cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
-Download-URL: https://github.com/sequana/sequana/archive/0.8.2.tar.gz
-Description: DAMONA
-        ######
-        
-        
-        .. image:: https://badge.fury.io/py/damona.svg
-            :target: https://pypi.python.org/pypi/damona
-        
-        
-        .. image:: https://github.com/cokelaer/damona/actions/workflows/main.yml/badge.svg
-           :target: https://github.com/cokelaer/damona/actions/workflows/main.yml
-        
-        .. image:: https://coveralls.io/repos/github/cokelaer/damona/badge.svg?branch=master
-            :target: https://coveralls.io/github/cokelaer/damona?branch=master
-        
-        .. image:: http://readthedocs.org/projects/damona/badge/?version=latest
-            :target: http://damona.readthedocs.org/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://zenodo.org/badge/282275608.svg
-           :target: https://zenodo.org/badge/latestdoi/282275608
-        
-        
-        :Python version: Python 3.7, 3.8, 3.9
-        :Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
-        :Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
-        :Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
-        
-        Overview
-        ========
-        
-        Damona is a singularity environment manager.
-        
-        Damona started as a small collections of singularity recipes to help installing third-party tools for
-        `Sequana NGS pipelines <https://sequana.readthedocs.io>`_.
-        
-        Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
-        
-        In a nutshell, Damona combines the logic of Conda environments with the
-        reproducibility of singularity containers. We believe that it could be useful for
-        other projects and therefore decided to release it as an independent tool.
-        
-        As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
-        
-        Installation
-        ============
-        
-        If you are in a hurry, just type::
-        
-            pip install damona --upgrade
-        
-        You must install `Singularity <https://sylabs.io/docs>`_ to make use of **Damona**. 
-        
-        If you are familiar with conda, I believe you can do::
-        
-            conda install singularity
-        
-        Type **damona** in a shell. This will initiate the tool with a config file in your HOME/.config/damona directory for bash shell and `fish shell <https://fishshell.com/>`_ users.
-        
-        Bash users should add this code in their ~/.bashrc file::
-        
-            source ~/.config/damona/damona.sh
-        
-        and fishshell users should add the following code in their ~/.config/fish/config.fish file::
-        
-            source ~/.config/damona/damona.fish
-        
-        Open a new shell and you are ready to go. Please see the `Installation in details`_ section for more information.
-        
-        Quick Start
-        ===========
-        
-        **Damona** needs environments to work with.
-        First, let us *create* one, which is called TEST::
-        
-            damona env --create TEST
-        
-        Second, we need to *activate* it. Subsequent insallation will happen in this environment::
-        
-            damona activate TEST
-        
-        From there, we can install some binaries/images::
-        
-            damona install fastqc:0.11.9
-        
-        That's it. Time to test. Type **fastqc**.
-        
-        To rename this TEST example::
-        
-            damona env --rename TEST --new-name prod
-        
-        or delete it::
-        
-            damona env --delete prod
-        
-        See more examples hereafter or in the user guide on https://damona.readthedocs.io
-        
-        Motivation
-        ==========
-        
-        As stated on their website, `Conda <https:/docs.conda.io/en/latest>`_ is
-        an open source **package** management system
-        and **environment** management system.
-        Conda provides pre-compiled releases of software; they can be installed in
-        different local environments that do not interfer with your system. This has
-        great advantages for developers. For example, you can install a pre-compiled
-        libraries in a minute instead of trying to compile it yourself including all
-        dependencies. Different communities have emerged using this
-        framework. One of them is `Bioconda <https://bioconda.github.io>`_, which is dedicated to bioinformatics.
-        
-        Another great tool that emerged in the last years is
-        `Singularity <https://sylabs.io/docs>`_. Singularity containers can be used
-        to package entire scientific workflows,
-        software and libraries, and even data. It is a simple file that can be shared
-        between environments and guarantee exectution and reproducibility.
-        
-        Originally, Conda provided pre-compiled version of a software. Nowadays, it also provides
-        a docker and a singularity image of the tool. On the other side, Singularity can include an
-        entire conda environment. As you can see everything is there to build reproducible tools and
-        environment.
-        
-        Now, what about a software in development that depends on third-party packages ? 
-        You would create a conda environment and starts installing the required packages.
-        Quickly, you will install another package that will break your environment due
-        to unresolved conlicts; this is not common but it happens. In the worst case
-        scenario, the environment is broken. In facilities where users depends on you,
-        it can be quite stresful and time-consuming to maintain several such
-        environments. This is why we have moved little by little to a very light conda
-        environment where known-to-cause-problem packages have been shipped into
-        singularity containers. This means we have to create aliases to those
-        singularities. The singularities can be simple executable containers or full
-        environment containers with many executables inside. In both cases, one need to
-        manage those containers for different users, pipelines, versions etc. This
-        started to be cumbersome to have containers in different places and update
-        script that generate the aliases to those executables.
-        
-        
-        That's where **damona** started: we wanted to combine the conda-like environment 
-        framework to manage our singularity containers more easily.
-        
-        Although **Damona** was started with the `Sequana projet <https://sequana.readthedocs.io>`_,
-        **Damona** may be useful for others developers who wish to have a quick and easy
-        solution for their users when they need to install third-party libraries.
-        
-        Before showing real-case examples, let us install the software itself and 
-        understand the details.
-        
-        
-        
-        Installation in details
-        =======================
-        
-        The is the egg and chicken paradox. To get reproducible container with
-        singularity, at some point you need to install singularity itself. That the first
-        of the two software that you will need to install. Instructions
-        are on `singularity web site <https://sylabs.io/guides/3.6/user-guide/>`_. This
-        is not obvious to be honest. You need the GO language to be installed as well. I
-        personally installed from source and it worked like a charm.
-        
-        Second, you need **Damona**. This is a pure Python sotfware with only a few
-        dependencies. Install it with the **pip** software provided with your Python
-        installation (Python 3.X)::
-        
-            pip install damona --upgrade
-        
-        Type **damona** to create the Damona tree structure. Images and binaries 
-        will be saved in your home directory within the
-        ~/.config/damona directory. There, special files should be available:
-        **damona.sh**, **damona.fish**  and **damona.cfg**. Check that those files are present.
-        
-        Finally, you need to tell your system where to find damona. For bashrc users,
-        please add this line to you bashrc file::
-        
-            source ~/.config/damona/damona.sh
-        
-        open a new shell and type **damona** and you should be ready to go.
-        
-        For fishshell users, please add this line in **~/.config/fish/config.fish***::
-        
-            source ~/.config/damona/damona.fish
-        
-        Tutorial
-        ============
-        
-        The **Damona** standalone is called **damona**. It has a documentation that should suffice for most users.
-        
-        The main documentation is obtained using::
-        
-            damona --help
-        
-        where you will see the list of **Damona** commands (may be different with time) (may be::
-        
-            activate
-            clean
-            deactivate
-            env
-            export
-            info
-            install
-            list
-            remove
-            search
-            stats
-        
-        To get help for the *install* command, type::
-        
-            damona install --help
-        
-        
-        1. *list* available environments
-        --------------------------------
-        
-        By default you have an environment called **base**. Unlike the **base** environment found in **conda**, it is not
-        essential and may be altered. However, it cannot be removed or created. You can check the list of environments using::
-        
-            damona env
-        
-        2. *create* environments
-        ------------------------
-        All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
-        
-            damona env --create TEST
-        
-        There, you have a *bin* directory where binaries are going to be installed.
-        
-        You can check that it has been created::
-        
-            damona env
-        
-        Note the last line telling you that::
-        
-            Your current env is 'TEST'.
-        
-        3. activate and deactivate environments
-        ----------------------------------------
-        
-        In order to install new binaries or software package, you must activate an environment. You may activate several but the last one is the *active* one. Let us activate the *TEST* environment::
-        
-            damona activate TEST
-        
-        Check that it is active using::
-        
-            damona env
-        
-        and look at the last line. It should look like::
-        
-            Your current env is 'TEST'.
-        
-        What is going on when you activate an environment called TEST ? Simple: we append the directory ~/.config/damona/envs/TEST/bin to your PATH where binaries are searched for. This directory is removed when you use the *deactivate* command.
-        
-        ::
-        
-            damona deactivate TEST
-            damona env 
-        
-        should remove the TEST environment from your PATH. You may activate several and deactivate them. In such case, the
-        environments behave as a Last In First Out principle::
-        
-            damona activate base
-            damona activate TEST
-            damona deactivate 
-        
-        Removes the last activated environments. While this set of commands is more specific::
-        
-            damona activate base
-            damona activate TEST
-            damona deactivate base
-        
-        and keep the TEST environment only in your PATH.
-        
-        4. **install** a software
-        --------------------------
-        
-        Let us now consider that the TEST environment is active.
-        
-        Damona provides software that may have several releases. Each software/release comes with binaries that will be
-        installed together with the underlying singularity image.::
-        
-            damona install fastqc:0.11.9
-        
-        Here, the singularity image corresponding to the release 0.11.9 of the **fastqc** software is downloaded. Then, binaries registered in this release are installed (here the **fastqc** binary only).
-        
-        All images are stored in *~/.config/damona/images* and are shared between environments. 
-        
-        
-        5. Get **info** about installed images and binaries
-        ----------------------------------------------------
-        
-        You can get the binaries installed in an environment (and the images used by
-        them) using the **info** command::
-        
-            damona info TEST
-        
-        
-        6. Search the registry
-        ------------------------
-        
-        By default, we provide recipes (26 in Dec 2021 ; 38 releases) available in **Damona**. 
-        They can be searched for using::
-        
-            damona search PATTERN
-        
-        External registry can be set-up. For instance, a damona registry is accessible
-        as follows (for demonstration)::
-        
-            damona search fastqc --url damona
-        
-        Where *damona* is an alias defined in the .config/damona/damona.cfg that
-        is set to https://biomics.pasteur.fr/drylab/damona/registry.txt
-        
-        You may retrieve images from a website where a registry exists (see the developer
-        guide to create a registry yourself).
-        
-        
-        7. combine two different environments
-        --------------------------------------
-        
-        In damona, you can have sereral environments in parallel and later activate the
-        one you wish to use. Let us create a new one::
-        
-            damone env --create test1
-        
-        and check that you now have one more environment::
-        
-            damona env
-        
-        We want to create an alias to the previously downloaded image of fastqc tool but
-        in the *test1* environment. First we activate the newly create environment::
-        
-            damona activate test1
-        
-        then, we install the container::
-        
-            damona install fastqc:0.11.9
-        
-        This will not download the image again. It will just create a binary in the
-        ~/.config/damona/envs/test1/bin directory.
-        
-        you can combine this new environemnt with the base one::
-        
-            damona activate base
-        
-        If you are interested to know more, please see the User Guide and Developer
-        guide here below.
-        
-        Changelog
-        =========
-        
-        ========= ========================================================================
-        Version   Description
-        ========= ========================================================================
-        0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
-                  * add seqkit recipe and container
-                  * add shustring
-        0.8.1     * Include ability to interact with biocontainers by allowing retrieval
-                    of all biocontainers docker images using this syntax:
-                    'damona install biocontainers/xx:1.2.3' Note that although 9000 
-                    containers are available, in practice, only about 1000 dockers are 
-                    on dockerhub, which is already nice :-)
-                  * 
-        0.8.0     * Fix regression to install a software with its version
-        0.7.1     * Implement the fish shell 
-                  * add command "damona list"
-                  * rename recipes/ directory into software/ and created a new library/ 
-                    directory for images used as library, that are not installed.
-        0.7.0     * Check that singularity is installed
-                  * implement the remove command 
-                    https://github.com/cokelaer/damona/issues/15
-                  * more recipes cleanup (https://github.com/cokelaer/damona/issues/12)
-                  * removed damona recipes (pure python package)
-                  * cleanup all recipes
-                  * add zenodo stats (for admin)
-        0.6.0     * add ability to upload images on zenodo. No need for external 
-                    repositories.
-                  * ability to add/delete a software from different images
-                  * implement --help for the activate/deactivate (non trivial)
-                  * add --rename option in 'damona env'
-                  * 'base' environment is now at the same level as other environments
-                  * better bash script; no need for DAMONA_EXE variable anymore.
-        0.5.3     * Fixing config/shell 
-        0.5.2     * add missing shell package
-        0.5.1     * add DAMONA_SINGULARITY_OPTIONS env variable in the binary
-                  * Fix the way binaries are found in the releases.
-                  * new recipes: rtools
-                  * new releases: sequana_tools_0.10.0
-                  * Fix shell script to handle DAMONA_EXE variable 
-        0.5.0     * Major refactoring. 
-        
-                    - Simplification of the registries (dropping notion of exe/set 
-                      class
-                    - Main script should now be fully functional with functional
-                      activation/deactivation. 
-                    - New command to build images from local recipes or dockerhub 
-                      entries.
-                    - Install command can now install local container. 
-                    - DAMONA_PATH can be set to install damona images/binaries 
-                      anywhere, not just in local home. 
-                    - check md5 of images to not download/copy again
-        0.4.3     * Implement damona activate/deactivate
-        0.4.2     * Fix typo in the creation of aliases for 'set' containers
-        0.4.1     * implemented aliases for the --from-url option stored in a
-                    damona.cfg file
-        0.4.0     * implemented the 'env' and 'activate' command
-                  * ability to setup an external registry on any https and retrieve
-                    registry from there to download external images
-        0.3.X     * add gffread, rnadiff recipes
-        0.3.0     * A stable version with documentation and >95% coverage read-yto-use
-        0.2.3     * add new recipes (rnadiff)
-        0.2.2     * Download latest if no version provided
-                  * include *build* command to build image locally
-        0.2.1     fixed manifest
-        0.2.0     first working version of damona to pull image locally with binaries
-        0.1.1     small update to fix RTD, travis, coveralls
-        0.1       first release to test feasibility of the project
-        ========= ========================================================================
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
-        
 Keywords: NGS,singularity
 Platform: Linux
 Platform: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -449,7 +24,440 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: testing
 Provides-Extra: doc
+License-File: LICENSE
+
+DAMONA
+######
+
+
+.. image:: https://badge.fury.io/py/damona.svg
+    :target: https://pypi.python.org/pypi/damona
+
+
+.. image:: https://github.com/cokelaer/damona/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/cokelaer/damona/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/cokelaer/damona/badge.svg?branch=master
+    :target: https://coveralls.io/github/cokelaer/damona?branch=master
+
+.. image:: http://readthedocs.org/projects/damona/badge/?version=latest
+    :target: http://damona.readthedocs.org/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://zenodo.org/badge/282275608.svg
+   :target: https://zenodo.org/badge/latestdoi/282275608
+
+
+:Python version: Python 3.7, 3.8, 3.9
+:Source: See  `http://github.com/cokelaer/damona <https://github.com/cokelaer/damona/>`__.
+:Issues: Please fill a report on `github <https://github.com/cokelaer/damona/issues>`__
+:Platform: This is currently only available for Linux distribution with bash shell (contributions are welcome to port the tool on MacOSX and other platforms)
+
+Overview
+========
+
+Damona is a singularity environment manager.
+
+Damona started as a small collections of singularity recipes to help installing third-party tools for
+`Sequana NGS pipelines <https://sequana.readthedocs.io>`_.
+
+Damona is now used in production to create reproducible environments where singularity images and their associated binaries are installed altogether.
+
+In a nutshell, Damona combines the logic of Conda environments with the
+reproducibility of singularity containers. We believe that it could be useful for
+other projects and therefore decided to release it as an independent tool.
+
+As of 30th Dec 2021, **Damona** contains 26 software, 38 releases, 105 binaries.
+
+Installation
+============
+
+If you are in a hurry, just type::
+
+    pip install damona --upgrade
+
+You must install `Singularity <https://sylabs.io/docs>`_ to make use of **Damona**. 
+
+If you are familiar with conda, I believe you can do::
+
+    conda install singularity
+
+Type **damona** in a shell. This will initiate the tool with a config file in your HOME/.config/damona directory for bash shell and `fish shell <https://fishshell.com/>`_ users.
+
+Bash users should add this code in their ~/.bashrc file::
+
+    source ~/.config/damona/damona.sh
+
+and fishshell users should add the following code in their ~/.config/fish/config.fish file::
+
+    source ~/.config/damona/damona.fish
+
+Open a new shell and you are ready to go. Please see the `Installation in details`_ section for more information.
+
+Quick Start
+===========
+
+**Damona** needs environments to work with.
+First, let us *create* one, which is called TEST::
+
+    damona env --create TEST
+
+Second, we need to *activate* it. Subsequent insallation will happen in this environment::
+
+    damona activate TEST
+
+From there, we can install some binaries/images::
+
+    damona install fastqc:0.11.9
+
+That's it. Time to test. Type **fastqc**.
+
+To rename this TEST example::
+
+    damona env --rename TEST --new-name prod
+
+or delete it::
+
+    damona env --delete prod
+
+See more examples hereafter or in the user guide on https://damona.readthedocs.io
+
+Motivation
+==========
+
+As stated on their website, `Conda <https:/docs.conda.io/en/latest>`_ is
+an open source **package** management system
+and **environment** management system.
+Conda provides pre-compiled releases of software; they can be installed in
+different local environments that do not interfer with your system. This has
+great advantages for developers. For example, you can install a pre-compiled
+libraries in a minute instead of trying to compile it yourself including all
+dependencies. Different communities have emerged using this
+framework. One of them is `Bioconda <https://bioconda.github.io>`_, which is dedicated to bioinformatics.
+
+Another great tool that emerged in the last years is
+`Singularity <https://sylabs.io/docs>`_. Singularity containers can be used
+to package entire scientific workflows,
+software and libraries, and even data. It is a simple file that can be shared
+between environments and guarantee exectution and reproducibility.
+
+Originally, Conda provided pre-compiled version of a software. Nowadays, it also provides
+a docker and a singularity image of the tool. On the other side, Singularity can include an
+entire conda environment. As you can see everything is there to build reproducible tools and
+environment.
+
+Now, what about a software in development that depends on third-party packages ? 
+You would create a conda environment and starts installing the required packages.
+Quickly, you will install another package that will break your environment due
+to unresolved conlicts; this is not common but it happens. In the worst case
+scenario, the environment is broken. In facilities where users depends on you,
+it can be quite stresful and time-consuming to maintain several such
+environments. This is why we have moved little by little to a very light conda
+environment where known-to-cause-problem packages have been shipped into
+singularity containers. This means we have to create aliases to those
+singularities. The singularities can be simple executable containers or full
+environment containers with many executables inside. In both cases, one need to
+manage those containers for different users, pipelines, versions etc. This
+started to be cumbersome to have containers in different places and update
+script that generate the aliases to those executables.
+
+
+That's where **damona** started: we wanted to combine the conda-like environment 
+framework to manage our singularity containers more easily.
+
+Although **Damona** was started with the `Sequana projet <https://sequana.readthedocs.io>`_,
+**Damona** may be useful for others developers who wish to have a quick and easy
+solution for their users when they need to install third-party libraries.
+
+Before showing real-case examples, let us install the software itself and 
+understand the details.
+
+
+
+Installation in details
+=======================
+
+The is the egg and chicken paradox. To get reproducible container with
+singularity, at some point you need to install singularity itself. That the first
+of the two software that you will need to install. Instructions
+are on `singularity web site <https://sylabs.io/guides/3.6/user-guide/>`_. This
+is not obvious to be honest. You need the GO language to be installed as well. I
+personally installed from source and it worked like a charm.
+
+Second, you need **Damona**. This is a pure Python sotfware with only a few
+dependencies. Install it with the **pip** software provided with your Python
+installation (Python 3.X)::
+
+    pip install damona --upgrade
+
+Type **damona** to create the Damona tree structure. Images and binaries 
+will be saved in your home directory within the
+~/.config/damona directory. There, special files should be available:
+**damona.sh**, **damona.fish**  and **damona.cfg**. Check that those files are present.
+
+Finally, you need to tell your system where to find damona. For bashrc users,
+please add this line to you bashrc file::
+
+    source ~/.config/damona/damona.sh
+
+open a new shell and type **damona** and you should be ready to go.
+
+For fishshell users, please add this line in **~/.config/fish/config.fish***::
+
+    source ~/.config/damona/damona.fish
+
+Tutorial
+============
+
+The **Damona** standalone is called **damona**. It has a documentation that should suffice for most users.
+
+The main documentation is obtained using::
+
+    damona --help
+
+where you will see the list of **Damona** commands (may be different with time) (may be::
+
+    activate
+    clean
+    deactivate
+    env
+    export
+    info
+    install
+    list
+    remove
+    search
+    stats
+
+To get help for the *install* command, type::
+
+    damona install --help
+
+
+1. *list* available environments
+--------------------------------
+
+By default you have an environment called **base**. Unlike the **base** environment found in **conda**, it is not
+essential and may be altered. However, it cannot be removed or created. You can check the list of environments using::
+
+    damona env
+
+2. *create* environments
+------------------------
+All environments are stored in *~/.config/damona/envs/*. You can create a new one as follows::
+
+    damona env --create TEST
+
+There, you have a *bin* directory where binaries are going to be installed.
+
+You can check that it has been created::
+
+    damona env
+
+Note the last line telling you that::
+
+    Your current env is 'TEST'.
+
+3. activate and deactivate environments
+----------------------------------------
+
+In order to install new binaries or software package, you must activate an environment. You may activate several but the last one is the *active* one. Let us activate the *TEST* environment::
+
+    damona activate TEST
+
+Check that it is active using::
+
+    damona env
+
+and look at the last line. It should look like::
+
+    Your current env is 'TEST'.
+
+What is going on when you activate an environment called TEST ? Simple: we append the directory ~/.config/damona/envs/TEST/bin to your PATH where binaries are searched for. This directory is removed when you use the *deactivate* command.
+
+::
+
+    damona deactivate TEST
+    damona env 
+
+should remove the TEST environment from your PATH. You may activate several and deactivate them. In such case, the
+environments behave as a Last In First Out principle::
+
+    damona activate base
+    damona activate TEST
+    damona deactivate 
+
+Removes the last activated environments. While this set of commands is more specific::
+
+    damona activate base
+    damona activate TEST
+    damona deactivate base
+
+and keep the TEST environment only in your PATH.
+
+4. **install** a software
+--------------------------
+
+Let us now consider that the TEST environment is active.
+
+Damona provides software that may have several releases. Each software/release comes with binaries that will be
+installed together with the underlying singularity image.::
+
+    damona install fastqc:0.11.9
+
+Here, the singularity image corresponding to the release 0.11.9 of the **fastqc** software is downloaded. Then, binaries registered in this release are installed (here the **fastqc** binary only).
+
+All images are stored in *~/.config/damona/images* and are shared between environments. 
+
+
+5. Get **info** about installed images and binaries
+----------------------------------------------------
+
+You can get the binaries installed in an environment (and the images used by
+them) using the **info** command::
+
+    damona info TEST
+
+
+6. Search the registry
+------------------------
+
+By default, we provide recipes (26 in Dec 2021 ; 38 releases) available in **Damona**. 
+They can be searched for using::
+
+    damona search PATTERN
+
+External registry can be set-up. For instance, a damona registry is accessible
+as follows (for demonstration)::
+
+    damona search fastqc --url damona
+
+Where *damona* is an alias defined in the .config/damona/damona.cfg that
+is set to https://biomics.pasteur.fr/drylab/damona/registry.txt
+
+You may retrieve images from a website where a registry exists (see the developer
+guide to create a registry yourself).
+
+
+7. combine two different environments
+--------------------------------------
+
+In damona, you can have sereral environments in parallel and later activate the
+one you wish to use. Let us create a new one::
+
+    damone env --create test1
+
+and check that you now have one more environment::
+
+    damona env
+
+We want to create an alias to the previously downloaded image of fastqc tool but
+in the *test1* environment. First we activate the newly create environment::
+
+    damona activate test1
+
+then, we install the container::
+
+    damona install fastqc:0.11.9
+
+This will not download the image again. It will just create a binary in the
+~/.config/damona/envs/test1/bin directory.
+
+you can combine this new environemnt with the base one::
+
+    damona activate base
+
+If you are interested to know more, please see the User Guide and Developer
+guide here below.
+
+
+
+Changelog
+=========
+
+========= ========================================================================
+Version   Description
+========= ========================================================================
+0.8.3     * create registry specifically for the sandbox (for testing)
+          * add damona community in the uploads
+          * add pbbam, bioconvert, busco, canu, ccs
+          * add polypolish, samtools 1.16.1, sequana 0.14.6, flye 2.9, canu 2.1.1
+            circlator 1.5.5, hifiasm
+0.8.2     * add idr, samtools, homer, bamtools, bedtools, sequana_denovo
+          * add seqkit recipe and container
+          * add shustring
+0.8.1     * Include ability to interact with biocontainers by allowing retrieval
+            of all biocontainers docker images using this syntax:
+            'damona install biocontainers/xx:1.2.3' Note that although 9000 
+            containers are available, in practice, only about 1000 dockers are 
+            on dockerhub, which is already nice :-)
+          * 
+0.8.0     * Fix regression to install a software with its version
+0.7.1     * Implement the fish shell 
+          * add command "damona list"
+          * rename recipes/ directory into software/ and created a new library/ 
+            directory for images used as library, that are not installed.
+0.7.0     * Check that singularity is installed
+          * implement the remove command 
+            https://github.com/cokelaer/damona/issues/15
+          * more recipes cleanup (https://github.com/cokelaer/damona/issues/12)
+          * removed damona recipes (pure python package)
+          * cleanup all recipes
+          * add zenodo stats (for admin)
+0.6.0     * add ability to upload images on zenodo. No need for external 
+            repositories.
+          * ability to add/delete a software from different images
+          * implement --help for the activate/deactivate (non trivial)
+          * add --rename option in 'damona env'
+          * 'base' environment is now at the same level as other environments
+          * better bash script; no need for DAMONA_EXE variable anymore.
+0.5.3     * Fixing config/shell 
+0.5.2     * add missing shell package
+0.5.1     * add DAMONA_SINGULARITY_OPTIONS env variable in the binary
+          * Fix the way binaries are found in the releases.
+          * new recipes: rtools
+          * new releases: sequana_tools_0.10.0
+          * Fix shell script to handle DAMONA_EXE variable 
+0.5.0     * Major refactoring. 
+
+            - Simplification of the registries (dropping notion of exe/set 
+              class
+            - Main script should now be fully functional with functional
+              activation/deactivation. 
+            - New command to build images from local recipes or dockerhub 
+              entries.
+            - Install command can now install local container. 
+            - DAMONA_PATH can be set to install damona images/binaries 
+              anywhere, not just in local home. 
+            - check md5 of images to not download/copy again
+0.4.3     * Implement damona activate/deactivate
+0.4.2     * Fix typo in the creation of aliases for 'set' containers
+0.4.1     * implemented aliases for the --from-url option stored in a
+            damona.cfg file
+0.4.0     * implemented the 'env' and 'activate' command
+          * ability to setup an external registry on any https and retrieve
+            registry from there to download external images
+0.3.X     * add gffread, rnadiff recipes
+0.3.0     * A stable version with documentation and >95% coverage read-yto-use
+0.2.3     * add new recipes (rnadiff)
+0.2.2     * Download latest if no version provided
+          * include *build* command to build image locally
+0.2.1     fixed manifest
+0.2.0     first working version of damona to pull image locally with binaries
+0.1.1     small update to fix RTD, travis, coveralls
+0.1       first release to test feasibility of the project
+========= ========================================================================
+
+
+
+
+
+
+
+
+
+
```

### Comparing `damona-0.8.2/damona.egg-info/SOURCES.txt` & `damona-0.8.3/damona.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+.gitignore
+.readthedocs.yml
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
+.github/workflows/bash_test.yml
+.github/workflows/fish_test.yml
+.github/workflows/main.yml
+.github/workflows/pypi.yml
 damona/__init__.py
 damona/admin.py
 damona/builders.py
 damona/common.py
 damona/config.py
 damona/environ.py
 damona/install.py
@@ -21,121 +27,170 @@
 damona.egg-info/entry_points.txt
 damona.egg-info/not-zip-safe
 damona.egg-info/requires.txt
 damona.egg-info/top_level.txt
 damona/biocontainers/__init__.py
 damona/biocontainers/registry.yaml
 damona/library/__init__.py
+damona/library/R/Makefile
 damona/library/R/Singularity.R_3.6.3
 damona/library/R/Singularity.R_4.0.2
 damona/library/R/registry.yaml
+damona/library/conda/README.rst
 damona/library/conda/Singularity.conda_4.7.12
 damona/library/conda/Singularity.conda_4.9.2
 damona/library/conda/registry.yaml
+damona/library/rust/Singularity.rust
+damona/library/ubuntu/Singularity.ubuntu_16.04
+damona/library/ubuntu/Singularity.ubuntu_18.04
+damona/library/ubuntu/registry.yaml
 damona/papers/__init__.py
 damona/shell/__init__.py
+damona/shell/damona_comp.sh
 damona/shell/bash/__init__.py
 damona/shell/bash/damona.sh
 damona/shell/fish/damona.fish
 damona/software/__init__.py
+damona/software/RIPseeker/Singularity.RIPseeker_1.0.0
+damona/software/RIPseeker/registry.yaml
 damona/software/art/Singularity.art_2.5.8
 damona/software/art/Singularity.art_3.11.14
 damona/software/art/registry.yaml
 damona/software/bamtools/Singularity.bamtools_2.5.2
 damona/software/bamtools/registry.yaml
 damona/software/bbtools/Singularity.bbtools_38.94.0
 damona/software/bbtools/registry.yaml
+damona/software/bcl2fastq/Makefile
+damona/software/bcl2fastq/README.rst
 damona/software/bcl2fastq/Singularity.bcl2fastq_2.20.0
 damona/software/bcl2fastq/registry.yaml
 damona/software/bedtools/Singularity.bedtools_2.30.0
 damona/software/bedtools/registry.yaml
 damona/software/bioconvert/Singularity.bioconvert_0.6.1
 damona/software/bioconvert/Singularity.bioconvert_0.6.2
 damona/software/bioconvert/Singularity.bioconvert_0.6.3
+damona/software/bioconvert/Singularity.bioconvert_1.0.0
 damona/software/bioconvert/registry.yaml
 damona/software/bowtie/Singularity.bowtie_1.3.1
 damona/software/bowtie/registry.yaml
 damona/software/bowtie2/Singularity.bowtie2_2.3.4
 damona/software/bowtie2/Singularity.bowtie2_2.4.2
 damona/software/bowtie2/registry.yaml
+damona/software/busco/Singularity.busco_5.4.6
+damona/software/busco/registry.yaml
+damona/software/bwa/Singularity.bwa_0.7.17
+damona/software/bwa/registry.yaml
 damona/software/canu/Singularity.canu_1.6.0
 damona/software/canu/Singularity.canu_1.8.0
+damona/software/canu/Singularity.canu_2.1.1
 damona/software/canu/registry.yaml
+damona/software/ccs/Singularity.ccs_6.4.0
+damona/software/ccs/registry.yaml
+damona/software/circlator/Singularity.circlator_1.5.5
+damona/software/circlator/registry.yaml
 damona/software/falco/Singularity.falco_0.2.1
 damona/software/falco/Singularity.falco_1.0.0
 damona/software/falco/registry.yaml
 damona/software/fastp/Singularity.fastp_0.23.2
 damona/software/fastp/registry.yaml
 damona/software/fastqc/Singularity.fastqc_0.11.8
 damona/software/fastqc/Singularity.fastqc_0.11.9
 damona/software/fastqc/Singularity.fastqc_0.11.9_py3
 damona/software/fastqc/registry.yaml
 damona/software/flye/Singularity.flye_2.9.0
+damona/software/flye/Singularity.flye_2.9.1
 damona/software/flye/registry.yaml
 damona/software/gffread/Singularity.gffread_0.12.1
 damona/software/gffread/registry.yaml
 damona/software/graphviz/Singularity.graphviz_2.43.0
 damona/software/graphviz/registry.yaml
+damona/software/graphviz/test.dot
+damona/software/graphviz/test.sh
 damona/software/gzip/Singularity.gzip_1.9.0
 damona/software/gzip/registry.yaml
+damona/software/hifiasm/Singularity.hifiasm_0.19.1
+damona/software/hifiasm/registry.yaml
+damona/software/hisat2/README.rst
 damona/software/hisat2/registry.yaml
 damona/software/homer/Singularity.homer_4.11.0
 damona/software/homer/registry.yaml
 damona/software/idr/Singularity.idr_2.0.3
 damona/software/idr/registry.yaml
 damona/software/igvtools/Singularity.igvtools_2.12.0
 damona/software/igvtools/registry.yaml
+damona/software/kraken/Makefile
 damona/software/kraken/Singularity.kraken_1.1.0
 damona/software/kraken/Singularity.kraken_2.0.9
 damona/software/kraken/registry.yaml
+damona/software/mergegi/Singularity.mergegi_0.0.1
+damona/software/mergegi/registry.yaml
 damona/software/minimap2/Singularity.minimap2_2.17.0
 damona/software/minimap2/Singularity.minimap2_2.23.0
+damona/software/minimap2/Singularity.minimap2_2.24.0
 damona/software/minimap2/registry.yaml
+damona/software/pbbam/Singularity.pbbam_2.1.0
+damona/software/pbbam/Singularity.pbbam_2.3.0
+damona/software/pbbam/registry.yaml
 damona/software/phantompeakqualtools/Singularity.phantompeakqualtools_1.2.2
 damona/software/phantompeakqualtools/registry.yaml
+damona/software/picard/Singularity.picard_2.26
 damona/software/pigz/Singularity.pigz_2.4.0
 damona/software/pigz/registry.yaml
+damona/software/polypolish/Singularity.polypolish_0.5.0
+damona/software/polypolish/registry.yaml
 damona/software/prokka/Singularity.prokka_1.14.5
 damona/software/prokka/registry.yaml
+damona/software/pycoqc/Singularity.pycoqc_2.5.2
+damona/software/pycoqc/registry.yaml
 damona/software/quast/Singularity.quast_5.0.2
 damona/software/quast/registry.yaml
 damona/software/rnadiff/Singularity.rnadiff_1.7.1
 damona/software/rnadiff/registry.yaml
 damona/software/rnaseqc/Singularity.rnaseqc_2.35.0
 damona/software/rnaseqc/registry.yaml
 damona/software/rtools/Singularity.rtools_1.0.0
 damona/software/rtools/Singularity.rtools_1.1.0
 damona/software/rtools/Singularity.rtools_1.2.0
 damona/software/rtools/registry.yaml
+damona/software/salmon/Makefile
 damona/software/salmon/Singularity.salmon_1.3.0
 damona/software/salmon/registry.yaml
 damona/software/samtools/Singularity.samtools_1.15.0
+damona/software/samtools/Singularity.samtools_1.16.1
 damona/software/samtools/registry.yaml
+damona/software/samtools_minimap2/Singularity.samtools_1.17_minimap2_2.24.0
+damona/software/samtools_minimap2/registry.yaml
 damona/software/seqkit/Singularity.seqkit_2.1.0
+damona/software/seqkit/Singularity.seqkit_2.4.0
 damona/software/seqkit/registry.yaml
 damona/software/seqtk/Singularity.seqtk_1.3.0
 damona/software/seqtk/registry.yaml
 damona/software/sequana/Singularity.sequana_0.12.6
+damona/software/sequana/Singularity.sequana_0.14.6
 damona/software/sequana/registry.yaml
 damona/software/sequana_denovo/Singularity.sequana_denovo_0.0.2
 damona/software/sequana_denovo/registry.yaml
 damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.1.0
 damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.2.0
+damona/software/sequana_perl_tools/Singularity.sequana_perl_tools_0.3.0
 damona/software/sequana_perl_tools/registry.yaml
 damona/software/sequana_ribofinder/Singularity.sequana_ribofinder_0.12.0
 damona/software/sequana_ribofinder/registry.yaml
+damona/software/sequana_tools/README.txt
 damona/software/sequana_tools/Singularity.sequana_tools_0.10.0
 damona/software/sequana_tools/Singularity.sequana_tools_0.11.0
 damona/software/sequana_tools/Singularity.sequana_tools_0.12.0
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.1
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.2
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.3
 damona/software/sequana_tools/Singularity.sequana_tools_0.14.5
+damona/software/sequana_tools/Singularity.sequana_tools_0.14.6
 damona/software/sequana_tools/Singularity.sequana_tools_0.9.0
 damona/software/sequana_tools/registry.yaml
 damona/software/shustring/Singularity.shustring_2.6.0
 damona/software/shustring/registry.yaml
 damona/software/snpeff/Singularity.snpeff_5.1.0
 damona/software/trf/Singularity.trf_4.10.0
 damona/software/trf/registry.yaml
+damona/software/ucsc/README.rst
 damona/software/ucsc/Singularity.ucsc_3.7.7
 damona/software/ucsc/registry.yaml
```

### Comparing `damona-0.8.2/setup.py` & `damona-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 from setuptools import setup, find_packages
 import glob
 
 _MAJOR               = 0
 _MINOR               = 8
-_MICRO               = 2
+_MICRO               = 3
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 
 metainfo = {
     'authors': {"main": ("Thomas Cokelaer", "thomas.cokelaer@pasteur.fr")},
     'maintainer': {"main": ("Thomas Cokelaer", "thomas.cokelaer@pasteur.fr")},
```

