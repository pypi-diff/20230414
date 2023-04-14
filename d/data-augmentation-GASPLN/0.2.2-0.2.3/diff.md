# Comparing `tmp/data_augmentation_GASPLN-0.2.2.tar.gz` & `tmp/data_augmentation_GASPLN-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_augmentation_GASPLN-0.2.2.tar", last modified: Thu Apr 13 02:49:45 2023, max compression
+gzip compressed data, was "data_augmentation_GASPLN-0.2.3.tar", last modified: Fri Apr 14 01:48:31 2023, max compression
```

## Comparing `data_augmentation_GASPLN-0.2.2.tar` & `data_augmentation_GASPLN-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.683981 data_augmentation_GASPLN-0.2.2/
--rw-rw-rw-   0        0        0    35823 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       24 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      217 2023-04-13 02:49:45.684499 data_augmentation_GASPLN-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9130 2023-04-13 02:49:17.000000 data_augmentation_GASPLN-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.643902 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/
--rw-rw-rw-   0        0        0     9497 2023-04-13 02:48:58.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.676203 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/data/
--rw-rw-rw-   0        0        0  7024004 2023-04-06 12:32:05.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
-drwxrwxrwx   0        0        0        0 2023-04-13 02:49:45.676203 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/
--rw-rw-rw-   0        0        0      217 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-13 02:49:45.000000 data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 02:49:45.686023 data_augmentation_GASPLN-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-13 02:49:34.000000 data_augmentation_GASPLN-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 01:48:31.419112 data_augmentation_GASPLN-0.2.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-14 01:46:11.000000 data_augmentation_GASPLN-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-14 01:46:11.000000 data_augmentation_GASPLN-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      217 2023-04-14 01:48:31.419112 data_augmentation_GASPLN-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10451 2023-04-14 01:46:11.000000 data_augmentation_GASPLN-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 01:48:31.406113 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN/
+-rw-rw-rw-   0        0        0     9472 2023-04-14 01:47:29.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 01:48:31.413113 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN/data/
+-rw-rw-rw-   0        0        0  7024004 2023-04-14 01:46:11.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet
+drwxrwxrwx   0        0        0        0 2023-04-14 01:48:31.412112 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-04-14 01:48:31.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-14 01:48:31.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 01:48:31.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-14 01:48:31.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-14 01:48:31.000000 data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 01:48:31.420112 data_augmentation_GASPLN-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-14 01:48:28.000000 data_augmentation_GASPLN-0.2.3/setup.py
```

### Comparing `data_augmentation_GASPLN-0.2.2/LICENSE` & `data_augmentation_GASPLN-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.2.2/README.md` & `data_augmentation_GASPLN-0.2.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # Data Augmentation Library for Portuguese (Brazil)
 
+**Para uma versão deste README em Português, clique [aqui](README_pt_BR.md).**
+
 This is a research project developed in collaboration with the [GASPLN](https://wp.ufpel.edu.br/gaspln/) research group of the Federal University of Pelotas (UFPel) aimed at creating a Python library for Data Augmentation in Portuguese (Brazil).
 
 ## Table of Contents
+
 - [Installation](#installation)  
 - [Usage](#usage)
     - [Synonym Replacement](#synonyms-replacement-function)
     - [Back Translation](#back-translation-function)
     - [Character Swap](#character-swap-function)
     - [Random Swap](#random-swap-function)
     - [Add Noise](#add-noise-function)
     - [Text Augmentation](#text-augmentation-function)
+- [Synonyms Dataset](#synonyms-dataset)
 
 
 # Installation
 
 The package is available on PyPI and can be easily installed using pip:
 
 ```bash
@@ -27,21 +31,23 @@
 python -m spacy download pt_core_news_sm
 ```
 
 # Usage
 
 ## Synonyms Replacement Function
 
-This function is used to replace a percentage of words in a given text string with their synonyms. It takes three arguments: `text`, `synonyms_df`, and `percentage`.
+This function is used to replace a percentage of words in a given text string with their synonyms. It takes two arguments: `text` and `percentage`.
 
-### Arguments:
+***For information about the synonym dataset used in the function, navigate to [Synonyms Dataset](#synonyms-dataset).***
 
-* `text` (str): The input text to be processed. This can be any string, but should ideally be a full sentence or paragraph for best results.
+### Arguments
 
-* `percentage` (float, optional): The percentage of words in the input `text` that should be replaced with their synonyms. The default value is 0.25, which means that 25% of the words in the input text will be replaced.
+- `text` (str): The input text to be processed. This can be any string, but should ideally be a full sentence or paragraph for best results.
+
+- `percentage` (float, optional): The percentage of words in the input `text` that should be replaced with their synonyms. The default value is 0.25, which means that 25% of the words in the input text will be replaced.
 
 ### Example Usage:
 
 Here's an example of how to use the `synonyms_replacement` function:
 
 ```python
 from data_augmentation_GASPLN import synonyms_replacement
@@ -52,21 +58,23 @@
 
 # Print the result
 print(augmented_text)
 ```
 
 ## Back Translation Function
 
-This function performs back translation of the given text, iterating over the provided languages in the list. 
+This function performs back translation of the given text, iterating over the provided languages in the list.
+
+### Arguments
 
-### Arguments:
+- `text` (str): The input text to be translated.
 
-* `text` (str): The input text to be translated. 
-* `languages` (List[str]): The list of languages to be used for back translation, excluding the original language. The last language in the list must be Portuguese, unless it is the only language in the list (it will be automatically added if not provided).
-* `translator` (str): The name of the translator to be used for back translation. Must be one available at https://pypi.org/project/translators/#supported-translation-services
+- `languages` (List[str]): The list of languages to be used for back translation, excluding the original language.
+
+- `translator` (str): The name of the translator to be used for back translation. Must be one available at https://pypi.org/project/translators/#supported-translation-services
 
 ### Example Usage:
 
 ```python
 from data_augmentation_GASPLN import back_translation
 
 # Call the function with the following parameters
@@ -80,19 +88,19 @@
 print(augmented_text)
 ```
 
 ## Character Swap Function
 
 This function is used to swap characters in words of the input text with a given probability, except for words with less than or equal to 3 letters or for punctuation marks, keeping their positions in the word. It takes two arguments: `text` and `prob`.
 
-### Arguments:
+### Arguments
 
-* `text` (str): The input text to swap characters in. This can be any string, but should ideally be a full sentence or paragraph for best results.
+- `text` (str): The input text to swap characters in. This can be any string, but should ideally be a full sentence or paragraph for best results.
 
-* `prob` (float, optional): The probability of swapping characters in each eligible word. The default value is 0.25, which means that there is a 25% chance of swapping characters in each eligible word.
+- `prob` (float, optional): The probability of swapping characters in each eligible word. The default value is 0.25, which means that there is a 25% chance of swapping characters in each eligible word.
 
 ### Example Usage:
 
 Here's an example of how to use the `character_swap` function:
 
 ```python
 from data_augmentation_GASPLN import character_swap
@@ -105,25 +113,25 @@
 print(augmented_text)
 ```
 
 ## Random Swap Function
 
 This function randomly swaps words in a text. You can specify either the percentage of words to swap, or the number of words to swap, or the probability of swapping each word (with a default of 20%).
 
-### Arguments:
+### Arguments
 
-* `text` (str): The input text to swap words in. This can be any string.
+- `text` (str): The input text to swap words in. This can be any string.
 
-* `percentage` (float, optional): The percentage of words to swap in the input text. The default value is None.
+- `percentage` (float, optional): The percentage of words to swap in the input text. The default value is None.
 
-* `num_words` (int, optional): The number of words to swap in the input text. The default value is None.
+- `num_words` (int, optional): The number of words to swap in the input text. The default value is None.
 
-* `prob` (float, optional): The probability of swapping each word in the input text. The default value is 0.15.
+- `prob` (float, optional): The probability of swapping each word in the input text. The default value is 0.15.
 
-### Example Usage:
+### Example Usage
 
 Here's an example of how to use the `random_swap` function:
 
 ```python
 from data_augmentation_GASPLN import random_swap
 
 # Call the function with the following parameters
@@ -134,23 +142,23 @@
 print(augmented_text)
 ```
 
 ## Add Noise Function
 
 This function is used to add noise to a percentage of the words in a given text string by inserting or removing letters, and swapping punctuations with a small probability. It takes three arguments: `text`, `word_noise_prob`, and `char_noise_prob`.
 
-### Arguments:
+### Arguments
 
-* `text` (str): The input text to be processed. This can be any string, but should ideally be a full sentence or paragraph for best results.
+- `text` (str): The input text to be processed. This can be any string, but should ideally be a full sentence or paragraph for best results.
 
-* `word_noise_prob` (float, optional): The probability of adding noise to a given word. The default value is 0.2, which means that 20% of the words in the input text will have noise added to them.
+- `word_noise_prob` (float, optional): The probability of adding noise to a given word. The default value is 0.2, which means that 20% of the words in the input text will have noise added to them.
 
-* `char_noise_prob` (float, optional): The probability of adding or removing a letter from a given word. The default value is 0.2, which means that there is a 20% chance that a letter will be added or removed from a word.
+- `char_noise_prob` (float, optional): The probability of adding or removing a letter from a given word. The default value is 0.2, which means that there is a 20% chance that a letter will be added or removed from a word.
 
-### Example Usage:
+### Example Usage
 
 Here's an example of how to use the `add_noise` function:
 
 ```python
 from data_augmentation_GASPLN import add_noise
 
 # Call the function with the following parameters
@@ -160,47 +168,47 @@
 # Print the result
 print(augmented_text)
 ```
 ## Text Augmentation Function
 
 This function applies multiple text augmentation techniques to the input text. It takes several arguments that determine which techniques are used and with what parameters.
 
-### Arguments:
+### Arguments
 
-* `text` (str): The input text to be processed.
+- `text` (str): The input text to be processed.
 
-* `use_synonyms` (bool, optional): Whether or not to use synonym replacement. Default is `True`.
+- `use_synonyms` (bool, optional): Whether or not to use synonym replacement. Default is `True`.
 
-* `synonyms_percentage` (float, optional): The percentage of words in the input text that should be replaced with their synonyms. Default is 0.5.
+- `synonyms_percentage` (float, optional): The percentage of words in the input text that should be replaced with their synonyms. Default is 0.5.
 
-* `use_back_translation` (bool, optional): Whether or not to use back translation. Default is `False`.
+- `use_back_translation` (bool, optional): Whether or not to use back translation. Default is `False`.
 
-* `languages` (List[str], optional): A list of two-letter language codes representing the languages to translate the text to and back from. Default is `['en', 'es']`.
+- `languages` (List[str], optional): A list of two-letter language codes representing the languages to translate the text to and back from. Default is `['en', 'es']`.
 
-* `translator` (str, optional): The name of the translator to use for back translation. Currently, the only supported value is `'google'`. Default is `'google'`.
+- `translator` (str, optional): The name of the translator to use for back translation. Currently, the only supported value is `'google'`. Default is `'google'`.
 
-* `use_character_swap` (bool, optional): Whether or not to use character swap. Default is `False`.
+- `use_character_swap` (bool, optional): Whether or not to use character swap. Default is `False`.
 
-* `char_swap_prob` (float, optional): The probability of swapping a character in a word. Default is 0.25.
+- `char_swap_prob` (float, optional): The probability of swapping a character in a word. Default is 0.25.
 
-* `use_random_swap` (bool, optional): Whether or not to use random word swap. Default is `False`.
+- `use_random_swap` (bool, optional): Whether or not to use random word swap. Default is `False`.
 
-* `random_swap_percentage` (float, optional): The percentage of words in the input text to swap with other words. If `num_words` is specified, this parameter is ignored. Default is `None`.
+- `random_swap_percentage` (float, optional): The percentage of words in the input text to swap with other words. If `num_words` is specified, this parameter is ignored. Default is `None`.
 
-* `num_words` (int, optional): The number of words to swap with other words in the input text. If `num_words` is specified, `random_swap_percentage` is ignored. Default is `None`.
+- `num_words` (int, optional): The number of words to swap with other words in the input text. If `num_words` is specified, `random_swap_percentage` is ignored. Default is `None`.
 
-* `random_swap_prob` (float, optional): The probability of swapping a word in the text. Default is 0.15.
+- `random_swap_prob` (float, optional): The probability of swapping a word in the text. Default is 0.15.
 
-* `use_add_noise` (bool, optional): Whether or not to add noise to the text. Default is `True`.
+- `use_add_noise` (bool, optional): Whether or not to add noise to the text. Default is `True`.
 
-* `word_noise_prob` (float, optional): The probability of adding noise to a word in the text. Default is 0.2.
+- `word_noise_prob` (float, optional): The probability of adding noise to a word in the text. Default is 0.2.
 
-* `char_noise_prob` (float, optional): The probability of adding or removing a character in a word in the text. Default is 0.2.
+- `char_noise_prob` (float, optional): The probability of adding or removing a character in a word in the text. Default is 0.2.
 
-### Example Usage:
+### Example Usage
 
 Here's an example of how to use the `text_augmentation` function:
 
 ```python
 from data_augmentation_GASPLN import text_augmentation
 
 # Call the function with the following parameters
@@ -210,8 +218,17 @@
                                     use_back_translation=True, languages=['en', 'fr'], translator='google', 
                                     use_character_swap=True, char_swap_prob=0.3, 
                                     use_random_swap=True, num_words=2, random_swap_prob=0.2, 
                                     use_add_noise=True, word_noise_prob=0.3, char_noise_prob=0.3)
 
 # Print the result
 print(augmented_text)
-```
+```
+
+## Synonyms Dataset
+
+To generate the synonyms dataset used in this project, a collection of words from the Portuguese language vocabulary was initially made through web scraping from the [Common Orthographic Vocabulary of the Portuguese Language]((https://voc.cplp.org/index.php?action=simplesearch&query=a&sel=start)) and concatenated with the [list of Brazilian Portuguese words](https://www.ime.usp.br/~pf/dicios/br-utf8.txt) provided by the [Institute of Mathematics and Statistics of the University of São Paulo (IME-USP)](https://www.ime.usp.br/). The result was a list of 458,437 words.
+
+Next, the [Dicio API](https://github.com/ThiagoNelsi/dicio-api), provided [Thiago Nelsi do Couto](https://github.com/ThiagoNelsi), was used to generate a dataset with the words and their respective synonyms. With this, the project offers a database rich in words and synonyms that can be used in various applications.
+
+The list of Portuguese language vocabulary words and the synonyms dictionary can be found in the [data](data_augmentation_GASPLN/data) folder of this repository.
+The notebooks used for collecting and generating the synonyms dictionary can be found in the [web_scraping](web_scraping) folder of this repository.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/__init__.py` & `data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                       use_add_noise: bool = True, word_noise_prob: float = 0.2, char_noise_prob: float = 0.2) -> str:
     """
     Apply multiple text augmentation techniques to the input text.
     """
     
     # Use synonyms to replace some words in the text
     if use_synonyms:
-        text = synonyms_replacement(text, synonyms_df=synonyms_df, percentage=synonyms_percentage)
+        text = synonyms_replacement(text, percentage=synonyms_percentage)
         
     # Use back translation to translate the text to a different language and back to the original
     if use_back_translation:
         text = back_translation(text, languages=languages, translator=translator)
         
     # Swap characters in the text
     if use_character_swap:
```

### Comparing `data_augmentation_GASPLN-0.2.2/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet` & `data_augmentation_GASPLN-0.2.3/data_augmentation_GASPLN/data/synonyms_pt_BR.parquet`

 * *Files identical despite different names*

### Comparing `data_augmentation_GASPLN-0.2.2/setup.py` & `data_augmentation_GASPLN-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='data_augmentation_GASPLN',
-    version='0.2.2',
+    version='0.2.3',
     author='Artur Melchiori Cerri',
     author_email='arturmelchiori@gmail.com',
     description='Data augmentation for Portuguese language',
     install_requires=[
         "spacy",
         "nltk",
         "pandas",
```

