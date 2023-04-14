# Comparing `tmp/slate-nlp-1.0.3.tar.gz` & `tmp/slate-nlp-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slate-nlp-1.0.3.tar", last modified: Sun Sep  8 00:08:07 2019, max compression
+gzip compressed data, was "slate-nlp-1.1.1.tar", last modified: Fri Apr 14 03:42:01 2023, max compression
```

## Comparing `slate-nlp-1.0.3.tar` & `slate-nlp-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,55 @@
-drwxr-xr-x   0 jkk        (501) staff       (20)        0 2019-09-08 00:08:07.000000 slate-nlp-1.0.3/
--rw-r--r--   0 jkk        (501) staff       (20)    21929 2019-09-08 00:08:07.000000 slate-nlp-1.0.3/PKG-INFO
--rw-r--r--   0 jkk        (501) staff       (20)    18448 2019-09-06 16:42:10.000000 slate-nlp-1.0.3/README.md
--rw-r--r--   0 jkk        (501) staff       (20)       67 2019-09-08 00:08:07.000000 slate-nlp-1.0.3/setup.cfg
--rw-r--r--   0 jkk        (501) staff       (20)     1090 2019-09-08 00:08:02.000000 slate-nlp-1.0.3/setup.py
-drwxr-xr-x   0 jkk        (501) staff       (20)        0 2019-09-08 00:08:07.000000 slate-nlp-1.0.3/slate/
--rw-r--r--   0 jkk        (501) staff       (20)       15 2019-07-16 20:03:55.000000 slate-nlp-1.0.3/slate/__init__.py
--rw-r--r--   0 jkk        (501) staff       (20)       66 2019-07-16 21:14:28.000000 slate-nlp-1.0.3/slate/__main__.py
--rw-r--r--   0 jkk        (501) staff       (20)    19450 2019-09-06 14:41:43.000000 slate-nlp-1.0.3/slate/annotate.py
--rw-r--r--   0 jkk        (501) staff       (20)     9207 2019-07-16 17:10:19.000000 slate-nlp-1.0.3/slate/config.py
--rw-r--r--   0 jkk        (501) staff       (20)    37662 2019-09-06 16:39:32.000000 slate-nlp-1.0.3/slate/data.py
--rw-r--r--   0 jkk        (501) staff       (20)    21729 2019-09-06 14:42:03.000000 slate-nlp-1.0.3/slate/view.py
-drwxr-xr-x   0 jkk        (501) staff       (20)        0 2019-09-08 00:08:07.000000 slate-nlp-1.0.3/slate_nlp.egg-info/
--rw-r--r--   0 jkk        (501) staff       (20)    21929 2019-09-08 00:08:06.000000 slate-nlp-1.0.3/slate_nlp.egg-info/PKG-INFO
--rw-r--r--   0 jkk        (501) staff       (20)      294 2019-09-08 00:08:06.000000 slate-nlp-1.0.3/slate_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 jkk        (501) staff       (20)        1 2019-09-08 00:08:06.000000 slate-nlp-1.0.3/slate_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 jkk        (501) staff       (20)       47 2019-09-08 00:08:06.000000 slate-nlp-1.0.3/slate_nlp.egg-info/entry_points.txt
--rw-r--r--   0 jkk        (501) staff       (20)        6 2019-09-08 00:08:06.000000 slate-nlp-1.0.3/slate_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.241189 slate-nlp-1.1.1/
+-rw-r--r--   0 jkum0593   (503) staff       (20)      121 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/.gitignore
+-rw-r--r--   0 jkum0593   (503) staff       (20)      780 2023-04-14 03:03:02.000000 slate-nlp-1.1.1/LICENSE.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)    22691 2023-04-14 03:42:01.241028 slate-nlp-1.1.1/PKG-INFO
+-rw-r--r--   0 jkum0593   (503) staff       (20)    20942 2023-04-10 11:28:24.000000 slate-nlp-1.1.1/README.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)      213 2022-10-24 01:09:40.000000 slate-nlp-1.1.1/_config.yml
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.228370 slate-nlp-1.1.1/_includes/
+-rw-r--r--   0 jkum0593   (503) staff       (20)      399 2022-10-24 01:08:59.000000 slate-nlp-1.1.1/_includes/head-custom-google-analytics.html
+-rw-r--r--   0 jkum0593   (503) staff       (20)     3596 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/ideas-for-improvement.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)     3854 2023-04-10 06:01:14.000000 slate-nlp-1.1.1/ner-book.config
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.231468 slate-nlp-1.1.1/paper/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    12450 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.bib
+-rw-r--r--   0 jkum0593   (503) staff       (20)   447789 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.pdf
+-rw-r--r--   0 jkum0593   (503) staff       (20)    22052 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.sty
+-rw-r--r--   0 jkum0593   (503) staff       (20)    24066 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.tex
+-rw-r--r--   0 jkum0593   (503) staff       (20)     2244 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/comparison.tex
+-rw-r--r--   0 jkum0593   (503) staff       (20)      434 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/makefile
+-rw-r--r--   0 jkum0593   (503) staff       (20)     4356 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/post-publish-supp.tex
+-rw-r--r--   0 jkum0593   (503) staff       (20)   342538 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/screenshot-adjudicate.png
+-rw-r--r--   0 jkum0593   (503) staff       (20)   198920 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/screenshot.png
+-rw-r--r--   0 jkum0593   (503) staff       (20)     1095 2023-04-14 03:41:56.000000 slate-nlp-1.1.1/pyproject.toml
+-rw-r--r--   0 jkum0593   (503) staff       (20)       38 2023-04-14 03:42:01.241231 slate-nlp-1.1.1/setup.cfg
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.236742 slate-nlp-1.1.1/slate/
+-rw-r--r--   0 jkum0593   (503) staff       (20)       15 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/slate/__init__.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)       66 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/slate/__main__.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)    19913 2023-04-10 11:27:42.000000 slate-nlp-1.1.1/slate/annotate.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)     9207 2023-04-07 01:20:03.000000 slate-nlp-1.1.1/slate/config.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)    38565 2023-04-10 11:29:42.000000 slate-nlp-1.1.1/slate/data.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)    21415 2023-04-10 06:31:20.000000 slate-nlp-1.1.1/slate/view.py
+-rwxr-xr-x   0 jkum0593   (503) staff       (20)       95 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/slate.py
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.237748 slate-nlp-1.1.1/slate_nlp.egg-info/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    22691 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 jkum0593   (503) staff       (20)     1291 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)        1 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)       46 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/entry_points.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)        6 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.238489 slate-nlp-1.1.1/tutorial/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    17655 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/config-example.txt
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.240660 slate-nlp-1.1.1/tutorial/data/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    12086 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)       55 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations0
+-rw-r--r--   0 jkum0593   (503) staff       (20)       87 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations1
+-rw-r--r--   0 jkum0593   (503) staff       (20)      166 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations2
+-rw-r--r--   0 jkum0593   (503) staff       (20)      220 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations3
+-rw-r--r--   0 jkum0593   (503) staff       (20)        6 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations0
+-rw-r--r--   0 jkum0593   (503) staff       (20)       12 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations1
+-rw-r--r--   0 jkum0593   (503) staff       (20)       18 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations2
+-rw-r--r--   0 jkum0593   (503) staff       (20)       24 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations3
+-rw-r--r--   0 jkum0593   (503) staff       (20)    14560 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data1.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)       32 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_file_list.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)      220 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/list_with_disagreements.category.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)      198 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/list_with_disagreements.link.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)     2318 2023-04-10 11:28:10.000000 slate-nlp-1.1.1/tutorial/label.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)     2417 2023-04-10 11:28:14.000000 slate-nlp-1.1.1/tutorial/link.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)     4628 2023-04-10 06:25:50.000000 slate-nlp-1.1.1/tutorial/ner.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `slate-nlp-1.0.3/PKG-INFO` & `slate-nlp-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,357 +1,425 @@
 Metadata-Version: 2.1
 Name: slate-nlp
-Version: 1.0.3
+Version: 1.1.1
 Summary: A terminal-based text annotation tool
-Home-page: https://jkk.name/slate/
-Author: Jonathan K. Kummerfeld
-Author-email: jkk@berkeley.edu
-License: UNKNOWN
-Description: This is a tool for labeling text documents.
-        Slate supports annotation at different scales (spans of characters, tokens, and lines, or a document) and of different types (free text, labels, and links).
-        This covers a range of tasks, such as Part-of-Speech tagging, Named Entity Recognition, Text Classification (including Sentiment Analysis), Discourse Structure, and more.
+Author-email: "Jonathan K. Kummerfeld" <jonathan.kummerfeld@sydney.edu.au>
+License: Copyright (c) 2016-2023 Jonathan K Kummerfeld <jonathan.kummerfeld@sydney.edu.au>
         
-        Why use this tool over the range of other text annotation tools out there?
-        
-        - Fast
-        - Trivial installation
-        - Focuses all of the screen space on annotation (good for large fonts)
-        - Terminal based, so it works in constrained environments (e.g. only allowed ssh access to a machine)
-        - Not difficult to configure and modify
-        
-        Note - this repository is **not** for the "Segment and Link-based Annotation Tool, Enhanced", which can be found [here](https://bitbucket.org/dainkaplan/slate/wiki/Home) and was first presented at [LREC 2010](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf).
-        See 'Citing' below for additional notes on that work.
-        
-        ## Installation
-        
-        Two options:
-        
-        ### 1. Install with pip
-        ```bash
-        pip install slate-nlp
-        ```
-        
-        Then run from any directory in one of two ways:
-        ```
-        slate
-        python -m slate
-        ```
-        
-        ### 2. Or download and run without installing
-        Either download as a zip file:
-        ```bash
-        curl https://codeload.github.com/jkkummerfeld/slate/zip/master -o "slate.zip"
-        unzip slate.zip
-        cd slate-master
-        ```
-        Or clone the repository:
-        ```bash
-        git clone https://github.com/jkkummerfeld/slate
-        cd slate
-        ```
-        
-        Then run with either of:
-        ```
-        python slate.py
-        ./slate.py
-        ```
-        To run from another directory, use:
-        ```
-        python PATH_TO_SLATE/slate.py
-        PATH_TO_SLATE/slate.py
-        ```
-        
-        ### Requirements
-        
-        The code requires only Python (2 or 3) and can be run out of the box.
-        Your terminal must be at least 80 characters wide and 20 tall to use the tool.
-        
-        ## Citing
-        
-        If you use this tool in your work, please cite:
-        
-        ```
-        @InProceedings{acl19slate,
-          title     = {SLATE: A Super-Lightweight Annotation Tool for Experts},
-          author    = {Jonathan K. Kummerfeld},
-          booktitle = {Proceedings of {ACL} 2019, System Demonstrations},
-          location  = {Florence, Italy},
-          month     = {July},
-          year      = {2019},
-          pages     = {},
-          url       = {https://github.com/jkkummerfeld/slate/raw/master/paper/acl19slate.pdf},
-          software  = {https://jkk.name/slate},
-        }
-        ```
-        
-        While presenting this work at ACL I learned of another annotation tool called SLATE.
-        That tool was first described in "Annotation Process Management Revisited", [Kaplan et al. (LREC 2010)](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf) and then in "Slate - A Tool for Creating and Maintaining Annotated Corpora", [Kaplan et al. (JLCL 2011)](https://jlcl.org/content/2-allissues/12-Heft2-2011/11.pdf).
-        It takes a very different approach, using a web based interface that includes a suite of project management tools as well as annotation.
-        The code it available at [https://bitbucket.org/dainkaplan/slate/wiki/Home](https://bitbucket.org/dainkaplan/slate/wiki/Home).
-        
-        ## Getting Started
-        
-        Note: if you used pip to install, reaplce `python slate.py` with `slate` everywhere below.
-        
-        Run `python slate.py <filename>` to start annotating `<filename>` with labels over spans of tokens.
-        The entire interface is contained in your terminal, there is no GUI.
-        With command line arguments you can vary properties such as the type of annotation (labels or links) and scope of annotation (characters, tokens, lines, documents).
-        
-        The input file should be plain text, organised however you like.
-        Prepare the data with your favourite sentence splitting and/or tokenisation software (e.g., [SpaCy](https://spacy.io)).
-        If you use Python 3 then unicode should be supported, but the code has not been tested extensively with non-English text (please share any issues!).
-        
-        When you start the tool it displays a set of core commands by default.
-        These are also specified below, along with additional commands.
-        
-        The tool saves annotations in a separate file (`<filename>.annotations` by default, this can be varied with a file list as described below).
-        Annotation files are formatted with one line per annotated item.
-        The item is specified with a tuple of numbers.
-        For labels, the item is followed by a hyphen and the list of labels.
-        For links, there are two items on the line before the hyphen.
-        For example, these are two annotation files, one for labels of token spans and the other for links between lines:
-        
-        ```
-        ==> label.annotations <==
-        (2, 1) - label:a
-        ((3, 5), (3, 8)) - label:a
-        (7, 8) - label:s label:a
-        
-        ==> link.annotations <==
-        13 0 - 
-        13 7 - 
-        16 7 - 
-        ```
-        
-        A few notes:
-        - The second label annotation is on a span of tokens, going from 5 to 8 on line 3.
-        - The third label annotation has two labels.
-        - The line annotations only have one number to specify the item.
-        - When the same line is linked to multiple other lines, each link is a separate item.
-        
-        ### Tutorials
-        
-        Included in this repository are a set of interactive tutorials that teach you how to use the tool from within the tool itself.
-        
-        Task | Command
-        ---- | --------
-        Labelling spans of text in a document | `python slate.py tutorial/label.md -t categorical -s token -o -hh -l log.tutorial.label.txt`
-        Linking lines in a document | `python slate.py tutorial/link.md -t link -s line -o -hh -l log.tutorial.link.txt`
-        Comparing annotations | To be created
-        
-        ### Example Workflow
-        
-        This tool has already been used for two annotation efforts involving multiple annotators ([Durrett et al., 2017](http://jkk.name/publication/emnlp17forums/) and [Kummerfeld et al., 2018](http://jkk.name/publication/arxiv18disentangle/)).
-        Our workflow was as follows:
-        
-        - Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
-        - Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
-        - Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
-        
-        ## Detailed Usage Instructions
-        
-        ### Invocation options
-        
-        ```
-        usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
-                        [-s {character,token,line,document}] [-c CONFIG_FILE]
-                        [-l LOG_PREFIX] [-ld] [-hh] [-r] [-o] [-ps] [-pf]
-                        [--do-not-show-linked] [--alternate-comparisons]
-                        [data [data ...]]
-        
-        A tool for annotating text data.
-        
-        positional arguments:
-          data                  Files to be annotated
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -d DATA_LIST [DATA_LIST ...], --data-list DATA_LIST [DATA_LIST ...]
-                                Files containing lists of files to be annotated
-          -t {categorical,link}, --ann-type {categorical,link}
-                                The type of annotation being done.
-          -s {character,token,line,document}, --ann-scope {character,token,line,document}
-                                The scope of annotation being done.
-          -c CONFIG_FILE, --config-file CONFIG_FILE
-                                A file containing configuration information.
-          -l LOG_PREFIX, --log-prefix LOG_PREFIX
-                                Prefix for logging files
-          -ld, --log-debug      Provide detailed logging.
-          -hh, --hide-help      Do not show help on startup.
-          -r, --readonly        Do not allow changes or save annotations.
-          -o, --overwrite       If they exist already, read abd overwrite output
-                                files.
-          -ps, --prevent-self-links
-                                Prevent an item from being linked to itself.
-          -pf, --prevent-forward-links
-                                Prevent a link from an item to one after it.
-          --do-not-show-linked  Do not have a special color to indicate any linked
-                                token.
-          --alternate-comparisons
-                                Activate alternative way of showing different
-                                annotations (one colour per set of markings, rather
-                                than counts).
-        ```
-        
-        You may also define arguments in a file and pass them in as follows:
-        
-        ```bash
-        python slate.py @arguments.txt
-        ```
-        
-        ### Keybindings
-        
-        The tool shows files one at a time in plain text. Commands are:
-        
-        Type                        | Key                                                       | Labelling Affect                 | Linking Affect
-        --------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
-        Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
-        &nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
-        &nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
-        &nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
-        &nbsp;                      | <kbd>J</kbd> or [<kbd>Shift</kbd> + <kbd>&larr;</kbd>]        | go to the start of the line      | move linking item to the left
-        &nbsp;                      | <kbd>I</kbd> or [<kbd>Shift</kbd> + <kbd>&uarr;</kbd>]        | go to first line                 | move linking item up a line
-        &nbsp;                      | <kbd>O</kbd> or [<kbd>Shift</kbd> + <kbd>&darr;</kbd>]        | go to last line                  | move linking item down a line
-        &nbsp;                      | <kbd>:</kbd> or [<kbd>Shift</kbd> + <kbd>&rarr;</kbd>]        | go to the end of the line        | move linking item to the right
-        Edit Span                   | <kbd>m</kbd>                                              | extend left                      | extend selected item left
-        &nbsp;                      | <kbd>k</kbd>                                              | contract left side               | contract selected item left
-        &nbsp;                      | <kbd>/</kbd>                                              | extend right                     | extend selected item right
-        &nbsp;                      | <kbd>l</kbd>                                              | contract right side              | contract selected item right
-        &nbsp;                      | <kbd>M</kbd>                                              | -                                | extend linking item left
-        &nbsp;                      | <kbd>K</kbd>                                              | -                                | contract linking item left
-        &nbsp;                      | <kbd>?</kbd>                                              | -                                | extend linking item right
-        &nbsp;                      | <kbd>L</kbd>                                              | -                                | contract linking item right
-        Label Annotation (default)  | <kbd>Space</kbd> then <kbd>a</kbd>                        | [un]mark this item as a          | -
-        &nbsp;                      | <kbd>Space</kbd> then <kbd>s</kbd>                        | [un]mark this item as s          | -
-        &nbsp;                      | <kbd>Space</kbd> then <kbd>d</kbd>                        | [un]mark this item as d          | -
-        &nbsp;                      | <kbd>Space</kbd> then <kbd>v</kbd>                        | [un]mark this item as v          | -
-        Link Annotation             | <kbd>d</kbd>                                              | -                                | create a link and move right / down
-        &nbsp;                      | <kbd>D</kbd>                                              | -                                | create a link
-        Either Annotation mode      | <kbd>u</kbd>                                              | undo annotation on this item     | undo all annotations for the current item
-        
-        Shared commands:
-        
-        Type                        | Mode   | Key                                             | Affect               
-        --------------------------- | ------ | ----------------------------------------------- | ----------------------------
-        Searching                   | Normal | <kbd>\\</kbd>                                    | enter query editing mode
-        &nbsp;                      | Query  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit query editing mode
-        &nbsp;                      | Query  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in query
-        &nbsp;                      | Query  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to query
-        &nbsp;                      | Normal | <kbd>p</kbd>                                    | go to previous match
-        &nbsp;                      | Normal | <kbd>n</kbd>                                    | go to next match
-        &nbsp;                      | Normal | <kbd>P</kbd>                                    | go to previous match for linking line
-        &nbsp;                      | Normal | <kbd>N</kbd>                                    | go to next match for linking line
-        Assigning text labels       | Normal | <kbd>t</kbd>                                    | enter label editing mode
-        &nbsp;                      | Label  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit label editing mode and assign the label
-        &nbsp;                      | Label  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in label
-        &nbsp;                      | Label  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to label
-        Saving, exiting, etc        | Normal | <kbd>]</kbd>                                    | save and go to next file         
-        &nbsp;                      | Normal | <kbd>[</kbd>                                    | save and go to previous file     
-        &nbsp;                      | Normal | <kbd>q</kbd>                                    | save and quit                    
-        &nbsp;                      | Normal | <kbd>s</kbd>                                    | save                             
-        &nbsp;                      | Normal | <kbd>Q</kbd>                                    | quit                             
-        Misc                        | Normal | <kbd>#</kbd>                                    | toggle line numbers
-        &nbsp;                      | Normal | <kbd>h</kbd>                                    | toggle help info (default on)    
-        &nbsp;                      | Normal | <kbd>{</kbd> or <kbd>PAGE-UP</kbd>              | shift view up 5 lines
-        &nbsp;                      | Normal | <kbd>}</kbd> or <kbd>PAGE-DOWN</kbd>            | shift view down 5 lines
-        &nbsp;                      | Normal | <kbd>></kbd> then <kbd>p</kbd>                  | toggle showing progress through files
-        &nbsp;                      | Normal | <kbd>></kbd> then <kbd>l</kbd>                  | toggle showing legend for labels
-        &nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
-        
-        Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
-        
-        ### Misc
-        
-        To annotate multiple files, specify more than one as an argument.
-        For greater control, provide a list of files in a file specified with `--data-list`.
-        The list should be formatted as follows, where [] indicate optional values:
-        
-        ```
-        raw_file [annotation_file [starting_position [additional_annotation_files]]]
-        ```
-        
-        For example, these commands will create a file list, use it, then return to it later:
-        
-        ```bash
-        find . -name *txt > filenames_todo
-        ./slate.py -d filenames_todo -l do_later
-        # ... do some work, then quit, go away, come back...
-        ./slate.py -d do_later.todo -l do_even_later -o
-        ```
-        
-        Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
-        Otherwise the system will complain that you are overwriting existing annotation files.
-        
-        When the `additional_annotation_files` are included it activates an adjudication mode.
-        By default, all annotations that appear in all additional files are added to the current annotations.
-        Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
-        
-        Note - adjudication has not been as thoroughly tested.
-        Please share any issues you come across!
-        
-        ## Customisation
-        
-        Colours and keys are customisable. For labelling, the default is:
-        
-         - Underlined, current selected item
-         - Green on black, 'a' items
-         - Blue on black, 's' items
-         - Magenta on black, 'd' items
-         - Red on black, 'v' items
-         - Cyan on black, multiple types for a single token
-        
-        For linking, the default is:
-        
-         - Underlined, current selected item
-         - Green on black, current linking item
-         - Blue on black, item is linked to the current linking item
-         - Yellow on black, item is in some link, though not with the current linking item
-        
-        ### Modifying the Code
-        
-        Slate has a relatively small codebase (~2,200 lines) and is designed to make adding new functionality not too hard.
-        The code is divided up as follows:
-        
-         - `annotate.py`, the main program, this has the core loop that gets user input.
-         - `config.py`, contains the default configuration, including colours and keyboard bindings.
-         - `data.py`, classes to read, store and write data.
-         - `view.py`, rendering the screen.
-        
-        Logic for determining what colour goes where is split across two parts of the code.
-        In `data.py`, the set of labels for an item is determined.
-        In `view.py`, that set of labels is used to choose a suitable colour.
-        
-        Adding a new command involves:
-        
-         - Adding the name and key to `input_action_list` in `config.py`
-         - Adding a mapping from the name to a function in `action_to_function` in `annotate.py`
-         - Adding or modifying a function in `annotate.py`
-         - Modifying `data.py` or `view.py` to apply the action
-        
-        # Questions
-        
-        If you have a question please either:
-        
-        - Open an issue on [github](https://github.com/jkkummerfeld/slate/issues).
-        - Mail me at [jkummerf@umich.edu](mailto:jkummerf@umich.edu).
-        
-        # Contributions
-        
-        If you find a bug in the code, please submit an issue, or even better, a pull request with a fix.
-        
-        # Acknowledgments
-        
-        This tool is based in part upon work supported by IBM under contract 4915012629, and by ONR under MURI grant N000140911081.
-        Any opinions, findings, conclusions or recommendations expressed are those of the authors and do not necessarily reflect the views of IBM.
-        
-        
-Keywords: nlp annotation labeling natural-language-processing text-annotation
-Platform: UNKNOWN
+        Permission to use, copy, modify, and/or distribute this software for any
+        purpose with or without fee is hereby granted, provided that the above
+        copyright notice and this permission notice appear in all copies.
+        
+        THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+        REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+        FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+        INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+        LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+        OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+        PERFORMANCE OF THIS SOFTWARE.
+        
+Project-URL: Homepage, https://jkk.name/slate/
+Project-URL: Bug Tracker, https://github.com/jkkummerfeld/slate/issues
+Keywords: nlp,annotation,labeling,natural-language-processing,text-annotation
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*, <4
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,<4,>=2.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+This is a tool for labeling text documents.
+Slate supports annotation at different scales (spans of characters, tokens, and lines, or a document) and of different types (free text, labels, and links).
+This covers a range of tasks, such as Part-of-Speech tagging, Named Entity Recognition, Text Classification (including Sentiment Analysis), Discourse Structure, and more.
+
+Why use this tool over the range of other text annotation tools out there?
+
+- Fast
+- Trivial installation
+- Focuses all of the screen space on annotation (good for large fonts)
+- Terminal based, so it works in constrained environments (e.g. only allowed ssh access to a machine)
+- Not difficult to configure and modify
+
+Note - this repository is **not** for the "Segment and Link-based Annotation Tool, Enhanced", which can be found [here](https://bitbucket.org/dainkaplan/slate/wiki/Home) and was first presented at [LREC 2010](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf).
+See 'Citing' below for additional notes on that work.
+
+## Installation
+
+Two options:
+
+### 1. Install with pip
+```bash
+pip install slate-nlp
+```
+
+Then run from any directory in one of two ways:
+```
+slate
+python -m slate
+```
+
+### 2. Or download and run without installing
+Either download as a zip file:
+```bash
+curl https://codeload.github.com/jkkummerfeld/slate/zip/master -o "slate.zip"
+unzip slate.zip
+cd slate-master
+```
+Or clone the repository:
+```bash
+git clone https://github.com/jkkummerfeld/slate
+cd slate
+```
+
+Then run with either of:
+```
+python slate.py
+./slate.py
+```
+To run from another directory, use:
+```
+python PATH_TO_SLATE/slate.py
+PATH_TO_SLATE/slate.py
+```
+
+### Requirements
+
+The code requires only Python (2 or 3) and can be run out of the box.
+Your terminal must be at least 80 characters wide and 20 tall to use the tool.
+
+## Citing
+
+If you use this tool in your work, please cite:
+
+```
+@InProceedings{acl19slate,
+  title     = {SLATE: A Super-Lightweight Annotation Tool for Experts},
+  author    = {Jonathan K. Kummerfeld},
+  booktitle = {Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics: System Demonstrations},
+  location  = {Florence, Italy},
+  month     = {July},
+  year      = {2019},
+  pages     = {7--12},
+  doi       = {10.18653/v1/P19-3002},
+  url       = {https://aclweb.org/anthology/papers/P/P19/P19-3002/},
+  software  = {https://jkk.name/slate},
+}
+```
+
+While presenting this work at ACL I learned of another annotation tool called SLATE.
+That tool was first described in "Annotation Process Management Revisited", [Kaplan et al. (LREC 2010)](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf) and then in "Slate - A Tool for Creating and Maintaining Annotated Corpora", [Kaplan et al. (JLCL 2011)](https://jlcl.org/content/2-allissues/12-Heft2-2011/11.pdf).
+It takes a very different approach, using a web based interface that includes a suite of project management tools as well as annotation.
+The code it available at [https://bitbucket.org/dainkaplan/slate/wiki/Home](https://bitbucket.org/dainkaplan/slate/wiki/Home).
+
+## Getting Started
+
+Note: if you used pip to install, reaplce `python slate.py` with `slate` everywhere below.
+
+Run `python slate.py <filename>` to start annotating `<filename>` with labels over spans of tokens.
+The entire interface is contained in your terminal, there is no GUI.
+With command line arguments you can vary properties such as the type of annotation (labels or links) and scope of annotation (characters, tokens, lines, documents).
+
+The input file should be plain text, organised however you like.
+Prepare the data with your favourite sentence splitting and/or tokenisation software (e.g., [SpaCy](https://spacy.io)).
+If you use Python 3 then unicode should be supported, but the code has not been tested extensively with non-English text (please share any issues!).
+
+When you start the tool it displays a set of core commands by default.
+These are also specified below, along with additional commands.
+
+The tool saves annotations in a separate file (`<filename>.annotations` by default, this can be varied with a file list as described below).
+Annotation files are formatted with one line per annotated item.
+The item is specified with a tuple of numbers.
+For labels, the item is followed by a hyphen and the list of labels.
+For links, there are two items on the line before the hyphen.
+For example, these are two annotation files, one for labels of token spans and the other for links between lines:
+
+```
+==> label.annotations <==
+(2, 1) - label:a
+((3, 5), (3, 8)) - label:a
+(7, 8) - label:s label:a
+
+==> link.annotations <==
+13 0 - 
+13 7 - 
+16 7 - 
+```
+
+A few notes:
+- The second label annotation is on a span of tokens, going from 5 to 8 on line 3.
+- The third label annotation has two labels.
+- The line annotations only have one number to specify the item.
+- When the same line is linked to multiple other lines, each link is a separate item.
+
+### Tutorials
+
+Included in this repository are a set of interactive tutorials that teach you how to use the tool from within the tool itself.
+
+Task | Command
+---- | --------
+Named Entity Recognition annotation |  `python slate.py tutorial/ner.md -t categorical -s token -o -c ner-book.config -l log.tutorial.ner.txt -sl -sm`
+Labelling spans of text in a document | `python slate.py tutorial/label.md -t categorical -s token -o -l log.tutorial.label.txt`
+Linking lines in a document | `python slate.py tutorial/link.md -t link -s line -o -l log.tutorial.link.txt`
+
+### Example Workflow
+
+This tool has already been used for two annotation efforts involving multiple annotators ([Durrett et al., 2017](http://jkk.name/publication/emnlp17forums/) and [Kummerfeld et al., 2018](http://jkk.name/publication/arxiv18disentangle/)).
+Our workflow was as follows:
+
+- Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
+- Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
+- Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
+
+### Comparing Annotations
+
+To use adjudication mode, create a file, `example.txt`, similar to the following (you can have as many annotators as you like):
+
+```
+raw-text0 adjudicated-anno0 ((1000,),(1000,)) anno0.1 anno0.2 anno0.3
+raw-text1 adjudicated-anno1 ((1000,),(1000,)) anno1.1 anno1.2
+raw-text2 adjudicated-anno2 ((1000,),(1000,)) anno2.1 anno2.2 anno2.3 anno2.4
+```
+
+To save time, it is best to initialise `adjudicated-annoN` with the lines everyone agreed on:
+
+```
+for i in 0 1 2 ; do
+  count=`ls anno${i}.* | wc -l`
+  cat anno${i}.* | sort | uniq -c | awk -v count=$count '$1 == count' | sed 's/^ *[0-9]* *//' > matching
+done
+```
+
+Then run the tool as if you are annotating, for example for linking lines:
+
+```
+python ../learn-anno/slate/slate.py -d example.txt -pf -t link -s line -o -l log.adj.txt --do-not-show-linked
+```
+
+## Detailed Usage Instructions
+
+### Invocation options
+
+```
+usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
+                [-s {character,token,line,document}] [-c CONFIG_FILE] [-l LOG_PREFIX] [-ld]
+                [-sh] [-sl] [-sp] [-sm] [-r] [-o] [-ps] [-pf] [--do-not-show-linked]
+                [--alternate-comparisons]
+                [data ...]
+
+A tool for annotating text data.
+
+positional arguments:
+  data                  Files to be annotated
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -d DATA_LIST [DATA_LIST ...], --data-list DATA_LIST [DATA_LIST ...]
+                        Files containing lists of files to be annotated
+  -t {categorical,link}, --ann-type {categorical,link}
+                        The type of annotation being done.
+  -s {character,token,line,document}, --ann-scope {character,token,line,document}
+                        The scope of annotation being done.
+  -c CONFIG_FILE, --config-file CONFIG_FILE
+                        A file containing configuration information.
+  -l LOG_PREFIX, --log-prefix LOG_PREFIX
+                        Prefix for logging files
+  -ld, --log-debug      Provide detailed logging.
+  -sh, --show-help      Show help on startup.
+  -sl, --show-legend    Start with legend showing.
+  -sp, --show-progress  Start with progress showing.
+  -sm, --show-mark      Start with mark showing.
+  -r, --readonly        Do not allow changes or save annotations.
+  -o, --overwrite       If they exist already, read and overwrite output files.
+  -ps, --prevent-self-links
+                        Prevent an item from being linked to itself.
+  -pf, --prevent-forward-links
+                        Prevent a link from an item to one after it.
+  --do-not-show-linked  Do not have a special color to indicate any linked token.
+  --alternate-comparisons
+                        Activate alternative way of showing different annotations (one colour
+                        per set of markings, rather than counts).
+```
+
+You may also define arguments in a file and pass them in as follows:
+
+```bash
+python slate.py @arguments.txt
+```
+
+### Keybindings
+
+The tool shows files one at a time in plain text. Default commands are:
+
+Type                        | Key                                                       | Labelling Affect                 | Linking Affect
+--------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
+Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
+&nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
+&nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
+&nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
+&nbsp;                      | <kbd>J</kbd> or [<kbd>Shift</kbd> + <kbd>&larr;</kbd>]        | go to the start of the line      | move linking item to the left
+&nbsp;                      | <kbd>I</kbd> or [<kbd>Shift</kbd> + <kbd>&uarr;</kbd>]        | go to first line                 | move linking item up a line
+&nbsp;                      | <kbd>O</kbd> or [<kbd>Shift</kbd> + <kbd>&darr;</kbd>]        | go to last line                  | move linking item down a line
+&nbsp;                      | <kbd>:</kbd> or [<kbd>Shift</kbd> + <kbd>&rarr;</kbd>]        | go to the end of the line        | move linking item to the right
+Edit Span                   | <kbd>m</kbd>                                              | extend left                      | extend selected item left
+&nbsp;                      | <kbd>k</kbd>                                              | contract left side               | contract selected item left
+&nbsp;                      | <kbd>/</kbd>                                              | extend right                     | extend selected item right
+&nbsp;                      | <kbd>l</kbd>                                              | contract right side              | contract selected item right
+&nbsp;                      | <kbd>M</kbd>                                              | -                                | extend linking item left
+&nbsp;                      | <kbd>K</kbd>                                              | -                                | contract linking item left
+&nbsp;                      | <kbd>?</kbd>                                              | -                                | extend linking item right
+&nbsp;                      | <kbd>L</kbd>                                              | -                                | contract linking item right
+Label Annotation (default)  | <kbd>Space</kbd> then <kbd>a</kbd>                        | [un]mark this item as a          | -
+&nbsp;                      | <kbd>Space</kbd> then <kbd>s</kbd>                        | [un]mark this item as s          | -
+&nbsp;                      | <kbd>Space</kbd> then <kbd>d</kbd>                        | [un]mark this item as d          | -
+&nbsp;                      | <kbd>Space</kbd> then <kbd>v</kbd>                        | [un]mark this item as v          | -
+Link Annotation             | <kbd>d</kbd>                                              | -                                | create a link and move right / down
+&nbsp;                      | <kbd>D</kbd>                                              | -                                | create a link
+Either Annotation mode      | <kbd>u</kbd>                                              | undo annotation on this item     | undo all annotations for the current item
+
+Shared commands:
+
+Type                        | Mode   | Key                                             | Affect               
+--------------------------- | ------ | ----------------------------------------------- | ----------------------------
+Searching                   | Normal | <kbd>\\</kbd>                                    | enter query editing mode
+&nbsp;                      | Query  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit query editing mode
+&nbsp;                      | Query  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in query
+&nbsp;                      | Query  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to query
+&nbsp;                      | Normal | <kbd>p</kbd>                                    | go to previous match
+&nbsp;                      | Normal | <kbd>n</kbd>                                    | go to next match
+&nbsp;                      | Normal | <kbd>P</kbd>                                    | go to previous match for linking line
+&nbsp;                      | Normal | <kbd>N</kbd>                                    | go to next match for linking line
+Assigning text labels       | Normal | <kbd>t</kbd>                                    | enter label editing mode
+&nbsp;                      | Label  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit label editing mode and assign the label
+&nbsp;                      | Label  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in label
+&nbsp;                      | Label  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to label
+Saving, exiting, etc        | Normal | <kbd>]</kbd>                                    | save and go to next file         
+&nbsp;                      | Normal | <kbd>[</kbd>                                    | save and go to previous file     
+&nbsp;                      | Normal | <kbd>q</kbd>                                    | save and quit                    
+&nbsp;                      | Normal | <kbd>s</kbd>                                    | save                             
+&nbsp;                      | Normal | <kbd>Q</kbd>                                    | quit                             
+Misc                        | Normal | <kbd>#</kbd>                                    | toggle line numbers
+&nbsp;                      | Normal | <kbd>h</kbd>                                    | toggle help info (default on)    
+&nbsp;                      | Normal | <kbd>{</kbd> or <kbd>PAGE-UP</kbd>              | shift view up 5 lines
+&nbsp;                      | Normal | <kbd>}</kbd> or <kbd>PAGE-DOWN</kbd>            | shift view down 5 lines
+&nbsp;                      | Normal | <kbd>></kbd> then <kbd>p</kbd>                  | toggle showing progress through files
+&nbsp;                      | Normal | <kbd>></kbd> then <kbd>l</kbd>                  | toggle showing legend for labels
+&nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
+
+Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
+
+### Misc
+
+To annotate multiple files, specify more than one as an argument.
+For greater control, provide a list of files in a file specified with `--data-list` / `-d`.
+The list should be formatted as follows, where [] indicate optional values:
+
+```
+raw_file [annotation_file [starting_position [additional_annotation_files]]]
+```
+
+For example, these commands will create a file list, use it, then return to it later:
+
+```bash
+find . -name *txt > filenames_todo
+./slate.py -d filenames_todo -l do_later
+# ... do some work, then quit, go away, come back...
+./slate.py -d do_later.todo -l do_even_later -o
+```
+
+Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
+Otherwise the system will complain that you are overwriting existing annotation files.
+
+When the `additional_annotation_files` are included it activates an adjudication mode.
+By default, all annotations that appear in all additional files are added to the current annotations.
+Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
+
+## Customisation
+
+Colours and keys are customisable. For labelling, the default is:
+
+ - Underlined, current selected item
+ - Green on black, 'a' items
+ - Blue on black, 's' items
+ - Magenta on black, 'd' items
+ - Red on black, 'v' items
+ - Cyan on black, multiple types for a single token
+
+For linking, the default is:
+
+ - Underlined, current selected item
+ - Green on black, current linking item
+ - Blue on black, item is linked to the current linking item
+ - Yellow on black, item is in some link, though not with the current linking item
+
+### Modifying the Code
+
+Slate has a relatively small codebase (~2,200 lines) and is designed to make adding new functionality not too hard.
+The code is divided up as follows:
+
+ - `annotate.py`, the main program, this has the core loop that gets user input.
+ - `config.py`, contains the default configuration, including colours and keyboard bindings.
+ - `data.py`, classes to read, store and write data.
+ - `view.py`, rendering the screen.
+
+Logic for determining what colour goes where is split across two parts of the code.
+In `data.py`, the set of labels for an item is determined.
+In `view.py`, that set of labels is used to choose a suitable colour.
+
+Adding a new command involves:
+
+ - Adding the name and key to `input_action_list` in `config.py`
+ - Adding a mapping from the name to a function in `action_to_function` in `annotate.py`
+ - Adding or modifying a function in `annotate.py`
+ - Modifying `data.py` or `view.py` to apply the action
+
+#### Changing the label set / Adding labels
+
+The label set is defined in your config file (see an example config [here](https://github.com/jkkummerfeld/slate/blob/master/tutorial/config-example.txt)).
+
+See lines like this for label definitions:
+
+```
+Label:          a                         SPACE_a green
+```
+
+The format is:
+```
+Label:        <label>                    <command> <colour>
+```
+
+You can add / edit / remove these lines to define your own label scheme. For example, for NER you may want to do:
+
+```
+Label:          O                         SPACE_a green
+Label:          LOC                       SPACE_s blue
+Label:          PER                       SPACE_d red
+Label:          ORG                       SPACE_f yellow
+Label:          MISC                      SPACE_v magenta
+```
+
+The current set of available colours is: [green, blue, white, cyan, magenta, red, yellow].
+Note that by default white is used for regular text and cyan is used for cases where multiple labels apply to the same content.
+
+To define more colours, edit the top of `slate/config.py`.
+By varying both the text colour (foreground) and background colour you can achieve quite a range of variations.
+You can also define any RGB colour you want using the curses [init_color](https://docs.python.org/3/library/curses.html#curses.init_color) function and the [init_pair](https://docs.python.org/3/library/curses.html#curses.init_pair) function.
+
+# Questions
+
+If you have a question please either:
+
+- Open an issue on [github](https://github.com/jkkummerfeld/slate/issues).
+- Mail me at [jonathan.kummerfeld@sydney.edu.au](mailto:jonathan.kummerfeld@sydney.edu.au).
+
+# Contributions
+
+If you find a bug in the code, please submit an issue, or even better, a pull request with a fix.
+
+# Acknowledgments
+
+This tool is based in part upon work supported by IBM under contract 4915012629, and by ONR under MURI grant N000140911081.
+Any opinions, findings, conclusions or recommendations expressed are those of the authors and do not necessarily reflect the views of IBM.
+
```

### Comparing `slate-nlp-1.0.3/README.md` & `slate-nlp-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,20 +61,21 @@
 
 If you use this tool in your work, please cite:
 
 ```
 @InProceedings{acl19slate,
   title     = {SLATE: A Super-Lightweight Annotation Tool for Experts},
   author    = {Jonathan K. Kummerfeld},
-  booktitle = {Proceedings of {ACL} 2019, System Demonstrations},
+  booktitle = {Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics: System Demonstrations},
   location  = {Florence, Italy},
   month     = {July},
   year      = {2019},
-  pages     = {},
-  url       = {https://github.com/jkkummerfeld/slate/raw/master/paper/acl19slate.pdf},
+  pages     = {7--12},
+  doi       = {10.18653/v1/P19-3002},
+  url       = {https://aclweb.org/anthology/papers/P/P19/P19-3002/},
   software  = {https://jkk.name/slate},
 }
 ```
 
 While presenting this work at ACL I learned of another annotation tool called SLATE.
 That tool was first described in "Annotation Process Management Revisited", [Kaplan et al. (LREC 2010)](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf) and then in "Slate - A Tool for Creating and Maintaining Annotated Corpora", [Kaplan et al. (JLCL 2011)](https://jlcl.org/content/2-allissues/12-Heft2-2011/11.pdf).
 It takes a very different approach, using a web based interface that includes a suite of project management tools as well as annotation.
@@ -122,37 +123,62 @@
 
 ### Tutorials
 
 Included in this repository are a set of interactive tutorials that teach you how to use the tool from within the tool itself.
 
 Task | Command
 ---- | --------
-Labelling spans of text in a document | `python slate.py tutorial/label.md -t categorical -s token -o -hh -l log.tutorial.label.txt`
-Linking lines in a document | `python slate.py tutorial/link.md -t link -s line -o -hh -l log.tutorial.link.txt`
-Comparing annotations | To be created
+Named Entity Recognition annotation |  `python slate.py tutorial/ner.md -t categorical -s token -o -c ner-book.config -l log.tutorial.ner.txt -sl -sm`
+Labelling spans of text in a document | `python slate.py tutorial/label.md -t categorical -s token -o -l log.tutorial.label.txt`
+Linking lines in a document | `python slate.py tutorial/link.md -t link -s line -o -l log.tutorial.link.txt`
 
 ### Example Workflow
 
 This tool has already been used for two annotation efforts involving multiple annotators ([Durrett et al., 2017](http://jkk.name/publication/emnlp17forums/) and [Kummerfeld et al., 2018](http://jkk.name/publication/arxiv18disentangle/)).
 Our workflow was as follows:
 
 - Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
 - Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
 - Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
 
+### Comparing Annotations
+
+To use adjudication mode, create a file, `example.txt`, similar to the following (you can have as many annotators as you like):
+
+```
+raw-text0 adjudicated-anno0 ((1000,),(1000,)) anno0.1 anno0.2 anno0.3
+raw-text1 adjudicated-anno1 ((1000,),(1000,)) anno1.1 anno1.2
+raw-text2 adjudicated-anno2 ((1000,),(1000,)) anno2.1 anno2.2 anno2.3 anno2.4
+```
+
+To save time, it is best to initialise `adjudicated-annoN` with the lines everyone agreed on:
+
+```
+for i in 0 1 2 ; do
+  count=`ls anno${i}.* | wc -l`
+  cat anno${i}.* | sort | uniq -c | awk -v count=$count '$1 == count' | sed 's/^ *[0-9]* *//' > matching
+done
+```
+
+Then run the tool as if you are annotating, for example for linking lines:
+
+```
+python ../learn-anno/slate/slate.py -d example.txt -pf -t link -s line -o -l log.adj.txt --do-not-show-linked
+```
+
 ## Detailed Usage Instructions
 
 ### Invocation options
 
 ```
 usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
-                [-s {character,token,line,document}] [-c CONFIG_FILE]
-                [-l LOG_PREFIX] [-ld] [-hh] [-r] [-o] [-ps] [-pf]
-                [--do-not-show-linked] [--alternate-comparisons]
-                [data [data ...]]
+                [-s {character,token,line,document}] [-c CONFIG_FILE] [-l LOG_PREFIX] [-ld]
+                [-sh] [-sl] [-sp] [-sm] [-r] [-o] [-ps] [-pf] [--do-not-show-linked]
+                [--alternate-comparisons]
+                [data ...]
 
 A tool for annotating text data.
 
 positional arguments:
   data                  Files to be annotated
 
 optional arguments:
@@ -164,39 +190,39 @@
   -s {character,token,line,document}, --ann-scope {character,token,line,document}
                         The scope of annotation being done.
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         A file containing configuration information.
   -l LOG_PREFIX, --log-prefix LOG_PREFIX
                         Prefix for logging files
   -ld, --log-debug      Provide detailed logging.
-  -hh, --hide-help      Do not show help on startup.
+  -sh, --show-help      Show help on startup.
+  -sl, --show-legend    Start with legend showing.
+  -sp, --show-progress  Start with progress showing.
+  -sm, --show-mark      Start with mark showing.
   -r, --readonly        Do not allow changes or save annotations.
-  -o, --overwrite       If they exist already, read abd overwrite output
-                        files.
+  -o, --overwrite       If they exist already, read and overwrite output files.
   -ps, --prevent-self-links
                         Prevent an item from being linked to itself.
   -pf, --prevent-forward-links
                         Prevent a link from an item to one after it.
-  --do-not-show-linked  Do not have a special color to indicate any linked
-                        token.
+  --do-not-show-linked  Do not have a special color to indicate any linked token.
   --alternate-comparisons
-                        Activate alternative way of showing different
-                        annotations (one colour per set of markings, rather
-                        than counts).
+                        Activate alternative way of showing different annotations (one colour
+                        per set of markings, rather than counts).
 ```
 
 You may also define arguments in a file and pass them in as follows:
 
 ```bash
 python slate.py @arguments.txt
 ```
 
 ### Keybindings
 
-The tool shows files one at a time in plain text. Commands are:
+The tool shows files one at a time in plain text. Default commands are:
 
 Type                        | Key                                                       | Labelling Affect                 | Linking Affect
 --------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
 Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
 &nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
 &nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
 &nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
@@ -250,15 +276,15 @@
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
 
 Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
 
 ### Misc
 
 To annotate multiple files, specify more than one as an argument.
-For greater control, provide a list of files in a file specified with `--data-list`.
+For greater control, provide a list of files in a file specified with `--data-list` / `-d`.
 The list should be formatted as follows, where [] indicate optional values:
 
 ```
 raw_file [annotation_file [starting_position [additional_annotation_files]]]
 ```
 
 For example, these commands will create a file list, use it, then return to it later:
@@ -273,17 +299,14 @@
 Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
 Otherwise the system will complain that you are overwriting existing annotation files.
 
 When the `additional_annotation_files` are included it activates an adjudication mode.
 By default, all annotations that appear in all additional files are added to the current annotations.
 Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
 
-Note - adjudication has not been as thoroughly tested.
-Please share any issues you come across!
-
 ## Customisation
 
 Colours and keys are customisable. For labelling, the default is:
 
  - Underlined, current selected item
  - Green on black, 'a' items
  - Blue on black, 's' items
@@ -315,20 +338,52 @@
 Adding a new command involves:
 
  - Adding the name and key to `input_action_list` in `config.py`
  - Adding a mapping from the name to a function in `action_to_function` in `annotate.py`
  - Adding or modifying a function in `annotate.py`
  - Modifying `data.py` or `view.py` to apply the action
 
+#### Changing the label set / Adding labels
+
+The label set is defined in your config file (see an example config [here](https://github.com/jkkummerfeld/slate/blob/master/tutorial/config-example.txt)).
+
+See lines like this for label definitions:
+
+```
+Label:          a                         SPACE_a green
+```
+
+The format is:
+```
+Label:        <label>                    <command> <colour>
+```
+
+You can add / edit / remove these lines to define your own label scheme. For example, for NER you may want to do:
+
+```
+Label:          O                         SPACE_a green
+Label:          LOC                       SPACE_s blue
+Label:          PER                       SPACE_d red
+Label:          ORG                       SPACE_f yellow
+Label:          MISC                      SPACE_v magenta
+```
+
+The current set of available colours is: [green, blue, white, cyan, magenta, red, yellow].
+Note that by default white is used for regular text and cyan is used for cases where multiple labels apply to the same content.
+
+To define more colours, edit the top of `slate/config.py`.
+By varying both the text colour (foreground) and background colour you can achieve quite a range of variations.
+You can also define any RGB colour you want using the curses [init_color](https://docs.python.org/3/library/curses.html#curses.init_color) function and the [init_pair](https://docs.python.org/3/library/curses.html#curses.init_pair) function.
+
 # Questions
 
 If you have a question please either:
 
 - Open an issue on [github](https://github.com/jkkummerfeld/slate/issues).
-- Mail me at [jkummerf@umich.edu](mailto:jkummerf@umich.edu).
+- Mail me at [jonathan.kummerfeld@sydney.edu.au](mailto:jonathan.kummerfeld@sydney.edu.au).
 
 # Contributions
 
 If you find a bug in the code, please submit an issue, or even better, a pull request with a fix.
 
 # Acknowledgments
```

### Comparing `slate-nlp-1.0.3/slate/annotate.py` & `slate-nlp-1.1.1/slate/annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,16 +331,22 @@
         # No blinking cursor
         curses.curs_set(0)
 
         self.cfilename = 0
         self.filename, start_pos, output_file, annotation_files = self.filenames[self.cfilename]
         self.datum = Datum(self.filename, self.config, output_file, annotation_files)
         self.get_view(self.config, self.cfilename, len(self.filenames), start_pos)
-        if not self.args.hide_help:
+        if self.args.show_help:
             self.view.toggle_help()
+        if self.args.show_progress:
+            self.view.toggle_progress()
+        if self.args.show_legend:
+            self.view.toggle_legend()
+        if self.args.show_mark:
+            self.view.toggle_current_mark()
 
         last_num = None
         at_end = None
         nsteps = 0
         user_input = []
         while True:
             # Draw screen
@@ -434,40 +440,45 @@
     parser.add_argument('-l', '--log-prefix',
             default="annotation_log."+ stime,
             help='Prefix for logging files')
     parser.add_argument('-ld', '--log-debug',
             action='store_true',
             help='Provide detailed logging.')
 
-    parser.add_argument('-hh', '--hide-help',
+    parser.add_argument('-sh', '--show-help',
             action='store_true',
-            help='Do not show help on startup.')
+            help='Show help on startup.')
+    parser.add_argument('-sl', '--show-legend',
+            action='store_true',
+            help='Start with legend showing.')
+    parser.add_argument('-sp', '--show-progress',
+            action='store_true',
+            help='Start with progress showing.')
+    parser.add_argument('-sm', '--show-mark',
+            action='store_true',
+            help='Start with mark showing.')
+
     parser.add_argument('-r', '--readonly',
             action='store_true',
             help='Do not allow changes or save annotations.')
     parser.add_argument('-o', '--overwrite',
-            default=False,
             action='store_true',
-            help='If they exist already, read abd overwrite output files.')
+            help='If they exist already, read and overwrite output files.')
 
     parser.add_argument('-ps', '--prevent-self-links',
-            default=False,
             action='store_true',
             help='Prevent an item from being linked to itself.')
     parser.add_argument('-pf', '--prevent-forward-links',
-            default=False,
             action='store_true',
             help='Prevent a link from an item to one after it.')
 
     parser.add_argument('--do-not-show-linked',
-            default=False,
             action='store_true',
             help='Do not have a special color to indicate any linked token.')
     parser.add_argument('--alternate-comparisons',
-            default=False,
             action='store_true',
             help='Activate alternative way of showing different annotations '
             '(one colour per set of markings, rather than counts).')
 
     args = parser.parse_args()
 
     if len(args.data) == 0 and args.data_list is None:
```

### Comparing `slate-nlp-1.0.3/slate/config.py` & `slate-nlp-1.1.1/slate/config.py`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.0.3/slate/data.py` & `slate-nlp-1.1.1/slate/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -793,14 +793,42 @@
         if best is None and cycle:
             if direction == 'next':
                 best = first
             else:
                 best = last
         return best
 
+    def get_overlapping_spans(self, cursor):
+        ans = []
+
+        # Set colors for cursor and linking pos
+        for item in self.annotations:
+            matched = False
+            cpos = cursor.start
+            while True:
+                for span in item.spans:
+                    pos = span.start
+                    while True:
+                        if pos == cpos:
+                            matched = True
+                            break
+                        if pos == span.end:
+                            break
+                        pos = self.doc.get_next_pos(pos)
+                    if matched:
+                        break
+                if matched:
+                    break
+                if cpos == cursor.end:
+                    break
+                cpos = self.doc.get_next_pos(cpos)
+            if matched:
+                ans.append(item)
+        return ans
+
     def get_all_markings(self, cursor, linking_pos):
         ans = {}
 
         # Set colors for cursor and linking pos
         pos = cursor.start
         while True:
             ans.setdefault(pos, []).append('cursor')
```

### Comparing `slate-nlp-1.0.3/slate/view.py` & `slate-nlp-1.1.1/slate/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import print_function
 
 import _curses
 import logging
 import curses
 import re
 import sys
+import textwrap
 
 from .config import *
 from .data import Span, span_compare_ge, span_compare_le
 
 class View(object):
     def __init__(self, window, cursor, linking_pos, datum, my_config, cnum, total_num, prev_view=None):
         self.config = my_config
@@ -39,14 +40,15 @@
                 self.legend.append(("{} {}".format(label, "+".join(info[0])), label))
 
         if self.config.args.prevent_self_links and self.cursor == self.linking_pos:
             # TODO: In this case move the linking pos along one step
             pass
 
     def instructions(self):
+        # TODO: Have this based on the config file
         shared = [
             "Misc      | ] [                   | save and go to next ] / previous [ file",
             "          | q Q                   | quit with or without saving            ",
             "          | s                     | save the current file                  ",
         ]
         if self.config.annotation_type == 'link':
             return [
@@ -267,15 +269,16 @@
             if first_span is None:
                 first_span = Span('character', self.datum.doc, (line_no, 0, 0))
 
             # Set
             row += 1
             column = number_width
             if (not trial) and column > 0:
-                self.window.addstr(row, 0, str(line_no), curses.color_pair(LINE_NUMBER_COLOR))
+                if row < height:
+                    self.window.addstr(row, 0, str(line_no), curses.color_pair(LINE_NUMBER_COLOR))
             for token_no, token in enumerate(line):
                 # Check if we are going on to the next line and adjust
                 # accordingly.
                 space_before = 1 if column > number_width else 0
                 wide_token = False
                 if column + len(token) + space_before > width:
                     if token_no != 0:
@@ -381,26 +384,19 @@
         if len(current_search) > 0: extra_text_lines.append(current_search)
         if len(current_typing) > 0: extra_text_lines.append(current_typing)
 
         # Get colors for content
         markings = self.datum.get_all_markings(self.cursor, self.linking_pos)
 ###        logging.debug("markings: {}".format(markings))
         if self.show_current_mark:
-            for key in markings:
-                logging.debug("marking: {}: {}".format(key, markings[key]))
-                marks = markings[key]
-                if 'cursor' in marks:
-                    for mark in marks:
-                        if mark in self.config.labels:
-                            extra_text_lines.append("Current: "+ mark)
-                        elif 'compare-' in mark and 'ref' not in mark:
-                            parts = mark.split("-")
-                            count = len(self.datum.other_annotations) - int(parts[-2])
-                            label = parts[-1]
-                            extra_text_lines.append("{} marked as {}".format(count, label))
+            matched = self.datum.get_overlapping_spans(self.cursor)
+            matched = ["Current:"] + [str(v) for v in matched]
+            matched = textwrap.wrap(' '.join(matched), width - 1)
+            for line in matched:
+                extra_text_lines.append(line)
 
         # First, plan instructions
         main_height = height
         space_needed = len(extra_text_lines)
         if space_needed > 0:
             space_needed += 1
         elif len(self.datum.other_annotations) > 0:
@@ -422,15 +418,15 @@
         number_width = 0
         if self.line_numbers:
             count = 1
             lines = len(self.datum.doc.lines)
             while lines > 1:
                 count += 1
                 lines /= 10
-            number_width = count
+            number_width = count + 1
             main_width -= number_width
 
         # Do dry runs, shifting top down until the position is visible
         while not self.do_contents(main_height, main_width, markings, number_width, True):
             self.top += 1
 
         # Next, draw contents
```

### Comparing `slate-nlp-1.0.3/slate_nlp.egg-info/PKG-INFO` & `slate-nlp-1.1.1/slate_nlp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,357 +1,425 @@
 Metadata-Version: 2.1
 Name: slate-nlp
-Version: 1.0.3
+Version: 1.1.1
 Summary: A terminal-based text annotation tool
-Home-page: https://jkk.name/slate/
-Author: Jonathan K. Kummerfeld
-Author-email: jkk@berkeley.edu
-License: UNKNOWN
-Description: This is a tool for labeling text documents.
-        Slate supports annotation at different scales (spans of characters, tokens, and lines, or a document) and of different types (free text, labels, and links).
-        This covers a range of tasks, such as Part-of-Speech tagging, Named Entity Recognition, Text Classification (including Sentiment Analysis), Discourse Structure, and more.
+Author-email: "Jonathan K. Kummerfeld" <jonathan.kummerfeld@sydney.edu.au>
+License: Copyright (c) 2016-2023 Jonathan K Kummerfeld <jonathan.kummerfeld@sydney.edu.au>
         
-        Why use this tool over the range of other text annotation tools out there?
-        
-        - Fast
-        - Trivial installation
-        - Focuses all of the screen space on annotation (good for large fonts)
-        - Terminal based, so it works in constrained environments (e.g. only allowed ssh access to a machine)
-        - Not difficult to configure and modify
-        
-        Note - this repository is **not** for the "Segment and Link-based Annotation Tool, Enhanced", which can be found [here](https://bitbucket.org/dainkaplan/slate/wiki/Home) and was first presented at [LREC 2010](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf).
-        See 'Citing' below for additional notes on that work.
-        
-        ## Installation
-        
-        Two options:
-        
-        ### 1. Install with pip
-        ```bash
-        pip install slate-nlp
-        ```
-        
-        Then run from any directory in one of two ways:
-        ```
-        slate
-        python -m slate
-        ```
-        
-        ### 2. Or download and run without installing
-        Either download as a zip file:
-        ```bash
-        curl https://codeload.github.com/jkkummerfeld/slate/zip/master -o "slate.zip"
-        unzip slate.zip
-        cd slate-master
-        ```
-        Or clone the repository:
-        ```bash
-        git clone https://github.com/jkkummerfeld/slate
-        cd slate
-        ```
-        
-        Then run with either of:
-        ```
-        python slate.py
-        ./slate.py
-        ```
-        To run from another directory, use:
-        ```
-        python PATH_TO_SLATE/slate.py
-        PATH_TO_SLATE/slate.py
-        ```
-        
-        ### Requirements
-        
-        The code requires only Python (2 or 3) and can be run out of the box.
-        Your terminal must be at least 80 characters wide and 20 tall to use the tool.
-        
-        ## Citing
-        
-        If you use this tool in your work, please cite:
-        
-        ```
-        @InProceedings{acl19slate,
-          title     = {SLATE: A Super-Lightweight Annotation Tool for Experts},
-          author    = {Jonathan K. Kummerfeld},
-          booktitle = {Proceedings of {ACL} 2019, System Demonstrations},
-          location  = {Florence, Italy},
-          month     = {July},
-          year      = {2019},
-          pages     = {},
-          url       = {https://github.com/jkkummerfeld/slate/raw/master/paper/acl19slate.pdf},
-          software  = {https://jkk.name/slate},
-        }
-        ```
-        
-        While presenting this work at ACL I learned of another annotation tool called SLATE.
-        That tool was first described in "Annotation Process Management Revisited", [Kaplan et al. (LREC 2010)](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf) and then in "Slate - A Tool for Creating and Maintaining Annotated Corpora", [Kaplan et al. (JLCL 2011)](https://jlcl.org/content/2-allissues/12-Heft2-2011/11.pdf).
-        It takes a very different approach, using a web based interface that includes a suite of project management tools as well as annotation.
-        The code it available at [https://bitbucket.org/dainkaplan/slate/wiki/Home](https://bitbucket.org/dainkaplan/slate/wiki/Home).
-        
-        ## Getting Started
-        
-        Note: if you used pip to install, reaplce `python slate.py` with `slate` everywhere below.
-        
-        Run `python slate.py <filename>` to start annotating `<filename>` with labels over spans of tokens.
-        The entire interface is contained in your terminal, there is no GUI.
-        With command line arguments you can vary properties such as the type of annotation (labels or links) and scope of annotation (characters, tokens, lines, documents).
-        
-        The input file should be plain text, organised however you like.
-        Prepare the data with your favourite sentence splitting and/or tokenisation software (e.g., [SpaCy](https://spacy.io)).
-        If you use Python 3 then unicode should be supported, but the code has not been tested extensively with non-English text (please share any issues!).
-        
-        When you start the tool it displays a set of core commands by default.
-        These are also specified below, along with additional commands.
-        
-        The tool saves annotations in a separate file (`<filename>.annotations` by default, this can be varied with a file list as described below).
-        Annotation files are formatted with one line per annotated item.
-        The item is specified with a tuple of numbers.
-        For labels, the item is followed by a hyphen and the list of labels.
-        For links, there are two items on the line before the hyphen.
-        For example, these are two annotation files, one for labels of token spans and the other for links between lines:
-        
-        ```
-        ==> label.annotations <==
-        (2, 1) - label:a
-        ((3, 5), (3, 8)) - label:a
-        (7, 8) - label:s label:a
-        
-        ==> link.annotations <==
-        13 0 - 
-        13 7 - 
-        16 7 - 
-        ```
-        
-        A few notes:
-        - The second label annotation is on a span of tokens, going from 5 to 8 on line 3.
-        - The third label annotation has two labels.
-        - The line annotations only have one number to specify the item.
-        - When the same line is linked to multiple other lines, each link is a separate item.
-        
-        ### Tutorials
-        
-        Included in this repository are a set of interactive tutorials that teach you how to use the tool from within the tool itself.
-        
-        Task | Command
-        ---- | --------
-        Labelling spans of text in a document | `python slate.py tutorial/label.md -t categorical -s token -o -hh -l log.tutorial.label.txt`
-        Linking lines in a document | `python slate.py tutorial/link.md -t link -s line -o -hh -l log.tutorial.link.txt`
-        Comparing annotations | To be created
-        
-        ### Example Workflow
-        
-        This tool has already been used for two annotation efforts involving multiple annotators ([Durrett et al., 2017](http://jkk.name/publication/emnlp17forums/) and [Kummerfeld et al., 2018](http://jkk.name/publication/arxiv18disentangle/)).
-        Our workflow was as follows:
-        
-        - Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
-        - Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
-        - Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
-        
-        ## Detailed Usage Instructions
-        
-        ### Invocation options
-        
-        ```
-        usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
-                        [-s {character,token,line,document}] [-c CONFIG_FILE]
-                        [-l LOG_PREFIX] [-ld] [-hh] [-r] [-o] [-ps] [-pf]
-                        [--do-not-show-linked] [--alternate-comparisons]
-                        [data [data ...]]
-        
-        A tool for annotating text data.
-        
-        positional arguments:
-          data                  Files to be annotated
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -d DATA_LIST [DATA_LIST ...], --data-list DATA_LIST [DATA_LIST ...]
-                                Files containing lists of files to be annotated
-          -t {categorical,link}, --ann-type {categorical,link}
-                                The type of annotation being done.
-          -s {character,token,line,document}, --ann-scope {character,token,line,document}
-                                The scope of annotation being done.
-          -c CONFIG_FILE, --config-file CONFIG_FILE
-                                A file containing configuration information.
-          -l LOG_PREFIX, --log-prefix LOG_PREFIX
-                                Prefix for logging files
-          -ld, --log-debug      Provide detailed logging.
-          -hh, --hide-help      Do not show help on startup.
-          -r, --readonly        Do not allow changes or save annotations.
-          -o, --overwrite       If they exist already, read abd overwrite output
-                                files.
-          -ps, --prevent-self-links
-                                Prevent an item from being linked to itself.
-          -pf, --prevent-forward-links
-                                Prevent a link from an item to one after it.
-          --do-not-show-linked  Do not have a special color to indicate any linked
-                                token.
-          --alternate-comparisons
-                                Activate alternative way of showing different
-                                annotations (one colour per set of markings, rather
-                                than counts).
-        ```
-        
-        You may also define arguments in a file and pass them in as follows:
-        
-        ```bash
-        python slate.py @arguments.txt
-        ```
-        
-        ### Keybindings
-        
-        The tool shows files one at a time in plain text. Commands are:
-        
-        Type                        | Key                                                       | Labelling Affect                 | Linking Affect
-        --------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
-        Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
-        &nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
-        &nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
-        &nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
-        &nbsp;                      | <kbd>J</kbd> or [<kbd>Shift</kbd> + <kbd>&larr;</kbd>]        | go to the start of the line      | move linking item to the left
-        &nbsp;                      | <kbd>I</kbd> or [<kbd>Shift</kbd> + <kbd>&uarr;</kbd>]        | go to first line                 | move linking item up a line
-        &nbsp;                      | <kbd>O</kbd> or [<kbd>Shift</kbd> + <kbd>&darr;</kbd>]        | go to last line                  | move linking item down a line
-        &nbsp;                      | <kbd>:</kbd> or [<kbd>Shift</kbd> + <kbd>&rarr;</kbd>]        | go to the end of the line        | move linking item to the right
-        Edit Span                   | <kbd>m</kbd>                                              | extend left                      | extend selected item left
-        &nbsp;                      | <kbd>k</kbd>                                              | contract left side               | contract selected item left
-        &nbsp;                      | <kbd>/</kbd>                                              | extend right                     | extend selected item right
-        &nbsp;                      | <kbd>l</kbd>                                              | contract right side              | contract selected item right
-        &nbsp;                      | <kbd>M</kbd>                                              | -                                | extend linking item left
-        &nbsp;                      | <kbd>K</kbd>                                              | -                                | contract linking item left
-        &nbsp;                      | <kbd>?</kbd>                                              | -                                | extend linking item right
-        &nbsp;                      | <kbd>L</kbd>                                              | -                                | contract linking item right
-        Label Annotation (default)  | <kbd>Space</kbd> then <kbd>a</kbd>                        | [un]mark this item as a          | -
-        &nbsp;                      | <kbd>Space</kbd> then <kbd>s</kbd>                        | [un]mark this item as s          | -
-        &nbsp;                      | <kbd>Space</kbd> then <kbd>d</kbd>                        | [un]mark this item as d          | -
-        &nbsp;                      | <kbd>Space</kbd> then <kbd>v</kbd>                        | [un]mark this item as v          | -
-        Link Annotation             | <kbd>d</kbd>                                              | -                                | create a link and move right / down
-        &nbsp;                      | <kbd>D</kbd>                                              | -                                | create a link
-        Either Annotation mode      | <kbd>u</kbd>                                              | undo annotation on this item     | undo all annotations for the current item
-        
-        Shared commands:
-        
-        Type                        | Mode   | Key                                             | Affect               
-        --------------------------- | ------ | ----------------------------------------------- | ----------------------------
-        Searching                   | Normal | <kbd>\\</kbd>                                    | enter query editing mode
-        &nbsp;                      | Query  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit query editing mode
-        &nbsp;                      | Query  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in query
-        &nbsp;                      | Query  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to query
-        &nbsp;                      | Normal | <kbd>p</kbd>                                    | go to previous match
-        &nbsp;                      | Normal | <kbd>n</kbd>                                    | go to next match
-        &nbsp;                      | Normal | <kbd>P</kbd>                                    | go to previous match for linking line
-        &nbsp;                      | Normal | <kbd>N</kbd>                                    | go to next match for linking line
-        Assigning text labels       | Normal | <kbd>t</kbd>                                    | enter label editing mode
-        &nbsp;                      | Label  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit label editing mode and assign the label
-        &nbsp;                      | Label  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in label
-        &nbsp;                      | Label  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to label
-        Saving, exiting, etc        | Normal | <kbd>]</kbd>                                    | save and go to next file         
-        &nbsp;                      | Normal | <kbd>[</kbd>                                    | save and go to previous file     
-        &nbsp;                      | Normal | <kbd>q</kbd>                                    | save and quit                    
-        &nbsp;                      | Normal | <kbd>s</kbd>                                    | save                             
-        &nbsp;                      | Normal | <kbd>Q</kbd>                                    | quit                             
-        Misc                        | Normal | <kbd>#</kbd>                                    | toggle line numbers
-        &nbsp;                      | Normal | <kbd>h</kbd>                                    | toggle help info (default on)    
-        &nbsp;                      | Normal | <kbd>{</kbd> or <kbd>PAGE-UP</kbd>              | shift view up 5 lines
-        &nbsp;                      | Normal | <kbd>}</kbd> or <kbd>PAGE-DOWN</kbd>            | shift view down 5 lines
-        &nbsp;                      | Normal | <kbd>></kbd> then <kbd>p</kbd>                  | toggle showing progress through files
-        &nbsp;                      | Normal | <kbd>></kbd> then <kbd>l</kbd>                  | toggle showing legend for labels
-        &nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
-        
-        Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
-        
-        ### Misc
-        
-        To annotate multiple files, specify more than one as an argument.
-        For greater control, provide a list of files in a file specified with `--data-list`.
-        The list should be formatted as follows, where [] indicate optional values:
-        
-        ```
-        raw_file [annotation_file [starting_position [additional_annotation_files]]]
-        ```
-        
-        For example, these commands will create a file list, use it, then return to it later:
-        
-        ```bash
-        find . -name *txt > filenames_todo
-        ./slate.py -d filenames_todo -l do_later
-        # ... do some work, then quit, go away, come back...
-        ./slate.py -d do_later.todo -l do_even_later -o
-        ```
-        
-        Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
-        Otherwise the system will complain that you are overwriting existing annotation files.
-        
-        When the `additional_annotation_files` are included it activates an adjudication mode.
-        By default, all annotations that appear in all additional files are added to the current annotations.
-        Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
-        
-        Note - adjudication has not been as thoroughly tested.
-        Please share any issues you come across!
-        
-        ## Customisation
-        
-        Colours and keys are customisable. For labelling, the default is:
-        
-         - Underlined, current selected item
-         - Green on black, 'a' items
-         - Blue on black, 's' items
-         - Magenta on black, 'd' items
-         - Red on black, 'v' items
-         - Cyan on black, multiple types for a single token
-        
-        For linking, the default is:
-        
-         - Underlined, current selected item
-         - Green on black, current linking item
-         - Blue on black, item is linked to the current linking item
-         - Yellow on black, item is in some link, though not with the current linking item
-        
-        ### Modifying the Code
-        
-        Slate has a relatively small codebase (~2,200 lines) and is designed to make adding new functionality not too hard.
-        The code is divided up as follows:
-        
-         - `annotate.py`, the main program, this has the core loop that gets user input.
-         - `config.py`, contains the default configuration, including colours and keyboard bindings.
-         - `data.py`, classes to read, store and write data.
-         - `view.py`, rendering the screen.
-        
-        Logic for determining what colour goes where is split across two parts of the code.
-        In `data.py`, the set of labels for an item is determined.
-        In `view.py`, that set of labels is used to choose a suitable colour.
-        
-        Adding a new command involves:
-        
-         - Adding the name and key to `input_action_list` in `config.py`
-         - Adding a mapping from the name to a function in `action_to_function` in `annotate.py`
-         - Adding or modifying a function in `annotate.py`
-         - Modifying `data.py` or `view.py` to apply the action
-        
-        # Questions
-        
-        If you have a question please either:
-        
-        - Open an issue on [github](https://github.com/jkkummerfeld/slate/issues).
-        - Mail me at [jkummerf@umich.edu](mailto:jkummerf@umich.edu).
-        
-        # Contributions
-        
-        If you find a bug in the code, please submit an issue, or even better, a pull request with a fix.
-        
-        # Acknowledgments
-        
-        This tool is based in part upon work supported by IBM under contract 4915012629, and by ONR under MURI grant N000140911081.
-        Any opinions, findings, conclusions or recommendations expressed are those of the authors and do not necessarily reflect the views of IBM.
-        
-        
-Keywords: nlp annotation labeling natural-language-processing text-annotation
-Platform: UNKNOWN
+        Permission to use, copy, modify, and/or distribute this software for any
+        purpose with or without fee is hereby granted, provided that the above
+        copyright notice and this permission notice appear in all copies.
+        
+        THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+        REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+        FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+        INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+        LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+        OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+        PERFORMANCE OF THIS SOFTWARE.
+        
+Project-URL: Homepage, https://jkk.name/slate/
+Project-URL: Bug Tracker, https://github.com/jkkummerfeld/slate/issues
+Keywords: nlp,annotation,labeling,natural-language-processing,text-annotation
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=2.6, !=3.0.*, !=3.1.*, !=3.2.*, <4
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,<4,>=2.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+This is a tool for labeling text documents.
+Slate supports annotation at different scales (spans of characters, tokens, and lines, or a document) and of different types (free text, labels, and links).
+This covers a range of tasks, such as Part-of-Speech tagging, Named Entity Recognition, Text Classification (including Sentiment Analysis), Discourse Structure, and more.
+
+Why use this tool over the range of other text annotation tools out there?
+
+- Fast
+- Trivial installation
+- Focuses all of the screen space on annotation (good for large fonts)
+- Terminal based, so it works in constrained environments (e.g. only allowed ssh access to a machine)
+- Not difficult to configure and modify
+
+Note - this repository is **not** for the "Segment and Link-based Annotation Tool, Enhanced", which can be found [here](https://bitbucket.org/dainkaplan/slate/wiki/Home) and was first presented at [LREC 2010](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf).
+See 'Citing' below for additional notes on that work.
+
+## Installation
+
+Two options:
+
+### 1. Install with pip
+```bash
+pip install slate-nlp
+```
+
+Then run from any directory in one of two ways:
+```
+slate
+python -m slate
+```
+
+### 2. Or download and run without installing
+Either download as a zip file:
+```bash
+curl https://codeload.github.com/jkkummerfeld/slate/zip/master -o "slate.zip"
+unzip slate.zip
+cd slate-master
+```
+Or clone the repository:
+```bash
+git clone https://github.com/jkkummerfeld/slate
+cd slate
+```
+
+Then run with either of:
+```
+python slate.py
+./slate.py
+```
+To run from another directory, use:
+```
+python PATH_TO_SLATE/slate.py
+PATH_TO_SLATE/slate.py
+```
+
+### Requirements
+
+The code requires only Python (2 or 3) and can be run out of the box.
+Your terminal must be at least 80 characters wide and 20 tall to use the tool.
+
+## Citing
+
+If you use this tool in your work, please cite:
+
+```
+@InProceedings{acl19slate,
+  title     = {SLATE: A Super-Lightweight Annotation Tool for Experts},
+  author    = {Jonathan K. Kummerfeld},
+  booktitle = {Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics: System Demonstrations},
+  location  = {Florence, Italy},
+  month     = {July},
+  year      = {2019},
+  pages     = {7--12},
+  doi       = {10.18653/v1/P19-3002},
+  url       = {https://aclweb.org/anthology/papers/P/P19/P19-3002/},
+  software  = {https://jkk.name/slate},
+}
+```
+
+While presenting this work at ACL I learned of another annotation tool called SLATE.
+That tool was first described in "Annotation Process Management Revisited", [Kaplan et al. (LREC 2010)](http://www.lrec-conf.org/proceedings/lrec2010/pdf/129_Paper.pdf) and then in "Slate - A Tool for Creating and Maintaining Annotated Corpora", [Kaplan et al. (JLCL 2011)](https://jlcl.org/content/2-allissues/12-Heft2-2011/11.pdf).
+It takes a very different approach, using a web based interface that includes a suite of project management tools as well as annotation.
+The code it available at [https://bitbucket.org/dainkaplan/slate/wiki/Home](https://bitbucket.org/dainkaplan/slate/wiki/Home).
+
+## Getting Started
+
+Note: if you used pip to install, reaplce `python slate.py` with `slate` everywhere below.
+
+Run `python slate.py <filename>` to start annotating `<filename>` with labels over spans of tokens.
+The entire interface is contained in your terminal, there is no GUI.
+With command line arguments you can vary properties such as the type of annotation (labels or links) and scope of annotation (characters, tokens, lines, documents).
+
+The input file should be plain text, organised however you like.
+Prepare the data with your favourite sentence splitting and/or tokenisation software (e.g., [SpaCy](https://spacy.io)).
+If you use Python 3 then unicode should be supported, but the code has not been tested extensively with non-English text (please share any issues!).
+
+When you start the tool it displays a set of core commands by default.
+These are also specified below, along with additional commands.
+
+The tool saves annotations in a separate file (`<filename>.annotations` by default, this can be varied with a file list as described below).
+Annotation files are formatted with one line per annotated item.
+The item is specified with a tuple of numbers.
+For labels, the item is followed by a hyphen and the list of labels.
+For links, there are two items on the line before the hyphen.
+For example, these are two annotation files, one for labels of token spans and the other for links between lines:
+
+```
+==> label.annotations <==
+(2, 1) - label:a
+((3, 5), (3, 8)) - label:a
+(7, 8) - label:s label:a
+
+==> link.annotations <==
+13 0 - 
+13 7 - 
+16 7 - 
+```
+
+A few notes:
+- The second label annotation is on a span of tokens, going from 5 to 8 on line 3.
+- The third label annotation has two labels.
+- The line annotations only have one number to specify the item.
+- When the same line is linked to multiple other lines, each link is a separate item.
+
+### Tutorials
+
+Included in this repository are a set of interactive tutorials that teach you how to use the tool from within the tool itself.
+
+Task | Command
+---- | --------
+Named Entity Recognition annotation |  `python slate.py tutorial/ner.md -t categorical -s token -o -c ner-book.config -l log.tutorial.ner.txt -sl -sm`
+Labelling spans of text in a document | `python slate.py tutorial/label.md -t categorical -s token -o -l log.tutorial.label.txt`
+Linking lines in a document | `python slate.py tutorial/link.md -t link -s line -o -l log.tutorial.link.txt`
+
+### Example Workflow
+
+This tool has already been used for two annotation efforts involving multiple annotators ([Durrett et al., 2017](http://jkk.name/publication/emnlp17forums/) and [Kummerfeld et al., 2018](http://jkk.name/publication/arxiv18disentangle/)).
+Our workflow was as follows:
+
+- Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
+- Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
+- Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
+
+### Comparing Annotations
+
+To use adjudication mode, create a file, `example.txt`, similar to the following (you can have as many annotators as you like):
+
+```
+raw-text0 adjudicated-anno0 ((1000,),(1000,)) anno0.1 anno0.2 anno0.3
+raw-text1 adjudicated-anno1 ((1000,),(1000,)) anno1.1 anno1.2
+raw-text2 adjudicated-anno2 ((1000,),(1000,)) anno2.1 anno2.2 anno2.3 anno2.4
+```
+
+To save time, it is best to initialise `adjudicated-annoN` with the lines everyone agreed on:
+
+```
+for i in 0 1 2 ; do
+  count=`ls anno${i}.* | wc -l`
+  cat anno${i}.* | sort | uniq -c | awk -v count=$count '$1 == count' | sed 's/^ *[0-9]* *//' > matching
+done
+```
+
+Then run the tool as if you are annotating, for example for linking lines:
+
+```
+python ../learn-anno/slate/slate.py -d example.txt -pf -t link -s line -o -l log.adj.txt --do-not-show-linked
+```
+
+## Detailed Usage Instructions
+
+### Invocation options
+
+```
+usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
+                [-s {character,token,line,document}] [-c CONFIG_FILE] [-l LOG_PREFIX] [-ld]
+                [-sh] [-sl] [-sp] [-sm] [-r] [-o] [-ps] [-pf] [--do-not-show-linked]
+                [--alternate-comparisons]
+                [data ...]
+
+A tool for annotating text data.
+
+positional arguments:
+  data                  Files to be annotated
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -d DATA_LIST [DATA_LIST ...], --data-list DATA_LIST [DATA_LIST ...]
+                        Files containing lists of files to be annotated
+  -t {categorical,link}, --ann-type {categorical,link}
+                        The type of annotation being done.
+  -s {character,token,line,document}, --ann-scope {character,token,line,document}
+                        The scope of annotation being done.
+  -c CONFIG_FILE, --config-file CONFIG_FILE
+                        A file containing configuration information.
+  -l LOG_PREFIX, --log-prefix LOG_PREFIX
+                        Prefix for logging files
+  -ld, --log-debug      Provide detailed logging.
+  -sh, --show-help      Show help on startup.
+  -sl, --show-legend    Start with legend showing.
+  -sp, --show-progress  Start with progress showing.
+  -sm, --show-mark      Start with mark showing.
+  -r, --readonly        Do not allow changes or save annotations.
+  -o, --overwrite       If they exist already, read and overwrite output files.
+  -ps, --prevent-self-links
+                        Prevent an item from being linked to itself.
+  -pf, --prevent-forward-links
+                        Prevent a link from an item to one after it.
+  --do-not-show-linked  Do not have a special color to indicate any linked token.
+  --alternate-comparisons
+                        Activate alternative way of showing different annotations (one colour
+                        per set of markings, rather than counts).
+```
+
+You may also define arguments in a file and pass them in as follows:
+
+```bash
+python slate.py @arguments.txt
+```
+
+### Keybindings
+
+The tool shows files one at a time in plain text. Default commands are:
+
+Type                        | Key                                                       | Labelling Affect                 | Linking Affect
+--------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
+Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
+&nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
+&nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
+&nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
+&nbsp;                      | <kbd>J</kbd> or [<kbd>Shift</kbd> + <kbd>&larr;</kbd>]        | go to the start of the line      | move linking item to the left
+&nbsp;                      | <kbd>I</kbd> or [<kbd>Shift</kbd> + <kbd>&uarr;</kbd>]        | go to first line                 | move linking item up a line
+&nbsp;                      | <kbd>O</kbd> or [<kbd>Shift</kbd> + <kbd>&darr;</kbd>]        | go to last line                  | move linking item down a line
+&nbsp;                      | <kbd>:</kbd> or [<kbd>Shift</kbd> + <kbd>&rarr;</kbd>]        | go to the end of the line        | move linking item to the right
+Edit Span                   | <kbd>m</kbd>                                              | extend left                      | extend selected item left
+&nbsp;                      | <kbd>k</kbd>                                              | contract left side               | contract selected item left
+&nbsp;                      | <kbd>/</kbd>                                              | extend right                     | extend selected item right
+&nbsp;                      | <kbd>l</kbd>                                              | contract right side              | contract selected item right
+&nbsp;                      | <kbd>M</kbd>                                              | -                                | extend linking item left
+&nbsp;                      | <kbd>K</kbd>                                              | -                                | contract linking item left
+&nbsp;                      | <kbd>?</kbd>                                              | -                                | extend linking item right
+&nbsp;                      | <kbd>L</kbd>                                              | -                                | contract linking item right
+Label Annotation (default)  | <kbd>Space</kbd> then <kbd>a</kbd>                        | [un]mark this item as a          | -
+&nbsp;                      | <kbd>Space</kbd> then <kbd>s</kbd>                        | [un]mark this item as s          | -
+&nbsp;                      | <kbd>Space</kbd> then <kbd>d</kbd>                        | [un]mark this item as d          | -
+&nbsp;                      | <kbd>Space</kbd> then <kbd>v</kbd>                        | [un]mark this item as v          | -
+Link Annotation             | <kbd>d</kbd>                                              | -                                | create a link and move right / down
+&nbsp;                      | <kbd>D</kbd>                                              | -                                | create a link
+Either Annotation mode      | <kbd>u</kbd>                                              | undo annotation on this item     | undo all annotations for the current item
+
+Shared commands:
+
+Type                        | Mode   | Key                                             | Affect               
+--------------------------- | ------ | ----------------------------------------------- | ----------------------------
+Searching                   | Normal | <kbd>\\</kbd>                                    | enter query editing mode
+&nbsp;                      | Query  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit query editing mode
+&nbsp;                      | Query  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in query
+&nbsp;                      | Query  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to query
+&nbsp;                      | Normal | <kbd>p</kbd>                                    | go to previous match
+&nbsp;                      | Normal | <kbd>n</kbd>                                    | go to next match
+&nbsp;                      | Normal | <kbd>P</kbd>                                    | go to previous match for linking line
+&nbsp;                      | Normal | <kbd>N</kbd>                                    | go to next match for linking line
+Assigning text labels       | Normal | <kbd>t</kbd>                                    | enter label editing mode
+&nbsp;                      | Label  | <kbd>?</kbd> or <kbd>Enter</kbd>                    | exit label editing mode and assign the label
+&nbsp;                      | Label  | <kbd>!</kbd> or <kbd>Backspace</kbd>                    | delete last character in label
+&nbsp;                      | Label  | characters except <kbd>?</kbd> and <kbd>!</kbd> | add character to label
+Saving, exiting, etc        | Normal | <kbd>]</kbd>                                    | save and go to next file         
+&nbsp;                      | Normal | <kbd>[</kbd>                                    | save and go to previous file     
+&nbsp;                      | Normal | <kbd>q</kbd>                                    | save and quit                    
+&nbsp;                      | Normal | <kbd>s</kbd>                                    | save                             
+&nbsp;                      | Normal | <kbd>Q</kbd>                                    | quit                             
+Misc                        | Normal | <kbd>#</kbd>                                    | toggle line numbers
+&nbsp;                      | Normal | <kbd>h</kbd>                                    | toggle help info (default on)    
+&nbsp;                      | Normal | <kbd>{</kbd> or <kbd>PAGE-UP</kbd>              | shift view up 5 lines
+&nbsp;                      | Normal | <kbd>}</kbd> or <kbd>PAGE-DOWN</kbd>            | shift view down 5 lines
+&nbsp;                      | Normal | <kbd>></kbd> then <kbd>p</kbd>                  | toggle showing progress through files
+&nbsp;                      | Normal | <kbd>></kbd> then <kbd>l</kbd>                  | toggle showing legend for labels
+&nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
+
+Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
+
+### Misc
+
+To annotate multiple files, specify more than one as an argument.
+For greater control, provide a list of files in a file specified with `--data-list` / `-d`.
+The list should be formatted as follows, where [] indicate optional values:
+
+```
+raw_file [annotation_file [starting_position [additional_annotation_files]]]
+```
+
+For example, these commands will create a file list, use it, then return to it later:
+
+```bash
+find . -name *txt > filenames_todo
+./slate.py -d filenames_todo -l do_later
+# ... do some work, then quit, go away, come back...
+./slate.py -d do_later.todo -l do_even_later -o
+```
+
+Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
+Otherwise the system will complain that you are overwriting existing annotation files.
+
+When the `additional_annotation_files` are included it activates an adjudication mode.
+By default, all annotations that appear in all additional files are added to the current annotations.
+Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
+
+## Customisation
+
+Colours and keys are customisable. For labelling, the default is:
+
+ - Underlined, current selected item
+ - Green on black, 'a' items
+ - Blue on black, 's' items
+ - Magenta on black, 'd' items
+ - Red on black, 'v' items
+ - Cyan on black, multiple types for a single token
+
+For linking, the default is:
+
+ - Underlined, current selected item
+ - Green on black, current linking item
+ - Blue on black, item is linked to the current linking item
+ - Yellow on black, item is in some link, though not with the current linking item
+
+### Modifying the Code
+
+Slate has a relatively small codebase (~2,200 lines) and is designed to make adding new functionality not too hard.
+The code is divided up as follows:
+
+ - `annotate.py`, the main program, this has the core loop that gets user input.
+ - `config.py`, contains the default configuration, including colours and keyboard bindings.
+ - `data.py`, classes to read, store and write data.
+ - `view.py`, rendering the screen.
+
+Logic for determining what colour goes where is split across two parts of the code.
+In `data.py`, the set of labels for an item is determined.
+In `view.py`, that set of labels is used to choose a suitable colour.
+
+Adding a new command involves:
+
+ - Adding the name and key to `input_action_list` in `config.py`
+ - Adding a mapping from the name to a function in `action_to_function` in `annotate.py`
+ - Adding or modifying a function in `annotate.py`
+ - Modifying `data.py` or `view.py` to apply the action
+
+#### Changing the label set / Adding labels
+
+The label set is defined in your config file (see an example config [here](https://github.com/jkkummerfeld/slate/blob/master/tutorial/config-example.txt)).
+
+See lines like this for label definitions:
+
+```
+Label:          a                         SPACE_a green
+```
+
+The format is:
+```
+Label:        <label>                    <command> <colour>
+```
+
+You can add / edit / remove these lines to define your own label scheme. For example, for NER you may want to do:
+
+```
+Label:          O                         SPACE_a green
+Label:          LOC                       SPACE_s blue
+Label:          PER                       SPACE_d red
+Label:          ORG                       SPACE_f yellow
+Label:          MISC                      SPACE_v magenta
+```
+
+The current set of available colours is: [green, blue, white, cyan, magenta, red, yellow].
+Note that by default white is used for regular text and cyan is used for cases where multiple labels apply to the same content.
+
+To define more colours, edit the top of `slate/config.py`.
+By varying both the text colour (foreground) and background colour you can achieve quite a range of variations.
+You can also define any RGB colour you want using the curses [init_color](https://docs.python.org/3/library/curses.html#curses.init_color) function and the [init_pair](https://docs.python.org/3/library/curses.html#curses.init_pair) function.
+
+# Questions
+
+If you have a question please either:
+
+- Open an issue on [github](https://github.com/jkkummerfeld/slate/issues).
+- Mail me at [jonathan.kummerfeld@sydney.edu.au](mailto:jonathan.kummerfeld@sydney.edu.au).
+
+# Contributions
+
+If you find a bug in the code, please submit an issue, or even better, a pull request with a fix.
+
+# Acknowledgments
+
+This tool is based in part upon work supported by IBM under contract 4915012629, and by ONR under MURI grant N000140911081.
+Any opinions, findings, conclusions or recommendations expressed are those of the authors and do not necessarily reflect the views of IBM.
+
```

