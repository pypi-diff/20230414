# Comparing `tmp/dask_histogram-2023.4.0.tar.gz` & `tmp/dask_histogram-2023.4.1.tar.gz`

## Comparing `dask_histogram-2023.4.0.tar` & `dask_histogram-2023.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29132 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/config.py
--rw-r--r--   0        0        0    36197 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/README.md
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29278 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    39039 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.1/PKG-INFO
```

### Comparing `dask_histogram-2023.4.0/src/dask_histogram/__init__.py` & `dask_histogram-2023.4.1/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/src/dask_histogram/bins.py` & `dask_histogram-2023.4.1/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/src/dask_histogram/boost.py` & `dask_histogram-2023.4.1/src/dask_histogram/boost.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,19 @@
         metadata: Any = None,
     ) -> None:
         """Construct a Histogram object."""
         super().__init__(*axes, storage=storage, metadata=metadata)
         self._staged: AggHistogram | None = None
         self._dask_name: str | None = None
         self._dask: HighLevelGraph | None = None
+        self._histref = (
+            axes if isinstance(axes, tuple) else (axes,),
+            storage,
+            metadata,
+        )
 
     def __iadd__(self, other):
         if self.staged_fills() and other.staged_fills():
             self._staged += other._staged
         elif not self.staged_fills() and other.staged_fills():
             self._staged = other._staged
         if self.staged_fills():
@@ -240,15 +245,15 @@
         elif len(args) == 1 and args[0].ndim == 2:
             pass
         elif len(args) > 1:
             pass
         else:
             raise ValueError(f"Cannot interpret input data: {args}")
 
-        new_fill = factory(*args, histref=self, weights=weight, sample=sample)
+        new_fill = factory(*args, histref=self._histref, weights=weight, sample=sample)
         if self._staged is None:
             self._staged = new_fill
         else:
             self._staged += new_fill
         self._dask = self._staged.__dask_graph__()
         self._dask_name = self._staged.name
```

### Comparing `dask_histogram-2023.4.0/src/dask_histogram/core.py` & `dask_histogram-2023.4.1/src/dask_histogram/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,145 +56,203 @@
 
 def _blocked_sa(
     data: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; single argument; unweighted; no sample."""
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
     if data.ndim == 1:
-        return clone(histref).fill(data)
+        return thehist.fill(data)
     elif data.ndim == 2:
-        return clone(histref).fill(*(data.T))
+        return thehist.fill(*(data.T))
     else:
         raise ValueError("Data must be one or two dimensional.")
 
 
 def _blocked_sa_s(
     data: Any,
     sample: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; single argument; unweighted; with sample."""
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
     if data.ndim == 1:
-        return clone(histref).fill(data, sample=sample)
+        return thehist.fill(data, sample=sample)
     elif data.ndim == 2:
-        return clone(histref).fill(*(data.T), sample=sample)
+        return thehist.fill(*(data.T), sample=sample)
     else:
         raise ValueError("Data must be one or two dimensional.")
 
 
 def _blocked_sa_w(
     data: Any,
     weights: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; single argument; weighted; no sample."""
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
     if data.ndim == 1:
-        return clone(histref).fill(data, weight=weights)
+        return thehist.fill(data, weight=weights)
     elif data.ndim == 2:
-        return clone(histref).fill(*(data.T), weight=weights)
+        return thehist.fill(*(data.T), weight=weights)
     else:
         raise ValueError("Data must be one or two dimensional.")
 
 
 def _blocked_sa_w_s(
     data: Any,
     weights: Any,
     sample: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; single argument; weighted; with sample."""
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
     if data.ndim == 1:
-        return clone(histref).fill(data, weight=weights, sample=sample)
+        return thehist.fill(data, weight=weights, sample=sample)
     elif data.ndim == 2:
-        return clone(histref).fill(*(data.T), weight=weights, sample=sample)
+        return thehist.fill(*(data.T), weight=weights, sample=sample)
     else:
         raise ValueError("Data must be one or two dimensional.")
 
 
 def _blocked_ma(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; multiargument; unweighted; no sample."""
-    return clone(histref).fill(*data)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*data)
 
 
 def _blocked_ma_s(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; multiargument; unweighted; with sample."""
     sample = data[-1]
     data = data[:-1]
-    return clone(histref).fill(*data, sample=sample)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*data, sample=sample)
 
 
 def _blocked_ma_w(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; multiargument; weighted; no sample."""
     weights = data[-1]
     data = data[:-1]
-    return clone(histref).fill(*data, weight=weights)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*data, weight=weights)
 
 
 def _blocked_ma_w_s(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; multiargument; weighted; with sample."""
     weights = data[-2]
     sample = data[-1]
     data = data[:-2]
-    return clone(histref).fill(*data, weight=weights, sample=sample)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*data, weight=weights, sample=sample)
 
 
 def _blocked_df(
     data: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
-    return clone(histref).fill(*(data[c] for c in data.columns), weight=None)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*(data[c] for c in data.columns), weight=None)
 
 
 def _blocked_df_s(
     data: Any,
     sample: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
-    return clone(histref).fill(*(data[c] for c in data.columns), sample=sample)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*(data[c] for c in data.columns), sample=sample)
 
 
 def _blocked_df_w(
     data: Any,
     weights: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; single argument; weighted; no sample."""
-    return clone(histref).fill(*(data[c] for c in data.columns), weight=weights)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*(data[c] for c in data.columns), weight=weights)
 
 
 def _blocked_df_w_s(
     data: Any,
     weights: Any,
     sample: Any,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     """Blocked calculation; single argument; weighted; with sample."""
-    return clone(histref).fill(
-        *(data[c] for c in data.columns), weight=weights, sample=sample
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
     )
+    return thehist.fill(*(data[c] for c in data.columns), weight=weights, sample=sample)
 
 
 def _blocked_dak(
     data: Any,
     weights: Any | None,
     sample: Any | None,
     *,
@@ -213,30 +271,40 @@
         theweights.layout._touch_data(recursive=True)
         theweights = weights.layout.form.length_zero_array()
 
     if isinstance(thesample, ak.Array) and ak.backend(thesample) == "typetracer":
         thesample.layout._touch_data(recursive=True)
         thesample = sample.layout.form.length_zero_array()
 
-    return clone(histref).fill(thedata, weight=theweights, sample=thesample)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(thedata, weight=theweights, sample=thesample)
 
 
 def _blocked_dak_ma(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
 
     thedata = list(data)
     for idata, adatum in enumerate(thedata):
         if isinstance(adatum, ak.Array) and ak.backend(adatum) == "typetracer":
             adatum.layout._touch_data(recursive=True)
             thedata[idata] = adatum.layout.form.length_zero_array()
 
-    return clone(histref).fill(*tuple(thedata))
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*tuple(thedata))
 
 
 def _blocked_dak_ma_w(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
@@ -248,15 +316,20 @@
             adatum.layout._touch_data(recursive=True)
             thedata[idata] = adatum.layout.form.length_zero_array()
 
     if isinstance(theweights, ak.Array) and ak.backend(theweights) == "typetracer":
         theweights.layout._touch_data(recursive=True)
         theweights = data[-1].layout.form.length_zero_array()
 
-    return clone(histref).fill(*tuple(thedata), weight=theweights)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*tuple(thedata), weight=theweights)
 
 
 def _blocked_dak_ma_s(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
@@ -268,15 +341,20 @@
             adatum.layout._touch_data(recursive=True)
             thedata[idata] = adatum.layout.form.length_zero_array()
 
     if isinstance(thesample, ak.Array) and ak.backend(thesample) == "typetracer":
         thesample.layout._touch_data(recursive=True)
         thesample = data[-1].layout.form.length_zero_array()
 
-    return clone(histref).fill(*tuple(thedata), sample=thesample)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*tuple(thedata), sample=thesample)
 
 
 def _blocked_dak_ma_w_s(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
@@ -293,15 +371,20 @@
         theweights.layout._touch_data(recursive=True)
         theweights = data[-2].layout.form.length_zero_array()
 
     if isinstance(thesample, ak.Array) and ak.backend(thesample) == "typetracer":
         thesample.layout._touch_data(recursive=True)
         thesample = data[-1].layout.form.length_zero_array()
 
-    return clone(histref).fill(*tuple(thedata), weight=theweights, sample=thesample)
+    thehist = (
+        clone(histref)
+        if not isinstance(histref, tuple)
+        else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
+    )
+    return thehist.fill(*tuple(thedata), weight=theweights, sample=thesample)
 
 
 def optimize(
     dsk: Mapping,
     keys: Hashable | list[Hashable] | set[Hashable],
     **kwargs: Any,
 ) -> Mapping:
@@ -899,27 +982,32 @@
         arrays will not be stored in a list (`histogram2d` style
         return).
 
     """
     from dask.array import Array, asarray
 
     name = f"to-dask-array-{tokenize(agghist)}"
-    zeros = (0,) * agghist.histref.ndim
+    thehist = agghist.histref
+    if isinstance(thehist, tuple):
+        thehist = bh.Histogram(
+            *agghist.histref[0], storage=agghist.histref[1], metadata=agghist.histref[2]
+        )
+    zeros = (0,) * thehist.ndim
     dsk = {(name, *zeros): (lambda x, f: x.to_numpy(flow=f)[0], agghist.name, flow)}
     graph = HighLevelGraph.from_collections(name, dsk, dependencies=(agghist,))
-    shape = agghist.histref.shape
+    shape = thehist.shape
     if flow:
         shape = tuple(i + 2 for i in shape)
-    int_storage = agghist.histref.storage_type in (
+    int_storage = thehist.storage_type in (
         bh.storage.Int64,
         bh.storage.AtomicInt64,
     )
     dt = int if int_storage else float
     c = Array(graph, name=name, shape=shape, chunks=shape, dtype=dt)
-    axes = agghist.histref.axes
+    axes = thehist.axes
 
     if flow:
         edges = [
             asarray(np.concatenate([[-np.inf], ax.edges, [np.inf]])) for ax in axes
         ]
     else:
         edges = [asarray(ax.edges) for ax in axes]
```

### Comparing `dask_histogram-2023.4.0/src/dask_histogram/routines.py` & `dask_histogram-2023.4.1/src/dask_histogram/routines.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/src/dask_histogram/sizeof.py` & `dask_histogram-2023.4.1/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/.gitignore` & `dask_histogram-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/LICENSE` & `dask_histogram-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/README.md` & `dask_histogram-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/pyproject.toml` & `dask_histogram-2023.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.0/PKG-INFO` & `dask_histogram-2023.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
```

