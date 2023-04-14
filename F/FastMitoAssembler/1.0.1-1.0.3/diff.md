# Comparing `tmp/FastMitoAssembler-1.0.1.tar.gz` & `tmp/FastMitoAssembler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastMitoAssembler-1.0.1.tar", last modified: Mon Apr 10 07:43:59 2023, max compression
+gzip compressed data, was "FastMitoAssembler-1.0.3.tar", last modified: Fri Apr 14 05:57:49 2023, max compression
```

## Comparing `FastMitoAssembler-1.0.1.tar` & `FastMitoAssembler-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-10 07:43:59.870678 FastMitoAssembler-1.0.1/
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-10 07:43:59.588482 FastMitoAssembler-1.0.1/FastMitoAssembler/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      406 2023-04-03 03:31:09.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     2146 2023-04-03 05:50:43.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/banner.txt
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-10 07:43:59.791342 FastMitoAssembler-1.0.1/FastMitoAssembler/bin/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        0 2023-04-03 09:20:29.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/bin/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1994 2023-04-06 15:10:37.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/bin/_other.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     3246 2023-04-07 04:04:25.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/bin/_run.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1085 2023-04-03 09:41:09.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/bin/main.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1043 2023-03-31 08:52:14.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/config.py
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-10 07:43:59.831800 FastMitoAssembler-1.0.1/FastMitoAssembler/smk/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      324 2023-04-07 03:57:50.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/smk/config.yaml
--rw-r--r--   0 suqingdong  (1000) disease   (8039)    10512 2023-04-10 02:32:36.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/smk/main.smk
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      508 2023-04-06 07:21:50.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/util.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      252 2023-04-06 14:26:08.000000 FastMitoAssembler-1.0.1/FastMitoAssembler/version.json
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-04-10 07:43:59.707197 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     3939 2023-04-10 07:43:57.000000 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      630 2023-04-10 07:43:57.000000 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-04-10 07:43:57.000000 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       70 2023-04-10 07:43:57.000000 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/entry_points.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       30 2023-04-10 07:43:57.000000 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       18 2023-04-10 07:43:57.000000 FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/top_level.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      144 2023-04-03 03:25:57.000000 FastMitoAssembler-1.0.1/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     3939 2023-04-10 07:43:59.864417 FastMitoAssembler-1.0.1/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     3257 2023-04-10 07:39:26.000000 FastMitoAssembler-1.0.1/README.md
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       30 2023-04-07 03:06:19.000000 FastMitoAssembler-1.0.1/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-04-10 07:43:59.875527 FastMitoAssembler-1.0.1/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1252 2023-04-03 09:31:59.000000 FastMitoAssembler-1.0.1/setup.py
+drwxr-xr-x   0 suqingdong  (8411) COG       (9318)        0 2023-04-14 05:57:49.396024 FastMitoAssembler-1.0.3/
+drwxr-xr-x   0 suqingdong  (8411) COG       (9318)        0 2023-04-14 05:57:49.322277 FastMitoAssembler-1.0.3/FastMitoAssembler/
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)      618 2023-04-11 03:48:02.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/__init__.py
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     2146 2023-04-03 05:50:43.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/banner.txt
+drwxr-xr-x   0 suqingdong  (8411) COG       (9318)        0 2023-04-14 05:57:49.373228 FastMitoAssembler-1.0.3/FastMitoAssembler/bin/
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)        0 2023-04-03 09:20:29.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/bin/__init__.py
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     2033 2023-04-11 03:53:15.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/bin/_other.py
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     4608 2023-04-12 10:07:28.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/bin/_run.py
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     1201 2023-04-11 03:55:09.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/bin/main.py
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     1043 2023-03-31 08:52:14.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/config.py
+drwxr-xr-x   0 suqingdong  (8411) COG       (9318)        0 2023-04-14 05:57:49.389062 FastMitoAssembler-1.0.3/FastMitoAssembler/smk/
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)      324 2023-04-11 03:43:17.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/smk/config.yaml
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)    11374 2023-04-12 06:38:18.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/smk/main.smk
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)       30 2023-04-11 03:51:50.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/smk/options.yaml
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)      685 2023-04-11 03:51:31.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/util.py
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)      252 2023-04-12 07:16:42.000000 FastMitoAssembler-1.0.3/FastMitoAssembler/version.json
+drwxr-xr-x   0 suqingdong  (8411) COG       (9318)        0 2023-04-14 05:57:49.354783 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     5137 2023-04-14 05:57:46.000000 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)      665 2023-04-14 05:57:46.000000 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)        1 2023-04-14 05:57:46.000000 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)       70 2023-04-14 05:57:46.000000 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/entry_points.txt
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)       30 2023-04-14 05:57:46.000000 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)       18 2023-04-14 05:57:46.000000 FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/top_level.txt
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)      144 2023-04-03 03:25:57.000000 FastMitoAssembler-1.0.3/MANIFEST.in
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     5137 2023-04-14 05:57:49.394929 FastMitoAssembler-1.0.3/PKG-INFO
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     4455 2023-04-13 02:00:43.000000 FastMitoAssembler-1.0.3/README.md
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)       30 2023-04-07 03:06:19.000000 FastMitoAssembler-1.0.3/requirements.txt
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)       38 2023-04-14 05:57:49.397398 FastMitoAssembler-1.0.3/setup.cfg
+-rw-r--r--   0 suqingdong  (8411) COG       (9318)     1252 2023-04-03 09:31:59.000000 FastMitoAssembler-1.0.3/setup.py
```

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler/banner.txt` & `FastMitoAssembler-1.0.3/FastMitoAssembler/banner.txt`

 * *Files identical despite different names*

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler/bin/_other.py` & `FastMitoAssembler-1.0.3/FastMitoAssembler/bin/_other.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from FastMitoAssembler import util
 
 ORGANELLE_DB_LIST = ['all', 'embplant_pt', 'embplant_mt', 'embplant_nr', 'fungus_mt', 'fungus_nr', 'animal_mt', 'other_pt']
 
 NCBI_TAXDUMP = 'https://ftp.ncbi.nih.gov/pub/taxonomy/taxdump.tar.gz'
 
-@click.group(help='prepare data')
+@click.group(help=click.style('prepare database', fg='cyan', bold=True))
 def prepare():
     pass
 
 
 @prepare.command(help='prepare ete3.NCBITaxa')
 @click.option('--taxdump_file', help=f'the taxdump file of NCBI, you can mamually download it from: {NCBI_TAXDUMP}')
 def ncbitaxa(**kwargs):
```

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler/bin/_run.py` & `FastMitoAssembler-1.0.3/FastMitoAssembler/bin/_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,92 @@
 import os
 import json
 
-import yaml
 import click
 import snakemake
 
-from FastMitoAssembler import MAIN_SMK, CONFIG_DEFAULT
+from FastMitoAssembler import (
+    MAIN_SMK,
+    DEFAULT_CONFIG_FILE,
+    DEFAULT_CONFIG,
+    DEFAULT_OPTION_FILE,
+    DEFAULT_OPTIONS,
+    util,
+)
 
-
-@click.command(help='run the workflow', no_args_is_help=True)
+@click.command(help=click.style('run the workflow', fg='cyan', bold=True), no_args_is_help=True)
 # custom configs
 @click.option('-r', '--reads_dir', help='the root directory of reads')
 @click.option('-o', '--result_dir', help='the directory of result', default='result', show_default=True)
-@click.option('-d', '--organelle_database', help='the database for GetOrganelle', default='animal_mt', show_default=True)
+@click.option('-d', '--organelle_database', help='the database for GetOrganelle', default=DEFAULT_CONFIG['organelle_database'], show_default=True)
 @click.option('-s', '--samples', help='the sample name', multiple=True)
 @click.option('--fq_path_pattern', help='the path pattern of fastq file', default='{sample}/{sample}_1.clean.fq.gz', show_default=True)
 
 # optional configs
-@click.option('--genetic_code', help='the genetic code table', type=int, default=5, show_default=True)
-@click.option('--genome_min_size', help='the min size of genome', type=int, default=12000, show_default=True)
-@click.option('--genome_max_size', help='the max size of genome', type=int, default=22000, show_default=True)
-@click.option('--insert_size', help='the in', type=int, default=39, show_default=True)
-@click.option('--kmer_size', help='the K-mer size used in NOVOPlasty assembly', type=int, default=39, show_default=True)
-@click.option('--read_length', help='the read length of Illumina short reads', type=int, default=150, show_default=True)
-@click.option('--max_mem_gb', help='the limit of RAM usage for NOVOPlasty (unit: GB)', type=int, default=5, show_default=True)
+@click.option('--genetic_code', help='the genetic code table', type=int, default=DEFAULT_CONFIG['genetic_code'], show_default=True)
+@click.option('--genome_min_size', help='the min size of genome', type=int, default=DEFAULT_CONFIG['genome_min_size'], show_default=True)
+@click.option('--genome_max_size', help='the max size of genome', type=int, default=DEFAULT_CONFIG['genome_max_size'], show_default=True)
+@click.option('--insert_size', help='the in', type=int, default=DEFAULT_CONFIG['insert_size'], show_default=True)
+@click.option('--kmer_size', help='the K-mer size used in NOVOPlasty assembly', type=int, default=DEFAULT_CONFIG['kmer_size'], show_default=True)
+@click.option('--read_length', help='the read length of Illumina short reads', type=int, default=DEFAULT_CONFIG['read_length'], show_default=True)
+@click.option('--max_mem_gb', help='the limit of RAM usage for NOVOPlasty (unit: GB)', type=int, default=DEFAULT_CONFIG['max_mem_gb'], show_default=True)
 
 @click.option('--seed_input', help='use a specific seed input, .fasta, or .gb')
 @click.option('--genes', help='the specific genes')
 
-# snakefile and configfile
+# snakefile, configfile and optionfile
 @click.option('--snakefile', help='the main snakefile', default=MAIN_SMK, show_default=True)
-@click.option('--configfile', help=f'the configfile for snakefile, template: {CONFIG_DEFAULT}')
+@click.option('--configfile', help=f'the configfile for snakefile, template: {DEFAULT_CONFIG_FILE}')
+@click.option('--optionfile', help=f'the optionfile for snakefile, template: {DEFAULT_OPTION_FILE}')
 
 ## snakemke options
-@click.option('--cores', help='use at most N CPU cores/jobs in parallel', type=int, default=4, show_default=True)
+@click.option('--cores', help='use at most N CPU cores/jobs in parallel', type=int, default=DEFAULT_OPTIONS['cores'], show_default=True)
 @click.option('--dryrun', help='do not execute anything, and display what would bedone', is_flag=True)
 def run(**kwargs):
 
     config = {}
     arguments = (
         'reads_dir result_dir organelle_database samples '
         'genetic_code genome_min_size genome_max_size insert_size kmer_size '
         'read_length max_mem_gb seed_input genes fq_path_pattern '
     ).strip().split()
     for key in arguments:
-        if kwargs[key]:
-            config[key] = kwargs[key]
+        config[key] = kwargs[key]
 
     # higher priority
     if kwargs['configfile'] and os.path.isfile(kwargs['configfile']):
         click.secho('>>> reading config from file: {configfile}'.format(**kwargs), fg='green', err=True)
-        with open(kwargs['configfile']) as f:
-            data = yaml.load(f, Loader=yaml.FullLoader)
-            for key, value in data.items():
-                if value:
-                    config[key] = value
+        data = util.read_yaml(kwargs['configfile'])
+        for key, value in data.items():
+            if value != '':
+                config[key] = value
     click.secho('>>> Configs:\n' + json.dumps(config, indent=2), fg='green', err=True)
 
+    if not (config['reads_dir'] and config['samples']):
+        click.secho(f'reads_dir and samples must supply!', err=True, fg='red')
+        exit(1)
+
+    for sample in config['samples']:
+        fq1 = os.path.join(config['reads_dir'], config['fq_path_pattern']).format(sample=sample)
+        if not os.path.isfile(fq1):
+            click.secho(f'reads file not exists, please check: {fq1}', err=True, fg='red')
+            exit(1)
+
+    if not all([isinstance(sample, str) for sample in config['samples']]):
+        click.secho('sample name must be a string, please check your input: {samples}'.format(**config), fg='red')
+        exit(1)
+
     options = {
         'cores': kwargs['cores'],
         'dryrun': kwargs['dryrun'],
         'printshellcmds': True,
     }
+    if kwargs['optionfile'] and os.path.isfile(kwargs['optionfile']):
+        click.secho('>>> reading options from file: {optionfile}'.format(**kwargs), fg='green', err=True)
+        data = util.read_yaml(kwargs['optionfile'])
+        for key, value in data.items():
+            if value != '':
+                options[key] = value
+
     click.secho('>>> Options:\n' + json.dumps(options, indent=2), fg='green', err=True)
 
     snakemake.snakemake(kwargs['snakefile'], config=config, **options)
-
```

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler/bin/main.py` & `FastMitoAssembler-1.0.3/FastMitoAssembler/bin/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import json
 
 import yaml
 import click
 import snakemake
 
-from FastMitoAssembler import MAIN_SMK, CONFIG_DEFAULT, VERSION, BANNER
+from FastMitoAssembler import MAIN_SMK, DEFAULT_CONFIG_FILE, DEFAULT_OPTION_FILE, VERSION, BANNER
 from FastMitoAssembler.bin._run import run
 from FastMitoAssembler.bin._other import prepare
 
 
 CONTEXT_SETTINGS = dict(
     help_option_names=['-?', '-h', '--help'], max_content_width=800,)
 BANNER = '\b\n'.join(BANNER.split('\n'))
 HELP = f'''\n\n\b\n{BANNER}\n'''
 
 
 __EPILOG__ = click.style('''
 \n\b
 Snakefile: {MAIN_SMK}
-Configfile: {CONFIG_DEFAULT}
+Configfile: {DEFAULT_CONFIG_FILE}
+Optionfile: {DEFAULT_OPTION_FILE}
 
 Contact: {author}<{author_email}>
-''', fg='white').format(MAIN_SMK=MAIN_SMK, CONFIG_DEFAULT=CONFIG_DEFAULT, **VERSION)
+''', fg='white').format(MAIN_SMK=MAIN_SMK, DEFAULT_CONFIG_FILE=DEFAULT_CONFIG_FILE, DEFAULT_OPTION_FILE=DEFAULT_OPTION_FILE, **VERSION)
 
 
 @click.group(
     context_settings=CONTEXT_SETTINGS,
     name=VERSION['prog'],
     help=click.style(HELP, fg='cyan', italic=True),
     epilog=__EPILOG__,
```

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler/config.py` & `FastMitoAssembler-1.0.3/FastMitoAssembler/config.py`

 * *Files identical despite different names*

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler/smk/main.smk` & `FastMitoAssembler-1.0.3/FastMitoAssembler/smk/main.smk`

 * *Files 9% similar despite different names*

```diff
@@ -31,52 +31,62 @@
 # MitozAnnotate configuration
 CLADE = config.get('clade', 'Annelida-segmented-worms')
 GENETIC_CODE = config.get('genetic_code', 5)
 THREAD_NUMBER = config.get('thread_number', 20)
 # ==============================================================
 
 # ==============================================================
+# Log directory
+LOG_DIR = Path(config.get("log_dir", "logs")).resolve()
 # Output directory
 RESULT_DIR = Path(config.get("result_dir", "result")).resolve()
 SAMPLE_DIR = partial(os.path.join, RESULT_DIR, "{sample}")
 MEANGS_DIR = partial(SAMPLE_DIR, "1.MEANGS")
 NOVOPLASTY_DIR = partial(SAMPLE_DIR, "2.NOVOPlasty")
-ORGANELL_DIR = partial(SAMPLE_DIR, "3.GetOrganelle")
+ORGANELLE_DIR = partial(SAMPLE_DIR, "3.GetOrganelle")
 MITOZ_ANNO_DIR = partial(SAMPLE_DIR, "4.MitozAnnotate")
-MITOZ_ANNO_RESULT_DIR = partial(MITOZ_ANNO_DIR, f"{{sample}}.{ORGANELLE_DB}.K127.scaffolds.graph1.1.path_sequence.new.fasta.result")
+MITOZ_ANNO_RESULT_DIR = partial(MITOZ_ANNO_DIR, f"{{sample}}.{ORGANELLE_DB}.get_organelle.fasta.result")
+
+# Benchmark directory
+BENCHMARK_DIR = Path(config.get("benchmark_dir", "benchmark")).resolve()
+
+# input/output
+seed_fas = MEANGS_DIR("{sample}_deep_detected_mito.fas")
+novoplasty_config = NOVOPLASTY_DIR("config.txt")
+novoplasty_fasta = NOVOPLASTY_DIR("{sample}.novoplasty.fasta")
+organelle_fasta_new = ORGANELLE_DIR(f"{ORGANELLE_DB}.get_organelle.fasta")
 # ==============================================================
 
 # ==============================================================
 # Read data
 READS_DIR = Path(config.get("reads_dir", ".")).resolve()
 FQ_PATH_PATTERN = config.get('fq_path_pattern', '{sample}/{sample}_1.clean.fq.gz')
 FQ1 = READS_DIR.joinpath(FQ_PATH_PATTERN)
 FQ2 = READS_DIR.joinpath(FQ_PATH_PATTERN.replace('1', '2'))
 
 
 # FQ1 = READS_DIR.joinpath("{sample}_1.clean.fq.gz")
 # FQ2 = READS_DIR.joinpath("{sample}_2.clean.fq.gz")
 READS_NUM_5G = round(5e9 / 2 / READ_LENGTH)
+CUT_5G_DATA = config.get('cut_5g_data', 'yes')
 # ==============================================================
 
 # default target
 rule all:
     """
     Specify the output files for all samples using the expand function.
     """
     message: "Congratulations, the pipeline process is complete!"
     input:
-        expand(
-            MITOZ_ANNO_RESULT_DIR("circos.png"),
-            sample=SAMPLES,
-        ),
+        expand(MITOZ_ANNO_RESULT_DIR("circos.png"), sample=SAMPLES),
+        expand(MITOZ_ANNO_RESULT_DIR("summary.txt"), sample=SAMPLES),
+        expand(MITOZ_ANNO_RESULT_DIR(f"{{sample}}_{ORGANELLE_DB}.get_organelle.fasta_mitoscaf.fa.gbf"), sample=SAMPLES),
     run:
         print('ok')
 
-
 rule MEANGS:
     """
     Detect and retrieve the longest mitochondrial sequence using MEANGS.
     - https://github.com/YanCCscu/MEANGS/
 
     Input:
     fq1, fq2: Paired clean FASTQ format files.
@@ -91,22 +101,24 @@
     Note:
     Keep the first reads only as output
     """
     input:
         fq1=FQ1,
         fq2=FQ2,
     output:
-        seed_fas=MEANGS_DIR("{sample}_deep_detected_mito.fas"),
+        seed_fas=seed_fas,
     params:
         outdir=MEANGS_DIR(),
         seed_input=SEED_INPUT,
     message: "MEANGS for sample: {wildcards.sample}"
+    log: LOG_DIR.joinpath('{sample}', 'meangs.log')
+    benchmark: BENCHMARK_DIR.joinpath('{sample}', 'meangs.stat')
     shell:
         """
-        mkdir -p {params.outdir}
+        (mkdir -p {params.outdir}
         cd {params.outdir}
 
         seed_input={params.seed_input}
 
         if [[ $seed_input =~ \.gb[kf]?$ ]];then
             genbank.py -f fasta $seed_input | seqkit head -n1 -w0 -o {output.seed_fas}
         elif [[ $seed_input =~ \.fa[sta]*$ ]];then
@@ -117,15 +129,15 @@
                 -2 {input.fq2} \\
                 -o {wildcards.sample} \\
                 -t 2 \\
                 -n 2000000 \\
                 -i 350 \\
                 --deepin
             seqkit head -n1 -w0 -o {output.seed_fas} {wildcards.sample}/{wildcards.sample}_deep_detected_mito.fas
-        fi
+        fi) 2>{log}.stderr 1>{log}.stdout
         """
 
 rule NOVOPlasty_config:
     """
     Generate the configuration file for NOVOPlasty.
 
     Input:
@@ -137,23 +149,21 @@
 
     Parameters:
     output_path: Output directory.
     """
     input:
         fq1=FQ1,
         fq2=FQ2,
-        seed_fas=MEANGS_DIR("{sample}_deep_detected_mito.fas"),
+        seed_fas=seed_fas,
     output:
-        novoplasty_config=NOVOPLASTY_DIR("config.txt"),
+        novoplasty_config=novoplasty_config,
     params:
         output_path=NOVOPLASTY_DIR() + os.path.sep,
     message: "NOVOPlasty_config for sample: {wildcards.sample}"
     run:
-
-
         with safe_open(output.novoplasty_config, "w") as out:
             context = NOVOPLASTY_CONFIG_TPL.render(
                 seed_fasta=input.seed_fas,
                 sample=wildcards.sample,
                 fq1=input.fq1,
                 fq2=input.fq2,
                 output_path=params.output_path,
@@ -175,62 +185,70 @@
     fq1, fq2: Paired clean FASTQ format files.
     novoplasty_config: The configuration file for NOVOPlasty.
 
     Output:
     novoplasty_contigs_new: The assembled mitochondrial genome in FASTA format.
     """
     input:
-        novoplasty_config=NOVOPLASTY_DIR("config.txt"),
+        novoplasty_config=novoplasty_config,
     output:
-        novoplasty_contigs=NOVOPLASTY_DIR("Contigs_1_{sample}.fasta"),
-        novoplasty_contigs_new=NOVOPLASTY_DIR("Contigs_1_{sample}.new.fasta"),
+        novoplasty_fasta=novoplasty_fasta,
+    params:
+        output_path = NOVOPLASTY_DIR(),
     message: "NOVOPlasty for sample: {wildcards.sample}"
+    log: LOG_DIR.joinpath('{sample}', 'novoplasty.log')
+    benchmark: BENCHMARK_DIR.joinpath('{sample}', 'novoplasty.stat')
     shell:
         """
+        (
+        cd {params.output_path}
+
         NOVOPlasty.pl -c {input.novoplasty_config}
 
         # remove +xxx
         seqkit replace -w0 \\
             -p "\+.+" -r "" \\
-            -o {output.novoplasty_contigs_new} \\
-            {output.novoplasty_contigs}
+            -o {output.novoplasty_fasta} \\
+            *{wildcards.sample}.fasta
+        ) 2>{log}.stderr 1>{log}.stdout
         """
 
 rule GetOrganelle:
     """
     Assemble mitochondrial genome using GetOrganelle.
     - https://github.com/Kinggerm/GetOrganelle
 
     Input:
     fq1, fq2: Paired clean FASTQ format files.
     novoplasty_contigs_new: The contig sequences generated by NOVOPlasty.
 
     Output:
-    organelle_fasta: Intermediary assembled mitochondrial genome in FASTA format.
     organelle_fasta_new: The improved version of organelle_fasta after the second assembly by GetOrganelle
 
     Params:
     output_path: Output directory.
 
     Note:
     This rule use 5G data as input.
     """
     input:
         fq1=FQ1,
         fq2=FQ2,
-        novoplasty_contigs_new=NOVOPLASTY_DIR("Contigs_1_{sample}.new.fasta"),
+        novoplasty_fasta=novoplasty_fasta,
     output:
-        organelle_fasta=ORGANELL_DIR("organelle", f"{ORGANELLE_DB}.K127.scaffolds.graph1.1.path_sequence.fasta"),
-        organelle_fasta_new=ORGANELL_DIR(f"{ORGANELLE_DB}.K127.scaffolds.graph1.1.path_sequence.new.fasta"),
+        organelle_fasta_new=organelle_fasta_new,
     params:
-        output_path=ORGANELL_DIR(),
-        output_path_temp=ORGANELL_DIR("organelle"),
+        output_path=ORGANELLE_DIR(),
+        output_path_temp=ORGANELLE_DIR("organelle"),
     message: "GetOrganelle for sample: {wildcards.sample}"
+    log: LOG_DIR.joinpath('{sample}', 'get_organelle.log')
+    benchmark: BENCHMARK_DIR.joinpath('{sample}', 'get_organelle.stat')
     shell:
         """
+        (
         mkdir -p {params.output_path}
         cd {params.output_path}
 
         # get 5G data
         if [ ! -e {wildcards.sample}_1.5G.fq.gz ];then
             seqkit stats {input.fq1} > {wildcards.sample}.fq1.stats.txt
             reads_num_fq1=$(awk 'NR==2{{print $4}}' {wildcards.sample}.fq1.stats.txt | sed 's#,##g')
@@ -252,22 +270,24 @@
             -2 {wildcards.sample}_2.5G.fq.gz \\
             -R 20 \\
             -k 21,33,45,55,65,75,85,95,105,111,127 \\
             -F {ORGANELLE_DB} \\
             -o {params.output_path_temp} \\
             --reduce-reads-for-coverage inf \\
             --max-reads inf \\
-            -s {input.novoplasty_contigs_new}
+            -s {input.novoplasty_fasta}
 
         # replace '+', 'circular' characters
         seqkit replace -w0 \\
-            -p ".*(circulars).*" -r "{wildcards.sample} topology=circular" \\
-            -p ".+" -r "{wildcards.sample} topology=linear" \\
-            -o {output.organelle_fasta_new} \\
-            {output.organelle_fasta}
+            -p ".*(circular).*" -r "{wildcards.sample} topology=circular" \\
+            organelle/*fasta |
+        seqkit replace -w0 \\
+            -p "^scaffold.*" -r "{wildcards.sample} topology=linear" \\
+            -o {output.organelle_fasta_new}
+        ) 2>{log}.stderr 1>{log}.stdout
     """
 
 rule MitozAnnotate:
     """
     Annotate mitochondrial genome using MitoZ.
     - https://github.com/linzhi2013/MitoZ
 
@@ -276,34 +296,38 @@
     organelle_fasta_new: Path to the assembled mitochondrial genome in FASTA format generated by GetOrganelle.
 
     Outputs:
     circos: Path to the circular plot of the annotated mitochondrial genome.
 
     Params:
     outdir: Path to the directory where the output files should be saved.
-
     """
     input:
         fq1=FQ1,
         fq2=FQ2,
-        organelle_fasta_new=ORGANELL_DIR(f"{ORGANELLE_DB}.K127.scaffolds.graph1.1.path_sequence.new.fasta"),
+        organelle_fasta_new=organelle_fasta_new,
     output:
-        # circos=MITOZ_ANNO_DIR(f"{{sample}}.{ORGANELLE_DB}.K127.scaffolds.graph1.1.path_sequence.new.fasta.result", "circos.png"),
         circos=MITOZ_ANNO_RESULT_DIR("circos.png"),
+        summary=MITOZ_ANNO_RESULT_DIR("summary.txt"),
+        genbank=MITOZ_ANNO_RESULT_DIR(f"{{sample}}_{ORGANELLE_DB}.get_organelle.fasta_mitoscaf.fa.gbf"),
     params:
         outdir=MITOZ_ANNO_DIR()
     message: "MitozAnnotate for sample: {wildcards.sample}"
+    log: LOG_DIR.joinpath('{sample}', 'mitoz_annotate.log')
+    benchmark: BENCHMARK_DIR.joinpath('{sample}', 'mitoz_annotate.stat')
     shell:
         """
+        (
         mkdir -p {params.outdir}
         cd {params.outdir}
 
         mitoz annotate \\
             --outprefix {wildcards.sample} \\
             --thread_number {THREAD_NUMBER} \\
             --fastafiles {input.organelle_fasta_new} \\
             --fq1 {input.fq1} \\
             --fq2 {input.fq2} \\
             --species_name "{wildcards.sample}" \\
             --genetic_code {GENETIC_CODE} \\
             --clade {CLADE}
+        ) 2>{log}.stderr 1>{log}.stdout
         """
```

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/PKG-INFO` & `FastMitoAssembler-1.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,10 @@
-Metadata-Version: 2.1
-Name: FastMitoAssembler
-Version: 1.0.1
-Summary: Fast Assembler Workflow for MitoGenome
-Home-page: https://github.com/suqingdong/FastMitoAssembler
-Author: suqingdong
-Author-email: suqingdong1114@gmail.com
-License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-Description-Content-Type: text/markdown
-
 # Fast Assembler Workflow for MitoGenome
 > `FastMitoAssembler` is a software for fast, accurate assembly of mitochondrial genomes and generation of annotation documents.
 
-### Softwares
-- [MEANGS](https://github.com/YanCCscu/meangs)
-- [NOVOplasty](https://github.com/Edith1715/NOVOplasty)
-- [GetOrganelle](https://github.com/Kinggerm/GetOrganelle)
-- [SPAdes](https://github.com/ablab/spades)
-- [MitoZ](https://github.com/linzhi2013/MitoZ)
-- [NCBI-Blast](https://blast.ncbi.nlm.nih.gov/doc/blast-help/downloadblastdata.html)
-
 ### Installation
 #### 1. create environment
 ```bash
 # method 1: use conda [slowly and need large resources]
 conda env create -f environment.yml
 
 # method 2: use mamba [*recommended*]
@@ -68,41 +42,49 @@
 #### 3. install FastMitoAssembler
 ```bash
 python -m pip install -U FastMitoAssembler
 # or
 python -m pip install -U dist/FastMitoAssembler*whl
 ```
 
-### Prepare
+### Prepare Database
 ```bash
 FastMitoAssembler prepare
 
 # 1. prepare ete3.NCBITaxa
-- `FastMitoAssembler prepare ncbitaxa # download taxdump.tar.gz automaticlly`
-
+FastMitoAssembler prepare ncbitaxa # download taxdump.tar.gz automaticlly
 FastMitoAssembler prepare ncbitaxa --taxdump_file taxdump.tar.gz 
 
 # 2. prepare database for GetOrganelle
 FastMitoAssembler prepare organelle --list  # list configured databases
 FastMitoAssembler prepare organelle -a animal_mt  # config a single database
-FastMitoAssembler prepare organelle -a animal_mt -a embplant_mt # config multiple databaes
+FastMitoAssembler prepare organelle -a animal_mt -a embplant_mt # config multiple databases
 FastMitoAssembler prepare organelle -a all  # config all databases
+```
+
+### Run Workflow
 
-### Usage
+`config.yaml` example:
+```yaml
+reads_dir: '../data/'
+samples: ['2222-4']
+fq_path_pattern: '{sample}/{sample}_1.clean.fq.gz' # the reads 1 path pattern relative to `reads_dir`
+```
+see the main Snakefile and Template configfile with: `FastMitoAssembler --help` 
 #### Use with Client
 ```bash
-FastMitoAssembler
+FastMitoAssembler --help
 
 FastMitoAssembler run --help
 
 # run with configfile [recommended]
 FastMitoAssembler run --configfile config.yaml
 
 # run with parameters
-FastMitoAssembler run --reads-dir ../data --samples S1 --samples S2
+FastMitoAssembler run --reads_dir ../data --samples S1 --samples S2
 
 # set cores
 FastMitoAssembler run --configfile config.yaml --cores 8
 
 # dryrun the workflow
 FastMitoAssembler run --configfile config.yaml --dryrun
 ```
@@ -112,10 +94,46 @@
 snakemake -s /path/to/FastMitoAssembler/smk/main.smk -c config.yaml --cores 4
 
 snakemake -s /path/to/FastMitoAssembler/smk/main.smk -c config.yaml --cores 4 --printshellcmds
 
 snakemake -s /path/to/FastMitoAssembler/smk/main.smk -c config.yaml --printshellcmds --dryrun
 ```
 
-#### Use in Docker
-[docker](./docker/README.md)
+#### Use with Docker
+[docker-readme](./docker/README.md)
 
+
+### Example Results Directory
+- `[*]` represents the main result
+
+```
+result/
+└── 2222-4
+    ├── 1.MEANGS
+    │   ├── 2222-4
+    │   ├── 2222-4_deep_detected_mito.fas  [*]
+    │   └── scaffold_seeds.fas
+    ├── 2.NOVOPlasty
+    │   ├── config.txt
+    │   ├── Contigs_1_2222-4.fasta
+    │   ├── 2222-4.novoplasty.fasta  [*]
+    │   ├── contigs_tmp_2222-4.txt
+    │   └── log_2222-4.txt
+    ├── 3.GetOrganelle
+    │   ├── 2222-4_1.5G.fq.gz
+    │   ├── 2222-4_2.5G.fq.gz
+    │   ├── 2222-4.fq1.stats.txt
+    │   ├── animal_mt.get_organelle.fasta  [*]
+    │   └── organelle
+    └── 4.MitozAnnotate
+        ├── 2222-4.animal_mt.get_organelle.fasta.result  [*]
+        └── tmp_2222-4_animal_mt.get_organelle.fasta_mitoscaf.fa
+
+```
+
+##### Softwares Used
+- [MEANGS](https://github.com/YanCCscu/meangs)
+- [NOVOplasty](https://github.com/Edith1715/NOVOplasty)
+- [GetOrganelle](https://github.com/Kinggerm/GetOrganelle)
+- [SPAdes](https://github.com/ablab/spades)
+- [MitoZ](https://github.com/linzhi2013/MitoZ)
+- [NCBI-Blast](https://blast.ncbi.nlm.nih.gov/doc/blast-help/downloadblastdata.html)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FastMitoAssembler-1.0.1/FastMitoAssembler.egg-info/SOURCES.txt` & `FastMitoAssembler-1.0.3/FastMitoAssembler.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 FastMitoAssembler.egg-info/requires.txt
 FastMitoAssembler.egg-info/top_level.txt
 FastMitoAssembler/bin/__init__.py
 FastMitoAssembler/bin/_other.py
 FastMitoAssembler/bin/_run.py
 FastMitoAssembler/bin/main.py
 FastMitoAssembler/smk/config.yaml
-FastMitoAssembler/smk/main.smk
+FastMitoAssembler/smk/main.smk
+FastMitoAssembler/smk/options.yaml
```

### Comparing `FastMitoAssembler-1.0.1/setup.py` & `FastMitoAssembler-1.0.3/setup.py`

 * *Files identical despite different names*

