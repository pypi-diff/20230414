# Comparing `tmp/sbb_binarization-0.0.9.tar.gz` & `tmp/sbb_binarization-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbb_binarization-0.0.9.tar", last modified: Tue Apr 26 09:29:04 2022, max compression
+gzip compressed data, was "sbb_binarization-0.1.0.tar", last modified: Fri Apr 14 14:11:44 2023, max compression
```

## Comparing `sbb_binarization-0.0.9.tar` & `sbb_binarization-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kba       (1000) docker     (114)        0 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/
--rw-rw-r--   0 kba       (1000) docker     (114)    11357 2021-03-16 15:03:39.000000 sbb_binarization-0.0.9/LICENSE
--rw-rw-r--   0 kba       (1000) docker     (114)     1731 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/PKG-INFO
--rw-rw-r--   0 kba       (1000) docker     (114)     1404 2022-04-26 09:08:00.000000 sbb_binarization-0.0.9/README.md
-drwxrwxr-x   0 kba       (1000) docker     (114)        0 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/
--rw-rw-r--   0 kba       (1000) docker     (114)     1731 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) docker     (114)      395 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) docker     (114)        1 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) docker     (114)      102 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/entry_points.txt
--rw-rw-r--   0 kba       (1000) docker     (114)       86 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) docker     (114)       13 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarization.egg-info/top_level.txt
-drwxrwxr-x   0 kba       (1000) docker     (114)        0 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/sbb_binarize/
--rw-rw-r--   0 kba       (1000) docker     (114)       26 2021-03-16 15:03:39.000000 sbb_binarization-0.0.9/sbb_binarize/__init__.py
--rw-rw-r--   0 kba       (1000) docker     (114)      585 2021-03-16 15:03:39.000000 sbb_binarization-0.0.9/sbb_binarize/cli.py
--rw-rw-r--   0 kba       (1000) docker     (114)     1006 2022-04-26 09:25:12.000000 sbb_binarization-0.0.9/sbb_binarize/ocrd-tool.json
--rw-rw-r--   0 kba       (1000) docker     (114)     7590 2022-04-26 09:08:00.000000 sbb_binarization-0.0.9/sbb_binarize/ocrd_cli.py
--rw-rw-r--   0 kba       (1000) docker     (114)    12018 2022-04-26 09:08:00.000000 sbb_binarization-0.0.9/sbb_binarize/sbb_binarize.py
--rw-rw-r--   0 kba       (1000) docker     (114)       38 2022-04-26 09:29:04.000000 sbb_binarization-0.0.9/setup.cfg
--rw-rw-r--   0 kba       (1000) docker     (114)      969 2021-03-16 15:03:39.000000 sbb_binarization-0.0.9/setup.py
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-14 14:11:44.837093 sbb_binarization-0.1.0/
+-rw-rw-r--   0 kba       (1000) kba       (1000)    11357 2021-03-16 15:03:39.000000 sbb_binarization-0.1.0/LICENSE
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3300 2023-04-14 14:11:44.837093 sbb_binarization-0.1.0/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2993 2023-04-14 14:10:07.000000 sbb_binarization-0.1.0/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-14 14:11:44.837093 sbb_binarization-0.1.0/sbb_binarization.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3300 2023-04-14 14:11:44.000000 sbb_binarization-0.1.0/sbb_binarization.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)      395 2023-04-14 14:11:44.000000 sbb_binarization-0.1.0/sbb_binarization.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2023-04-14 14:11:44.000000 sbb_binarization-0.1.0/sbb_binarization.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)      101 2023-04-14 14:11:44.000000 sbb_binarization-0.1.0/sbb_binarization.egg-info/entry_points.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       75 2023-04-14 14:11:44.000000 sbb_binarization-0.1.0/sbb_binarization.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       13 2023-04-14 14:11:44.000000 sbb_binarization-0.1.0/sbb_binarization.egg-info/top_level.txt
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2023-04-14 14:11:44.837093 sbb_binarization-0.1.0/sbb_binarize/
+-rw-rw-r--   0 kba       (1000) kba       (1000)       26 2021-03-16 15:03:39.000000 sbb_binarization-0.1.0/sbb_binarize/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      509 2023-04-14 14:10:07.000000 sbb_binarization-0.1.0/sbb_binarize/cli.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     1851 2023-04-14 14:11:12.000000 sbb_binarization-0.1.0/sbb_binarize/ocrd-tool.json
+-rw-rw-r--   0 kba       (1000) kba       (1000)     7715 2023-04-14 14:10:07.000000 sbb_binarization-0.1.0/sbb_binarize/ocrd_cli.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    11325 2023-04-14 14:10:07.000000 sbb_binarization-0.1.0/sbb_binarize/sbb_binarize.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2023-04-14 14:11:44.841093 sbb_binarization-0.1.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      968 2023-04-14 14:10:07.000000 sbb_binarization-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sbb_binarization-0.0.9/LICENSE` & `sbb_binarization-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbb_binarization-0.0.9/sbb_binarize/ocrd-tool.json` & `sbb_binarization-0.1.0/sbb_binarize/ocrd-tool.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8227864583333333%*

 * *Differences: {"'tools'": "{'ocrd-sbb-binarize': {'parameters': {'model': {'description': 'Directory containing "*

 * *            'HDF5 or SavedModel/ProtoBuf models. Can be an absolute path or a path relative to the '*

 * *            'OCR-D resource location, the current working directory or the $SBB_BINARIZE_DATA '*

 * *            "environment variable (if set)'}}, 'resources': [OrderedDict([('url', "*

 * *            "'https://github.com/qurator-spk/sbb_binarization/releases/download/v0.0.11/saved_model_2020_01_16.zip'), "*

 * *            […]*

```diff
@@ -8,29 +8,47 @@
             "description": "Pixelwise binarization with selectional auto-encoders in Keras",
             "executable": "ocrd-sbb-binarize",
             "input_file_grp": [],
             "output_file_grp": [],
             "parameters": {
                 "model": {
                     "content-type": "text/directory",
-                    "description": "Directory containing HDF5 models. Can be an absolute path or a path relative to the current working directory or $SBB_BINARIZE_DATA environment variable (if set)",
+                    "description": "Directory containing HDF5 or SavedModel/ProtoBuf models. Can be an absolute path or a path relative to the OCR-D resource location, the current working directory or the $SBB_BINARIZE_DATA environment variable (if set)",
                     "format": "uri",
                     "required": true,
                     "type": "string"
                 },
                 "operation_level": {
                     "default": "page",
                     "description": "PAGE XML hierarchy level to operate on",
                     "enum": [
                         "page",
                         "region"
                     ],
                     "type": "string"
                 }
             },
+            "resources": [
+                {
+                    "description": "default models provided by github.com/qurator-spk (SavedModel format)",
+                    "name": "default",
+                    "path_in_archive": "saved_model_2020_01_16",
+                    "size": 563147331,
+                    "type": "archive",
+                    "url": "https://github.com/qurator-spk/sbb_binarization/releases/download/v0.0.11/saved_model_2020_01_16.zip"
+                },
+                {
+                    "description": "updated default models provided by github.com/qurator-spk (SavedModel format)",
+                    "name": "default-2021-03-09",
+                    "path_in_archive": ".",
+                    "size": 133230419,
+                    "type": "archive",
+                    "url": "https://github.com/qurator-spk/sbb_binarization/releases/download/v0.0.11/saved_model_2021_03_09.zip"
+                }
+            ],
             "steps": [
                 "preprocessing/optimization/binarization"
             ]
         }
     },
-    "version": "0.0.9"
+    "version": "0.1.0"
 }
```

### Comparing `sbb_binarization-0.0.9/sbb_binarize/ocrd_cli.py` & `sbb_binarization-0.1.0/sbb_binarize/ocrd_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,18 @@
 TOOL = 'ocrd-sbb-binarize'
 
 def cv2pil(img):
     return Image.fromarray(img.astype('uint8'))
 
 def pil2cv(img):
     # from ocrd/workspace.py
+    if img.mode in ('LA', 'RGBA'):
+        newimg = Image.new(img.mode[:-1], img.size, 'white')
+        newimg.paste(img, mask=img.getchannel('A'))
+        img = newimg
     color_conversion = cv2.COLOR_GRAY2BGR if img.mode in ('1', 'L') else  cv2.COLOR_RGB2BGR
     pil_as_np_array = np.array(img).astype('uint8') if img.mode == '1' else np.array(img)
     return cv2.cvtColor(pil_as_np_array, color_conversion)
 
 class SbbBinarizeProcessor(Processor):
 
     def __init__(self, *args, **kwargs):
@@ -102,44 +106,44 @@
             self.add_metadata(pcgts)
             pcgts.set_pcGtsId(file_id)
             page = pcgts.get_Page()
             page_image, page_xywh, _ = self.workspace.image_from_page(page, page_id, feature_filter='binarized')
 
             if oplevel == 'page':
                 LOG.info("Binarizing on 'page' level in page '%s'", page_id)
-                bin_image = cv2pil(self.binarizer.run(image=pil2cv(page_image), use_patches=True))
+                bin_image = cv2pil(self.binarizer.run(image=pil2cv(page_image)))
                 # update METS (add the image file):
                 bin_image_path = self.workspace.save_image_file(bin_image,
                         file_id + '.IMG-BIN',
                         page_id=input_file.pageId,
                         file_grp=self.output_file_grp)
                 page.add_AlternativeImage(AlternativeImageType(filename=bin_image_path, comments='%s,binarized' % page_xywh['features']))
 
             elif oplevel == 'region':
                 regions = page.get_AllRegions(['Text', 'Table'], depth=1)
                 if not regions:
                     LOG.warning("Page '%s' contains no text/table regions", page_id)
                 for region in regions:
                     region_image, region_xywh = self.workspace.image_from_segment(region, page_image, page_xywh, feature_filter='binarized')
-                    region_image_bin = cv2pil(binarizer.run(image=pil2cv(region_image), use_patches=True))
+                    region_image_bin = cv2pil(self.binarizer.run(image=pil2cv(region_image)))
                     region_image_bin_path = self.workspace.save_image_file(
                             region_image_bin,
                             "%s_%s.IMG-BIN" % (file_id, region.id),
                             page_id=input_file.pageId,
                             file_grp=self.output_file_grp)
                     region.add_AlternativeImage(
                         AlternativeImageType(filename=region_image_bin_path, comments='%s,binarized' % region_xywh['features']))
 
             elif oplevel == 'line':
                 region_line_tuples = [(r.id, r.get_TextLine()) for r in page.get_AllRegions(['Text'], depth=0)]
                 if not region_line_tuples:
                     LOG.warning("Page '%s' contains no text lines", page_id)
                 for region_id, line in region_line_tuples:
                     line_image, line_xywh = self.workspace.image_from_segment(line, page_image, page_xywh, feature_filter='binarized')
-                    line_image_bin = cv2pil(binarizer.run(image=pil2cv(line_image), use_patches=True))
+                    line_image_bin = cv2pil(self.binarizer.run(image=pil2cv(line_image)))
                     line_image_bin_path = self.workspace.save_image_file(
                             line_image_bin,
                             "%s_%s_%s.IMG-BIN" % (file_id, region_id, line.id),
                             page_id=input_file.pageId,
                             file_grp=self.output_file_grp)
                     line.add_AlternativeImage(
                         AlternativeImageType(filename=line_image_bin_path, comments='%s,binarized' % line_xywh['features']))
```

### Comparing `sbb_binarization-0.0.9/sbb_binarize/sbb_binarize.py` & `sbb_binarization-0.1.0/sbb_binarize/sbb_binarize.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,19 @@
     def __init__(self, model_dir, logger=None):
         self.model_dir = model_dir
         self.log = logger if logger else logging.getLogger('SbbBinarizer')
 
         self.start_new_session()
 
         self.model_files = glob('%s/*.h5' % self.model_dir)
-
+        if not self.model_files:
+            self.model_files = glob('%s/*/' % self.model_dir)
+        if not self.model_files:
+            raise ValueError(f"No models found in {self.model_dir}")
+        
         self.models = []
         for model_file in self.model_files:
             self.models.append(self.load_model(model_file))
 
     def start_new_session(self):
         config = tf.compat.v1.ConfigProto()
         config.gpu_options.allow_growth = True
@@ -48,21 +52,21 @@
 
     def end_session(self):
         tensorflow_backend.clear_session()
         self.session.close()
         del self.session
 
     def load_model(self, model_name):
-        model = load_model(join(self.model_dir, model_name), compile=False)
+        model = load_model(model_name, compile=False)
         model_height = model.layers[len(model.layers)-1].output_shape[1]
         model_width = model.layers[len(model.layers)-1].output_shape[2]
         n_classes = model.layers[len(model.layers)-1].output_shape[3]
         return model, model_height, model_width, n_classes
 
-    def predict(self, model_in, img, use_patches):
+    def predict(self, model_in, img):
         tensorflow_backend.set_session(self.session)
         model, model_height, model_width, n_classes = model_in
         
         img_org_h = img.shape[0]
         img_org_w = img.shape[1]
         
         if img.shape[0] < model_height and img.shape[1] >= model_width:
@@ -93,182 +97,169 @@
         else:
             index_start_h = 0
             index_start_w  = 0
             img_padded = np.copy(img)
             
             
         img = np.copy(img_padded)
-        
-            
 
-        if use_patches:
+        margin = int(0.1 * model_width)
 
-            margin = int(0.1 * model_width)
+        width_mid = model_width - 2 * margin
+        height_mid = model_height - 2 * margin
 
-            width_mid = model_width - 2 * margin
-            height_mid = model_height - 2 * margin
 
+        img = img / float(255.0)
 
-            img = img / float(255.0)
+        img_h = img.shape[0]
+        img_w = img.shape[1]
 
-            img_h = img.shape[0]
-            img_w = img.shape[1]
+        prediction_true = np.zeros((img_h, img_w, 3))
+        mask_true = np.zeros((img_h, img_w))
+        nxf = img_w / float(width_mid)
+        nyf = img_h / float(height_mid)
 
-            prediction_true = np.zeros((img_h, img_w, 3))
-            mask_true = np.zeros((img_h, img_w))
-            nxf = img_w / float(width_mid)
-            nyf = img_h / float(height_mid)
-
-            if nxf > int(nxf):
-                nxf = int(nxf) + 1
-            else:
-                nxf = int(nxf)
+        if nxf > int(nxf):
+            nxf = int(nxf) + 1
+        else:
+            nxf = int(nxf)
 
-            if nyf > int(nyf):
-                nyf = int(nyf) + 1
-            else:
-                nyf = int(nyf)
+        if nyf > int(nyf):
+            nyf = int(nyf) + 1
+        else:
+            nyf = int(nyf)
 
-            for i in range(nxf):
-                for j in range(nyf):
+        for i in range(nxf):
+            for j in range(nyf):
 
-                    if i == 0:
-                        index_x_d = i * width_mid
-                        index_x_u = index_x_d + model_width
-                    elif i > 0:
-                        index_x_d = i * width_mid
-                        index_x_u = index_x_d + model_width
+                if i == 0:
+                    index_x_d = i * width_mid
+                    index_x_u = index_x_d + model_width
+                elif i > 0:
+                    index_x_d = i * width_mid
+                    index_x_u = index_x_d + model_width
 
-                    if j == 0:
-                        index_y_d = j * height_mid
-                        index_y_u = index_y_d + model_height
-                    elif j > 0:
-                        index_y_d = j * height_mid
-                        index_y_u = index_y_d + model_height
+                if j == 0:
+                    index_y_d = j * height_mid
+                    index_y_u = index_y_d + model_height
+                elif j > 0:
+                    index_y_d = j * height_mid
+                    index_y_u = index_y_d + model_height
 
-                    if index_x_u > img_w:
-                        index_x_u = img_w
-                        index_x_d = img_w - model_width
-                    if index_y_u > img_h:
-                        index_y_u = img_h
-                        index_y_d = img_h - model_height
+                if index_x_u > img_w:
+                    index_x_u = img_w
+                    index_x_d = img_w - model_width
+                if index_y_u > img_h:
+                    index_y_u = img_h
+                    index_y_d = img_h - model_height
 
-                    img_patch = img[index_y_d:index_y_u, index_x_d:index_x_u, :]
+                img_patch = img[index_y_d:index_y_u, index_x_d:index_x_u, :]
 
-                    label_p_pred = model.predict(img_patch.reshape(1, img_patch.shape[0], img_patch.shape[1], img_patch.shape[2]))
+                label_p_pred = model.predict(img_patch.reshape(1, img_patch.shape[0], img_patch.shape[1], img_patch.shape[2]),
+                                             verbose=0)
 
-                    seg = np.argmax(label_p_pred, axis=3)[0]
+                seg = np.argmax(label_p_pred, axis=3)[0]
 
-                    seg_color = np.repeat(seg[:, :, np.newaxis], 3, axis=2)
+                seg_color = np.repeat(seg[:, :, np.newaxis], 3, axis=2)
 
-                    if i == 0 and j == 0:
-                        seg_color = seg_color[0:seg_color.shape[0] - margin, 0:seg_color.shape[1] - margin, :]
-                        seg = seg[0:seg.shape[0] - margin, 0:seg.shape[1] - margin]
+                if i == 0 and j == 0:
+                    seg_color = seg_color[0:seg_color.shape[0] - margin, 0:seg_color.shape[1] - margin, :]
+                    seg = seg[0:seg.shape[0] - margin, 0:seg.shape[1] - margin]
 
-                        mask_true[index_y_d + 0:index_y_u - margin, index_x_d + 0:index_x_u - margin] = seg
-                        prediction_true[index_y_d + 0:index_y_u - margin, index_x_d + 0:index_x_u - margin, :] = seg_color
+                    mask_true[index_y_d + 0:index_y_u - margin, index_x_d + 0:index_x_u - margin] = seg
+                    prediction_true[index_y_d + 0:index_y_u - margin, index_x_d + 0:index_x_u - margin, :] = seg_color
 
-                    elif i == nxf-1 and j == nyf-1:
-                        seg_color = seg_color[margin:seg_color.shape[0] - 0, margin:seg_color.shape[1] - 0, :]
-                        seg = seg[margin:seg.shape[0] - 0, margin:seg.shape[1] - 0]
+                elif i == nxf-1 and j == nyf-1:
+                    seg_color = seg_color[margin:seg_color.shape[0] - 0, margin:seg_color.shape[1] - 0, :]
+                    seg = seg[margin:seg.shape[0] - 0, margin:seg.shape[1] - 0]
 
-                        mask_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - 0] = seg
-                        prediction_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - 0, :] = seg_color
+                    mask_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - 0] = seg
+                    prediction_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - 0, :] = seg_color
 
-                    elif i == 0 and j == nyf-1:
-                        seg_color = seg_color[margin:seg_color.shape[0] - 0, 0:seg_color.shape[1] - margin, :]
-                        seg = seg[margin:seg.shape[0] - 0, 0:seg.shape[1] - margin]
+                elif i == 0 and j == nyf-1:
+                    seg_color = seg_color[margin:seg_color.shape[0] - 0, 0:seg_color.shape[1] - margin, :]
+                    seg = seg[margin:seg.shape[0] - 0, 0:seg.shape[1] - margin]
 
-                        mask_true[index_y_d + margin:index_y_u - 0, index_x_d + 0:index_x_u - margin] = seg
-                        prediction_true[index_y_d + margin:index_y_u - 0, index_x_d + 0:index_x_u - margin, :] = seg_color
+                    mask_true[index_y_d + margin:index_y_u - 0, index_x_d + 0:index_x_u - margin] = seg
+                    prediction_true[index_y_d + margin:index_y_u - 0, index_x_d + 0:index_x_u - margin, :] = seg_color
 
-                    elif i == nxf-1 and j == 0:
-                        seg_color = seg_color[0:seg_color.shape[0] - margin, margin:seg_color.shape[1] - 0, :]
-                        seg = seg[0:seg.shape[0] - margin, margin:seg.shape[1] - 0]
+                elif i == nxf-1 and j == 0:
+                    seg_color = seg_color[0:seg_color.shape[0] - margin, margin:seg_color.shape[1] - 0, :]
+                    seg = seg[0:seg.shape[0] - margin, margin:seg.shape[1] - 0]
 
-                        mask_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - 0] = seg
-                        prediction_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - 0, :] = seg_color
+                    mask_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - 0] = seg
+                    prediction_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - 0, :] = seg_color
 
-                    elif i == 0 and j != 0 and j != nyf-1:
-                        seg_color = seg_color[margin:seg_color.shape[0] - margin, 0:seg_color.shape[1] - margin, :]
-                        seg = seg[margin:seg.shape[0] - margin, 0:seg.shape[1] - margin]
+                elif i == 0 and j != 0 and j != nyf-1:
+                    seg_color = seg_color[margin:seg_color.shape[0] - margin, 0:seg_color.shape[1] - margin, :]
+                    seg = seg[margin:seg.shape[0] - margin, 0:seg.shape[1] - margin]
 
-                        mask_true[index_y_d + margin:index_y_u - margin, index_x_d + 0:index_x_u - margin] = seg
-                        prediction_true[index_y_d + margin:index_y_u - margin, index_x_d + 0:index_x_u - margin, :] = seg_color
+                    mask_true[index_y_d + margin:index_y_u - margin, index_x_d + 0:index_x_u - margin] = seg
+                    prediction_true[index_y_d + margin:index_y_u - margin, index_x_d + 0:index_x_u - margin, :] = seg_color
 
-                    elif i == nxf-1 and j != 0 and j != nyf-1:
-                        seg_color = seg_color[margin:seg_color.shape[0] - margin, margin:seg_color.shape[1] - 0, :]
-                        seg = seg[margin:seg.shape[0] - margin, margin:seg.shape[1] - 0]
+                elif i == nxf-1 and j != 0 and j != nyf-1:
+                    seg_color = seg_color[margin:seg_color.shape[0] - margin, margin:seg_color.shape[1] - 0, :]
+                    seg = seg[margin:seg.shape[0] - margin, margin:seg.shape[1] - 0]
 
-                        mask_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - 0] = seg
-                        prediction_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - 0, :] = seg_color
+                    mask_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - 0] = seg
+                    prediction_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - 0, :] = seg_color
 
-                    elif i != 0 and i != nxf-1 and j == 0:
-                        seg_color = seg_color[0:seg_color.shape[0] - margin, margin:seg_color.shape[1] - margin, :]
-                        seg = seg[0:seg.shape[0] - margin, margin:seg.shape[1] - margin]
+                elif i != 0 and i != nxf-1 and j == 0:
+                    seg_color = seg_color[0:seg_color.shape[0] - margin, margin:seg_color.shape[1] - margin, :]
+                    seg = seg[0:seg.shape[0] - margin, margin:seg.shape[1] - margin]
 
-                        mask_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - margin] = seg
-                        prediction_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - margin, :] = seg_color
+                    mask_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - margin] = seg
+                    prediction_true[index_y_d + 0:index_y_u - margin, index_x_d + margin:index_x_u - margin, :] = seg_color
 
-                    elif i != 0 and i != nxf-1 and j == nyf-1:
-                        seg_color = seg_color[margin:seg_color.shape[0] - 0, margin:seg_color.shape[1] - margin, :]
-                        seg = seg[margin:seg.shape[0] - 0, margin:seg.shape[1] - margin]
+                elif i != 0 and i != nxf-1 and j == nyf-1:
+                    seg_color = seg_color[margin:seg_color.shape[0] - 0, margin:seg_color.shape[1] - margin, :]
+                    seg = seg[margin:seg.shape[0] - 0, margin:seg.shape[1] - margin]
 
-                        mask_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - margin] = seg
-                        prediction_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - margin, :] = seg_color
+                    mask_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - margin] = seg
+                    prediction_true[index_y_d + margin:index_y_u - 0, index_x_d + margin:index_x_u - margin, :] = seg_color
 
-                    else:
-                        seg_color = seg_color[margin:seg_color.shape[0] - margin, margin:seg_color.shape[1] - margin, :]
-                        seg = seg[margin:seg.shape[0] - margin, margin:seg.shape[1] - margin]
+                else:
+                    seg_color = seg_color[margin:seg_color.shape[0] - margin, margin:seg_color.shape[1] - margin, :]
+                    seg = seg[margin:seg.shape[0] - margin, margin:seg.shape[1] - margin]
 
-                        mask_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - margin] = seg
-                        prediction_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - margin, :] = seg_color
-            
-            
-            
-            prediction_true = prediction_true[index_start_h: index_start_h+img_org_h, index_start_w: index_start_w+img_org_w,:]
-            prediction_true = prediction_true.astype(np.uint8)
+                    mask_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - margin] = seg
+                    prediction_true[index_y_d + margin:index_y_u - margin, index_x_d + margin:index_x_u - margin, :] = seg_color
+        
+        
+        
+        prediction_true = prediction_true[index_start_h: index_start_h+img_org_h, index_start_w: index_start_w+img_org_w,:]
+        prediction_true = prediction_true.astype(np.uint8)
 
-        else:
-            img_h_page = img.shape[0]
-            img_w_page = img.shape[1]
-            img = img / float(255.0)
-            img = resize_image(img, model_height, model_width)
-
-            label_p_pred = model.predict(img.reshape(1, img.shape[0], img.shape[1], img.shape[2]))
-
-            seg = np.argmax(label_p_pred, axis=3)[0]
-            seg_color = np.repeat(seg[:, :, np.newaxis], 3, axis=2)
-            prediction_true = resize_image(seg_color, img_h_page, img_w_page)
-            prediction_true = prediction_true.astype(np.uint8)
         return prediction_true[:,:,0]
 
-    def run(self, image=None, image_path=None, save=None, use_patches=False):
+    def run(self, image=None, image_path=None, save=None):
         if (image is not None and image_path is not None) or \
                (image is None and image_path is None):
             raise ValueError("Must pass either a opencv2 image or an image_path")
         if image_path is not None:
             image = cv2.imread(image_path)
         img_last = 0
         for n, (model, model_file) in enumerate(zip(self.models, self.model_files)):
             self.log.info('Predicting with model %s [%s/%s]' % (model_file, n + 1, len(self.model_files)))
 
-            res = self.predict(model, image, use_patches)
+            res = self.predict(model, image)
 
             img_fin = np.zeros((res.shape[0], res.shape[1], 3))
             res[:, :][res[:, :] == 0] = 2
             res = res - 1
             res = res * 255
             img_fin[:, :, 0] = res
             img_fin[:, :, 1] = res
             img_fin[:, :, 2] = res
 
             img_fin = img_fin.astype(np.uint8)
             img_fin = (res[:, :] == 0) * 255
             img_last = img_last + img_fin
 
-        kernel = np.ones((5, 5), np.uint8)
         img_last[:, :][img_last[:, :] > 0] = 255
         img_last = (img_last[:, :] == 0) * 255
         if save:
-            cv2.imwrite(save, img_last)
+            cv2.imwrite(save, img_last.astype(np.uint8), [
+                cv2.IMWRITE_PNG_BILEVEL, 1,
+                cv2.IMWRITE_JPEG_QUALITY, 100
+            ])
         return img_last
```

### Comparing `sbb_binarization-0.0.9/setup.py` & `sbb_binarization-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     version=version,
     description='Pixelwise binarization with selectional auto-encoders in Keras',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Vahid Rezanezhad',
     url='https://github.com/qurator-spk/sbb_binarization',
     license='Apache License 2.0',
-    packages=find_packages(exclude=('tests', 'docs')),
+    packages=find_packages(exclude=('test', 'repo')),
     include_package_data=True,
     package_data={'': ['*.json', '*.yml', '*.yaml']},
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
             'sbb_binarize=sbb_binarize.cli:main',
             'ocrd-sbb-binarize=sbb_binarize.ocrd_cli:cli',
```

