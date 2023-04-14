# Comparing `tmp/neosekai_api-1.0.0-py3-none-any.whl.zip` & `tmp/neosekai_api-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6337 bytes, number of entries: 11
+Zip file size: 6845 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      219 b- defN 23-Apr-12 07:51 neosekai_api/__init__.py
--rw-rw-rw-  2.0 fat     2474 b- defN 23-Apr-12 07:49 neosekai_api/chapter.py
--rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-12 07:50 neosekai_api/constants.py
+-rw-rw-rw-  2.0 fat     2573 b- defN 23-Apr-14 12:03 neosekai_api/chapter.py
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-14 10:50 neosekai_api/constants.py
 -rw-rw-rw-  2.0 fat      294 b- defN 23-Apr-05 08:07 neosekai_api/helper.py
--rw-rw-rw-  2.0 fat     4731 b- defN 23-Apr-12 07:47 neosekai_api/novel.py
--rw-rw-rw-  2.0 fat      789 b- defN 23-Apr-08 09:56 neosekai_api/test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1152 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      883 b- defN 23-Apr-12 07:58 neosekai_api-1.0.0.dist-info/RECORD
-11 files, 11757 bytes uncompressed, 4841 bytes compressed:  58.8%
+-rw-rw-rw-  2.0 fat     4735 b- defN 23-Apr-14 11:29 neosekai_api/novel.py
+-rw-rw-rw-  2.0 fat      135 b- defN 23-Apr-14 11:41 neosekai_api/test.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3165 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      883 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/RECORD
+11 files, 13219 bytes uncompressed, 5349 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: neosekai_api/novel.py
 Comment: 
 
 Filename: neosekai_api/test.py
 Comment: 
 
-Filename: neosekai_api-1.0.0.dist-info/LICENSE
+Filename: neosekai_api-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: neosekai_api-1.0.0.dist-info/METADATA
+Filename: neosekai_api-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: neosekai_api-1.0.0.dist-info/WHEEL
+Filename: neosekai_api-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: neosekai_api-1.0.0.dist-info/top_level.txt
+Filename: neosekai_api-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neosekai_api-1.0.0.dist-info/RECORD
+Filename: neosekai_api-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neosekai_api/chapter.py

```diff
@@ -1,36 +1,36 @@
 from neosekai_api.novel import Novel
 import requests
 from bs4 import BeautifulSoup
+from neosekai_api.helper import heavy_translate
 
 
 class NovelChapter:
     '''
     NovelChapter object
 
     :params _url : The Mangadex Chapter URL
     '''
 
     def __init__(self, _url: str) -> None:
         self.url = self.__urlformatter(_url)
         self.__response_object = requests.get(self.url, timeout=10)
-        self.details = self.chapter_details()
         self.volume = self.details['volume']
         self.name = self.details['chapter_name']
         self.release_date = self.details['release_date']
 
     def __urlformatter(self, _url):
         """
         formats url to standard form to be used in the program
         """
         __url = ''
         if 'https://' not in _url:
-            _url == 'https://' + _url
+            __url = 'https://' + _url
         else:
-            return _url
+            return __url
 
     def chapter_details(self):
         """
         returns chapter details : 
 
         - chapter volume
         - chapter name
@@ -43,27 +43,27 @@
         novel_url = self.url[:self.url.index('/', 43)]
         novel = Novel(novel_url)
         index_page = novel.get_index_page()
         for i in index_page:
             if index_page[i]['url'] == self.url:
                 return index_page[i]
 
-    def get_chapter_content(self):
+    def get_chapter_content(self, fancy=True):
         """
         returns main chapter content in JSON format
 
         JSON format:
         ```json
             {
                 "1" : {
                     "type" : '...', "content" : '...'
                 }
             }
         ```
-        - each key will be a paragraph
+        - each key will be a paragraphs
         - ```type```  can have a value of ```text``` for textual content
         - ```type``` can have a value of ```img``` if the content is an image. link to the image will be provided in ```content```
 
         """
         soup = BeautifulSoup(self.__response_object.text, 'lxml')
         div = soup.find('div', attrs={'class': 'text-left'})
         paras = div.find_all('p')
@@ -75,8 +75,11 @@
                                    'content': i.span.text.strip()}
                 n += 1
             elif i.img != None:
                 content[str(n)] = {'type': 'img', 'content': i.img['src']}
                 n += 1
             else:
                 continue
-        return content
+        if fancy:
+            return content
+        else:
+            return heavy_translate(content)
```

## neosekai_api/constants.py

```diff
@@ -1 +1 @@
-VERSION = '1.0.0'
+VERSION = '1.1.0'
```

## neosekai_api/novel.py

```diff
@@ -7,22 +7,22 @@
 class Novel:
     """
     Novel Object
     """
 
     def __init__(self, url):
         self.url = url
-        self.response_object = requests.get(self.url, timeout=10)
+        self._response_object = requests.get(self.url, timeout=10)
         self.novel_tags = self.__initialiser()
 
     def __initialiser(self):
         '''
         returns novel tags as ```dict```
         '''
-        soup = BeautifulSoup(self.response_object.content, 'lxml')
+        soup = BeautifulSoup(self._response_object.content, 'lxml')
 
         # finding title
         title = soup.find('title').text.split(' - NeoSekai')[0]
 
         # finding rating
         rating = soup.find('span', attrs={'id': 'averagerate'}).parent.text + \
             'out of ' + soup.find('span', attrs={'id': 'countrate'}).text
@@ -72,15 +72,15 @@
 
     def get_synopsis(self, fancy=True):
         """
         returns the synopsis text
 
         fancy : if False, replaces all fancy punctuation marks with regular ones.
         """
-        soup = BeautifulSoup(self.response_object.content, 'lxml')
+        soup = BeautifulSoup(self._response_object.content, 'lxml')
         synopsis = soup.find('div', attrs={
             'class': ['summary__content', 'show-more']}).text
 
         if fancy:
             return synopsis
         else:
             return heavy_translate(synopsis)
@@ -100,15 +100,15 @@
                 },
 
                 "2" : {'...'}
             }
         ```
         """
         url = 'https://www.neosekaitranslations.com/wp-admin/admin-ajax.php'
-        soup = BeautifulSoup(self.response_object.content, 'lxml')
+        soup = BeautifulSoup(self._response_object.content, 'lxml')
         data_id = soup.find(
             'div', attrs={'id': 'manga-chapters-holder'})['data-id']
         data = {'action': 'manga_get_chapters', 'manga': data_id}
         soup_2 = BeautifulSoup(requests.post(url, data).content, 'lxml')
         content_dict = {}
         main_wrapper = soup_2.find('ul', attrs={'class': 'main version-chap'})
         volumes_li = list(main_wrapper.find_all(
```

## neosekai_api/test.py

```diff
@@ -1,19 +1,4 @@
-import requests
-from bs4 import BeautifulSoup
-# data = {'action': 'tw_ajax', 'type': 'pagination', 'id': 930068, 'page': 2}
-# url = 'https://readlightnovels.net/wp-admin/admin-ajax.php'
-# print(requests.post(url, data, allow_redirects=True).text)
-# url = "https://www.neosekaitranslations.com/novel/saijo-no-osewa-takane-no-hana-ln/volume-2/v2-chp-2-part-3/"
+from neosekai_api import Novel
 
-# r = requests.get(
-#     url, allow_redirects=False)
-# with open('ch-vavcksbk-5-jitumo.html', 'w', encoding='utf-8') as f:
-#     f.write(r.text)
-soup = BeautifulSoup(open('ch-vavcksbk-5-jitumo.html',
-                     encoding='utf-8').read(), 'lxml')
-div = soup.find('div', attrs={'class': 'text-left'})
-p = div.find_all('p')
-for i in p:
-    print(i.img)
-    if i.img != None:
-        print(i.img['src'])
+novel = Novel('https://www.neosekaitranslations.com/novel/oresuki/')
+print(novel.get_index_page())
```

## Comparing `neosekai_api-1.0.0.dist-info/LICENSE` & `neosekai_api-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

