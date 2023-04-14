# Comparing `tmp/pythainlp-4.0.0.tar.gz` & `tmp/pythainlp-4.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythainlp-4.0.0.tar", last modified: Fri Apr 14 12:24:52 2023, max compression
+gzip compressed data, was "pythainlp-4.0.0b1.tar", last modified: Sat Apr  1 16:29:41 2023, max compression
```

## Comparing `pythainlp-4.0.0.tar` & `pythainlp-4.0.0b1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.206679 pythainlp-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-04-14 12:24:44.000000 pythainlp-4.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-14 12:24:44.000000 pythainlp-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-14 12:24:44.000000 pythainlp-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-04-14 12:24:52.206679 pythainlp-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-04-14 12:24:44.000000 pythainlp-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-04-14 12:24:44.000000 pythainlp-4.0.0/README_TH.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp/
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp/augment/
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp/augment/lm/
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/lm/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/lm/wangchanberta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp/augment/word2vec/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/word2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/word2vec/bpemb_wv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/word2vec/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/word2vec/ltw2v.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/word2vec/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/augment/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/benchmarks/word_tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/cli/soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/cli/tag.py
--rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/cli/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/oscar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/th_en_translit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/tnc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/ttc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/corpus/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/generate/
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/generate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/generate/thai2fit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/khavee/
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/khavee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19801 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/khavee/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/khavee/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/parse/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/parse/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/parse/esupar_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/parse/spacy_thai_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/parse/transformers_ud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/parse/ud_goeswith.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/soundex/
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/soundex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/soundex/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/soundex/lk82.py
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/soundex/metasound.py
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/soundex/prayut_and_somchaip.py
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/soundex/udom83.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/spell/
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/spell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/spell/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/spell/phunspell.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/spell/pn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/spell/symspellpy.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/spell/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.194679 pythainlp-4.0.0/pythainlp/summarize/
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/summarize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/summarize/freq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/summarize/keybert.py
--rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/summarize/mt5.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.198679 pythainlp-4.0.0/pythainlp/tag/
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/_tag_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/chunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/crfchunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/locations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/orchid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/pos_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/thai_nner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/thainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/unigram.py
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tag/wangchanberta_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.198679 pythainlp-4.0.0/pythainlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/attacut.py
--rw-r--r--   0 runner    (1001) docker     (122)    26351 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/crfcls.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/crfcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/deepcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/etcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/longest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/multi_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/nercut.py
--rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/newmm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/nlpo3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/oskut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/sefr_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/ssg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/tcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/tcc_p.py
--rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/thaisumcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tokenize/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.198679 pythainlp-4.0.0/pythainlp/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tools/misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/tools/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.198679 pythainlp-4.0.0/pythainlp/translate/
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3440 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/translate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/translate/en_th.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/translate/th_fr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/translate/zh_th.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.202679 pythainlp-4.0.0/pythainlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/ipa.py
--rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/iso_11940.py
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/royin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/spoonerism.py
--rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/thai2rom.py
--rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/thai2rom_onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/thaig2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/w2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     5847 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/transliterate/wunsen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.202679 pythainlp-4.0.0/pythainlp/ulmfit/
--rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/ulmfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/ulmfit/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/ulmfit/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/ulmfit/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.202679 pythainlp-4.0.0/pythainlp/util/
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/emojiconv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/keywords.py
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/numtoword.py
--rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/phoneme.py
--rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/strftime.py
--rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/syllable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/thai.py
--rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/util/wordtonum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.202679 pythainlp-4.0.0/pythainlp/wangchanberta/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/wangchanberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/wangchanberta/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.202679 pythainlp-4.0.0/pythainlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-04-14 12:24:44.000000 pythainlp-4.0.0/pythainlp/word_vector/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.190679 pythainlp-4.0.0/pythainlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-14 12:24:52.000000 pythainlp-4.0.0/pythainlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-14 12:24:52.206679 pythainlp-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-04-14 12:24:44.000000 pythainlp-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.206679 pythainlp-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:24:52.206679 pythainlp-4.0.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/data/eval-details-input.json
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/data/eval-input.yml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/data/input.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/data/sentences.yml
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_khavee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)    55078 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_transliterate.py
--rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_ulmfit.py
--rw-r--r--   0 runner    (1001) docker     (122)    36563 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_wangchanberta.py
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-04-14 12:24:44.000000 pythainlp-4.0.0/tests/test_word_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.040075 pythainlp-4.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-04-01 16:29:41.040075 pythainlp-4.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/README_TH.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.012075 pythainlp-4.0.0b1/pythainlp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.016075 pythainlp-4.0.0b1/pythainlp/augment/
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.016075 pythainlp-4.0.0b1/pythainlp/augment/lm/
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/lm/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/lm/wangchanberta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.016075 pythainlp-4.0.0b1/pythainlp/augment/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/word2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/word2vec/bpemb_wv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/word2vec/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/word2vec/ltw2v.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/word2vec/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/augment/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.016075 pythainlp-4.0.0b1/pythainlp/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/benchmarks/word_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.016075 pythainlp-4.0.0b1/pythainlp/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/cli/soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/cli/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/cli/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.020075 pythainlp-4.0.0b1/pythainlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/oscar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/th_en_translit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/tnc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/ttc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/corpus/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.020075 pythainlp-4.0.0b1/pythainlp/generate/
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/generate/thai2fit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.020075 pythainlp-4.0.0b1/pythainlp/khavee/
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/khavee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18722 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/khavee/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/khavee/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.020075 pythainlp-4.0.0b1/pythainlp/parse/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/parse/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/parse/esupar_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/parse/spacy_thai_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/parse/transformers_ud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/parse/ud_goeswith.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.020075 pythainlp-4.0.0b1/pythainlp/soundex/
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/soundex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/soundex/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/soundex/lk82.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/soundex/metasound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/soundex/prayut_and_somchaip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/soundex/udom83.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.020075 pythainlp-4.0.0b1/pythainlp/spell/
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/spell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/spell/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/spell/phunspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/spell/pn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/spell/symspellpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/spell/tltk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.024075 pythainlp-4.0.0b1/pythainlp/summarize/
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/summarize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/summarize/freq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/summarize/keybert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/summarize/mt5.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.024075 pythainlp-4.0.0b1/pythainlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/_tag_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/crfchunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/orchid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/pos_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/thai_nner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/thainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3822 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/unigram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tag/wangchanberta_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.028075 pythainlp-4.0.0b1/pythainlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/attacut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26351 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/crfcls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/crfcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/deepcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/etcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/longest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/multi_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/nercut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/newmm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/nlpo3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/oskut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/sefr_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/ssg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/tcc_p.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/thaisumcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1510 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tokenize/tltk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.028075 pythainlp-4.0.0b1/pythainlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tools/misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/tools/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.028075 pythainlp-4.0.0b1/pythainlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3440 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/translate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/translate/en_th.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/translate/th_fr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/translate/zh_th.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.032075 pythainlp-4.0.0b1/pythainlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/iso_11940.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/royin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/spoonerism.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/thai2rom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/thai2rom_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/thaig2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/w2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5847 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/transliterate/wunsen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.032075 pythainlp-4.0.0b1/pythainlp/ulmfit/
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/ulmfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/ulmfit/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/ulmfit/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/ulmfit/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.036075 pythainlp-4.0.0b1/pythainlp/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/emojiconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/numtoword.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/phoneme.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/syllable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/thai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/util/wordtonum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.036075 pythainlp-4.0.0b1/pythainlp/wangchanberta/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/wangchanberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/wangchanberta/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.036075 pythainlp-4.0.0b1/pythainlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/pythainlp/word_vector/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.016075 pythainlp-4.0.0b1/pythainlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-01 16:29:40.000000 pythainlp-4.0.0b1/pythainlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-01 16:29:41.040075 pythainlp-4.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.040075 pythainlp-4.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-01 16:29:41.040075 pythainlp-4.0.0b1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/data/eval-details-input.json
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/data/eval-input.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/data/input.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/data/sentences.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_khavee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55078 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_ulmfit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36563 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_wangchanberta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-04-01 16:29:30.000000 pythainlp-4.0.0b1/tests/test_word_vector.py
```

### Comparing `pythainlp-4.0.0/CONTRIBUTING.md` & `pythainlp-4.0.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/LICENSE` & `pythainlp-4.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/PKG-INFO` & `pythainlp-4.0.0b1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 4.0.0
+Version: 4.0.0b1
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
-Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
+Project-URL: Documentation, https://pythainlp.github.io/docs/3.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
 Project-URL: Source Code, https://github.com/PyThaiNLP/pythainlp
 Project-URL: Bug Tracker, https://github.com/PyThaiNLP/pythainlp/issues
 Description: 
         ![PyThaiNLP Logo](https://avatars0.githubusercontent.com/u/32934255?s=200&v=4)
         
         PyThaiNLP is a Python library for Thai natural language processing.
@@ -35,15 +35,15 @@
         ```
         
         Some functionalities, like named-entity recognition, required extra packages.
         See https://github.com/PyThaiNLP/pythainlp for installation options.
         
 Keywords: pythainlp,NLP,natural language processing,text analytics,text processing,localization,computational linguistics,ThaiNLP,Thai NLP,Thai language
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Thai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
@@ -63,14 +63,15 @@
 Provides-Extra: textaugment
 Provides-Extra: wangchanberta
 Provides-Extra: mt5
 Provides-Extra: wordnet
 Provides-Extra: generate
 Provides-Extra: sefr_cut
 Provides-Extra: spell
+Provides-Extra: tltk
 Provides-Extra: oskut
 Provides-Extra: nlpo3
 Provides-Extra: onnx
 Provides-Extra: thai_nner
 Provides-Extra: esupar
 Provides-Extra: spacy_thai
 Provides-Extra: transformers_ud
```

### Comparing `pythainlp-4.0.0/README.md` & `pythainlp-4.0.0b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 **News**
 
 > Now, You can contact or ask any questions with the PyThaiNLP team. <a href="https://matrix.to/#/#thainlp:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
 
 | Version | Description | Status |
 |:------:|:--:|:------:|
-| [4.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/714) |
-| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 4.1  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [3.1](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/643) |
+| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 4.0  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/714) |
 
 
 ## Getting Started
 
 - PyThaiNLP 2 requires Python 3.6+. Python 2.7 users can use PyThaiNLP 1.6. See [2.0 change log](https://github.com/PyThaiNLP/pythainlp/issues/118) | [Upgrading from 1.7](https://pythainlp.github.io/docs/2.0/notes/pythainlp-1_7-2_0.html) | [Upgrading ThaiNER from 1.7](https://github.com/PyThaiNLP/pythainlp/wiki/Upgrade-ThaiNER-from-PyThaiNLP-1.7-to-PyThaiNLP-2.0)
 - [PyThaiNLP Get Started notebook](https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html) | [API document](https://pythainlp.github.io/docs) | [Tutorials](https://pythainlp.github.io/tutorials)
 - [Official website](https://pythainlp.github.io/) | [PyPI](https://pypi.org/project/pythainlp/) | [Facebook page](https://www.facebook.com/pythainlp/)
```

#### html2text {}

```diff
@@ -7,18 +7,18 @@
 similar to [NLTK](https://www.nltk.org/) with focus on Thai language. PyThaiNLP
 à¹à¸à¹à¸à¹à¸¥à¸à¸²à¸£à¸µà¸ à¸²à¸©à¸²à¹à¸à¸à¸­à¸à¸ªà¸³à¸«à¸£à¸±à¸à¸à¸£à¸°à¸¡à¸§à¸¥à¸à¸¥à¸ à¸²à¸©à¸²à¸à¸£à¸£à¸¡à¸à¸²à¸à¸´
 à¸à¸¥à¹à¸²à¸¢à¸à¸±à¸ NLTK à¹à¸à¸¢à¹à¸à¹à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢
 [à¸à¸¹à¸£à¸²à¸¢à¸¥à¸°à¹à¸­à¸µà¸¢à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢à¹à¸à¹à¸à¸µà¹
 README_TH.MD](https://github.com/PyThaiNLP/pythainlp/blob/dev/README_TH.md)
 **News** > Now, You can contact or ask any questions with the PyThaiNLP team.
 [Chat_on_Matrix] | Version | Description | Status | |:------:|:--:|:------:| |
-[4.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log]
-(https://github.com/PyThaiNLP/pythainlp/issues/714) | | [`dev`](https://
-github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 4.1 | [Change
-Log](https://github.com/PyThaiNLP/pythainlp/issues/788) | ## Getting Started -
+[3.1](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log]
+(https://github.com/PyThaiNLP/pythainlp/issues/643) | | [`dev`](https://
+github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 4.0 | [Change
+Log](https://github.com/PyThaiNLP/pythainlp/issues/714) | ## Getting Started -
 PyThaiNLP 2 requires Python 3.6+. Python 2.7 users can use PyThaiNLP 1.6. See
 [2.0 change log](https://github.com/PyThaiNLP/pythainlp/issues/118) |
 [Upgrading from 1.7](https://pythainlp.github.io/docs/2.0/notes/pythainlp-1_7-
 2_0.html) | [Upgrading ThaiNER from 1.7](https://github.com/PyThaiNLP/
 pythainlp/wiki/Upgrade-ThaiNER-from-PyThaiNLP-1.7-to-PyThaiNLP-2.0) -
 [PyThaiNLP Get Started notebook](https://pythainlp.github.io/tutorials/
 notebooks/pythainlp_get_started.html) | [API document](https://
```

### Comparing `pythainlp-4.0.0/README_TH.md` & `pythainlp-4.0.0b1/README_TH.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 **ข่าวสาร**
 
 > คุณสามารถพูดคุยหรือแชทกับทีม PyThaiNLP หรือผู้สนับสนุนคนอื่น ๆ ได้ที่ <a href="https://matrix.to/#/#thainlp:matrix.org" rel="noopener" target="_blank"><img src="https://matrix.to/img/matrix-badge.svg" alt="Chat on Matrix"></a>
 
 | รุ่น | คำอธิบาย | สถานะ |
 |:------:|:--:|:------:|
-| [4.0](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/714) |
-| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 4.1  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/788) |
+| [3.1](https://github.com/PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/643) |
+| [`dev`](https://github.com/PyThaiNLP/pythainlp/tree/dev) | Release Candidate for 4.0  | [Change Log](https://github.com/PyThaiNLP/pythainlp/issues/714) |
 
 ติดตามพวกเราบน [PyThaiNLP Facebook page](https://www.facebook.com/pythainlp/) เพื่อรับข่าวสารเพิ่มเติม
 
 
 ## เริ่มต้นกับ PyThaiNLP
 
 พวกเราได้จัดทำ [PyThaiNLP Get Started Tutorial](https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html) สำหรับสำรวจความสามารถของ PyThaiNLP; พวกเรามีเอกสารสอนใช้งาน สามารถศึกษาได้ที่ [หน้า tutorial](https://pythainlp.github.io/tutorials).
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
            [Codacy_Badge] [FOSSA_Status] [Google_Colab_Badge] [DOI]
 PyThaiNLP
 à¹à¸à¹à¸à¹à¸¥à¸à¸²à¸£à¸µà¸ à¸²à¸©à¸²à¹à¸à¸à¸­à¸à¸ªà¸³à¸«à¸£à¸±à¸à¸à¸£à¸°à¸¡à¸§à¸¥à¸à¸¥à¸ à¸²à¸©à¸²à¸à¸£à¸£à¸¡à¸à¸²à¸à¸´
 à¹à¸à¸¢à¹à¸à¹à¸à¸ à¸²à¸©à¸²à¹à¸à¸¢ **à¸à¹à¸²à¸§à¸ªà¸²à¸£** >
 à¸à¸¸à¸à¸ªà¸²à¸¡à¸²à¸£à¸à¸à¸¹à¸à¸à¸¸à¸¢à¸«à¸£à¸·à¸­à¹à¸à¸à¸à¸±à¸à¸à¸µà¸¡
 PyThaiNLP à¸«à¸£à¸·à¸­à¸à¸¹à¹à¸ªà¸à¸±à¸à¸ªà¸à¸¸à¸à¸à¸à¸­à¸·à¹à¸ à¹
 à¹à¸à¹à¸à¸µà¹ [Chat_on_Matrix] | à¸£à¸¸à¹à¸ | à¸à¸³à¸­à¸à¸´à¸à¸²à¸¢ |
-à¸ªà¸à¸²à¸à¸° | |:------:|:--:|:------:| | [4.0](https://github.com/
+à¸ªà¸à¸²à¸à¸° | |:------:|:--:|:------:| | [3.1](https://github.com/
 PyThaiNLP/pythainlp/releases) | Stable | [Change Log](https://github.com/
-PyThaiNLP/pythainlp/issues/714) | | [`dev`](https://github.com/PyThaiNLP/
-pythainlp/tree/dev) | Release Candidate for 4.1 | [Change Log](https://
-github.com/PyThaiNLP/pythainlp/issues/788) |
+PyThaiNLP/pythainlp/issues/643) | | [`dev`](https://github.com/PyThaiNLP/
+pythainlp/tree/dev) | Release Candidate for 4.0 | [Change Log](https://
+github.com/PyThaiNLP/pythainlp/issues/714) |
 à¸à¸´à¸à¸à¸²à¸¡à¸à¸§à¸à¹à¸£à¸²à¸à¸ [PyThaiNLP Facebook page](https://
 www.facebook.com/pythainlp/
 ) à¹à¸à¸·à¹à¸­à¸£à¸±à¸à¸à¹à¸²à¸§à¸ªà¸²à¸£à¹à¸à¸´à¹à¸¡à¹à¸à¸´à¸¡ ##
 à¹à¸£à¸´à¹à¸¡à¸à¹à¸à¸à¸±à¸ PyThaiNLP
 à¸à¸§à¸à¹à¸£à¸²à¹à¸à¹à¸à¸±à¸à¸à¸³ [PyThaiNLP Get Started Tutorial]
 (https://pythainlp.github.io/tutorials/notebooks/pythainlp_get_started.html)
 à¸ªà¸³à¸«à¸£à¸±à¸à¸ªà¸³à¸£à¸§à¸à¸à¸§à¸²à¸¡à¸ªà¸²à¸¡à¸²à¸£à¸à¸à¸­à¸
```

### Comparing `pythainlp-4.0.0/pythainlp/__init__.py` & `pythainlp-4.0.0b1/pythainlp/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/__main__.py` & `pythainlp-4.0.0b1/pythainlp/__main__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/__init__.py` & `pythainlp-4.0.0b1/pythainlp/augment/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/lm/__init__.py` & `pythainlp-4.0.0b1/pythainlp/augment/lm/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/lm/fasttext.py` & `pythainlp-4.0.0b1/pythainlp/augment/lm/fasttext.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/lm/wangchanberta.py` & `pythainlp-4.0.0b1/pythainlp/augment/lm/wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/word2vec/__init__.py` & `pythainlp-4.0.0b1/pythainlp/augment/word2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/word2vec/bpemb_wv.py` & `pythainlp-4.0.0b1/pythainlp/augment/word2vec/bpemb_wv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/word2vec/core.py` & `pythainlp-4.0.0b1/pythainlp/augment/word2vec/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/word2vec/ltw2v.py` & `pythainlp-4.0.0b1/pythainlp/augment/word2vec/ltw2v.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/word2vec/thai2fit.py` & `pythainlp-4.0.0b1/pythainlp/augment/word2vec/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/augment/wordnet.py` & `pythainlp-4.0.0b1/pythainlp/augment/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/benchmarks/__init__.py` & `pythainlp-4.0.0b1/pythainlp/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/benchmarks/word_tokenization.py` & `pythainlp-4.0.0b1/pythainlp/benchmarks/word_tokenization.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/cli/__init__.py` & `pythainlp-4.0.0b1/pythainlp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/cli/benchmark.py` & `pythainlp-4.0.0b1/pythainlp/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/cli/data.py` & `pythainlp-4.0.0b1/pythainlp/cli/data.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/cli/soundex.py` & `pythainlp-4.0.0b1/pythainlp/cli/soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/cli/tag.py` & `pythainlp-4.0.0b1/pythainlp/cli/tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/cli/tokenize.py` & `pythainlp-4.0.0b1/pythainlp/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/__init__.py` & `pythainlp-4.0.0b1/pythainlp/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/common.py` & `pythainlp-4.0.0b1/pythainlp/corpus/common.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/conceptnet.py` & `pythainlp-4.0.0b1/pythainlp/corpus/conceptnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/core.py` & `pythainlp-4.0.0b1/pythainlp/corpus/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/oscar.py` & `pythainlp-4.0.0b1/pythainlp/corpus/oscar.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/th_en_translit.py` & `pythainlp-4.0.0b1/pythainlp/corpus/th_en_translit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/tnc.py` & `pythainlp-4.0.0b1/pythainlp/corpus/tnc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/ttc.py` & `pythainlp-4.0.0b1/pythainlp/corpus/ttc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/util.py` & `pythainlp-4.0.0b1/pythainlp/corpus/util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/corpus/wordnet.py` & `pythainlp-4.0.0b1/pythainlp/corpus/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/generate/__init__.py` & `pythainlp-4.0.0b1/pythainlp/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/generate/core.py` & `pythainlp-4.0.0b1/pythainlp/generate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/generate/thai2fit.py` & `pythainlp-4.0.0b1/pythainlp/generate/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/khavee/__init__.py` & `pythainlp-4.0.0b1/pythainlp/khavee/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/khavee/core.py` & `pythainlp-4.0.0b1/pythainlp/khavee/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Union
 from pythainlp.tokenize import subword_tokenize
-from pythainlp.util import sound_syllable
 
 
 class KhaveeVerifier:
     def __init__(self):
         """
         KhaveeVerifier: Thai Poetry verifier
         """
@@ -76,23 +75,21 @@
             elif i == 'อ':
                 countoa += 1
                 sara.append('ออ')
             elif i == 'ั' and 'ว' in word:
                 sara.append('อัว')
             elif i == 'ไ' or i == 'ใ':
                 sara.append('ไอ') 
-            elif i == '็':
-                sara.append('ออ')
             elif 'รร' in word:
                 if self.check_marttra(word) == 'กม':
                     sara.append('อำ')
                 else:
                     sara.append('อะ')
         # Incase ออ
-        if countoa == 1 and 'อ' in word[-1] and 'เ' not in word:
+        if countoa == 1 and 'อ' in word[-1]:
             sara.remove('ออ')
         # In case เอ เอ 
         countA = 0
         for i in sara:
             if i == 'เอ':
                 countA = countA + 1
             if countA > 1:
@@ -180,20 +177,15 @@
             if word[-1] != 'ร':
                 sara.append('โอะ')
             else:
                 sara.append('ออ') 
         elif sara == [] and len(word) == 3:
             sara.append('ออ') 
         
-        # incase บ่ 
-        if 'บ่' in word:
-            sara = []
-            sara.append('ออ')
-
-        if sara == []:  
+        if sara == []:
             return 'Cant find Sara in this word'
         else:
             return sara[0]
 
 
     def check_marttra(self, word: str) -> str:
         """
@@ -240,21 +232,17 @@
         elif word[-1] in ['จ','ช','ซ','ฎ','ฏ','ฐ','ฑ','ฒ','ด','ต','ถ','ท','ธ','ศ','ษ','ส'] :
             return 'กด'
         elif word[-1] in ['ญ',', ณ' ,'น' ,'ร' ,'ล' ,'ฬ']:
             return 'กน'
         elif word[-1] in ['บ', 'ป', 'พ', 'ฟ', 'ภ']:
             return 'กบ'
         else:
-           if '็' in word:
-               return 'กา'
-           else:
-               return 'Cant find Marttra in this word'
-           
+           return 'Cant find Marttra in this word'
 
-    def is_sumpus(self, word1: str,word2: str) -> bool:
+    def check_sumpus(self, word1: str,word2: str) -> bool:
         """
         Check the rhyme between two words.
 
         :param str word1: Thai word
         :param str word2: Thai word
         :return: boolen
         :rtype: bool
@@ -262,18 +250,18 @@
         :Example:
         ::
 
             from pythainlp.khavee import KhaveeVerifier
 
             kv = KhaveeVerifier()
 
-            print(kv.is_sumpus('สรร','อัน'))
+            print(kv.check_sumpus('สรร','อัน'))
             # output: True
 
-            print(kv.is_sumpus('สรร','แมว'))
+            print(kv.check_sumpus('สรร','แมว'))
             # output: False
         """
         marttra1 = self.check_marttra(word1)
         marttra2 = self.check_marttra(word2)
         sara1 = self.check_sara(word1)
         sara2 = self.check_sara(word2)
         if sara1 == 'อะ' and marttra1 == 'เกย':
@@ -288,21 +276,15 @@
         elif sara2 == 'อำ' and marttra2 == 'กม':
             sara2 = 'อำ'
             marttra2 = 'กา'
         if marttra1 == marttra2 and sara1 == sara2:
             return True
         else:
             return False
-        
-    def check_karu_lahu(self,text):
-        if (self.check_marttra(text) != 'กา' or (self.check_marttra(text) == 'กา' and self.check_sara(text) in ['อา','อี', 'อือ', 'อู', 'เอ', 'แอ', 'โอ', 'ออ', 'เออ', 'เอีย', 'เอือ' ,'อัว']) or self.check_sara(text) in ['อำ','ไอ','เอา']) and text not in ['บ่','ณ','ธ','ก็']:
-            return 'karu'
-        else:
-            return 'lahu'
-        
+
     def check_klon(self, text: str,k_type: int=8) -> Union[List[str], str]:
         """
         Check the suitability of the poem according to Thai principles.
 
         :param str text: Thai poem
         :param int k_type: Type of Thai poem
         :return: the check of the suitability of the poem according to Thai principles.
@@ -345,23 +327,23 @@
                         list_sumpus_sent4.append(sub_sent[-1])
                 if len(list_sumpus_sent1) != len(list_sumpus_sent2h) or len(list_sumpus_sent2h) != len(list_sumpus_sent2l) or len(list_sumpus_sent2l) != len(list_sumpus_sent3) or len(list_sumpus_sent3) != len(list_sumpus_sent4)  or len(list_sumpus_sent4) != len(list_sumpus_sent1):
                     return 'The poem does not complete 4 sentences.'
                 else:
                     for i in range(len(list_sumpus_sent1)):
                         countwrong = 0
                         for j in list_sumpus_sent2h[i]:
-                            if self.is_sumpus(list_sumpus_sent1[i],j) == False:
+                            if self.check_sumpus(list_sumpus_sent1[i],j) == False:
                                     countwrong +=1
                         if  countwrong > 3:
                             error.append('Cant find rhyme between paragraphs '+str((list_sumpus_sent1[i],list_sumpus_sent2h[i]))+'in paragraph '+str(i+1))
-                        if self.is_sumpus(list_sumpus_sent2l[i],list_sumpus_sent3[i]) == False:
+                        if self.check_sumpus(list_sumpus_sent2l[i],list_sumpus_sent3[i]) == False:
                             # print(sumpus_sent2l,sumpus_sent3)
                             error.append('Cant find rhyme between paragraphs '+str((list_sumpus_sent2l[i],list_sumpus_sent3[i]))+'in paragraph '+str(i+1))
                         if i > 0:
-                            if self.is_sumpus(list_sumpus_sent2l[i],list_sumpus_sent4[i-1]) == False:
+                            if self.check_sumpus(list_sumpus_sent2l[i],list_sumpus_sent4[i-1]) == False:
                                 error.append('Cant find rhyme between paragraphs '+str((list_sumpus_sent2l[i],list_sumpus_sent4[i-1]))+'in paragraph '+str(i+1))
                     if error == []:
                         return 'The poem is correct according to the principle.'
                     else:
                         return error
             except:
                 return 'Something went wrong Make sure you enter it in correct form of klon 8.'
@@ -390,40 +372,39 @@
                 if len(list_sumpus_sent1) != len(list_sumpus_sent2h) or len(list_sumpus_sent2h) != len(list_sumpus_sent2l) or len(list_sumpus_sent2l) != len(list_sumpus_sent3) or len(list_sumpus_sent3) != len(list_sumpus_sent4)  or len(list_sumpus_sent4) != len(list_sumpus_sent1):
                     return 'The poem does not complete 4 sentences.'
                 else:
                     for i in range(len(list_sumpus_sent1)):
                         countwrong = 0
                         for j in list_sumpus_sent2h[i]:
                             # print(list_sumpus_sent1[i],j)
-                            if self.is_sumpus(list_sumpus_sent1[i],j) == False:
+                            if self.check_sumpus(list_sumpus_sent1[i],j) == False:
                                     countwrong +=1
                         if  countwrong > 1:
                             error.append('Cant find rhyme between paragraphs '+str((list_sumpus_sent1[i],list_sumpus_sent2h[i]))+'in paragraph '+str(i+1))
-                        if self.is_sumpus(list_sumpus_sent2l[i],list_sumpus_sent3[i]) == False:
+                        if self.check_sumpus(list_sumpus_sent2l[i],list_sumpus_sent3[i]) == False:
                             # print(sumpus_sent2l,sumpus_sent3)
                             error.append('Cant find rhyme between paragraphs '+str((list_sumpus_sent2l[i],list_sumpus_sent3[i]))+'in paragraph '+str(i+1))
                         if i > 0:
-                            if self.is_sumpus(list_sumpus_sent2l[i],list_sumpus_sent4[i-1]) == False:
+                            if self.check_sumpus(list_sumpus_sent2l[i],list_sumpus_sent4[i-1]) == False:
                                 error.append('Cant find rhyme between paragraphs '+str((list_sumpus_sent2l[i],list_sumpus_sent4[i-1]))+'in paragraph '+str(i+1))
                     if error == []:
                         return 'The poem is correct according to the principle.'
                     else:
                         return error
             except:
                 return 'Something went wrong Make sure you enter it in correct form.'
             
         else:
             return 'Something went wrong Make sure you enter it in correct form.'
-        
-    def check_aek_too(self, text: Union[List[str], str], dead_syllable_as_aek:bool = False) -> Union[List[bool], List[str], bool, str]:
+
+    def check_aek_too(self, text: Union[List[str], str]) -> Union[List[bool], List[str], bool, str]:
         """
         Thai tonal word checker
 
-        :param Union[List[str], str] text: Thai word or list of Thai words
-        :param bool dead_syllable_as_aek: if True, dead syllable will be considered as aek
+        :param str or list[str] text: Thai word or list of Thai words
         :return: the check if the word is aek or too or False(not both) or list of the check if input is list
         :rtype: Union[List[bool], List[str], bool, str]
 
         :Example:
         ::
 
             from pythainlp.khavee import KhaveeVerifier
@@ -431,25 +412,21 @@
             kv = KhaveeVerifier()
 
             # การเช็คคำเอกโท
             print(kv.check_aek_too('เอง'), kv.check_aek_too('เอ่ง'), kv.check_aek_too('เอ้ง'))
             ## -> False, aek, too
             print(kv.check_aek_too(['เอง', 'เอ่ง', 'เอ้ง'])) # ใช้ List ได้เหมือนกัน
             ## -> [False, 'aek', 'too']
-
-
         """
         if isinstance(text, list):
-            return [self.check_aek_too(t, dead_syllable_as_aek) for t in text]
+            return [self.check_aek_too(t) for t in text]
 
         if not isinstance(text, str):
             raise TypeError('text must be str or iterable list[str]')
 
         word_characters = [*text]
         if '่' in word_characters and not '้' in word_characters:
             return 'aek'
         elif '้' in word_characters and not '่' in word_characters:
             return 'too'
-        if dead_syllable_as_aek and sound_syllable(text) == 'dead':
-            return 'aek'
         else:
             return False
```

### Comparing `pythainlp-4.0.0/pythainlp/khavee/example.py` & `pythainlp-4.0.0b1/pythainlp/khavee/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 # -*- coding: utf-8 -*-
 import core
 kv = core.KhaveeVerifier()
 
 
 # การเช็คสระ
-print('เออ',kv.check_sara('เมอ'))
+print('เริง',kv.check_sara('เริง'))
 # 'เออ'
 
 # การเช็คมาตราตัวสะกด
-print('เทอว',kv.check_marttra('เทอว'))
+print('สาว',kv.check_marttra('สาว'))
 # 'เกอว'
 
 # การตรวจสอบคำสำผัสที่ถูกต้อง
-print('สรร อัน',kv.is_sumpus('สรร','อัน'))
+print('สรร อัน',kv.check_sumpus('สรร','อัน'))
 # True
 
 # การตรวจสอบคำสำผัสที่ผิด
-print('สรร ขวาน',kv.is_sumpus('สรร','ขวาน'))
+print('สรร อัน',kv.check_sumpus('หมัน','อัน'))
 # False
 
-# การตรวจสอบคำ ครุ ลหุ 
-print('สรร',kv.check_karu_lahu('สรร'))
-#karu
-# การตรวจสอบคำ ครุ ลหุ 
-print('ชิชะ',kv.check_karu_lahu('ชิชะ'))
-# lahu
-
 # การตรวจสอบกลอน 8 ที่ถูกฉันทลักษณ์
 print(kv.check_klon('''ณรงค์วุฒิผู้เปี่ยมวุฒิสมสง่า มากวิชาหาความรู้ไปสู่ผล 
 เรื่องฟิสิกส์คณิตศาสตร์เอิร์นอดทน เล่นเกมเก่งลำดับต้นของโรงเรียน
 ต่อมาหยกธนัชพรชอบนอนหลับ แต่ผลลัพธ์คือฉลาดเรื่องอ่านเขียน 
 เหมือนจะเล่นแต่เขายังพากเพียร ในการเรียนการเล่นบ้างคละกันไป
 นรภัทรพุกกะมานป่านจอมแก่น ทั่วแว่นแคว้นโดนเขาแกล้งไม่สงสัย
 เรื่องวิศวะเก่งกาจประหลาดใจ เรื่องฟิสิกส์ไร้ผู้ใดมาต่อกร
```

### Comparing `pythainlp-4.0.0/pythainlp/parse/__init__.py` & `pythainlp-4.0.0b1/pythainlp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/parse/core.py` & `pythainlp-4.0.0b1/pythainlp/parse/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/parse/esupar_engine.py` & `pythainlp-4.0.0b1/pythainlp/parse/esupar_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/parse/spacy_thai_engine.py` & `pythainlp-4.0.0b1/pythainlp/parse/spacy_thai_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/parse/transformers_ud.py` & `pythainlp-4.0.0b1/pythainlp/parse/transformers_ud.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/parse/ud_goeswith.py` & `pythainlp-4.0.0b1/pythainlp/parse/ud_goeswith.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/soundex/__init__.py` & `pythainlp-4.0.0b1/pythainlp/soundex/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/soundex/core.py` & `pythainlp-4.0.0b1/pythainlp/soundex/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/soundex/lk82.py` & `pythainlp-4.0.0b1/pythainlp/soundex/lk82.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/soundex/metasound.py` & `pythainlp-4.0.0b1/pythainlp/soundex/metasound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/soundex/prayut_and_somchaip.py` & `pythainlp-4.0.0b1/pythainlp/soundex/prayut_and_somchaip.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/soundex/udom83.py` & `pythainlp-4.0.0b1/pythainlp/soundex/udom83.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/spell/__init__.py` & `pythainlp-4.0.0b1/pythainlp/spell/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/spell/core.py` & `pythainlp-4.0.0b1/pythainlp/spell/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/spell/phunspell.py` & `pythainlp-4.0.0b1/pythainlp/spell/phunspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/spell/pn.py` & `pythainlp-4.0.0b1/pythainlp/spell/pn.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/spell/symspellpy.py` & `pythainlp-4.0.0b1/pythainlp/spell/symspellpy.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/spell/tltk.py` & `pythainlp-4.0.0b1/pythainlp/spell/tltk.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,13 @@
 
 Thai Language Toolkit
 
 :See Also:
     * \
         https://pypi.org/project/tltk/
 """
-try:
-    from tltk.nlp import spell_candidates
-except ImportError:
-    raise ImportError("Not found tltk! Please install tltk by pip install tltk")
+from tltk.nlp import spell_candidates
 from typing import List
 
 
 def spell(text: str) -> List[str]:
     return spell_candidates(text)
```

### Comparing `pythainlp-4.0.0/pythainlp/summarize/__init__.py` & `pythainlp-4.0.0b1/pythainlp/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/summarize/core.py` & `pythainlp-4.0.0b1/pythainlp/summarize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/summarize/freq.py` & `pythainlp-4.0.0b1/pythainlp/summarize/freq.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/summarize/keybert.py` & `pythainlp-4.0.0b1/pythainlp/summarize/keybert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/summarize/mt5.py` & `pythainlp-4.0.0b1/pythainlp/summarize/mt5.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/__init__.py` & `pythainlp-4.0.0b1/pythainlp/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/_tag_perceptron.py` & `pythainlp-4.0.0b1/pythainlp/tag/_tag_perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/blackboard.py` & `pythainlp-4.0.0b1/pythainlp/tag/blackboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/chunk.py` & `pythainlp-4.0.0b1/pythainlp/tag/chunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/crfchunk.py` & `pythainlp-4.0.0b1/pythainlp/tag/crfchunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/locations.py` & `pythainlp-4.0.0b1/pythainlp/tag/locations.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/named_entity.py` & `pythainlp-4.0.0b1/pythainlp/tag/named_entity.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/orchid.py` & `pythainlp-4.0.0b1/pythainlp/tag/orchid.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/perceptron.py` & `pythainlp-4.0.0b1/pythainlp/tag/perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/pos_tag.py` & `pythainlp-4.0.0b1/pythainlp/tag/pos_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/thai_nner.py` & `pythainlp-4.0.0b1/pythainlp/tag/thai_nner.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/thainer.py` & `pythainlp-4.0.0b1/pythainlp/tag/thainer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/tltk.py` & `pythainlp-4.0.0b1/pythainlp/tag/tltk.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Tuple, Union
-try:
-    from tltk import nlp
-except ImportError:
-    raise ImportError("Not found tltk! Please install tltk by pip install tltk")
+from tltk import nlp
 from pythainlp.tokenize import word_tokenize
 
 nlp.pos_load()
 nlp.ner_load()
 
 
 def pos_tag(words: List[str], corpus: str = "tnc") -> List[Tuple[str, str]]:
```

### Comparing `pythainlp-4.0.0/pythainlp/tag/unigram.py` & `pythainlp-4.0.0b1/pythainlp/tag/unigram.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tag/wangchanberta_onnx.py` & `pythainlp-4.0.0b1/pythainlp/tag/wangchanberta_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/__init__.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/_utils.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/_utils.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/attacut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/attacut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/core.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/crfcls.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/crfcls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/crfcut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/crfcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/deepcut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/deepcut.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 
 :See Also:
     * `GitHub repository <https://github.com/rkcosmos/deepcut>`_
 """
 
 from typing import List, Union
 
-try:
-    from deepcut import tokenize
-except ImportError:
-    raise ImportError("Please install deepcut by pip install deepcut")
+from deepcut import tokenize
 from pythainlp.util import Trie
 
 
 def segment(
     text: str, custom_dict: Union[Trie, List[str], str] = None
 ) -> List[str]:
     if not text or not isinstance(text, str):
```

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/etcc.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/etcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/longest.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/longest.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/multi_cut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/multi_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/nercut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/nercut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/newmm.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/newmm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/nlpo3.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/nlpo3.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/oskut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/oskut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/pyicu.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/sefr_cut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/sefr_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/ssg.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/ssg.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/tcc.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/tcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/tcc_p.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/tcc_p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/thaisumcut.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/thaisumcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tokenize/tltk.py` & `pythainlp-4.0.0b1/pythainlp/tokenize/tltk.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
-try:
-    from tltk.nlp import word_segment as tltk_segment
-    from tltk.nlp import syl_segment
-except ImportError:
-    raise ImportError("Not found tltk! Please install tltk by pip install tltk")
+from tltk.nlp import word_segment as tltk_segment
+from tltk.nlp import syl_segment
 
 
 def segment(text: str) -> List[str]:
     if not text or not isinstance(text, str):
         return []
     text = text.replace(" ", "<u/>")
     _temp = tltk_segment(text).replace("<u/>", " ").replace("<s/>", "")
```

### Comparing `pythainlp-4.0.0/pythainlp/tools/__init__.py` & `pythainlp-4.0.0b1/pythainlp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tools/misspell.py` & `pythainlp-4.0.0b1/pythainlp/tools/misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/tools/path.py` & `pythainlp-4.0.0b1/pythainlp/tools/path.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/translate/__init__.py` & `pythainlp-4.0.0b1/pythainlp/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/translate/core.py` & `pythainlp-4.0.0b1/pythainlp/translate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/translate/en_th.py` & `pythainlp-4.0.0b1/pythainlp/translate/en_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/translate/th_fr.py` & `pythainlp-4.0.0b1/pythainlp/translate/th_fr.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/translate/zh_th.py` & `pythainlp-4.0.0b1/pythainlp/translate/zh_th.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/__init__.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/core.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/ipa.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/ipa.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/iso_11940.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/iso_11940.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/lookup.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/lookup.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/pyicu.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/royin.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/royin.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/spoonerism.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/spoonerism.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/thai2rom.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/thai2rom.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/thai2rom_onnx.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/thai2rom_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/thaig2p.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/thaig2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/tltk.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/tltk.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-try:
-    from tltk.nlp import g2p, th2ipa, th2roman
-except ImportError:
-    raise ImportError("Not found tltk! Please install tltk by pip install tltk")
+from tltk.nlp import g2p, th2ipa, th2roman
 
 
 def romanize(text: str) -> str:
     """
     Transliterating thai text to the Latin alphabet with tltk.
 
     :param str text: Thai text to be romanized
```

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/w2p.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/w2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/transliterate/wunsen.py` & `pythainlp-4.0.0b1/pythainlp/transliterate/wunsen.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/ulmfit/__init__.py` & `pythainlp-4.0.0b1/pythainlp/ulmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/ulmfit/core.py` & `pythainlp-4.0.0b1/pythainlp/ulmfit/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/ulmfit/preprocess.py` & `pythainlp-4.0.0b1/pythainlp/ulmfit/preprocess.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/ulmfit/tokenizer.py` & `pythainlp-4.0.0b1/pythainlp/ulmfit/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/__init__.py` & `pythainlp-4.0.0b1/pythainlp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/collate.py` & `pythainlp-4.0.0b1/pythainlp/util/collate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/date.py` & `pythainlp-4.0.0b1/pythainlp/util/date.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/digitconv.py` & `pythainlp-4.0.0b1/pythainlp/util/digitconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/emojiconv.py` & `pythainlp-4.0.0b1/pythainlp/util/emojiconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/keyboard.py` & `pythainlp-4.0.0b1/pythainlp/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/keywords.py` & `pythainlp-4.0.0b1/pythainlp/util/keywords.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/normalize.py` & `pythainlp-4.0.0b1/pythainlp/util/normalize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/numtoword.py` & `pythainlp-4.0.0b1/pythainlp/util/numtoword.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/phoneme.py` & `pythainlp-4.0.0b1/pythainlp/util/phoneme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/strftime.py` & `pythainlp-4.0.0b1/pythainlp/util/strftime.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/syllable.py` & `pythainlp-4.0.0b1/pythainlp/util/syllable.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/thai.py` & `pythainlp-4.0.0b1/pythainlp/util/thai.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/thaiwordcheck.py` & `pythainlp-4.0.0b1/pythainlp/util/thaiwordcheck.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/time.py` & `pythainlp-4.0.0b1/pythainlp/util/time.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/trie.py` & `pythainlp-4.0.0b1/pythainlp/util/trie.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/util/wordtonum.py` & `pythainlp-4.0.0b1/pythainlp/util/wordtonum.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/wangchanberta/__init__.py` & `pythainlp-4.0.0b1/pythainlp/wangchanberta/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/wangchanberta/core.py` & `pythainlp-4.0.0b1/pythainlp/wangchanberta/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/word_vector/__init__.py` & `pythainlp-4.0.0b1/pythainlp/word_vector/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp/word_vector/core.py` & `pythainlp-4.0.0b1/pythainlp/word_vector/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp.egg-info/PKG-INFO` & `pythainlp-4.0.0b1/pythainlp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pythainlp
-Version: 4.0.0
+Version: 4.0.0b1
 Summary: Thai Natural Language Processing library
 Home-page: https://github.com/PyThaiNLP/pythainlp
 Author: PyThaiNLP
 Author-email: email@wannaphong.com
 License: Apache Software License 2.0
-Project-URL: Documentation, https://pythainlp.github.io/docs/4.0/
+Project-URL: Documentation, https://pythainlp.github.io/docs/3.0/
 Project-URL: Tutorials, https://pythainlp.github.io/tutorials/
 Project-URL: Source Code, https://github.com/PyThaiNLP/pythainlp
 Project-URL: Bug Tracker, https://github.com/PyThaiNLP/pythainlp/issues
 Description: 
         ![PyThaiNLP Logo](https://avatars0.githubusercontent.com/u/32934255?s=200&v=4)
         
         PyThaiNLP is a Python library for Thai natural language processing.
@@ -35,15 +35,15 @@
         ```
         
         Some functionalities, like named-entity recognition, required extra packages.
         See https://github.com/PyThaiNLP/pythainlp for installation options.
         
 Keywords: pythainlp,NLP,natural language processing,text analytics,text processing,localization,computational linguistics,ThaiNLP,Thai NLP,Thai language
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Thai
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
@@ -63,14 +63,15 @@
 Provides-Extra: textaugment
 Provides-Extra: wangchanberta
 Provides-Extra: mt5
 Provides-Extra: wordnet
 Provides-Extra: generate
 Provides-Extra: sefr_cut
 Provides-Extra: spell
+Provides-Extra: tltk
 Provides-Extra: oskut
 Provides-Extra: nlpo3
 Provides-Extra: onnx
 Provides-Extra: thai_nner
 Provides-Extra: esupar
 Provides-Extra: spacy_thai
 Provides-Extra: transformers_ud
```

### Comparing `pythainlp-4.0.0/pythainlp.egg-info/SOURCES.txt` & `pythainlp-4.0.0b1/pythainlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/pythainlp.egg-info/requires.txt` & `pythainlp-4.0.0b1/pythainlp.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 fastai<2.0
 bpemb>=0.3.2
 transformers>=4.22.1
 sefr_cut>=1.1
 phunspell>=0.1.6
 spylls>=0.1.5
 symspellpy>=6.7.6
+tltk>=1.3.8
 oskut>=1.3
 nlpo3>=1.2.2
 onnxruntime>=1.10.0
 thai_nner
 wunsen>=0.0.3
 spacy_thai>=0.7.1
 ufal.chu-liu-edmonds>=1.0.2
@@ -105,14 +106,17 @@
 [thai2rom]
 numpy>=1.22
 torch>=1.0.0
 
 [thai_nner]
 thai_nner
 
+[tltk]
+tltk>=1.3.8
+
 [transformers_ud]
 ufal.chu-liu-edmonds>=1.0.2
 transformers>=4.22.1
 
 [translate]
 fairseq>=0.10.0
 sacremoses>=0.0.41
```

### Comparing `pythainlp-4.0.0/setup.cfg` & `pythainlp-4.0.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/setup.py` & `pythainlp-4.0.0b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,8 @@
 ﻿# -*- coding: utf-8 -*-
-# Copyright (C) 2016-2023 PyThaiNLP Project
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 """
 Setup script for PyThaiNLP.
 
 https://github.com/PyThaiNLP/pythainlp
 """
 from setuptools import find_packages, setup
 
@@ -82,14 +69,15 @@
     "generate": ["fastai<2.0"],
     "sefr_cut": ["sefr_cut>=1.1"],
     "spell": [
         "phunspell>=0.1.6",
         "spylls>=0.1.5",
         "symspellpy>=6.7.6"
     ],
+    "tltk": ["tltk>=1.3.8"],
     "oskut": ["oskut>=1.3"],
     "nlpo3": ["nlpo3>=1.2.2"],
     "onnx": [
         "sentencepiece>=0.1.91",
         "numpy>=1.22",
         "onnxruntime>=1.10.0"
     ],
@@ -127,27 +115,28 @@
         "fastai<2.0",
         "bpemb>=0.3.2",
         "transformers>=4.22.1",
         "sefr_cut>=1.1",
         "phunspell>=0.1.6",
         "spylls>=0.1.5",
         "symspellpy>=6.7.6",
+        "tltk>=1.3.8",
         "oskut>=1.3",
         "nlpo3>=1.2.2",
         "onnxruntime>=1.10.0",
         "thai_nner",
         "wunsen>=0.0.3",
         "spacy_thai>=0.7.1",
         "ufal.chu-liu-edmonds>=1.0.2",
     ],
 }
 
 setup(
     name="pythainlp",
-    version="4.0.0",
+    version="4.0.0beta1",
     description="Thai Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="PyThaiNLP",
     author_email="email@wannaphong.com",
     url="https://github.com/PyThaiNLP/pythainlp",
     packages=find_packages(exclude=["tests", "tests.*"]),
@@ -172,15 +161,15 @@
         "localization",
         "computational linguistics",
         "ThaiNLP",
         "Thai NLP",
         "Thai language",
     ],
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: Thai",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Text Processing",
         "Topic :: Text Processing :: General",
@@ -188,15 +177,15 @@
     ],
     entry_points={
         "console_scripts": [
             "thainlp = pythainlp.__main__:main",
         ],
     },
     project_urls={
-        "Documentation": "https://pythainlp.github.io/docs/4.0/",
+        "Documentation": "https://pythainlp.github.io/docs/3.0/",
         "Tutorials": "https://pythainlp.github.io/tutorials/",
         "Source Code": "https://github.com/PyThaiNLP/pythainlp",
         "Bug Tracker": "https://github.com/PyThaiNLP/pythainlp/issues",
     },
 )
 
 # TODO: Check extras and decide to download additional data, like model files
```

### Comparing `pythainlp-4.0.0/tests/data/eval-details-input.json` & `pythainlp-4.0.0b1/tests/data/eval-details-input.json`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/data/sentences.yml` & `pythainlp-4.0.0b1/tests/data/sentences.yml`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_augment.py` & `pythainlp-4.0.0b1/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_benchmarks.py` & `pythainlp-4.0.0b1/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_cli.py` & `pythainlp-4.0.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_corpus.py` & `pythainlp-4.0.0b1/tests/test_corpus.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_generate.py` & `pythainlp-4.0.0b1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_khavee.py` & `pythainlp-4.0.0b1/tests/test_khavee.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 class TestKhaveePackage(unittest.TestCase):
     def test_check_sara(self):
         self.assertEqual(kv.check_sara('เริง'), 'เออ')
 
     def test_check_marttra(self):
         self.assertEqual(kv.check_marttra('สาว'), 'เกอว')
 
-    def test_is_sumpus(self):
-        self.assertTrue(kv.is_sumpus('สรร','อัน'))
-        self.assertFalse(kv.is_sumpus('สรร','แมว'))
+    def test_check_sumpus(self):
+        self.assertTrue(kv.check_sumpus('สรร','อัน'))
+        self.assertFalse(kv.check_sumpus('สรร','แมว'))
     
     def test_check_klon(self):
         self.assertEqual(
             kv.check_klon('''ฉันชื่อหมูกรอบ ฉันชอบกินไก่ แล้วก็วิ่งไล่ หมาชื่อนํ้าทอง ลคคนเก่ง เอ๋งเอ๋งคะนอง มีคนจับจอง เขาชื่อน้องเธียร''',k_type=4),
             'The poem is correct according to the principle.'
         )
         self.assertEqual(
```

### Comparing `pythainlp-4.0.0/tests/test_misspell.py` & `pythainlp-4.0.0b1/tests/test_misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_parse.py` & `pythainlp-4.0.0b1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_soundex.py` & `pythainlp-4.0.0b1/tests/test_soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_spell.py` & `pythainlp-4.0.0b1/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_summarize.py` & `pythainlp-4.0.0b1/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_tag.py` & `pythainlp-4.0.0b1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_tokenize.py` & `pythainlp-4.0.0b1/tests/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_translate.py` & `pythainlp-4.0.0b1/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_transliterate.py` & `pythainlp-4.0.0b1/tests/test_transliterate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_ulmfit.py` & `pythainlp-4.0.0b1/tests/test_ulmfit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_util.py` & `pythainlp-4.0.0b1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_wangchanberta.py` & `pythainlp-4.0.0b1/tests/test_wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.0/tests/test_word_vector.py` & `pythainlp-4.0.0b1/tests/test_word_vector.py`

 * *Files identical despite different names*

