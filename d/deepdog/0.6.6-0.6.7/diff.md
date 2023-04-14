# Comparing `tmp/deepdog-0.6.6.tar.gz` & `tmp/deepdog-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.6.6.tar", max compression
+gzip compressed data, was "deepdog-0.6.7.tar", max compression
```

## Comparing `deepdog-0.6.6.tar` & `deepdog-0.6.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0       73 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/meta.py
--rw-r--r--   0        0        0     6655 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     6576 2023-04-09 23:13:34.475057 deepdog-0.6.6/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      895 2023-04-09 23:13:34.479057 deepdog-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      630 2023-04-09 23:15:03.630427 deepdog-0.6.6/setup.py
--rw-r--r--   0        0        0      408 2023-04-09 23:15:03.630786 deepdog-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0       73 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/meta.py
+-rw-r--r--   0        0        0     6873 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     6794 2023-04-14 01:26:39.662616 deepdog-0.6.7/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      895 2023-04-14 01:26:39.666616 deepdog-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      630 2023-04-14 01:27:49.567318 deepdog-0.6.7/setup.py
+-rw-r--r--   0        0        0      408 2023-04-14 01:27:49.567639 deepdog-0.6.7/PKG-INFO
```

### Comparing `deepdog-0.6.6/deepdog/bayes_run.py` & `deepdog-0.6.7/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.6/deepdog/bayes_run_simulpairs.py` & `deepdog-0.6.7/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.6.6/deepdog/real_spectrum_run.py` & `deepdog-0.6.7/deepdog/real_spectrum_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 		monte_carlo_count: int = 10000,
 		monte_carlo_cycles: int = 10,
 		target_success: int = 100,
 		max_monte_carlo_cycles_steps: int = 10,
 		chunksize: int = CHUNKSIZE,
 		initial_seed: int = 12345,
 		use_fast_filter: bool = True,
+		cap_core_count: int = 0,
 	) -> None:
 		self.measurements = measurements
 		self.dot_inputs = [(measure.r, measure.f) for measure in self.measurements]
 
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
 			self.dot_inputs
 		)
@@ -119,14 +120,16 @@
 		self.use_fast_filter = use_fast_filter
 		ff_string = "no_fast_filter"
 		if self.use_fast_filter:
 			ff_string = "fast_filter"
 		self.filename = f"{timestamp}-{filename_slug}.realdata.{ff_string}.bayesrun.csv"
 		self.initial_seed = initial_seed
 
+		self.cap_core_count = cap_core_count
+
 	def go(self) -> None:
 		with open(self.filename, "a", newline="") as outfile:
 			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
 			writer.writeheader()
 
 		(
 			lows,
@@ -136,19 +139,22 @@
 		)
 
 		# define a new seed sequence for each run
 		seed_sequence = numpy.random.SeedSequence(self.initial_seed)
 
 		results = []
 		_logger.debug("Going to iterate over models now")
+		core_count = multiprocessing.cpu_count() - 1 or 1
+		if (self.cap_core_count >= 1) and (self.cap_core_count < core_count):
+			core_count = self.cap_core_count
+		_logger.info(f"Using {core_count} cores")
 		for model_count, (model, model_name) in enumerate(
 			zip(self.models, self.model_names)
 		):
 			_logger.debug(f"Doing model #{model_count}: {model_name}")
-			core_count = multiprocessing.cpu_count() - 1 or 1
 			with multiprocessing.Pool(core_count) as pool:
 				cycle_count = 0
 				cycle_success = 0
 				cycles = 0
 				while (cycles < self.max_monte_carlo_cycles_steps) and (
 					cycle_success <= self.target_success
 				):
```

### Comparing `deepdog-0.6.6/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.6.7/deepdog/temp_aware_real_spectrum_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 		filename_slug: str,
 		monte_carlo_count: int = 10000,
 		monte_carlo_cycles: int = 10,
 		target_success: int = 100,
 		max_monte_carlo_cycles_steps: int = 10,
 		chunksize: int = CHUNKSIZE,
 		initial_seed: int = 12345,
+		cap_core_count: int = 0,
 	) -> None:
 		self.measurements_dict = measurements_dict
 		self.dot_inputs_dict = {
 			k: [(measure.r, measure.f) for measure in measurements]
 			for k, measurements in measurements_dict.items()
 		}
 
@@ -122,14 +123,16 @@
 		self.probabilities = [1 / self.model_count] * self.model_count
 
 		timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
 		ff_string = "fast_filter"
 		self.filename = f"{timestamp}-{filename_slug}.realdata.{ff_string}.bayesrun.csv"
 		self.initial_seed = initial_seed
 
+		self.cap_core_count = cap_core_count
+
 	def go(self) -> None:
 		with open(self.filename, "a", newline="") as outfile:
 			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
 			writer.writeheader()
 
 		low_high_dict = {}
 		for temp, measurements in self.measurements_dict.items():
@@ -142,19 +145,22 @@
 			low_high_dict[temp] = (lows, highs)
 
 		# define a new seed sequence for each run
 		seed_sequence = numpy.random.SeedSequence(self.initial_seed)
 
 		results = []
 		_logger.debug("Going to iterate over models now")
+		core_count = multiprocessing.cpu_count() - 1 or 1
+		if (self.cap_core_count >= 1) and (self.cap_core_count < core_count):
+			core_count = self.cap_core_count
+		_logger.info(f"Using {core_count} cores")
 		for model_count, (model, model_name) in enumerate(
 			zip(self.models, self.model_names)
 		):
 			_logger.debug(f"Doing model #{model_count}: {model_name}")
-			core_count = multiprocessing.cpu_count() - 1 or 1
 			with multiprocessing.Pool(core_count) as pool:
 				cycle_count = 0
 				cycle_success = 0
 				cycles = 0
 				while (cycles < self.max_monte_carlo_cycles_steps) and (
 					cycle_success <= self.target_success
 				):
```

### Comparing `deepdog-0.6.6/pyproject.toml` & `deepdog-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.6.6"
+version = "0.6.7"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.10"
 pdme = "^0.8.6"
 numpy = "1.22.3"
```

### Comparing `deepdog-0.6.6/setup.py` & `deepdog-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.22.3', 'pdme>=0.8.6,<0.9.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.6.6',
+    'version': '0.6.7',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

