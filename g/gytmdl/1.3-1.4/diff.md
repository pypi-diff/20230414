# Comparing `tmp/gytmdl-1.3.tar.gz` & `tmp/gytmdl-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gytmdl-1.3.tar", last modified: Sun Mar 19 19:09:22 2023, max compression
+gzip compressed data, was "gytmdl-1.4.tar", last modified: Fri Apr 14 01:29:31 2023, max compression
```

## Comparing `gytmdl-1.3.tar` & `gytmdl-1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1176 2023-03-19 19:09:18.676307 gytmdl-1.3/.github/workflows/main.yml
--rw-r--r--   0        0        0       80 2023-03-19 19:09:18.676307 gytmdl-1.3/.gitignore
--rw-r--r--   0        0        0     2350 2023-03-19 19:09:18.676307 gytmdl-1.3/README.md
--rw-r--r--   0        0        0     4177 2023-03-19 19:09:18.676307 gytmdl-1.3/gytmdl/__init__.py
--rw-r--r--   0        0        0       63 2023-03-19 19:09:18.676307 gytmdl-1.3/gytmdl/__main__.py
--rw-r--r--   0        0        0     6704 2023-03-19 19:09:18.676307 gytmdl-1.3/gytmdl/gytmdl.py
--rw-r--r--   0        0        0      456 2023-03-19 19:09:18.676307 gytmdl-1.3/pyproject.toml
--rw-r--r--   0        0        0       18 2023-03-19 19:09:18.676307 gytmdl-1.3/requirements.txt
--rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 gytmdl-1.3/PKG-INFO
+-rw-r--r--   0        0        0     1176 2023-04-14 01:29:26.637009 gytmdl-1.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0       80 2023-04-14 01:29:26.637009 gytmdl-1.4/.gitignore
+-rw-r--r--   0        0        0     2350 2023-04-14 01:29:26.637009 gytmdl-1.4/README.md
+-rw-r--r--   0        0        0     4145 2023-04-14 01:29:26.637009 gytmdl-1.4/gytmdl/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-14 01:29:26.637009 gytmdl-1.4/gytmdl/__main__.py
+-rw-r--r--   0        0        0     6713 2023-04-14 01:29:26.637009 gytmdl-1.4/gytmdl/gytmdl.py
+-rw-r--r--   0        0        0      456 2023-04-14 01:29:26.637009 gytmdl-1.4/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-04-14 01:29:26.637009 gytmdl-1.4/requirements.txt
+-rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 gytmdl-1.4/PKG-INFO
```

### Comparing `gytmdl-1.3/.github/workflows/main.yml` & `gytmdl-1.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gytmdl-1.3/README.md` & `gytmdl-1.4/README.md`

 * *Files identical despite different names*

### Comparing `gytmdl-1.3/gytmdl/__init__.py` & `gytmdl-1.4/gytmdl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,96 +1,96 @@
 import shutil
 import argparse
 import traceback
 from .gytmdl import Gytmdl
 
-__version__ = '1.3'
+__version__ = '1.4'
 
 
 def main():
     if not shutil.which('ffmpeg'):
         raise Exception('ffmpeg is not on PATH')
     parser = argparse.ArgumentParser(
-        description = 'Download YouTube Music songs/albums/playlists with tags from YouTube Music',
-        formatter_class = argparse.ArgumentDefaultsHelpFormatter
+        description='Download YouTube Music songs/albums/playlists with tags from YouTube Music',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument(
         'url',
         help='YouTube Music song/album/playlist URL(s)',
         nargs='*',
-        metavar='<url>'
+        metavar='<url>',
     )
     parser.add_argument(
         '-u',
         '--urls-txt',
-        help = 'Read URLs from a text file',
-        nargs = '?'
+        help='Read URLs from a text file',
+        nargs='?',
     )
     parser.add_argument(
         '-t',
         '--temp-path',
-        default = 'temp',
-        help = 'Temp path'
+        default='temp',
+        help='Temp path',
     )
     parser.add_argument(
         '-f',
         '--final-path',
-        default = 'YouTube Music',
-        help = 'Final path'
+        default='YouTube Music',
+        help='Final path',
     )
     parser.add_argument(
         '-c',
         '--cookies-location',
-        default = 'cookies.txt',
-        help = 'Cookies location'
+        default='cookies.txt',
+        help='Cookies location',
     )
     parser.add_argument(
         '-i',
         '--itag',
-        default = '140',
-        help = 'itag (quality). Can be 141 (256kbps AAC, requires cookies), 251 (128kbps Opus) or 140 (128kbps AAC)',
-        choices = ['141', '251', '140']
+        default='140',
+        help='itag (quality). Can be 141 (256kbps AAC, requires cookies), 251 (128kbps Opus) or 140 (128kbps AAC)',
+        choices=['141', '251', '140'],
     )
     parser.add_argument(
         '-o',
         '--overwrite',
-        action = 'store_true',
-        help = 'Overwrite existing files'
+        action='store_true',
+        help='Overwrite existing files',
     )
     parser.add_argument(
         '-s',
         '--skip-cleanup',
-        action = 'store_true',
-        help = 'Skip cleanup'
+        action='store_true',
+        help='Skip cleanup',
     )
     parser.add_argument(
         '-e',
         '--print-exceptions',
-        action = 'store_true',
-        help = 'Print exceptions'
+        action='store_true',
+        help='Print exceptions',
     )
     parser.add_argument(
         '-v',
         '--version',
-        action = 'version',
-        version = f'%(prog)s {__version__}'
+        action='version',
+        version=f'%(prog)s {__version__}',
     )
     args = parser.parse_args()
     dl = Gytmdl(
         args.cookies_location,
         args.itag,
         args.final_path,
         args.temp_path,
         args.overwrite,
-        args.skip_cleanup
+        args.skip_cleanup,
     )
     if not args.url and not args.urls_txt:
         parser.error('you must specify an url or a text file using -u/--urls-txt.')
     if args.urls_txt:
-        with open(args.urls_txt, 'r', encoding = 'utf8') as f:
+        with open(args.urls_txt, 'r', encoding='utf8') as f:
             args.url = f.read().splitlines()
     download_queue = []
     error_count = 0
     for i, url in enumerate(args.url):
         try:
             download_queue.append(dl.get_download_queue(url.strip()))
         except KeyboardInterrupt:
```

### Comparing `gytmdl-1.3/gytmdl/gytmdl.py` & `gytmdl-1.4/gytmdl/gytmdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     
 
     @functools.lru_cache()
     def get_ydl_extract_info(self, url):
         ydl_opts = {
             'quiet': True,
             'no_warnings': True,
-            'extract_flat': True
+            'extract_flat': True,
         }
         if self.cookies_location.exists():
             ydl_opts['cookiefile'] = str(self.cookies_location)
         with YoutubeDL(ydl_opts) as ydl:
-            return ydl.extract_info(url, download = False)
+            return ydl.extract_info(url, download=False)
     
 
     def get_download_queue(self, url):
+        url = url.split('&')[0]
         download_info = []
         ydl_extract_info = self.get_ydl_extract_info(url)
         if not 'youtube' in ydl_extract_info['webpage_url']:
             raise Exception('Not a YouTube URL')
         if 'MPREb_' in ydl_extract_info['webpage_url_basename']:
             ydl_extract_info = self.get_ydl_extract_info(ydl_extract_info['url'])
         if 'playlist' in ydl_extract_info['webpage_url_basename']:
@@ -81,17 +82,17 @@
         video_id = ytmusic_watch_playlist['tracks'][0]['videoId']
         ytmusic_album = self.ytmusic.get_album(ytmusic_watch_playlist['tracks'][0]['album']['id'])
         tags = {
             '\xa9alb': [ytmusic_album['title']],
             'aART': [self.get_artist(ytmusic_album['artists'])],
             '\xa9ART': [self.get_artist(ytmusic_watch_playlist['tracks'][0]['artists'])],
             '\xa9cmt': [f'https://music.youtube.com/watch?v={video_id}'],
-            'covr': [MP4Cover(self.get_cover(f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}=w600'), MP4Cover.FORMAT_JPEG)],
+            'covr': [MP4Cover(self.get_cover(f'{ytmusic_watch_playlist["tracks"][0]["thumbnail"][0]["url"].split("=")[0]}=w600'))],
             '\xa9nam': [ytmusic_watch_playlist['tracks'][0]['title']],
-            'stik': [1]
+            'stik': [1],
         }
         if ytmusic_album.get('year'):
             tags['\xa9day'] = [ytmusic_album['year']]
         if ytmusic_watch_playlist['lyrics']:
             lyrics = self.ytmusic.get_lyrics(ytmusic_watch_playlist['lyrics'])['lyrics']        
             if lyrics is not None:
                 tags['\xa9lyr'] = [lyrics]
@@ -136,48 +137,48 @@
     def download(self, video_id, temp_location):
         ydl_opts = {
             'quiet': True,
             'no_warnings': True,
             'overwrites': self.overwrite,
             'fixup': 'never',
             'format': self.itag,
-            'outtmpl': str(temp_location)
+            'outtmpl': str(temp_location),
         }
         if self.cookies_location.exists():
             ydl_opts['cookiefile'] = str(self.cookies_location)
         with YoutubeDL(ydl_opts) as ydl:
             ydl.download('music.youtube.com/watch?v=' + video_id) 
     
 
     def fixup(self, temp_location, fixed_location):
         fixup = [
             'ffmpeg',
             '-loglevel',
             'error',
             '-i',
-            temp_location
+            temp_location,
         ]
         if self.itag == '251':
             fixup.extend([
                 '-f',
-                'mp4'
+                'mp4',
             ])
         subprocess.run(
             [
                 *fixup,
                 '-c',
                 'copy',
-                fixed_location
+                fixed_location,
             ],
-            check = True
+            check=True,
         )
     
 
     def make_final(self, final_location, fixed_location, tags):
-        final_location.parent.mkdir(parents = True, exist_ok = True)
+        final_location.parent.mkdir(parents=True, exist_ok=True)
         shutil.copy(fixed_location, final_location)
         file = MP4(final_location)
         file.clear()
         file.update(tags)
         file.save(final_location)
```

### Comparing `gytmdl-1.3/PKG-INFO` & `gytmdl-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gytmdl
-Version: 1.3
+Version: 1.4
 Summary: Download YouTube Music songs/albums/playlists with tags from YouTube Music
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: yt-dlp
 Requires-Dist: ytmusicapi
 Project-URL: repository, https://github.com/glomatico/gytmdl
```

