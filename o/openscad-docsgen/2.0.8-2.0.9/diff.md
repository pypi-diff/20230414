# Comparing `tmp/openscad_docsgen-2.0.8-py2.py3-none-any.whl.zip` & `tmp/openscad_docsgen-2.0.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 28675 bytes, number of entries: 16
+Zip file size: 28638 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     5681 b- defN 21-Dec-17 05:46 openscad_docsgen/__init__.py
--rw-r--r--  2.0 unx    31548 b- defN 21-Dec-17 05:46 openscad_docsgen/blocks.py
+-rw-r--r--  2.0 unx    31294 b- defN 21-Dec-24 01:07 openscad_docsgen/blocks.py
 -rw-r--r--  2.0 unx     1213 b- defN 21-Dec-17 05:46 openscad_docsgen/errorlog.py
 -rw-r--r--  2.0 unx     8904 b- defN 21-Dec-17 05:46 openscad_docsgen/imagemanager.py
 -rw-r--r--  2.0 unx     6282 b- defN 21-Dec-17 05:46 openscad_docsgen/mdimggen.py
--rw-r--r--  2.0 unx    43409 b- defN 21-Dec-19 02:59 openscad_docsgen/parser.py
+-rw-r--r--  2.0 unx    43123 b- defN 21-Dec-24 00:42 openscad_docsgen/parser.py
 -rw-r--r--  2.0 unx      303 b- defN 21-Dec-17 05:46 openscad_docsgen/target.py
 -rw-r--r--  2.0 unx     1552 b- defN 21-Dec-17 05:46 openscad_docsgen/target_githubwiki.py
 -rw-r--r--  2.0 unx     5615 b- defN 21-Dec-17 05:46 openscad_docsgen/target_wiki.py
 -rw-r--r--  2.0 unx      430 b- defN 21-Dec-17 05:46 openscad_docsgen/utils.py
--rw-r--r--  2.0 unx     1070 b- defN 21-Dec-19 03:11 openscad_docsgen-2.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     9061 b- defN 21-Dec-19 03:11 openscad_docsgen-2.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Dec-19 03:11 openscad_docsgen-2.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx      120 b- defN 21-Dec-19 03:11 openscad_docsgen-2.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 21-Dec-19 03:11 openscad_docsgen-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1394 b- defN 21-Dec-19 03:11 openscad_docsgen-2.0.8.dist-info/RECORD
-16 files, 116709 bytes uncompressed, 26357 bytes compressed:  77.4%
+-rw-r--r--  2.0 unx     1070 b- defN 21-Dec-24 01:10 openscad_docsgen-2.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9061 b- defN 21-Dec-24 01:10 openscad_docsgen-2.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 21-Dec-24 01:10 openscad_docsgen-2.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx      120 b- defN 21-Dec-24 01:10 openscad_docsgen-2.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 21-Dec-24 01:10 openscad_docsgen-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1394 b- defN 21-Dec-24 01:10 openscad_docsgen-2.0.9.dist-info/RECORD
+16 files, 116169 bytes uncompressed, 26320 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: openscad_docsgen/target_wiki.py
 Comment: 
 
 Filename: openscad_docsgen/utils.py
 Comment: 
 
-Filename: openscad_docsgen-2.0.8.dist-info/LICENSE
+Filename: openscad_docsgen-2.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: openscad_docsgen-2.0.8.dist-info/METADATA
+Filename: openscad_docsgen-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: openscad_docsgen-2.0.8.dist-info/WHEEL
+Filename: openscad_docsgen-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: openscad_docsgen-2.0.8.dist-info/entry_points.txt
+Filename: openscad_docsgen-2.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: openscad_docsgen-2.0.8.dist-info/top_level.txt
+Filename: openscad_docsgen-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: openscad_docsgen-2.0.8.dist-info/RECORD
+Filename: openscad_docsgen-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openscad_docsgen/blocks.py

```diff
@@ -291,21 +291,21 @@
 
     def get_tocfile_lines(self, target, n=1, currfile=""):
         sections = [
             sect for sect in self.children
             if isinstance(sect, SectionBlock)
         ]
         link = self.get_link(target, label=self.subtitle, currfile=currfile)
-        out = target.horizontal_rule()
+        out = []
         out.extend(target.header("{}. {}".format(n, link), lev=target.SECTION, esc=False))
         if self.summary:
             out.append(self.summary)
         if self.footnotes:
             for mark, note in self.footnotes:
-                out.append(target.italics(note))
+                out.append(target.line_with_break(target.italics(note)))
         out.extend(target.bullet_list_start())
         for n, sect in enumerate(sections):
             out.extend(sect.get_tocfile_lines(target, n=n+1, currfile=currfile))
         out.extend(target.bullet_list_end())
         return out
 
     def get_toc_lines(self, target, n=1, currfile=""):
@@ -322,26 +322,24 @@
 
     def get_cheatsheet_lines(self, controller, target):
         lines = []
         for child in self.get_children_by_title("Section"):
             lines.extend(child.get_cheatsheet_lines(controller, target))
         out = []
         if lines:
-            out.extend(target.horizontal_rule())
             out.extend(target.header("{}: {}".format(self.title, self.subtitle), lev=target.SUBSECTION))
             out.extend(lines)
         return out
 
     def get_file_lines(self, controller, target):
         out = target.header(str(self), lev=target.FILE)
         out.extend(target.markdown_block(self.get_markdown_body(controller, target)))
         for child in self.children:
             if not isinstance(child, SectionBlock):
                 out.extend(child.get_file_lines(controller, target))
-        out.extend(target.horizontal_rule())
         out.extend(target.header("Table of Contents", lev=target.SECTION))
         out.extend(self.get_toc_lines(target, currfile=self.origin.file))
         for child in self.children:
             if isinstance(child, SectionBlock):
                 out.extend(child.get_file_lines(controller, target))
         return out
 
@@ -382,15 +380,15 @@
         Return the markdown table of contents lines for the children in this
         section. This is returned as a series of bullet points.
         `indent` sets the level of indentation for the bullet points
         """
         out = []
         if self.subtitle:
             item = self.get_link(target, label=self.subtitle, currfile=currfile)
-            out.extend(target.bullet_list_item(item))
+            out.extend(target.bullet_list_item(target.line_with_break(item)))
             subsects = self.get_children_by_title("Subsection")
             if subsects:
                 out.extend(target.bullet_list_start())
                 for child in subsects:
                     out.extend(target.indent_lines(child.get_tocfile_lines(target, currfile=currfile)))
                 out.extend(target.bullet_list_end())
             out.extend(
@@ -466,15 +464,14 @@
 
     def get_file_lines(self, controller, target):
         """
         Return the markdown for this section. This includes the section
         heading and the markdown for the children.
         """
         out = []
-        out.extend(target.horizontal_rule())
         if self.subtitle:
             out.extend(target.header(str(self), lev=target.SECTION))
             out.extend(target.markdown_block(self.get_markdown_body(controller, target)))
         for child in self.children:
             out.extend(child.get_file_lines(controller, target))
         return out
 
@@ -558,24 +555,19 @@
 
     def get_file_lines(self, controller, target):
         """
         Return the markdown for this section. This includes the section
         heading and the markdown for the children.
         """
         out = []
-        out.extend(target.horizontal_rule())
         if self.subtitle:
             out.extend(target.header(str(self), lev=target.SUBSECTION))
             out.extend(target.markdown_block(self.get_markdown_body(controller, target)))
-        chout = []
         for child in self.children:
-            if chout:
-                chout.extend(target.horizontal_rule())
-            chout.extend(child.get_file_lines(controller, target))
-        out.extend(chout)
+            out.extend(child.get_file_lines(controller, target))
         return out
 
 
 class ItemBlock(LabelBlock):
     _paren_pat = re.compile(r'\([^\)]+\)')
 
     def __init__(self, title, subtitle, body, origin, parent=None):
@@ -672,19 +664,20 @@
             ["Topics"],
             ["Usage"]
         ]
         back_blocks = [
             ["See Also"],
             ["Example"]
         ]
+        children = self.sort_children(front_blocks, back_blocks)
         out = []
-        out.extend(target.horizontal_rule())
         out.extend(target.header(str(self), lev=target.ITEM))
-        for child in self.sort_children(front_blocks, back_blocks):
+        for child in children:
             out.extend(child.get_file_lines(controller, target))
+        out.extend(target.horizontal_rule())
         return out
 
 
 class ImageBlock(GenericBlock):
     def __init__(self, title, subtitle, body, origin, parent=None, meta=""):
         super().__init__(title, subtitle, body, origin, parent=parent)
         fileblock = parent
```

## openscad_docsgen/parser.py

```diff
@@ -734,15 +734,14 @@
         for fblock in prifiles:
             if not fblock.group and fblock.group not in groups:
                 groups.append(fblock.group)
 
         footmarks = []
         footnotes = {}
         out = target.header("Table of Contents")
-        out.extend(target.horizontal_rule())
         out.extend(target.header("List of Files", lev=target.SECTION))
         for group in groups:
             out.extend(target.block_header(group if group else "Miscellaneous"))
             out.extend(target.bullet_list_start())
             for fnum, fblock in enumerate(prifiles):
                 if fblock.group != group:
                     continue
@@ -760,15 +759,14 @@
                         footnotes[mark] = note
                     elif note != footnotes[mark]:
                         raise DocsGenException("FileFootnotes", 'Footnote "{}" conflicts with previous definition "{}", while declaring block:'.format(note, footnotes[mark]))
             out.extend(target.bullet_list_end())
 
         if footmarks:
             out.append("")
-            out.extend(target.horizontal_rule())
             out.extend(target.header("File Footnotes:", lev=target.SUBSECTION))
             for mark in footmarks:
                 out.append("{} = {}  ".format(mark, note))
             out.append("")
 
         for fnum, fblock in enumerate(prifiles):
             out.extend(fblock.get_tocfile_lines(self.opts.target, n=fnum+1, currfile=self.TOCFILE))
@@ -822,15 +820,14 @@
                     )
                 )
                 for ltr in ltrs_found
             )
         )
         for ltr in ltrs_found:
             topics = sorted(index_by_letter[ltr].keys())
-            out.extend(target.horizontal_rule())
             out.extend(target.header(ltr, lev=target.SUBSECTION))
             for topic in topics:
                 itemlist = index_by_letter[ltr][topic]
                 out.extend(target.header(topic, lev=target.ITEM))
                 out.extend(target.bullet_list_start())
                 sorted_items = sorted(itemlist, key=lambda x: x[0].lower())
                 for name, item in sorted_items:
@@ -890,15 +887,14 @@
             items = [
                 "{} (in {})".format(
                     item.get_link(target, label=name, currfile=self.INDEXFILE),
                     target.escape_entities(item.origin.file)
                 )
                 for name, item in index_by_letter[ltr]
             ]
-            out.extend(target.horizontal_rule())
             out.extend(target.header(ltr, lev=target.SUBSECTION))
             out.extend(target.bullet_list(items))
 
         out = target.postprocess(out)
         outfile = os.path.join(target.docs_dir, self.INDEXFILE)
         if not self.quiet:
             print("Writing {}...".format(outfile))
@@ -945,15 +941,14 @@
         out = []
         out.extend(target.line_with_break(target.get_link("Table of Contents", file="TOC", literalize=False)))
         out.extend(target.line_with_break(target.get_link("Function Index", file="Index", literalize=False)))
         out.extend(target.line_with_break(target.get_link("Topics Index", file="Topics", literalize=False)))
         out.extend(target.line_with_break(target.get_link("Cheat Sheet", file="CheatSheet", literalize=False)))
         out.extend(target.line_with_break(target.get_link("Tutorials", file="Tutorials", literalize=False)))
         out.extend(target.paragraph())
-        out.extend(target.horizontal_rule())
         out.extend(target.header("List of Files:", lev=target.SUBSECTION))
         for group in groups:
             out.extend(target.block_header(group if group else "Miscellaneous"))
             out.extend(target.bullet_list_start())
             for fnum, fblock in enumerate(prifiles):
                 if fblock.group != group:
                     continue
@@ -967,15 +962,14 @@
                     elif note != footnotes[mark]:
                         raise DocsGenException("FileFootnotes", 'Footnote "{}" conflicts with previous definition "{}", while declaring block:'.format(note, footnotes[mark]))
                 marks = target.footnote_marks(fblock.footnotes)
                 out.extend(target.bullet_list_item("{}{}".format(link, marks)))
             out.extend(target.bullet_list_end())
         if footmarks:
             out.append("")
-            out.extend(target.horizontal_rule())
             out.extend(target.header("File Footnotes:", lev=target.SUBSECTION))
             for mark in footmarks:
                 out.append("{} = {}  ".format(mark, note))
 
         out = target.postprocess(out)
         outfile = os.path.join(target.docs_dir, self.SIDEBARFILE)
         if not self.quiet:
```

## Comparing `openscad_docsgen-2.0.8.dist-info/LICENSE` & `openscad_docsgen-2.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openscad_docsgen-2.0.8.dist-info/METADATA` & `openscad_docsgen-2.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openscad-docsgen
-Version: 2.0.8
+Version: 2.0.9
 Summary: A processor to generate Markdown code documentation with images from OpenSCAD source comments.
 Home-page: https://github.com/revarbat/openscad_docsgen
 Author: Revar Desmera
 Author-email: revarbat@gmail.com
 License: MIT License
-Download-URL: https://github.com/revarbat/openscad_docsgen/archive/refs/tags/v2.0.8.zip
+Download-URL: https://github.com/revarbat/openscad_docsgen/archive/refs/tags/v2.0.9.zip
 Keywords: openscad documentation generation docsgen
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `openscad_docsgen-2.0.8.dist-info/RECORD` & `openscad_docsgen-2.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 openscad_docsgen/__init__.py,sha256=6aT-hgbUxkkhbifspvdpPSnrIrxIcAhviupTgC4sfeg,5681
-openscad_docsgen/blocks.py,sha256=pCTUTaMtOrhQ8TrCljXaafTg4WkbpmUb4VtewmH32Cs,31548
+openscad_docsgen/blocks.py,sha256=PhLbbm-hgg9learjZ6smeOKYdoLp6SepwI1YhuaaH9s,31294
 openscad_docsgen/errorlog.py,sha256=tFJzJWdZM-8lL3esjanAgHMa5is3Pvx_4ztuVbS3pak,1213
 openscad_docsgen/imagemanager.py,sha256=NWXBjtaHQW1z3TDL8GSz2BeuysP8KXXJz0jYm1UtukQ,8904
 openscad_docsgen/mdimggen.py,sha256=5eC5SFJFha5wHVQ6XVWG8j_qZ8TAqnobTVgsO3pilro,6282
-openscad_docsgen/parser.py,sha256=siCPSl43N5PiCH__kYZz5ioKIt1UiGCQGRAOcWRCaRo,43409
+openscad_docsgen/parser.py,sha256=k5NBaR3OJghzyKxCd6AHmem80AZtJgHiho8_zdBPM08,43123
 openscad_docsgen/target.py,sha256=a9ec_T_NBrrJONsY8AbOMdJjPtda_oiLcqxQIby1pZY,303
 openscad_docsgen/target_githubwiki.py,sha256=qR8O6CGC6NdBtjsFMLzfBnZ3gyvyqDh6kOTAnck1Yjg,1552
 openscad_docsgen/target_wiki.py,sha256=a_fs2BiL9U1SJELNKOGrQ7JIXIKMVNkRUrzcuZS7z4U,5615
 openscad_docsgen/utils.py,sha256=HtDKAWPZQHsU_8OAzuKLPhhOwVaE4Ae0PvEGfztlVHU,430
-openscad_docsgen-2.0.8.dist-info/LICENSE,sha256=Kpd8exhkGr8Mb2-aJCA3DZsMP1skw3U0YM0pmwDFUa4,1070
-openscad_docsgen-2.0.8.dist-info/METADATA,sha256=sN5-gfCuX01DbF3jt_X1QRg_xk3WzrliPSvJhH0aRjk,9061
-openscad_docsgen-2.0.8.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-openscad_docsgen-2.0.8.dist-info/entry_points.txt,sha256=DH3j9GsSpbTD2Cs0GHfehzpYQckSHA71UGxaWykPBcI,120
-openscad_docsgen-2.0.8.dist-info/top_level.txt,sha256=Ek1A_Y8Pb7oXosDSeQkKEWknK_WcvJplKjBf_QfjEik,17
-openscad_docsgen-2.0.8.dist-info/RECORD,,
+openscad_docsgen-2.0.9.dist-info/LICENSE,sha256=Kpd8exhkGr8Mb2-aJCA3DZsMP1skw3U0YM0pmwDFUa4,1070
+openscad_docsgen-2.0.9.dist-info/METADATA,sha256=WfstmOrQARaYB7tFOTiELE4VXiDj0uQ_pjiNncDTzuE,9061
+openscad_docsgen-2.0.9.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+openscad_docsgen-2.0.9.dist-info/entry_points.txt,sha256=DH3j9GsSpbTD2Cs0GHfehzpYQckSHA71UGxaWykPBcI,120
+openscad_docsgen-2.0.9.dist-info/top_level.txt,sha256=Ek1A_Y8Pb7oXosDSeQkKEWknK_WcvJplKjBf_QfjEik,17
+openscad_docsgen-2.0.9.dist-info/RECORD,,
```

