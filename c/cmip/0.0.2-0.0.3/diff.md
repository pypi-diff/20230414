# Comparing `tmp/cmip-0.0.2.tar.gz` & `tmp/cmip-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip-0.0.2.tar", last modified: Fri Apr 14 09:40:56 2023, max compression
+gzip compressed data, was "cmip-0.0.3.tar", last modified: Fri Apr 14 09:46:30 2023, max compression
```

## Comparing `cmip-0.0.2.tar` & `cmip-0.0.3.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.349835 cmip-0.0.2/
--rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      493 2023-04-14 09:40:56.348837 cmip-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      113 2022-12-15 09:05:59.000000 cmip-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.312827 cmip-0.0.2/cmip/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.323820 cmip-0.0.2/cmip/data/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/ad.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/chinese_frequency.tsv
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/letter_mapping.txt
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/data/pinyin.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.325819 cmip-0.0.2/cmip/gibberish/
--rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/gibberish/__init__.py
--rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/gibberish/gibberish.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.327819 cmip-0.0.2/cmip/image/
--rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.332821 cmip-0.0.2/cmip/text/
--rw-rw-rw-   0        0        0     2882 2023-04-14 09:40:30.000000 cmip-0.0.2/cmip/text/__init__.py
--rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.2/cmip/text/ac_automation.py
--rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/text/normalize.py
--rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/text/similarity.py
--rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.2/cmip/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.340825 cmip-0.0.2/cmip/web/
--rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.2/cmip/web/__init__.py
--rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.2/cmip/web/html.py
--rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/web/simhash_utils.py
--rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/web/utils.py
--rw-rw-rw-   0        0        0     4037 2023-03-01 10:38:36.000000 cmip-0.0.2/cmip/web/web_scraping.py
--rw-rw-rw-   0        0        0     3294 2023-04-14 09:29:32.000000 cmip-0.0.2/cmip/web/web_scraping2.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.344836 cmip-0.0.2/cmip/word_discover/
--rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/word_discover/__init__.py
--rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/word_discover/ngram.py
--rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.2/cmip/word_discover/word_discover.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.319822 cmip-0.0.2/cmip.egg-info/
--rw-rw-rw-   0        0        0      493 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      741 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 09:40:56.000000 cmip-0.0.2/cmip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 09:40:56.349835 cmip-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-14 09:40:49.000000 cmip-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:40:56.347839 cmip-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.2/test/__init__.py
--rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.2/test/test_ac_automation.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.415552 cmip-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2022-10-27 04:31:09.000000 cmip-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      493 2023-04-14 09:46:30.414546 cmip-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      113 2022-12-15 09:05:59.000000 cmip-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.373023 cmip-0.0.3/cmip/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.384554 cmip-0.0.3/cmip/data/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/data/ad.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/data/chinese_frequency.tsv
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/data/letter_mapping.txt
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/data/pinyin.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.388550 cmip-0.0.3/cmip/gibberish/
+-rw-rw-rw-   0        0        0        0 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/gibberish/__init__.py
+-rw-rw-rw-   0        0        0     2560 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/gibberish/gibberish.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.390547 cmip-0.0.3/cmip/image/
+-rw-rw-rw-   0        0        0     1347 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.397549 cmip-0.0.3/cmip/text/
+-rw-rw-rw-   0        0        0     2882 2023-04-14 09:40:30.000000 cmip-0.0.3/cmip/text/__init__.py
+-rw-rw-rw-   0        0        0     5071 2022-12-15 09:16:49.000000 cmip-0.0.3/cmip/text/ac_automation.py
+-rw-rw-rw-   0        0        0     1755 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/text/normalize.py
+-rw-rw-rw-   0        0        0      555 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/text/similarity.py
+-rw-rw-rw-   0        0        0     2403 2022-10-28 01:23:10.000000 cmip-0.0.3/cmip/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.405546 cmip-0.0.3/cmip/web/
+-rw-rw-rw-   0        0        0      482 2022-10-27 09:02:47.000000 cmip-0.0.3/cmip/web/__init__.py
+-rw-rw-rw-   0        0        0    33944 2023-03-03 05:43:41.000000 cmip-0.0.3/cmip/web/html.py
+-rw-rw-rw-   0        0        0     7136 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/web/simhash_utils.py
+-rw-rw-rw-   0        0        0      777 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/web/utils.py
+-rw-rw-rw-   0        0        0     3302 2023-04-14 09:45:49.000000 cmip-0.0.3/cmip/web/web_scraping.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.410550 cmip-0.0.3/cmip/word_discover/
+-rw-rw-rw-   0        0        0      163 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/word_discover/__init__.py
+-rw-rw-rw-   0        0        0     1864 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/word_discover/ngram.py
+-rw-rw-rw-   0        0        0     7008 2022-10-27 04:31:09.000000 cmip-0.0.3/cmip/word_discover/word_discover.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.379022 cmip-0.0.3/cmip.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-04-14 09:46:30.000000 cmip-0.0.3/cmip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-04-14 09:46:30.000000 cmip-0.0.3/cmip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:46:30.000000 cmip-0.0.3/cmip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-14 09:46:30.000000 cmip-0.0.3/cmip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:46:30.000000 cmip-0.0.3/cmip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:46:30.415552 cmip-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-14 09:46:26.000000 cmip-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:46:30.412548 cmip-0.0.3/test/
+-rw-rw-rw-   0        0        0        0 2022-12-09 06:53:07.000000 cmip-0.0.3/test/__init__.py
+-rw-rw-rw-   0        0        0     1415 2022-12-15 09:05:59.000000 cmip-0.0.3/test/test_ac_automation.py
```

### Comparing `cmip-0.0.2/LICENSE` & `cmip-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/gibberish/gibberish.py` & `cmip-0.0.3/cmip/gibberish/gibberish.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/image/__init__.py` & `cmip-0.0.3/cmip/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/text/__init__.py` & `cmip-0.0.3/cmip/text/__init__.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/text/ac_automation.py` & `cmip-0.0.3/cmip/text/ac_automation.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/text/normalize.py` & `cmip-0.0.3/cmip/text/normalize.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/text/similarity.py` & `cmip-0.0.3/cmip/text/similarity.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/utils.py` & `cmip-0.0.3/cmip/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/web/html.py` & `cmip-0.0.3/cmip/web/html.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/web/simhash_utils.py` & `cmip-0.0.3/cmip/web/simhash_utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/web/utils.py` & `cmip-0.0.3/cmip/web/utils.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/web/web_scraping.py` & `cmip-0.0.3/cmip/web/web_scraping.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,88 @@
 import asyncio
 from playwright.async_api import async_playwright
 import os
 import aiofiles
 from io import BytesIO
 from PIL import Image
-import tqdm
+from tqdm.asyncio import tqdm
 from cmip.web.utils import url2domain, decode_image
 
 
-async def event_handler_save_images(response, save_path) -> None:
+async def event_handler_save_images(response, folder) -> None:
     try:
-        if not response.headers.get("content-type", "").startswith("image"):
-            return
-        if response.headers.get("content-type", "").startswith("image/svg"):
-            return
-        image = await response.body()
-        if len(image) < 200:
-            return
-        file_hash = hash(os.path.basename(response.request.url))
-        check_path = os.path.join(save_path, f"{file_hash}.jpg")
-        if response.request.url.endswith("webp"):
-            byte_stream = BytesIO(image)
-            im = Image.open(byte_stream)
-            im = im.convert("RGB")
-            im.save(check_path)
-        else:
-            async with aiofiles.open(check_path, 'wb') as f:
-                await f.write(image)
+        content_type = response.headers.get("content-type", "")
+        if content_type.startswith("image") and not content_type.startswith("image/svg"):
+            image = await response.body()
+            url = response.request.url
+            if len(image) > 200:
+                file_hash = hash(os.path.basename(url))
+                _path = os.path.join(folder, f"{file_hash}-{len(image)}.jpg")
+                if url.endswith("webp"):
+                    byte_stream = BytesIO(image)
+                    im = Image.open(byte_stream)
+                    im = im.convert("RGB")
+                    im.save(_path)
+                else:
+                    async with aiofiles.open(_path, 'wb') as f:
+                        await f.write(image)
     except Exception as e:
-        print(e)
+        print(f"Error saving image: {response.request.url}, {e}")
 
 
-async def get_web(url, save_path, save_images=True):
-    try:
+async def fetch_url(semaphore, url, folder, save_images=True):
+    async with semaphore:
         async with async_playwright() as p:
-            browser_type = p.chromium
-            browser = await browser_type.launch()
-            page = await browser.new_page()
-            domain = url2domain(url)
-            save_dir = os.path.join(save_path, domain)
-            if not os.path.exists(save_dir):
-                os.makedirs(save_dir)
+            browser = await p.chromium.launch()
+            context = await browser.new_context()
+            page = await context.new_page()
             if save_images:
                 page.on("response", lambda response: asyncio.create_task(
-                    event_handler_save_images(response, save_dir)))
-            await page.goto(url, timeout=0)
-            await page.wait_for_timeout(10000)
-            # await page.wait_for_load_state("load")
-            await page.reload(wait_until="networkidle")
-            html = await page.content()
-            async with aiofiles.open(os.path.join(save_path, domain, "dynamic.html"), 'w', encoding='utf-8') as f:
-                await f.write(html)
-            images = await page.query_selector_all('img')
-            for idx, src in enumerate(
-                    set([await page.evaluate('(element) => element.src', image) for image in images])):
-                if src.startswith("data:image"):
-                    async with aiofiles.open(os.path.join(save_path, domain, f"{idx}.jpg"), 'wb') as f:
-                        await f.write(decode_image(src))
-            # await page.screenshot(path=f'example-{browser_type.name}.png', full_page=True)
-            await page.wait_for_load_state("domcontentloaded")
-            await page.wait_for_load_state("networkidle")
-            await browser.close()
-    except Exception as e:
-        # await browser.close()
-        print(">>", e)
-        return
-
-
-def web_scraping(urls, save_path, batch_size=4, save_images=True):
-
-    for _ in tqdm.tqdm(range(len(urls) // batch_size + 1), total=len(urls) // batch_size + 1, desc="Crawler Batchs:"):
-        batch = urls[:batch_size]
-        async def m(batch):
-            await asyncio.gather(*[get_web(url, save_path, save_images) for url in batch])
-        asyncio.run(m(batch))
-        urls = urls[batch_size:]
-
-
-if __name__ == '__main__':
-
-    urls = ["https://baidu.com", "https://qq.com"]
-
-    outdir = r"C:\data\家庭高危域名20230227"
-    urls = []
-    with open(r"C:\data\家庭下高危域名0227.txt", 'r', encoding='utf-8') as f:
-        for line in f:
-            line = line.strip()
-            if os.path.exists(os.path.join(outdir, line, "dynamic.html")):
-                # continue
-                pass
-            if not line.startswith("http"):
-                line = "http://" + line
-                urls.append(line)
-    print("域名数量：", len(urls))
-
-    for i in range(3):
-        if i == 0:
-            _urls = urls
-        else:
-            _urls = urls
-        web_scraping(_urls, outdir, batch_size=10, save_images=(i % 2 == 0))
+                    event_handler_save_images(response, folder)))
+            try:
+                await page.goto(url, wait_until="networkidle")
+                content = await page.content()
+
+                async with aiofiles.open(f"{folder}/dynamic.html", "w", encoding="utf-8") as f:
+                    await f.write(content)
+
+                images = await page.query_selector_all('img')
+                for idx, src in enumerate(
+                        set([await page.evaluate('(element) => element.src', image) for image in images])):
+                    if src.startswith("data:image"):
+                        async with aiofiles.open(os.path.join(folder, f"{idx}.jpg"), 'wb') as f:
+                            await f.write(decode_image(src))
+
+            except Exception as e:
+                print(f"Error fetching URL: {url}, {e}")
+
+            finally:
+                await page.close()
+                await context.close()
+                await browser.close()
+
+
+async def web_scraping(urls, max_concurrent_tasks=10):
+    semaphore = asyncio.Semaphore(max_concurrent_tasks)
+
+    tasks = []
+    for i, url in enumerate(urls):
+        folder = f"output/{url2domain(url)}"
+        os.makedirs(folder, exist_ok=True)
+        tasks.append(fetch_url(semaphore, url, folder))
 
+    try:
+        for result in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Fetching URLs"):
+            await result
+    except Exception as e:
+        print(f"Error in main: {e}")
+    finally:
+        await semaphore.acquire()
 
 
+if __name__ == "__main__":
+    urls = [
+        "https://baidu.com",
+        "https://qq.com",
+        # ...更多的URL
+    ]
+    asyncio.run(web_scraping(urls))
```

### Comparing `cmip-0.0.2/cmip/word_discover/ngram.py` & `cmip-0.0.3/cmip/word_discover/ngram.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip/word_discover/word_discover.py` & `cmip-0.0.3/cmip/word_discover/word_discover.py`

 * *Files identical despite different names*

### Comparing `cmip-0.0.2/cmip.egg-info/SOURCES.txt` & `cmip-0.0.3/cmip.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,13 +20,12 @@
 cmip/text/normalize.py
 cmip/text/similarity.py
 cmip/web/__init__.py
 cmip/web/html.py
 cmip/web/simhash_utils.py
 cmip/web/utils.py
 cmip/web/web_scraping.py
-cmip/web/web_scraping2.py
 cmip/word_discover/__init__.py
 cmip/word_discover/ngram.py
 cmip/word_discover/word_discover.py
 test/__init__.py
 test/test_ac_automation.py
```

### Comparing `cmip-0.0.2/setup.py` & `cmip-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cmip",
-    version="0.0.2",
+    version="0.0.3",
     author="geb",
     author_email="853934146@qq.com",
     description="An efficient information processing program.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikuh/cmip",
     packages=setuptools.find_packages(),
```

### Comparing `cmip-0.0.2/test/test_ac_automation.py` & `cmip-0.0.3/test/test_ac_automation.py`

 * *Files identical despite different names*

