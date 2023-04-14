# Comparing `tmp/braintracer-0.1.3.tar.gz` & `tmp/braintracer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintracer-0.1.3.tar", last modified: Wed Feb 15 16:05:31 2023, max compression
+gzip compressed data, was "braintracer-0.1.4.tar", last modified: Fri Apr 14 09:39:21 2023, max compression
```

## Comparing `braintracer-0.1.3.tar` & `braintracer-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 16:05:31.245772 braintracer-0.1.3/
--rw-rw-rw-   0        0        0    33092 2023-02-15 15:54:13.000000 braintracer-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      146 2023-02-11 09:26:39.000000 braintracer-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7036 2023-02-15 16:05:31.245772 braintracer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6010 2023-02-11 10:50:51.000000 braintracer-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 16:05:31.226425 braintracer-0.1.3/braintracer/
--rw-rw-rw-   0        0        0        0 2023-02-05 11:48:38.000000 braintracer-0.1.3/braintracer/__init__.py
--rw-rw-rw-   0        0        0    28001 2023-02-15 15:58:50.000000 braintracer-0.1.3/braintracer/analysis.py
--rw-rw-rw-   0        0        0       11 2023-02-11 08:52:34.000000 braintracer-0.1.3/braintracer/bt - TODO.sh
--rwxrwxrwx   0        0        0     4849 2023-02-15 15:58:30.000000 braintracer-0.1.3/braintracer/bt.bat
--rw-rw-rw-   0        0        0  2699119 2023-02-11 10:17:14.000000 braintracer-0.1.3/braintracer/bt_visualiser.ipynb
--rw-rw-rw-   0        0        0     8712 2023-02-15 15:58:20.000000 braintracer-0.1.3/braintracer/file_management.py
--rw-rw-rw-   0        0        0    45378 2023-02-15 15:58:57.000000 braintracer-0.1.3/braintracer/plotting.py
-drwxrwxrwx   0        0        0        0 2023-02-15 16:05:31.243617 braintracer-0.1.3/braintracer/sample_data/
--rw-rw-rw-   0        0        0   156626 2023-02-05 11:48:38.000000 braintracer-0.1.3/braintracer/sample_data/cells_FR197_Unet_g.csv
--rw-rw-rw-   0        0        0   125713 2023-02-05 11:48:38.000000 braintracer-0.1.3/braintracer/sample_data/cells_FR197_Unet_r.csv
--rw-rw-rw-   0        0        0    16571 2023-02-05 11:48:38.000000 braintracer-0.1.3/braintracer/sample_data/cells_FR200_Unet_g.csv
--rw-rw-rw-   0        0        0   204182 2023-02-05 11:48:38.000000 braintracer-0.1.3/braintracer/sample_data/cells_FR200_Unet_r.csv
--rw-rw-rw-   0        0        0  1049905 2023-02-05 11:48:38.000000 braintracer-0.1.3/braintracer/split_repair.ipynb
--rw-rw-rw-   0        0        0     3525 2023-02-15 16:01:11.000000 braintracer-0.1.3/braintracer/stack_transform - TODO.py
--rw-rw-rw-   0        0        0    65506 2020-09-24 18:10:29.000000 braintracer-0.1.3/braintracer/structures.csv
-drwxrwxrwx   0        0        0        0 2023-02-15 16:05:31.235401 braintracer-0.1.3/braintracer.egg-info/
--rw-rw-rw-   0        0        0     7036 2023-02-15 16:05:31.000000 braintracer-0.1.3/braintracer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-02-15 16:05:31.000000 braintracer-0.1.3/braintracer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 16:05:31.000000 braintracer-0.1.3/braintracer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      161 2023-02-15 16:05:31.000000 braintracer-0.1.3/braintracer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-15 16:05:31.000000 braintracer-0.1.3/braintracer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2023-02-10 09:00:24.000000 braintracer-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1276 2023-02-15 16:05:31.247761 braintracer-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:21.139041 braintracer-0.1.4/
+-rw-rw-rw-   0        0        0    33092 2023-02-15 15:54:13.000000 braintracer-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      146 2023-02-11 09:26:39.000000 braintracer-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7036 2023-04-14 09:39:21.139041 braintracer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6010 2023-02-11 10:50:51.000000 braintracer-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:21.121599 braintracer-0.1.4/braintracer/
+-rw-rw-rw-   0        0        0        0 2023-02-05 11:48:38.000000 braintracer-0.1.4/braintracer/__init__.py
+-rw-rw-rw-   0        0        0    24147 2023-04-14 08:56:53.000000 braintracer-0.1.4/braintracer/analysis.py
+-rw-rw-rw-   0        0        0   279395 2023-04-05 14:59:40.000000 braintracer-0.1.4/braintracer/anterograde_pipeline.ipynb
+-rwxrwxrwx   0        0        0     5007 2023-04-14 09:01:58.000000 braintracer-0.1.4/braintracer/bt.bat
+-rw-rw-rw-   0        0        0     5370 2023-02-28 15:06:17.000000 braintracer-0.1.4/braintracer/bt.sh
+-rw-rw-rw-   0        0        0  2699119 2023-02-11 10:17:14.000000 braintracer-0.1.4/braintracer/bt_visualiser.ipynb
+-rw-rw-rw-   0        0        0     9335 2023-04-12 10:51:52.000000 braintracer-0.1.4/braintracer/file_management.py
+-rw-rw-rw-   0        0        0    45873 2023-04-14 08:57:04.000000 braintracer-0.1.4/braintracer/plotting.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:21.137094 braintracer-0.1.4/braintracer/sample_data/
+-rw-rw-rw-   0        0        0   156626 2023-02-05 11:48:38.000000 braintracer-0.1.4/braintracer/sample_data/cells_FR197_Unet_g.csv
+-rw-rw-rw-   0        0        0   125713 2023-02-05 11:48:38.000000 braintracer-0.1.4/braintracer/sample_data/cells_FR197_Unet_r.csv
+-rw-rw-rw-   0        0        0    16571 2023-02-05 11:48:38.000000 braintracer-0.1.4/braintracer/sample_data/cells_FR200_Unet_g.csv
+-rw-rw-rw-   0        0        0   204182 2023-02-05 11:48:38.000000 braintracer-0.1.4/braintracer/sample_data/cells_FR200_Unet_r.csv
+-rw-rw-rw-   0        0        0  1049905 2023-02-05 11:48:38.000000 braintracer-0.1.4/braintracer/split_repair.ipynb
+-rw-rw-rw-   0        0        0    65506 2020-09-24 18:10:29.000000 braintracer-0.1.4/braintracer/structures.csv
+drwxrwxrwx   0        0        0        0 2023-04-14 09:39:21.129481 braintracer-0.1.4/braintracer.egg-info/
+-rw-rw-rw-   0        0        0     7036 2023-04-14 09:39:21.000000 braintracer-0.1.4/braintracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-04-14 09:39:21.000000 braintracer-0.1.4/braintracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:39:21.000000 braintracer-0.1.4/braintracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      161 2023-04-14 09:39:21.000000 braintracer-0.1.4/braintracer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 09:39:21.000000 braintracer-0.1.4/braintracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2023-02-10 09:00:24.000000 braintracer-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1276 2023-04-14 09:39:21.140041 braintracer-0.1.4/setup.cfg
```

### Comparing `braintracer-0.1.3/LICENSE.txt` & `braintracer-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/PKG-INFO` & `braintracer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: braintracer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A complete processing pipeline for anatomical neuronal tracing.
 Home-page: https://github.com/samclothier/braintracer
-Download-URL: https://github.com/samclothier/braintracer/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/samclothier/braintracer/archive/refs/tags/0.1.4.tar.gz
 Author: Sam Clothier
 Author-email: sam.clothier.18@ucl.ac.uk
 Keywords: neuroscience,tracing,anatomy,brainglobe,cellfinder,brainreg
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `braintracer-0.1.3/README.md` & `braintracer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/analysis.py` & `braintracer-0.1.4/braintracer/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import pickle, time, cv2
-import braintracer.braintracer.file_management as btf
-import braintracer.braintracer.plotting as btp
+import braintracer.file_management as btf
+import braintracer.plotting as btp
 import matplotlib.pyplot as plt
 import shortuuid as uid
 import pandas as pd
 import numpy as np
 from bg_atlasapi.bg_atlas import BrainGlobeAtlas
 from IPython.display import clear_output
 from sklearn import linear_model
@@ -34,50 +34,36 @@
 from matplotlib import cm
 
 datasets = []
 area_indexes = btf.open_file('structures.csv')
 atlas = btf.get_atlas()
 reference = btf.get_reference()
 network_name = 'Unet'
-fluorescence = False
 starter_region = None
 starter_ch1 = False
 grouped = True
 debug = False
 
 class Dataset:
-	def __init__(self, name, group, sig, bg, starters=None, atlas_25=False, fluorescence=False, ignore_autofluorescence=False, modify_starter=False, fluorescence_parameters=False):
+	def __init__(self, name, group, sig, bg, fluorescence=False, starters=None, atlas_25=False, modify_starter=False):
 		self.name, self.group, self.sig, self.bg, self.fluorescence = name, group, sig, bg, fluorescence
-		self.atlas = None # becomes used if the atlas is modified or fluorescence analysed
+		self.atlas = None # becomes used if the atlas is modified
 		if not fluorescence:
 			self.ch1_cells = btf.open_file(f'cells_{self.name}_{network_name}_{self.sig[0]}.csv', atlas_25=atlas_25)
-			#self.ch2_cells = btf.open_file(f'cells_{self.name}_{network_name}_{self.sig[-1]}.csv', atlas_25=atlas_25)
-			self.raw_ch1_cells_by_area = self.__count_cells(self.ch1_cells)
-			#self.raw_ch2_cells_by_area = self.__count_cells(self.ch2_cells)
-			self.ch1_cells_by_area = self.__propagate_cells_through_inheritance_tree(self.raw_ch1_cells_by_area)
-			#self.ch2_cells_by_area = self.__propagate_cells_through_inheritance_tree(self.raw_ch2_cells_by_area)
+		else:
+			self.ch1_cells = btf.open_file(f'binary_registered_{self.name}.npy', atlas_25=atlas_25) # check if atlas 25 works with anterograde pipeline
+		#self.ch2_cells = btf.open_file(f'cells_{self.name}_{network_name}_{self.sig[-1]}.csv', atlas_25=atlas_25)
+		self.raw_ch1_cells_by_area = self.__count_cells(self.ch1_cells)
+		#self.raw_ch2_cells_by_area = self.__count_cells(self.ch2_cells)
+		self.ch1_cells_by_area = self.__propagate_cells_through_inheritance_tree(self.raw_ch1_cells_by_area)
+		#self.ch2_cells_by_area = self.__propagate_cells_through_inheritance_tree(self.raw_ch2_cells_by_area)
+
 		datasets.append(self)
-		self.flr_by_area = None
 		self.area_volumes = None
 		self.true_postsynaptics = starters
-		if fluorescence:
-			try:
-				self.flr_by_area = btf.open_file(f'fluorescence_{self.name}.pkl')
-				print(f'Successfully opened saved fluorescence data for {self.name}')
-			except (OSError, IOError) as e:
-				print(f'Failed to open saved fluorescence data for {self.name}. Analysing fluorescence...')
-				if fluorescence_parameters:
-					self.analyse_fluorescence(correct_x_flip=True, check_after=400)
-				else:
-					self.analyse_fluorescence()
-				if self.flr_by_area != None:
-					btf.save(f'fluorescence_{self.name}', 'pkl', file=self.flr_by_area)
-					print(f'Saved fluorescence data for {self.name}.')
-				else:
-					print(f'Fluorescence data for {self.name} not saved because fluorescence not quantified correctly.')
 		global starter_region
 		if modify_starter: # starter region is always the global starter region
 			if starter_region is None:
 				print('Starter region unknown. Define it with bt.starter_region = \'IO\'')
 			with btf.HiddenPrints():
 				self.atlas = btf.get_atlas() #TODO: allow custom starter region modification
 			self.adapt_starter_area((452+175, 452+225), (627+90, 627+125), (1098+100, 1098+180))
@@ -155,24 +141,24 @@
 				id_path_list = [i for i in id_path_list if i != ''] # remove current indexes
 				for i in id_path_list: # propagate lowest area count through all parent areas
 					area_index = int(i)
 					new_counter.setdefault(area_index, 0)
 					new_counter[area_index] += count
 		return new_counter
 
-	def num_cells_in(self, area, ch1=None):
+	def num_cells_in(self, area, ch1=None, left=None):
 		'''
 		get the number of cells in a given brain area
 		WARNING: Used by internal functions before propagation; use only to query raw data
 		'''
 		area_idx = get_area_info([area])[1]
 		if ch1 == None:
-			return len(_get_cells_in(area_idx, self, ch1=True)[0]) + len(_get_cells_in(area_idx, self, ch1=False)[0])
+			return len(_get_cells_in(area_idx, self, ch1=True, left=left)[0]) + len(_get_cells_in(area_idx, self, ch1=False, left=left)[0])
 		else:
-			return len(_get_cells_in(area_idx, self, ch1=ch1)[0])
+			return len(_get_cells_in(area_idx, self, ch1=ch1, left=left)[0])
 
 	def presynaptics(self):
 		red_cells = self.num_cells(ch1=True)
 		IO_red = self.num_cells_in('IO', ch1=True)
 		CB_red = self.num_cells_in('CBX', ch1=True)
 		presynaptics = red_cells - (IO_red + CB_red)
 		return presynaptics
@@ -230,103 +216,14 @@
 			ax.set_xlabel(xlabel)
 			ax.set_ylabel('Cell count')
 			ax.set_xlim(0, atlas.shape[axis])
 		plot_dist(ax1, 2, xlabel='Distance from caudal end / um')
 		plot_dist(ax2, 0, xlabel='Distance from image left / um', legend=True)
 		plot_dist(ax3, 1, xlabel='Distance from image top / um')
 
-	def check_fluorescence(self, num, correct_z_flip=False, correct_x_flip=False, restrict_to_idx=None):
-		self.atlas = np.array(btf.open_file(f'atlas_{self.name}_r.tiff'))[0]
-		if correct_x_flip:
-			self.atlas = np.flip(self.atlas, axis=2)
-		if correct_z_flip:
-			self.atlas = np.flip(self.atlas, axis=0)
-		print(atlas.shape)
-		
-		subtracted_stack_files = btf.open_transformed_brain(self)
-		num_slices = len(subtracted_stack_files)
-		print(num_slices)
-		im = np.load(subtracted_stack_files[num])
-		print(im.shape)
-
-		# get values to scale pixels into registered atlas space
-		z_scalar = self.atlas.shape[0] / num_slices
-		y_scalar = self.atlas.shape[1] / im.shape[0]
-		x_scalar = self.atlas.shape[2] / im.shape[1]
-		print(z_scalar,y_scalar,x_scalar)
-
-		z_coords, y_coords, x_coords = np.array([]), np.array([]), np.array([])
-		atlas_z = int((num_slices - num) * z_scalar) - 1 # pick the closest atlas slice, -1 to start from zero
-		print(atlas_z)
-		y_pxs, x_pxs = np.nonzero(im) # get coordinates of 1s in this slice
-		x_coords = np.append(x_coords, list(map(lambda x: int(x * x_scalar), x_pxs)))
-		y_coords = np.append(y_coords, list(map(lambda y: int(y * y_scalar), y_pxs)))
-		z_coords = np.append(z_coords, [atlas_z] * len(x_pxs)) # add all the repeating z coordinates for this slice
-		coords = [list(x_coords.astype(int)), list(y_coords.astype(int)), list(z_coords.astype(int))]
-
-		x_vals, y_vals, z_vals = coords[0], coords[1], coords[2]
-		x_IO, y_IO, z_IO = np.array([]), np.array([]), np.array([])
-		seen_vals = []
-		for idx, z in enumerate(z_vals):
-			x = x_vals[idx]
-			y = y_vals[idx]
-			area_index = _get_area_index(self, z, x, y)
-			if area_index == restrict_to_idx:
-				x_IO = np.append(x_IO, x)
-				y_IO = np.append(y_IO, y)
-
-		atlas_im = self.atlas[atlas_z]
-		f, ax = plt.subplots(figsize=(10, 10))
-		ax.imshow(atlas_im, cmap='Greens', vmax=1000)
-		if restrict_to_idx is None:
-			ax.scatter(coords[0], coords[1], s=0.2)
-		else:
-			ax.scatter(x_IO, y_IO, s=0.2)
-
-	def analyse_fluorescence(self, correct_z_flip=False, correct_x_flip=False, check_after=200):
-		self.atlas = np.array(btf.open_file(f'atlas_{self.name}_r.tiff'))[0]
-		if correct_x_flip:
-			self.atlas = np.flip(self.atlas, axis=2)
-		if correct_z_flip:
-			self.atlas = np.flip(self.atlas, axis=0)
-		print(self.atlas.shape)
-		
-		subtracted_stack_files = btf.open_transformed_brain(self)
-		num_slices = len(subtracted_stack_files)
-		print(num_slices)
-		first_im = np.load(subtracted_stack_files[0])
-		print(first_im.shape)
-
-		# get values to scale pixels into registered atlas space
-		z_scalar = self.atlas.shape[0] / num_slices
-		y_scalar = self.atlas.shape[1] / first_im.shape[0]
-		x_scalar = self.atlas.shape[2] / first_im.shape[1]
-		print(z_scalar,y_scalar,x_scalar)
-
-		z_coords, y_coords, x_coords = np.array([]), np.array([]), np.array([])
-		for z, im in enumerate(tqdm(subtracted_stack_files)):
-			# take reverse of z
-			atlas_z = int((num_slices - z) * z_scalar) - 1 # pick the closest atlas slice, -1 to start from zero
-			y_pxs, x_pxs = np.nonzero(np.load(im)) # get coordinates of 1s in this slice
-			x_atlas = list(map(lambda x: int(x * x_scalar), x_pxs))
-			y_atlas = list(map(lambda y: int(y * y_scalar), y_pxs))
-			x_coords = np.append(x_coords, x_atlas)
-			y_coords = np.append(y_coords, y_atlas)
-			z_coords = np.append(z_coords, [atlas_z] * len(x_pxs)) # add all the repeating z coordinates for this slice
-			if check_after == z:
-				atlas_im = np.where(self.atlas[atlas_z] > 0, 1, 0)
-				f, ax = plt.subplots(figsize=(10, 10))
-				ax.imshow(atlas_im, cmap='Greens', interpolation=None)
-				ax.scatter(x_atlas, y_atlas, s=1)
-		coords = [list(x_coords.astype(int)), list(y_coords.astype(int)), list(z_coords.astype(int))]
-		
-		raw_fluorescence_by_area = self.__count_cells(coords)
-		fluorescence_by_area = self.__propagate_cells_through_inheritance_tree(raw_fluorescence_by_area)
-		self.flr_by_area = fluorescence_by_area
-
 	def project_slices(self, region, figsize=(10,6)):
 		start, end = region
 		subtracted_stack_files = btf.open_transformed_brain(self)
 
 		stack = []
 		for i in tqdm(range(start, end)):
 			im = np.load(subtracted_stack_files[i])
@@ -365,21 +262,28 @@
 			plt.show()
 			plt.figure(figsize=figsize)
 			plt.axis('off')
 			plt.imshow(res, cmap='binary', vmin=0, vmax=625)
 			if save:
 				btf.save(f'video_{self.name}_frame_{i}', as_type='png', dpi=80, vID=seq_id)
 
-	def get_tot_fluorescence(self, area_idxs):
-		if any(n < 0 for n in self.flr_by_area):
-			print(f'Warning: Brain regions have {sum(n < 0 for n in self.flr_by_area)} negative fluorescence values.')
-		_, area_idxs, _ = get_area_info(area_idxs) # make sure string area names are indexes
+	def get_cells_in_hemisphere(self, area): #, left=True):
+		# to query raw data:
+		num_total = self.num_cells_in(area, ch1=True, left=None)
+		num_left = self.num_cells_in(area, ch1=True, left=True)
+		num_right = self.num_cells_in(area, ch1=True, left=False)
+
+		# to get real answer:
+		parent, children = children_from(area, depth=0)
+		areas = [parent] + children
+		true_num_total = len(_get_cells_in(areas, self, ch1=True, left=None)[0])
+		true_num_left = len(_get_cells_in(areas, self, ch1=True, left=True)[0])
+		true_num_right = len(_get_cells_in(areas, self, ch1=True, left=False)[0])
 
-		return [self.flr_by_area[int(i)] for i in area_idxs]
-		# TODO: get area volumes with API
+		return (num_total, num_left, num_right), (true_num_total, true_num_left, true_num_right)
 
 
 class _Results: # singleton object
 	_instance = None
 	def __new__(cls):
 		if cls._instance is None:
 			cls._instance = super(_Results, cls).__new__(cls)
@@ -456,27 +360,35 @@
 	'''
 	im = atlas[z] if dataset.atlas is None else dataset.atlas[z] # happens when a dataset's atlas has been modified
 	if x < im.shape[1] and y < im.shape[0]: # not <= because index is (shape - 1)
 		area_index = int(im[y,x])
 		### USE atlas.structure_from_coords
 		#print(btf.atlas.structure_from_coords((z, y, x), as_acronym=True), area_index) # this works, but returns name 'IO'
 	else:
-		print('Warning: Point out of bounds')
+		if dataset.fluorescence is False: # don't warn if fluorescence because many transformed coordinates will be out of bounds
+			print('Warning: Point out of bounds')
 		return 0
 	if area_index >= 0:
 		return area_index
 	else:
 		print('Warning: Area index is < 0')
 		return 0
 
-def _get_cells_in(region, dataset, ch1=True):
+def _get_cells_in(region, dataset, ch1=True, left=None):
 	'''
 	return coordinates of cells within a defined region.
 	region: can be a list of area indexes, numpy array of a 3D area, or a tuple containing the coordinates bounding a cube
 	'''
+	def hemisphere_predicate(hemi):
+		if left == None:
+			return hemi == 'left' or hemi == 'right' # return true regardless of hemisphere
+		elif left == True:
+			return hemi == 'left'
+		elif left == False:
+			return hemi == 'right'
 	def is_in_region(z, x, y):
 		if isinstance(region, list):
 			areas = region
 			return _get_area_index(dataset, z, x, y) in areas
 		elif isinstance(region, int):
 			area = region
 			return _get_area_index(dataset, z, x, y) == area
@@ -486,19 +398,19 @@
 		elif isinstance(region, np.ndarray):
 			dilation = region
 			return dilation[z,y,x] == 1
 		else:
 			print(f'Unable to identify region type {type(region)} for returning cell coordinates.')
 	cells_x, cells_y, cells_z = [], [], []
 	cell_coords = dataset.ch1_cells if ch1 else dataset.ch2_cells
-	cls_x, cls_y, cls_z = cell_coords[0], cell_coords[1], cell_coords[2]
+	cls_x, cls_y, cls_z, cls_h = cell_coords[0], cell_coords[1], cell_coords[2], cell_coords[3]
 	for idx, z in enumerate(cls_z):
 		x = cls_x[idx]
 		y = cls_y[idx]
-		if is_in_region(z,x,y):
+		if is_in_region(z,x,y) and hemisphere_predicate(cls_h[idx]):
 			cells_x.append(x)
 			cells_y.append(y)
 			cells_z.append(z)
 	return cells_x, cells_y, cells_z
 
 def children_from(parent, depth):
 	'''
@@ -519,15 +431,15 @@
 	else:
 		for i in range(depth):
 			parents = list(map(lambda x: area_indexes.loc[area_indexes['parent_structure_id']==x].index.values.tolist(), parents))
 			parents = list(chain.from_iterable(parents))
 		children = parents
 	return parent, children
 
-def get_area_info(codes, new_counter=None):
+def get_area_info(codes, new_counter=None): # TODO: create functions where requested representation type is returned and starting type is not specified
 	'''
 	return area full-names, area indexes, and area cell count given short-letter codes or area indexes
 	'''
 	if not isinstance(codes, (list, np.ndarray)):
 		codes = [codes]
 	if isinstance(codes[0], (int, np.int32, np.int64)):
 		names = area_indexes.loc[codes, 'name'].tolist()
```

### Comparing `braintracer-0.1.3/braintracer/bt.bat` & `braintracer-0.1.4/braintracer/bt.bat`

 * *Files 3% similar despite different names*

```diff
@@ -38,48 +38,50 @@
 if /i "%c%" EQU "Y" goto :no_run
 if /i "%c%" EQU "N" goto :run
 goto :choice
 
 :run
 set /p np=Trained network path: 
 set /p res=Resolution (z x y; eg. 5 2 2): 
-set /p t=Threshold: 
+set /p orient=Orientation (post-ant, sup-inferior, l-r; eg. psr): 
+set /p t=Threshold (std-dev; eg. 20): 
+set /p bxy=Ball xy size (px; eg. 10): 
 set /p atres=Atlas resolution (um; eg. 10): 
 set /p reverse=Also perform cell detection in background channel against the signal channel (only works for one signal channel)? 
 
 (for %%s in (%s_chs%) do (
 	ECHO Running cellfinder...
 	cd %dataset%
 	if [%np%] == [] ( :: if no trained network
 		if not exist cellfinder_%s% (
-			cellfinder -s %%s -b %b% -o cellfinder_%%s -v %res% --orientation psr --threshold %t% --atlas allen_mouse_%atres%um --ball-xy-size 10
+			cellfinder -s %%s -b %b% -o cellfinder_%%s -v %res% --orientation %orient% --threshold %t% --atlas allen_mouse_%atres%um --ball-xy-size %bxy%
 		) else (
 			ECHO Results already exist for signal channel %%s!
 	)) else (
 		if not exist cellfinder_%s%_%nn% (
-			cellfinder -s %%s -b %b% -o cellfinder_%%s_%nn% -v %res% --orientation psr --threshold %t% --atlas allen_mouse_%atres%um --trained-model %np% --ball-xy-size 10
+			cellfinder -s %%s -b %b% -o cellfinder_%%s_%nn% -v %res% --orientation %orient% --threshold %t% --atlas allen_mouse_%atres%um --trained-model %np% --ball-xy-size %bxy%
 	))
 	cd ..
 	ECHO Copying results...
 	copy %dataset%\cellfinder_%%s_%nn%\registration\downsampled_standard_channel_0.tiff %folder%\downsampled_data\reg_%dataset%_%%s.tiff
 	copy %dataset%\cellfinder_%%s_%nn%\registration\downsampled_standard.tiff %folder%\downsampled_data\reg_%dataset%_%b%.tiff
 	copy %dataset%\cellfinder_%%s_%nn%\analysis\all_points.csv %folder%\cellfinder\cells_%dataset%_%nn%_%%s.csv
 ))
 :: do the same but without copying the downsampled images (they are identical to the forward run)
 if reverse EQU "Y" (
 	ECHO Running cellfinder...
 	cd %dataset%
 	if [%np%] == [] ( :: if no trained network
 		if not exist cellfinder_%b% (
-			cellfinder -s %b% -b %s_chs% -o cellfinder_%b% -v %res% --orientation psr --threshold %t% --atlas allen_mouse_%atres%um --ball-xy-size 10
+			cellfinder -s %b% -b %s_chs% -o cellfinder_%b% -v %res% --orientation %orient% --threshold %t% --atlas allen_mouse_%atres%um --ball-xy-size %bxy%
 		) else (
 			ECHO Results already exist for background channel %b%!
 	)) else (
 		if not exist cellfinder_%b%_%n_n% (
-			cellfinder -s %b% -b %s_chs% -o cellfinder_%b%_%nn% -v %res% --orientation psr --threshold %t% --atlas allen_mouse_%atres%um --trained-model %np% --ball-xy-size 10
+			cellfinder -s %b% -b %s_chs% -o cellfinder_%b%_%nn% -v %res% --orientation %orient% --threshold %t% --atlas allen_mouse_%atres%um --trained-model %np% --ball-xy-size %bxy%
 	))
 	cd ..
 	ECHO Copying results...
 	copy %dataset%\cellfinder_%b%\analysis\all_points.csv %folder%\cellfinder\cells_%dataset%_%nn%_%b%.csv
 )
 
 goto :end
```

### Comparing `braintracer-0.1.3/braintracer/bt_visualiser.ipynb` & `braintracer-0.1.4/braintracer/bt_visualiser.ipynb`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/file_management.py` & `braintracer-0.1.4/braintracer/file_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,64 +36,32 @@
 		child_dir = 'braintracer\\downsampled_data'
 	elif file_name.startswith('groundtruth_'):
 		child_dir = 'braintracer\\ground_truth'
 	elif file_name.startswith('structures'):
 		child_dir = None # local file, now part of the package
 	elif file_name.startswith('atlas'):
 		child_dir = 'braintracer\\registered_atlases'
-	elif file_name.startswith('fluorescence'):
+	elif file_name.startswith('binary_'):
 		child_dir = 'braintracer\\fluorescence'
 	elif file_name.startswith('injection_'):
 		child_dir = 'braintracer\\TRIO'
 	elif file_name.startswith('video_'):
 		assert vID is not None, 'video ID variable must be supplied for saving video frames'
 		child_dir = f'braintracer\\videos\\{file_name.split("_")[1]}_{vID}'
 	else:
 		raise ValueError('Unexpected file name. Braintracer accepts files with the following format:\ncells_[].xml/csv\nreg_[]_[].tiff\ngroundtruth_[].xml\nstructures.csv')
 
 	if child_dir is not None:
 		if not os.path.isdir(child_dir):
 			os.makedirs(child_dir)
 		path = os.path.join(script_dir, child_dir+'\\'+file_name)
 	else:
-		
 		path = os.path.join(package_dir, file_name)
 	return path
 
-def verify_image_integrity(dataset):
-	def code_comparisons(pre_code1, cur_code1, pre_code2, cur_code2):
-		pre_code1, cur_code1 = int(pre_code1), int(cur_code1)
-		pre_code2, cur_code2 = int(pre_code2), int(cur_code2) # convert all string codes to ints for comparison
-		if cur_code1 == pre_code1:
-			pass
-		elif (cur_code1 == pre_code1 + 1) and cur_code2 == 1:
-			pass
-		else:
-			return False
-		if cur_code2 == pre_code2 + 1:
-			return True
-		elif cur_code2 == 1 and pre_code2 == 8:
-			return True
-		else:
-			return False
-	for i in range(3):
-		channel_num = i + 1
-		path = os.path.join(script_dir, dataset, str(channel_num))
-		for root, dirs, files in os.walk(path):
-			prev_name = 'section_000_00.tif'
-			for file in files:
-				pre_code1 = prev_name.split('_')[1]
-				pre_code2 = prev_name.split('_')[-1][1]
-				cur_code1 = file.split('_')[1]
-				cur_code2 = file.split('_')[-1][1]
-				assert code_comparisons(pre_code1, cur_code1, pre_code2, cur_code2), f'Channel {i+1} warning: {file} does not follow previous file: {prev_name}'
-				prev_name = file
-			
-		print(f'Channel {i+1} successfully verified.')
-
 # opens xml files from napari containing cell points
 def open_file(name, atlas_25=False): # open files
 	all_X, all_Y, all_Z = [], [], []
 	neg_X, neg_Y, neg_Z = [], [], []
 	pos_X, pos_Y, pos_Z = [], [], []
 	file_path = _get_path(name)
 	ext = name.split('.')[-1]
@@ -130,38 +98,52 @@
 		return images
 	elif ext == 'csv':
 		if name.startswith('cells_'):
 			cell_df = pd.read_csv(file_path)
 			z_coords = cell_df['coordinate_atlas_axis_0'].to_list()
 			y_coords = cell_df['coordinate_atlas_axis_1'].to_list()
 			x_coords = cell_df['coordinate_atlas_axis_2'].to_list()
+			hemisphere = cell_df['hemisphere'].to_list()
 			if atlas_25:
 				z_coords = list(np.floor(np.array(z_coords) * 2.5).astype(int)) # convert coords in 25um atlas space to 10um
 				y_coords = list(np.floor(np.array(y_coords) * 2.5).astype(int))
 				x_coords = list(np.floor(np.array(x_coords) * 2.5).astype(int))
-			return [x_coords, y_coords, z_coords]
+			return [x_coords, y_coords, z_coords, hemisphere]
 		elif name.startswith('structures'):
 			area_indexes = pd.read_csv(file_path)
 			area_indexes = area_indexes.set_index('id')
 			return area_indexes
 		else:
 			print(f'Cannot load CSV with name {name}')
+	elif ext == 'npy':
+		coordinates = np.load(file_path)
+		coordinates = np.flip(coordinates.T, axis=0) # x, y, z
+		return coordinates.tolist()
 	elif ext == 'pkl':
 		return pickle.load(open(f'{file_path}', 'rb'))
 	else:
 		print('Unexpected file extension')
 		return None
 
 def open_transformed_brain(dataset):
 	name = dataset.name
 	path = os.path.join(script_dir, name+'\\'+'transform\\*')
 	assert os.path.isdir(path), f'Please provide transformed stack at {path}'
 	files = glob.glob(path)
 	return files
 
+def open_registered_stack(dataset):
+	if dataset.fluorescence:
+		name = f'binary_registered_stack_{dataset.name}.npy'
+		path = _get_path(name)
+		return np.load(path)
+	else:
+		stack = np.array(btf.open_file(f'reg_{dataset.name}_{dataset.sig[0]}.tiff'))[0]
+		return stack
+
 def get_atlas():
 	global atlas
 	return np.array(atlas.annotation)
 
 def get_reference():
 	global atlas
 	return np.array(atlas.reference)
@@ -220,14 +202,47 @@
 				for f in sorted(glob.glob(fp_in)))
 		# extract  first image from iterator
 		img = next(imgs)
 		# https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html#gif
 		img.save(fp=fp_out, format='GIF', append_images=imgs,
 				 save_all=True, duration=int((1/fps)*1000), loop=0)
 
+def verify_image_integrity(dataset):
+	def code_comparisons(pre_code1, cur_code1, pre_code2, cur_code2):
+		pre_code1, cur_code1 = int(pre_code1), int(cur_code1)
+		pre_code2, cur_code2 = int(pre_code2), int(cur_code2) # convert all string codes to ints for comparison
+		if cur_code1 == pre_code1:
+			pass
+		elif (cur_code1 == pre_code1 + 1) and cur_code2 == 1:
+			pass
+		else:
+			return False
+		if cur_code2 == pre_code2 + 1:
+			return True
+		elif cur_code2 == 1 and pre_code2 == 8:
+			return True
+		else:
+			return False
+	for i in range(3):
+		channel_num = i + 1
+		path = os.path.join(script_dir, dataset, str(channel_num))
+		if os.path.isdir(path):
+			for root, dirs, files in os.walk(path):
+				prev_name = 'section_000_00.tif'
+				for file in files:
+					pre_code1 = prev_name.split('_')[1]
+					pre_code2 = prev_name.split('_')[-1][1]
+					cur_code1 = file.split('_')[1]
+					cur_code2 = file.split('_')[-1][1]
+					assert code_comparisons(pre_code1, cur_code1, pre_code2, cur_code2), f'Channel {channel_num} warning: {file} does not follow previous file: {prev_name}'
+					prev_name = file
+			print(f'Channel {channel_num} successfully verified.')
+		else:
+			print(f'Channel {channel_num} does not exist. Try renaming channels to 1,2, and 3.')
+
 class HiddenPrints:
 	def __enter__(self):
 		self._original_stdout = sys.stdout
 		sys.stdout = open(os.devnull, 'w')
 
 	def __exit__(self, exc_type, exc_val, exc_tb):
 		sys.stdout.close()
```

### Comparing `braintracer-0.1.3/braintracer/plotting.py` & `braintracer-0.1.4/braintracer/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import plotly
-import braintracer.braintracer.file_management as btf
-import braintracer.braintracer.analysis as bt
+import braintracer.file_management as btf
+import braintracer.analysis as bt
 import matplotlib.pyplot as plt
 import matplotlib.colors as clrs
 import plotly.graph_objs as go
 import bgheatmaps as bgh
 import seaborn as sns
 import pandas as pd
 import numpy as np
@@ -63,25 +63,19 @@
 	ax.grid(axis=grid_orientation)
 	ax.set_title(fig_title)
 	return df
 
 def generate_summary_plot(ax=None):
 	summary_areas = ['CTX','CNU','TH','HY','MB','MY','P','CBX','CBN']
 	area_labels, _, _ = bt.get_area_info(summary_areas)
-	if bt.fluorescence:
-		datasets = [i for i in bt.datasets if i.fluorescence]
-		dataset_cells, axis_title = _fluorescence_by_area_across_fl_datasets(summary_areas, datasets, normalisation='ch1')
-	else:
-		datasets = [i for i in bt.datasets if not i.fluorescence]
-		dataset_cells, axis_title = _cells_in_areas_in_datasets(summary_areas, datasets, normalisation='ch1')
-		# Implement IO count subtraction from MY here
-		#IO_cells = bt.get_area_info('IO', dataset.ch1_cells_by_area)[2][0]
-		#cells[5] = cells[5] - IO_cells
-	
-	assert len(datasets) != 0, f'No datasets exist of type fluorescence={bt.fluorescence}'
+	datasets = [i for i in bt.datasets]# if not i.fluorescence]
+	dataset_cells, axis_title = _cells_in_areas_in_datasets(summary_areas, datasets, normalisation='ch1')
+	# Implement IO count subtraction from MY here
+	#IO_cells = bt.get_area_info('IO', dataset.ch1_cells_by_area)[2][0]
+	#cells[5] = cells[5] - IO_cells
 	if bt.debug:
 		print(dataset_cells)
 		percentages = [f'{sum(dataset):.1f}% ' for dataset in dataset_cells]
 		print(', '.join(percentages)+'cells are within brain boundaries and in non-tract and non-ventricular areas')
 	__draw_plot(ax, datasets, area_labels, dataset_cells, axis_title, fig_title='Whole brain', horizontal=True, l_space=0.2)
 
 def generate_custom_plot(area_names, title, normalisation='presynaptics', flr_log=False, horizontal=True, ax=None):
@@ -135,27 +129,29 @@
 	if areas is None:
 		summed = np.sum(dataset_cells, axis=0) # delete columns where mean is below threshold
 		averaged = summed / dataset_cells.shape[0]
 		idxs_to_remove = np.where(averaged <= threshold)[0]
 		dataset_cells = np.delete(dataset_cells, idxs_to_remove, axis=1)
 		area_labels = np.delete(area_labels, idxs_to_remove)
 		area_idxs = np.delete(area_idxs, idxs_to_remove) # also remove idxs so sort can work
-	print(list(area_idxs))
+	if bt.debug:
+		print(f'All areas: {list(area_idxs)}')
 
 	if sort is True:
 		#col_sorter = np.sum(dataset_cells, axis=0).argsort()[::-1] # sort columns by sum
 		#dataset_cells, area_labels = dataset_cells[:,col_sorter], area_labels[col_sorter]
 		new_labels = np.array([])
 		new_matrix = []
 		sorted_already = np.array([])
 		for i in area_idxs:
 			if i not in sorted_already:
 				children = bt.children_from(i, depth=0)[1]
 				present_children = [i for i in area_idxs if i in children and i not in sorted_already]
-				print(i, present_children)
+				if bt.debug:
+					print(f'Area {i} contains: {present_children}')
 				paired_arr = np.append(i, present_children)
 				new_labels = np.append(new_labels, paired_arr)
 				sorted_already = np.append(sorted_already, paired_arr)
 				for index in paired_arr:
 					i = np.where(area_idxs == index)[0]
 					new_matrix.append(list(dataset_cells[:,i].flatten()))
 		area_labels = bt.get_area_info(new_labels.astype(int))[0]
@@ -210,15 +206,17 @@
 
 def bin_3D_show(area_num=None, binsize=200, axis=2, sigma=None, subregions=None, subregion_depth=None, projcol='k', padding=10, vlim=None, ch1=True):
 	atlas_res = 10
 	assert binsize % atlas_res == 0, f'Binsize must be a multiple of atlas resolution ({atlas_res}um) to display correctly.'
 	x_bins, y_bins, z_bins = get_bins(0, binsize), get_bins(1, binsize), get_bins(2, binsize)
 	axes = [x for x in [0, 1, 2] if x != axis]
 	assert axis in [0, 1, 2], 'Must provide a valid axis number 0-2.'
-	regions = None
+	if area_num is None:
+		area_num = 997
+	regions = None # only define regions when subregion_depth and subregions = None
 	if subregion_depth is not None:
 		regions = bt.children_from(area_num, depth=subregion_depth)[1]
 	elif subregions is not None:
 		regions = subregions
 
 	f, (ax1, ax2) = plt.subplots(1,2, figsize=(10,5))
 	parent_projection, (px_min, py_min, pz_min), (px_max, py_max, pz_max) = bt.get_projection(area_num, padding=padding, axis=2-axis)
@@ -277,15 +275,19 @@
 				hist = hist[py_min : py_max, pz_min : pz_max]
 			hist_list.append(hist)
 		all_hists = np.array(hist_list) # get cell distributions for each dataset, ready for plotting
 		av_im = np.median(all_hists, axis=0) # get the mean cell distribution
 		av_im = av_im if axis == 0 else av_im.T # side-on orientation does not need axis swapping
 		cax = ax.imshow(av_im, cmap=cmap, vmin=0, vmax=vlim)
 		plt.colorbar(cax)
-		ax.set_title(f'{group} cell detection probability')
+
+		sum_cells = 0
+		for d in [d for d in bt.datasets if d.group == group]:
+			sum_cells = sum_cells + bt.get_area_info(area_num, d.ch1_cells_by_area)[2][0]
+		ax.set_title(f'{group} P(cell) (tot={av_im.shape[0]}, from={sum_cells})')
 
 	orig_cmap = plt.cm.RdBu
 	clrs_blue = orig_cmap(np.linspace(0.5, 1.0, 10))
 	clrs_reds = orig_cmap(np.linspace(0.0, 0.5, 10)[::-1])
 	cmap_blue = clrs.LinearSegmentedColormap.from_list("mycmap", clrs_blue)
 	cmap_reds = clrs.LinearSegmentedColormap.from_list("mycmap", clrs_reds)
 	plot_binned_average(ax1, axis, __get_bt_groups()[0], cmap=cmap_reds)
@@ -311,15 +313,17 @@
 			neg_num_points = points.shape
 			points_IO = np.array(bt._get_cells_in([83,528], d, ch1=ch1)).T
 			dims = np.maximum(points_IO.max(0),points.max(0))+1 # this and following line are to filter out IO points from points
 			points = points[~np.in1d(np.ravel_multi_index(points.T,dims),np.ravel_multi_index(points_IO.T,dims))]
 			if bt.debug:
 				print(f'Num neg points removed: {old_num_points[0] - neg_num_points[0]}, num IO+CBX points removed: {neg_num_points[0] - points.shape[0]}, num acc values: {points_IO.shape[0]}')
 		else:
-			points = np.array(bt._get_cells_in(area_num, d, ch1=ch1)).T
+			parent, children = bt.children_from(area_num, depth=0)
+			areas = [parent] + children
+			points = np.array(bt._get_cells_in(areas, d, ch1=ch1)).T
 		hist, binedges = np.histogramdd(points, bins=(x_bins, y_bins, z_bins), range=((0,1140),(0,800),(0,1320)), normed=False)
 		num_nonzero_bins.append(np.count_nonzero(hist)) # just debug stuff
 		last_hist_shape = hist.shape			
 		if sigma is not None: # 3D smooth # sigma = width of kernel
 			x, y, z = np.arange(-3,4,1), np.arange(-3,4,1), np.arange(-3,4,1) # coordinate arrays -- make sure they include (0,0)!
 			xx, yy, zz = np.meshgrid(x,y,z)
 			kernel = np.exp(-(xx**2 + yy**2 + zz**2)/(2*sigma**2))
@@ -353,14 +357,17 @@
 	else:
 		f, ax = plt.subplots(figsize=figsize)
 		f.set_facecolor('white')
 		divider = make_axes_locatable(ax)
 		cax = divider.append_axes('right', size='5%', pad=0.05)
 
 		cov = np.corrcoef(all_voxels, rowvar=1)
+		if np.isnan(np.sum(cov)):
+			cov = np.nan_to_num(cov, copy=True, nan=0.0)
+			print('Warning: All correlations probably NaN. Specified region likely contains no cells.')
 		if override_order is None:
 			if order_method is not None:
 				if not blind_order:
 					d1b, d2b = len(datasets1), len(datasets2)
 					print(f'Group 1: {d1b}, Group 2: {d2b}')
 					mat1 = cov[:d1b,:d1b]
 					mat2 = cov[d1b:,d1b:] # split the matrix up into two sub-matrices
@@ -482,25 +489,27 @@
 	bounds = np.abs(differences).max()
 	regions = dict(zip(areas, differences))
 	cbar_label = 'LS - LV inputs / postsynaptic cell'
 	if limit is not None:
 		bounds = np.abs(limit)
 	bgh.heatmap(regions, position=position, orientation=orientation, thickness=1000, atlas_name='allen_mouse_10um', format='2D', vmin=-bounds, vmax=bounds, cmap=cm.get_cmap(cmap)).show(show_legend=legend, cbar_label=cbar_label)
 
-def generate_heatmap_ratios(areas, orientation, position=None, normalisation='ch1', cmap='bwr', legend=True, limit=None):
+def generate_heatmap_ratios(areas, orientation, position=None, normalisation='ch1', cmap='bwr', legend=True, limit=None, add=False):
 	# orientation: 'frontal', 'sagittal', 'horizontal' or a tuple (x,y,z)
 	group_names = [i.group for i in bt.datasets]
 	if bt.fluorescence:
 		values, cbar_label = _fluorescence_by_area_across_fl_datasets(areas, bt.datasets, normalisation=normalisation)
 	else:
 		values, cbar_label = _cells_in_areas_in_datasets(areas, bt.datasets, normalisation=normalisation)
 	groups, cells = _compress_into_groups(group_names, values)
 	cells = np.array(cells)
 	print(cells[cells==0])
 	ratios = cells[0] / cells[1]
+	if add:
+		ratios = (cells[0] / cells[1]) + 1
 	differences = np.log10(ratios, where=ratios > 0) # calculate log ratio rather than absolute difference
 	bounds = np.abs(differences).max()
 	regions = dict(zip(areas, differences))
 	cbar_label = 'LS - LV inputs / postsynaptic cell'
 	if limit is not None:
 		bounds = np.abs(limit)
 	bgh.heatmap(regions, position=position, orientation=orientation, thickness=1000, atlas_name='allen_mouse_10um', format='2D', vmin=-bounds, vmax=bounds, cmap=cm.get_cmap(cmap)).show(show_legend=legend, cbar_label=cbar_label)
@@ -533,34 +542,39 @@
 	print(areas)
 	highest_value = np.max(cells) # remove regions in the bottom 1% from plot
 	g1_regions = dict(zip(areas, cells[0]))
 	g2_regions = dict(zip(areas, cells[1]))
 	bgh.heatmap(g1_regions, position=position, orientation='frontal', title=groups[0], thickness=1000, atlas_name='allen_mouse_10um', format='2D', vmin=0, vmax=highest_value, cmap=cm.get_cmap('hot')).show(show_legend=True, cbar_label=cbar_label)
 	bgh.heatmap(g2_regions, position=position, orientation='frontal', title=groups[1], thickness=1000, atlas_name='allen_mouse_10um', format='2D', vmin=0, vmax=highest_value, cmap=cm.get_cmap('hot')).show(show_legend=True, cbar_label=cbar_label)
 
-def generate_brain_overview(dataset, vmin=5, top_down=False, cmap='gray', ax=None):
+def generate_brain_overview(dataset, vmin=None, top_down=False, cmap='gray', ax=None):
 	if ax is None:
 		f, ax = plt.subplots(figsize=(10,6))
 		f.set_facecolor('white')
-	stack = np.array(btf.open_file(f'reg_{dataset.name}_{dataset.sig[0]}.tiff'))[0]
-	'''
-	nz = np.nonzero(stack)
-	z_min, y_min, x_min = nz[0].min(), nz[1].min(), nz[2].min()
-	z_max, y_max, x_max = nz[0].max(), nz[1].max(), nz[2].max()
-	if bt.debug:
-		print('x:'+str(x_min)+' '+str(x_max)+' y:'+str(y_min)+' '+str(y_max)+' z:'+str(z_min)+' '+str(z_max))
-	#cropped_stack = stack[z_min : z_max, y_min : y_max, x_min : x_max]
-	'''
+	stack = btf.open_registered_stack(dataset)
+	
 	axis = 1 if top_down else 2
-	projection = np.log(stack.max(axis=axis))
+	if dataset.fluorescence:
+		projection = np.log(np.sum(stack, axis=axis))
+	else:
+		projection = np.log(stack.max(axis=axis))
 	projection = projection.astype(int).T
 	im = ax.imshow(projection, vmin=vmin, cmap=cmap)
 	f.colorbar(im, label='log max px value along axis')
 	plt.axis('off')
 
+def generate_anterograde_stack(dataset, axis=0, vbounds=(None,None)):
+	vmin, vmax = vbounds
+	f, (ax1, ax2) = plt.subplots(1,2, figsize=(10,6))
+	f.set_facecolor('white')
+	stack = btf.open_registered_stack(dataset)
+	ax1.imshow(np.max(bt.atlas, axis=0), norm='log', cmap='Reds')
+	ax2.imshow(np.max(bt.reference, axis=0), norm='log', cmap='Reds')
+	ax2.imshow(np.sum(stack, axis=0), norm='log', vmin=vmin, vmax=vmax, cmap='Greys')
+
 def generate_mega_overview_figure(title):
 	f = plt.figure(figsize=(24, 35))
 	gs = f.add_gridspec(60, 30)
 	f.suptitle(title, y=0.92, size='xx-large', weight='bold')
 	f.set_facecolor('white')
 	ax1 = f.add_subplot(gs[0:9, 5:20])
 	ax_totals = f.add_subplot(gs[0:4, 24:27])
```

### Comparing `braintracer-0.1.3/braintracer/sample_data/cells_FR197_Unet_g.csv` & `braintracer-0.1.4/braintracer/sample_data/cells_FR197_Unet_g.csv`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/sample_data/cells_FR197_Unet_r.csv` & `braintracer-0.1.4/braintracer/sample_data/cells_FR197_Unet_r.csv`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/sample_data/cells_FR200_Unet_g.csv` & `braintracer-0.1.4/braintracer/sample_data/cells_FR200_Unet_g.csv`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/sample_data/cells_FR200_Unet_r.csv` & `braintracer-0.1.4/braintracer/sample_data/cells_FR200_Unet_r.csv`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/split_repair.ipynb` & `braintracer-0.1.4/braintracer/split_repair.ipynb`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer/structures.csv` & `braintracer-0.1.4/braintracer/structures.csv`

 * *Files identical despite different names*

### Comparing `braintracer-0.1.3/braintracer.egg-info/PKG-INFO` & `braintracer-0.1.4/braintracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: braintracer
-Version: 0.1.3
+Version: 0.1.4
 Summary: A complete processing pipeline for anatomical neuronal tracing.
 Home-page: https://github.com/samclothier/braintracer
-Download-URL: https://github.com/samclothier/braintracer/archive/refs/tags/0.1.3.tar.gz
+Download-URL: https://github.com/samclothier/braintracer/archive/refs/tags/0.1.4.tar.gz
 Author: Sam Clothier
 Author-email: sam.clothier.18@ucl.ac.uk
 Keywords: neuroscience,tracing,anatomy,brainglobe,cellfinder,brainreg
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `braintracer-0.1.3/braintracer.egg-info/SOURCES.txt` & `braintracer-0.1.4/braintracer.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 braintracer/__init__.py
 braintracer/analysis.py
-braintracer/bt - TODO.sh
+braintracer/anterograde_pipeline.ipynb
 braintracer/bt.bat
+braintracer/bt.sh
 braintracer/bt_visualiser.ipynb
 braintracer/file_management.py
 braintracer/plotting.py
 braintracer/split_repair.ipynb
-braintracer/stack_transform - TODO.py
 braintracer/structures.csv
 braintracer.egg-info/PKG-INFO
 braintracer.egg-info/SOURCES.txt
 braintracer.egg-info/dependency_links.txt
 braintracer.egg-info/requires.txt
 braintracer.egg-info/top_level.txt
 braintracer/sample_data/cells_FR197_Unet_g.csv
```

### Comparing `braintracer-0.1.3/setup.cfg` & `braintracer-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7261 696e 7472 6163 6572 0d0a   = braintracer..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 330d  version = 0.1.3.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 340d  version = 0.1.4.
 00000030: 0a61 7574 686f 7220 3d20 5361 6d20 436c  .author = Sam Cl
 00000040: 6f74 6869 6572 0d0a 6175 7468 6f72 5f65  othier..author_e
 00000050: 6d61 696c 203d 2073 616d 2e63 6c6f 7468  mail = sam.cloth
 00000060: 6965 722e 3138 4075 636c 2e61 632e 756b  ier.18@ucl.ac.uk
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4120 636f 6d70 6c65 7465 2070 726f 6365  A complete proce
 00000090: 7373 696e 6720 7069 7065 6c69 6e65 2066  ssing pipeline f
@@ -19,15 +19,15 @@
 00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f73 616d  //github.com/sam
 00000130: 636c 6f74 6869 6572 2f62 7261 696e 7472  clothier/braintr
 00000140: 6163 6572 0d0a 646f 776e 6c6f 6164 5f75  acer..download_u
 00000150: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
 00000160: 6875 622e 636f 6d2f 7361 6d63 6c6f 7468  hub.com/samcloth
 00000170: 6965 722f 6272 6169 6e74 7261 6365 722f  ier/braintracer/
 00000180: 6172 6368 6976 652f 7265 6673 2f74 6167  archive/refs/tag
-00000190: 732f 302e 312e 332e 7461 722e 677a 0d0a  s/0.1.3.tar.gz..
+00000190: 732f 302e 312e 342e 7461 722e 677a 0d0a  s/0.1.4.tar.gz..
 000001a0: 6b65 7977 6f72 6473 203d 200d 0a09 6e65  keywords = ...ne
 000001b0: 7572 6f73 6369 656e 6365 0d0a 0974 7261  uroscience...tra
 000001c0: 6369 6e67 0d0a 0961 6e61 746f 6d79 0d0a  cing...anatomy..
 000001d0: 0962 7261 696e 676c 6f62 650d 0a09 6365  .brainglobe...ce
 000001e0: 6c6c 6669 6e64 6572 0d0a 0962 7261 696e  llfinder...brain
 000001f0: 7265 670d 0a63 6c61 7373 6966 6965 7273  reg..classifiers
 00000200: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
```

