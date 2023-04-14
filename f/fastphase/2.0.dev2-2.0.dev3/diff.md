# Comparing `tmp/fastphase-2.0.dev2.tar.gz` & `tmp/fastphase-2.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fastphase-2.0.dev2.tar", last modified: Tue Jun 23 14:55:34 2020, max compression
+gzip compressed data, was "dist/fastphase-2.0.dev3.tar", last modified: Wed Jun 24 12:14:12 2020, max compression
```

## Comparing `fastphase-2.0.dev2.tar` & `fastphase-2.0.dev3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-06-23 14:55:34.353598 fastphase-2.0.dev2/
--rw-r-----   0 bservin   (1000) biomath   (1001)     1096 2020-06-23 14:55:34.353598 fastphase-2.0.dev2/PKG-INFO
--rw-r-----   0 bservin   (1000) biomath   (1001)      423 2020-05-07 14:04:40.000000 fastphase-2.0.dev2/README.md
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-06-23 14:55:34.337598 fastphase-2.0.dev2/fastphase/
--rw-r-----   0 bservin   (1000) biomath   (1001)        0 2020-05-07 14:04:40.000000 fastphase-2.0.dev2/fastphase/__init__.py
--rw-r-----   0 bservin   (1000) biomath   (1001)  1127303 2020-06-12 06:27:26.000000 fastphase-2.0.dev2/fastphase/calc_func.c
--rw-r-----   0 bservin   (1000) biomath   (1001)    30640 2020-06-12 06:27:10.000000 fastphase-2.0.dev2/fastphase/calc_func.pyx
--rw-r-----   0 bservin   (1000) biomath   (1001)  1916336 2020-06-23 14:50:55.000000 fastphase-2.0.dev2/fastphase/fastphase.c
--rw-r-----   0 bservin   (1000) biomath   (1001)    49053 2020-06-23 14:42:52.000000 fastphase-2.0.dev2/fastphase/fastphase.pyx
--rw-r-----   0 bservin   (1000) biomath   (1001)    21102 2020-06-23 14:42:42.000000 fastphase-2.0.dev2/fastphase/fastphase_ray.py
--rw-r-----   0 bservin   (1000) biomath   (1001)     3537 2020-06-23 14:11:58.000000 fastphase-2.0.dev2/fastphase/fphparams.py
--rw-r-----   0 bservin   (1000) biomath   (1001)     3537 2020-06-23 14:42:31.000000 fastphase-2.0.dev2/fastphase/params.py
-drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-06-23 14:55:34.349598 fastphase-2.0.dev2/fastphase.egg-info/
--rw-r-----   0 bservin   (1000) biomath   (1001)     1096 2020-06-23 14:55:33.000000 fastphase-2.0.dev2/fastphase.egg-info/PKG-INFO
--rw-r-----   0 bservin   (1000) biomath   (1001)      366 2020-06-23 14:55:34.000000 fastphase-2.0.dev2/fastphase.egg-info/SOURCES.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)        1 2020-06-23 14:55:33.000000 fastphase-2.0.dev2/fastphase.egg-info/dependency_links.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)       23 2020-06-23 14:55:33.000000 fastphase-2.0.dev2/fastphase.egg-info/requires.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)       10 2020-06-23 14:55:33.000000 fastphase-2.0.dev2/fastphase.egg-info/top_level.txt
--rw-r-----   0 bservin   (1000) biomath   (1001)       38 2020-06-23 14:55:34.353598 fastphase-2.0.dev2/setup.cfg
--rw-r-----   0 bservin   (1000) biomath   (1001)     2183 2020-06-23 14:55:02.000000 fastphase-2.0.dev2/setup.py
+drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-06-24 12:14:12.943637 fastphase-2.0.dev3/
+-rw-r-----   0 bservin   (1000) biomath   (1001)     1096 2020-06-24 12:14:12.939638 fastphase-2.0.dev3/PKG-INFO
+-rw-r-----   0 bservin   (1000) biomath   (1001)      423 2020-05-07 14:04:40.000000 fastphase-2.0.dev3/README.md
+drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-06-24 12:14:12.927637 fastphase-2.0.dev3/fastphase/
+-rw-r-----   0 bservin   (1000) biomath   (1001)        0 2020-05-07 14:04:40.000000 fastphase-2.0.dev3/fastphase/__init__.py
+-rw-r-----   0 bservin   (1000) biomath   (1001)  1111308 2020-06-24 12:12:11.000000 fastphase-2.0.dev3/fastphase/calc_func.c
+-rw-r-----   0 bservin   (1000) biomath   (1001)    30478 2020-06-24 12:08:58.000000 fastphase-2.0.dev3/fastphase/calc_func.pyx
+-rw-r-----   0 bservin   (1000) biomath   (1001)  1901514 2020-06-24 12:07:33.000000 fastphase-2.0.dev3/fastphase/fastphase.c
+-rw-r-----   0 bservin   (1000) biomath   (1001)    48898 2020-06-24 12:02:49.000000 fastphase-2.0.dev3/fastphase/fastphase.pyx
+-rw-r-----   0 bservin   (1000) biomath   (1001)    18708 2020-06-24 12:10:00.000000 fastphase-2.0.dev3/fastphase/fastphase_ray.py
+-rw-r-----   0 bservin   (1000) biomath   (1001)     3537 2020-06-23 14:11:58.000000 fastphase-2.0.dev3/fastphase/fphparams.py
+-rw-r-----   0 bservin   (1000) biomath   (1001)     3537 2020-06-23 14:42:31.000000 fastphase-2.0.dev3/fastphase/params.py
+drwxr-x---   0 bservin   (1000) biomath   (1001)        0 2020-06-24 12:14:12.939638 fastphase-2.0.dev3/fastphase.egg-info/
+-rw-r-----   0 bservin   (1000) biomath   (1001)     1096 2020-06-24 12:14:12.000000 fastphase-2.0.dev3/fastphase.egg-info/PKG-INFO
+-rw-r-----   0 bservin   (1000) biomath   (1001)      366 2020-06-24 12:14:12.000000 fastphase-2.0.dev3/fastphase.egg-info/SOURCES.txt
+-rw-r-----   0 bservin   (1000) biomath   (1001)        1 2020-06-24 12:14:12.000000 fastphase-2.0.dev3/fastphase.egg-info/dependency_links.txt
+-rw-r-----   0 bservin   (1000) biomath   (1001)       23 2020-06-24 12:14:12.000000 fastphase-2.0.dev3/fastphase.egg-info/requires.txt
+-rw-r-----   0 bservin   (1000) biomath   (1001)       10 2020-06-24 12:14:12.000000 fastphase-2.0.dev3/fastphase.egg-info/top_level.txt
+-rw-r-----   0 bservin   (1000) biomath   (1001)       38 2020-06-24 12:14:12.943637 fastphase-2.0.dev3/setup.cfg
+-rw-r-----   0 bservin   (1000) biomath   (1001)     2183 2020-06-24 12:14:10.000000 fastphase-2.0.dev3/setup.py
```

### Comparing `fastphase-2.0.dev2/PKG-INFO` & `fastphase-2.0.dev3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fastphase
-Version: 2.0.dev2
+Version: 2.0.dev3
 Summary: Python implementation of the fastPHASE model
 Home-page: https://forgemia.inra.fr/bertrand.servin/fastphase
 Author: Bertrand Servin
 Author-email: bertrand.servin@inrae.fr
 License: LGPL v3
 Description: # fastphase
```

### Comparing `fastphase-2.0.dev2/fastphase/calc_func.c` & `fastphase-2.0.dev3/fastphase/calc_func.c`

 * *Files 0% similar despite different names*

```diff
@@ -1835,15 +1835,15 @@
 static int __pyx_f_9fastphase_9calc_func_argmax(PyArrayObject *, int); /*proto*/
 static int __pyx_f_9fastphase_9calc_func_pair2idx(int, int, int); /*proto*/
 static __pyx_ctuple_int__and_int __pyx_f_9fastphase_9calc_func_idx2pair(int, int); /*proto*/
 static double __pyx_f_9fastphase_9calc_func_genprG(double, double, int); /*proto*/
 static double __pyx_f_9fastphase_9calc_func_probJ(int, int, double); /*proto*/
 static PyObject *__pyx_f_9fastphase_9calc_func_genViterbi(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9fastphase_9calc_func_genCalc(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
-static double __pyx_f_9fastphase_9calc_func_likprG(double, double, PyArrayObject *); /*proto*/
+static CYTHON_INLINE double __pyx_f_9fastphase_9calc_func_likprG(double, double, PyArrayObject *); /*proto*/
 static PyObject *__pyx_f_9fastphase_9calc_func_likCalc(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static double __pyx_f_9fastphase_9calc_func_happrG(double, int); /*proto*/
 static PyObject *__pyx_f_9fastphase_9calc_func_hapViterbi(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9fastphase_9calc_func_hapCalc(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
@@ -1864,15 +1864,14 @@
 static const char __pyx_k_k2[] = "k2";
 static const char __pyx_k_kp[] = "kp";
 static const char __pyx_k_ll[] = "ll";
 static const char __pyx_k_nK[] = "nK";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_rr[] = "rr";
 static const char __pyx_k_tt[] = "tt";
-static const char __pyx_k_exp[] = "exp";
 static const char __pyx_k_int[] = "int";
 static const char __pyx_k_kp1[] = "kp1";
 static const char __pyx_k_kp2[] = "kp2";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_u2p[] = "u2p";
 static const char __pyx_k_vit[] = "vit";
 static const char __pyx_k_args[] = "args";
@@ -1922,15 +1921,14 @@
 static PyObject *__pyx_n_s_calc_cost_matrix_geno_tot;
 static PyObject *__pyx_n_s_calc_cost_matrix_haplo;
 static PyObject *__pyx_n_s_calc_cost_matrix_haplo_tot;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_cost_mat;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_empty;
-static PyObject *__pyx_n_s_exp;
 static PyObject *__pyx_n_s_fastphase_calc_func;
 static PyObject *__pyx_kp_s_fastphase_calc_func_pyx;
 static PyObject *__pyx_n_s_float64;
 static PyObject *__pyx_n_s_genCalc;
 static PyObject *__pyx_n_s_genViterbi;
 static PyObject *__pyx_n_s_gg;
 static PyObject *__pyx_n_s_hapCalc;
@@ -9240,232 +9238,67 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/calc_func.pyx":424
- * 
+/* "fastphase/calc_func.pyx":425
  * ########################################### Genotype likelihood Calculations #####################################################
- * cdef double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
- *     cdef double rez
- *     cdef int i
+ * 
+ * cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
+ * 
  */
 
-static double __pyx_f_9fastphase_9calc_func_likprG(double __pyx_v_t1, double __pyx_v_t2, PyArrayObject *__pyx_v_gl) {
-  double __pyx_v_rez;
+static CYTHON_INLINE double __pyx_f_9fastphase_9calc_func_likprG(double __pyx_v_t1, double __pyx_v_t2, PyArrayObject *__pyx_v_gl) {
   __Pyx_LocalBuf_ND __pyx_pybuffernd_gl;
   __Pyx_Buffer __pyx_pybuffer_gl;
   double __pyx_r;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  double __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  Py_ssize_t __pyx_t_9;
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
   __Pyx_RefNannySetupContext("likprG", 0);
   __pyx_pybuffer_gl.pybuffer.buf = NULL;
   __pyx_pybuffer_gl.refcount = 0;
   __pyx_pybuffernd_gl.data = NULL;
   __pyx_pybuffernd_gl.rcbuffer = &__pyx_pybuffer_gl;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_gl.rcbuffer->pybuffer, (PyObject*)__pyx_v_gl, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 424, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_gl.rcbuffer->pybuffer, (PyObject*)__pyx_v_gl, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 425, __pyx_L1_error)
   }
   __pyx_pybuffernd_gl.diminfo[0].strides = __pyx_pybuffernd_gl.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_gl.diminfo[0].shape = __pyx_pybuffernd_gl.rcbuffer->pybuffer.shape[0];
 
-  /* "fastphase/calc_func.pyx":428
- *     cdef int i
+  /* "fastphase/calc_func.pyx":426
  * 
- *     rez = 0.0             # <<<<<<<<<<<<<<
- *     ## g = 0
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)
- */
-  __pyx_v_rez = 0.0;
-
-  /* "fastphase/calc_func.pyx":430
- *     rez = 0.0
- *     ## g = 0
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)             # <<<<<<<<<<<<<<
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
- *     rez += np.exp(gl[2])*t1*t2
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_exp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = 0;
-  if (__pyx_t_4 < 0) __pyx_t_4 += __pyx_pybuffernd_gl.diminfo[0].shape;
-  __pyx_t_2 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_gl.diminfo[0].strides))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble((1.0 - __pyx_v_t1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble((1.0 - __pyx_v_t2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 430, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_rez = __pyx_t_6;
-
-  /* "fastphase/calc_func.pyx":431
- *     ## g = 0
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)             # <<<<<<<<<<<<<<
- *     rez += np.exp(gl[2])*t1*t2
- *     return rez
- */
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rez); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_exp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = 1;
-  if (__pyx_t_7 < 0) __pyx_t_7 += __pyx_pybuffernd_gl.diminfo[0].shape;
-  __pyx_t_2 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_gl.diminfo[0].strides))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-    }
-  }
-  __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(((__pyx_v_t1 * (1.0 - __pyx_v_t2)) + ((1.0 - __pyx_v_t1) * __pyx_v_t2))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 431, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_rez = __pyx_t_6;
-
-  /* "fastphase/calc_func.pyx":432
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
- *     rez += np.exp(gl[2])*t1*t2             # <<<<<<<<<<<<<<
- *     return rez
- * 
- */
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_rez); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_exp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_9 = 2;
-  if (__pyx_t_9 < 0) __pyx_t_9 += __pyx_pybuffernd_gl.diminfo[0].shape;
-  __pyx_t_1 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_gl.diminfo[0].strides))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_t1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_t2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 432, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_rez = __pyx_t_6;
-
-  /* "fastphase/calc_func.pyx":433
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
- *     rez += np.exp(gl[2])*t1*t2
- *     return rez             # <<<<<<<<<<<<<<
+ * cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2             # <<<<<<<<<<<<<<
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):
  */
-  __pyx_r = __pyx_v_rez;
+  __pyx_t_1 = 0;
+  if (__pyx_t_1 < 0) __pyx_t_1 += __pyx_pybuffernd_gl.diminfo[0].shape;
+  __pyx_t_2 = 1;
+  if (__pyx_t_2 < 0) __pyx_t_2 += __pyx_pybuffernd_gl.diminfo[0].shape;
+  __pyx_t_3 = 2;
+  if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_pybuffernd_gl.diminfo[0].shape;
+  __pyx_r = (((((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_gl.diminfo[0].strides)) * (1.0 - __pyx_v_t1)) * (1.0 - __pyx_v_t2)) + ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_2, __pyx_pybuffernd_gl.diminfo[0].strides)) * ((__pyx_v_t1 * (1.0 - __pyx_v_t2)) + ((1.0 - __pyx_v_t1) * __pyx_v_t2)))) + (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_gl.diminfo[0].strides)) * __pyx_v_t1) * __pyx_v_t2));
   goto __pyx_L0;
 
-  /* "fastphase/calc_func.pyx":424
- * 
+  /* "fastphase/calc_func.pyx":425
  * ########################################### Genotype likelihood Calculations #####################################################
- * cdef double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
- *     cdef double rez
- *     cdef int i
+ * 
+ * cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
+ * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_8);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_gl.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
   __Pyx_WriteUnraisable("fastphase.calc_func.likprG", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
@@ -9474,16 +9307,16 @@
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_gl.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/calc_func.pyx":435
- *     return rez
+/* "fastphase/calc_func.pyx":428
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
 
 static PyObject *__pyx_pw_9fastphase_9calc_func_13likCalc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -9773,15 +9606,15 @@
   Py_ssize_t __pyx_t_221;
   Py_ssize_t __pyx_t_222;
   Py_ssize_t __pyx_t_223;
   Py_ssize_t __pyx_t_224;
   Py_ssize_t __pyx_t_225;
   Py_ssize_t __pyx_t_226;
   Py_ssize_t __pyx_t_227;
-  __pyx_t_5numpy_float64_t __pyx_t_228;
+  Py_ssize_t __pyx_t_228;
   Py_ssize_t __pyx_t_229;
   Py_ssize_t __pyx_t_230;
   Py_ssize_t __pyx_t_231;
   Py_ssize_t __pyx_t_232;
   Py_ssize_t __pyx_t_233;
   Py_ssize_t __pyx_t_234;
   Py_ssize_t __pyx_t_235;
@@ -9885,15 +9718,15 @@
   Py_ssize_t __pyx_t_333;
   Py_ssize_t __pyx_t_334;
   Py_ssize_t __pyx_t_335;
   Py_ssize_t __pyx_t_336;
   Py_ssize_t __pyx_t_337;
   Py_ssize_t __pyx_t_338;
   Py_ssize_t __pyx_t_339;
-  Py_ssize_t __pyx_t_340;
+  __pyx_t_5numpy_float64_t __pyx_t_340;
   Py_ssize_t __pyx_t_341;
   Py_ssize_t __pyx_t_342;
   Py_ssize_t __pyx_t_343;
   Py_ssize_t __pyx_t_344;
   Py_ssize_t __pyx_t_345;
   Py_ssize_t __pyx_t_346;
   Py_ssize_t __pyx_t_347;
@@ -9981,617 +9814,617 @@
   __pyx_pybuffernd_top.data = NULL;
   __pyx_pybuffernd_top.rcbuffer = &__pyx_pybuffer_top;
   __pyx_pybuffer_bot.pybuffer.buf = NULL;
   __pyx_pybuffer_bot.refcount = 0;
   __pyx_pybuffernd_bot.data = NULL;
   __pyx_pybuffernd_bot.rcbuffer = &__pyx_pybuffer_bot;
 
-  /* "fastphase/calc_func.pyx":436
+  /* "fastphase/calc_func.pyx":429
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  */
-  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 436, __pyx_L1_error)
+  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 429, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_aa;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alpha.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_alpha = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 436, __pyx_L1_error)
+      __PYX_ERR(0, 429, __pyx_L1_error)
     } else {__pyx_pybuffernd_alpha.diminfo[0].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alpha.diminfo[0].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_alpha.diminfo[1].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_alpha.diminfo[1].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_alpha = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":437
+  /* "fastphase/calc_func.pyx":430
  * cpdef likCalc(aa,tt,rr,ll,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
  */
-  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 437, __pyx_L1_error)
+  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 430, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_tt;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_theta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 437, __pyx_L1_error)
+      __PYX_ERR(0, 430, __pyx_L1_error)
     } else {__pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_theta = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":438
+  /* "fastphase/calc_func.pyx":431
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
  *     cdef int up2pz=u2p
  */
-  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 438, __pyx_L1_error)
+  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 431, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_rr;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rho.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_rho = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 438, __pyx_L1_error)
+      __PYX_ERR(0, 431, __pyx_L1_error)
     } else {__pyx_pybuffernd_rho.diminfo[0].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rho.diminfo[0].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_rho.diminfo[1].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_rho.diminfo[1].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_rho = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":439
+  /* "fastphase/calc_func.pyx":432
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll             # <<<<<<<<<<<<<<
  *     cdef int up2pz=u2p
  * 
  */
-  if (!(likely(((__pyx_v_ll) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_ll, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 439, __pyx_L1_error)
+  if (!(likely(((__pyx_v_ll) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_ll, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 432, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_ll;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_lik.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_lik = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 439, __pyx_L1_error)
+      __PYX_ERR(0, 432, __pyx_L1_error)
     } else {__pyx_pybuffernd_lik.diminfo[0].strides = __pyx_pybuffernd_lik.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_lik.diminfo[0].shape = __pyx_pybuffernd_lik.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_lik.diminfo[1].strides = __pyx_pybuffernd_lik.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_lik.diminfo[1].shape = __pyx_pybuffernd_lik.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_lik = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":440
+  /* "fastphase/calc_func.pyx":433
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
  *     cdef int up2pz=u2p             # <<<<<<<<<<<<<<
  * 
  *     ## cython declarations
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 440, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 433, __pyx_L1_error)
   __pyx_v_up2pz = __pyx_t_2;
 
-  /* "fastphase/calc_func.pyx":452
+  /* "fastphase/calc_func.pyx":445
  *     ## end cython declarations
  * 
  *     nLoc=alpha.shape[0]             # <<<<<<<<<<<<<<
  *     nK=alpha.shape[1]
  *     ##
  */
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_nLoc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":453
+  /* "fastphase/calc_func.pyx":446
  * 
  *     nLoc=alpha.shape[0]
  *     nK=alpha.shape[1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute backward probabilities
  */
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_nK = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":457
+  /* "fastphase/calc_func.pyx":450
  *     ## compute backward probabilities
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_nLoc);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 457, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 457, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 450, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_betaScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_betaScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 457, __pyx_L1_error)
+      __PYX_ERR(0, 450, __pyx_L1_error)
     } else {__pyx_pybuffernd_betaScale.diminfo[0].strides = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_betaScale.diminfo[0].shape = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_betaScale = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/calc_func.pyx":458
+  /* "fastphase/calc_func.pyx":451
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_nK);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 458, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 458, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 451, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tSumk.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_tSumk = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 458, __pyx_L1_error)
+      __PYX_ERR(0, 451, __pyx_L1_error)
     } else {__pyx_pybuffernd_tSumk.diminfo[0].strides = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tSumk.diminfo[0].shape = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_tSumk.diminfo[1].strides = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_tSumk.diminfo[1].shape = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_tSumk = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":459
+  /* "fastphase/calc_func.pyx":452
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_nLoc);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 459, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 459, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 459, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 452, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_tDoubleSum = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 459, __pyx_L1_error)
+      __PYX_ERR(0, 452, __pyx_L1_error)
     } else {__pyx_pybuffernd_tDoubleSum.diminfo[0].strides = __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tDoubleSum.diminfo[0].shape = __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_tDoubleSum = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/calc_func.pyx":460
+  /* "fastphase/calc_func.pyx":453
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for k1 in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_nK);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_nK);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 453, __pyx_L1_error)
   __pyx_t_10 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mBeta.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_mBeta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 460, __pyx_L1_error)
+      __PYX_ERR(0, 453, __pyx_L1_error)
     } else {__pyx_pybuffernd_mBeta.diminfo[0].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mBeta.diminfo[0].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mBeta.diminfo[1].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mBeta.diminfo[1].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_mBeta.diminfo[2].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_mBeta.diminfo[2].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_10 = 0;
   __pyx_v_mBeta = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "fastphase/calc_func.pyx":462
+  /* "fastphase/calc_func.pyx":455
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)
  * 
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             mBeta[nLoc-1,k1,k2]=1
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 462, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 455, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":463
+    /* "fastphase/calc_func.pyx":456
  * 
  *     for k1 in range(nK):
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             mBeta[nLoc-1,k1,k2]=1
  *     ## calc the marginal sum at locus M as in appendix A
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 463, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 456, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":464
+      /* "fastphase/calc_func.pyx":457
  *     for k1 in range(nK):
  *         for k2 in range(nK):
  *             mBeta[nLoc-1,k1,k2]=1             # <<<<<<<<<<<<<<
  *     ## calc the marginal sum at locus M as in appendix A
  *     for k1 in range(nK):
  */
-      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 457, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 457, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 457, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 464, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 457, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
       __pyx_t_4 = 0;
       __pyx_t_3 = 0;
       __pyx_t_5 = 0;
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_1, __pyx_int_1) < 0)) __PYX_ERR(0, 464, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_1, __pyx_int_1) < 0)) __PYX_ERR(0, 457, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
   }
 
-  /* "fastphase/calc_func.pyx":466
+  /* "fastphase/calc_func.pyx":459
  *             mBeta[nLoc-1,k1,k2]=1
  *     ## calc the marginal sum at locus M as in appendix A
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 459, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":467
+    /* "fastphase/calc_func.pyx":460
  *     ## calc the marginal sum at locus M as in appendix A
  *     for k1 in range(nK):
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 467, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":468
+      /* "fastphase/calc_func.pyx":461
  *     for k1 in range(nK):
  *         for k2 in range(nK):
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]             # <<<<<<<<<<<<<<
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]
  *     ## recurrent calculations backward
  */
-      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5);
       __pyx_t_1 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
       __pyx_t_1 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_lik), __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_lik), __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 468, __pyx_L1_error)
-      __pyx_t_6 = PyFloat_FromDouble(__pyx_f_9fastphase_9calc_func_likprG(__pyx_t_16, __pyx_t_17, ((PyArrayObject *)__pyx_t_1))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 461, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble(__pyx_f_9fastphase_9calc_func_likprG(__pyx_t_16, __pyx_t_17, ((PyArrayObject *)__pyx_t_1))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_18 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_18);
       PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_t_18);
       __pyx_t_1 = 0;
       __pyx_t_4 = 0;
       __pyx_t_18 = 0;
-      __pyx_t_18 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __pyx_t_19 = PyNumber_Multiply(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_19 = PyNumber_Multiply(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      __pyx_t_18 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_18);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_18);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_6);
       __pyx_t_18 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyNumber_Multiply(__pyx_t_19, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_4 = PyNumber_Multiply(__pyx_t_19, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3, __pyx_t_6) < 0)) __PYX_ERR(0, 468, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3, __pyx_t_6) < 0)) __PYX_ERR(0, 461, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
 
-    /* "fastphase/calc_func.pyx":469
+    /* "fastphase/calc_func.pyx":462
  *         for k2 in range(nK):
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]             # <<<<<<<<<<<<<<
  *     ## recurrent calculations backward
  *     for m in range(nLoc-1,0,-1):
  */
-    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_5);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_19); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_19); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-    __pyx_t_19 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_GIVEREF(__pyx_t_19);
     PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_t_19);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_4);
     __pyx_t_19 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-    __pyx_t_18 = PyNumber_Multiply(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_18 = PyNumber_Multiply(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 469, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3, __pyx_t_4) < 0)) __PYX_ERR(0, 469, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3, __pyx_t_4) < 0)) __PYX_ERR(0, 462, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
 
-  /* "fastphase/calc_func.pyx":471
+  /* "fastphase/calc_func.pyx":464
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]
  *     ## recurrent calculations backward
  *     for m in range(nLoc-1,0,-1):             # <<<<<<<<<<<<<<
  *         ## these loops could be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  */
-  __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 464, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (__pyx_t_2 = __pyx_t_11; __pyx_t_2 > 0; __pyx_t_2-=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":473
+    /* "fastphase/calc_func.pyx":466
  *     for m in range(nLoc-1,0,-1):
  *         ## these loops could be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(k1,nK):
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  */
-    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L1_error)
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_13; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":474
+      /* "fastphase/calc_func.pyx":467
  *         ## these loops could be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  */
-      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 467, __pyx_L1_error)
       __pyx_t_20 = __pyx_t_14;
       for (__pyx_t_21 = __pyx_v_k1; __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":475
+        /* "fastphase/calc_func.pyx":468
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]
  */
         __pyx_t_22 = __pyx_v_m;
@@ -10604,15 +10437,15 @@
         if (__pyx_t_25 < 0) __pyx_t_25 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         __pyx_t_26 = __pyx_v_m;
         __pyx_t_27 = __pyx_v_k2;
         if (__pyx_t_26 < 0) __pyx_t_26 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_27 < 0) __pyx_t_27 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         __pyx_v_temp = ((0.5 * __pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_rho.diminfo[1].strides)))) * ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_25, __pyx_pybuffernd_tSumk.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":476
+        /* "fastphase/calc_func.pyx":469
  *             for k2 in range(k1,nK):
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]
  */
         __pyx_t_28 = __pyx_v_m;
@@ -10623,27 +10456,27 @@
         __pyx_t_31 = __pyx_v_k1;
         if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_31 < 0) __pyx_t_31 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_32 = __pyx_v_m;
         __pyx_t_33 = __pyx_v_k2;
         if (__pyx_t_32 < 0) __pyx_t_32 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_33 < 0) __pyx_t_33 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 469, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 476, __pyx_L1_error)
+        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 469, __pyx_L1_error)
         __pyx_t_34 = __pyx_v_m;
         __pyx_t_35 = __pyx_v_k1;
         __pyx_t_36 = __pyx_v_k2;
         if (__pyx_t_34 < 0) __pyx_t_34 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_35 < 0) __pyx_t_35 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_36 < 0) __pyx_t_36 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         __pyx_v_temp = (__pyx_v_temp + ((__pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_rho.diminfo[1].strides))) * __pyx_f_9fastphase_9calc_func_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_31, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_3))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_36, __pyx_pybuffernd_mBeta.diminfo[2].strides))));
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "fastphase/calc_func.pyx":477
+        /* "fastphase/calc_func.pyx":470
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]
  *         ## marginal sum and real sum for loc m-1
  */
         __pyx_t_37 = __pyx_v_m;
@@ -10656,15 +10489,15 @@
         __pyx_t_41 = __pyx_v_k1;
         __pyx_t_42 = __pyx_v_k2;
         if (__pyx_t_40 < 0) __pyx_t_40 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_41 < 0) __pyx_t_41 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_42 < 0) __pyx_t_42 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_40, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_41, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_42, __pyx_pybuffernd_mBeta.diminfo[2].strides) = (__pyx_v_temp + (__pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_38, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
 
-        /* "fastphase/calc_func.pyx":478
+        /* "fastphase/calc_func.pyx":471
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]             # <<<<<<<<<<<<<<
  *         ## marginal sum and real sum for loc m-1
  *         for k1 in range(nK):
  */
         __pyx_t_43 = (__pyx_v_m - 1);
@@ -10679,39 +10512,39 @@
         if (__pyx_t_46 < 0) __pyx_t_46 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_47 < 0) __pyx_t_47 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_48 < 0) __pyx_t_48 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_47, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_48, __pyx_pybuffernd_mBeta.diminfo[2].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_43, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_44, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_45, __pyx_pybuffernd_mBeta.diminfo[2].strides));
       }
     }
 
-    /* "fastphase/calc_func.pyx":480
+    /* "fastphase/calc_func.pyx":473
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]
  *         ## marginal sum and real sum for loc m-1
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(nK):
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  */
-    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 473, __pyx_L1_error)
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_13; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":481
+      /* "fastphase/calc_func.pyx":474
  *         ## marginal sum and real sum for loc m-1
  *         for k1 in range(nK):
  *             for k2 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]
  */
-      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 481, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L1_error)
       __pyx_t_20 = __pyx_t_14;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":482
+        /* "fastphase/calc_func.pyx":475
  *         for k1 in range(nK):
  *             for k2 in range(nK):
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]             # <<<<<<<<<<<<<<
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]
  *         tScaleTemp=np.sum(mBeta[m-1])
  */
         __pyx_t_49 = (__pyx_v_m - 1);
@@ -10719,17 +10552,17 @@
         if (__pyx_t_49 < 0) __pyx_t_49 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_50 < 0) __pyx_t_50 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_51 = (__pyx_v_m - 1);
         __pyx_t_52 = __pyx_v_k2;
         if (__pyx_t_51 < 0) __pyx_t_51 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_52 < 0) __pyx_t_52 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_53 = (__pyx_v_m - 1);
-        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_53, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_53, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 482, __pyx_L1_error)
+        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 475, __pyx_L1_error)
         __pyx_t_54 = (__pyx_v_m - 1);
         __pyx_t_55 = __pyx_v_k1;
         __pyx_t_56 = __pyx_v_k2;
         if (__pyx_t_54 < 0) __pyx_t_54 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_55 < 0) __pyx_t_55 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_56 < 0) __pyx_t_56 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         __pyx_t_57 = (__pyx_v_m - 1);
@@ -10740,15 +10573,15 @@
         __pyx_t_60 = __pyx_v_k1;
         if (__pyx_t_59 < 0) __pyx_t_59 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_60 < 0) __pyx_t_60 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_59, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_60, __pyx_pybuffernd_tSumk.diminfo[1].strides) += ((__pyx_f_9fastphase_9calc_func_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_49, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_50, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_51, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_52, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_3)) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_54, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_55, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_56, __pyx_pybuffernd_mBeta.diminfo[2].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_57, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_58, __pyx_pybuffernd_alpha.diminfo[1].strides)));
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
 
-      /* "fastphase/calc_func.pyx":483
+      /* "fastphase/calc_func.pyx":476
  *             for k2 in range(nK):
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]             # <<<<<<<<<<<<<<
  *         tScaleTemp=np.sum(mBeta[m-1])
  *         ## tScaleTemp=0 a gerer <---
  */
       __pyx_t_61 = (__pyx_v_m - 1);
@@ -10760,235 +10593,235 @@
       if (__pyx_t_63 < 0) __pyx_t_63 += __pyx_pybuffernd_alpha.diminfo[0].shape;
       if (__pyx_t_64 < 0) __pyx_t_64 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_65 = (__pyx_v_m - 1);
       if (__pyx_t_65 < 0) __pyx_t_65 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_65, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) += ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_61, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_62, __pyx_pybuffernd_tSumk.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_63, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_64, __pyx_pybuffernd_alpha.diminfo[1].strides)));
     }
 
-    /* "fastphase/calc_func.pyx":484
+    /* "fastphase/calc_func.pyx":477
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]
  *         tScaleTemp=np.sum(mBeta[m-1])             # <<<<<<<<<<<<<<
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 477, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_sum); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_sum); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 477, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_12 = (__pyx_v_m - 1);
-    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_mBeta), __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_mBeta), __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 477, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_18))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_18);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_18);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_18, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_18, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_18, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 477, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-    __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 477, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_tScaleTemp = __pyx_t_17;
 
-    /* "fastphase/calc_func.pyx":486
+    /* "fastphase/calc_func.pyx":479
  *         tScaleTemp=np.sum(mBeta[m-1])
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:             # <<<<<<<<<<<<<<
  *             tScale=20
  *         else:
  */
     __pyx_t_66 = ((__pyx_v_tScaleTemp < 1e-20) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/calc_func.pyx":487
+      /* "fastphase/calc_func.pyx":480
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:
  *             tScale=20             # <<<<<<<<<<<<<<
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))
  */
       __pyx_v_tScale = 20;
 
-      /* "fastphase/calc_func.pyx":486
+      /* "fastphase/calc_func.pyx":479
  *         tScaleTemp=np.sum(mBeta[m-1])
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:             # <<<<<<<<<<<<<<
  *             tScale=20
  *         else:
  */
       goto __pyx_L21;
     }
 
-    /* "fastphase/calc_func.pyx":489
+    /* "fastphase/calc_func.pyx":482
  *             tScale=20
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))             # <<<<<<<<<<<<<<
  *         if tScale <=0:
  *             tScale=0
  */
     /*else*/ {
       __pyx_t_17 = (-log(__pyx_v_tScaleTemp));
       __pyx_t_16 = log(10.0);
       if (unlikely(__pyx_t_16 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 489, __pyx_L1_error)
+        __PYX_ERR(0, 482, __pyx_L1_error)
       }
       __pyx_v_tScale = ((int)(__pyx_t_17 / __pyx_t_16));
     }
     __pyx_L21:;
 
-    /* "fastphase/calc_func.pyx":490
+    /* "fastphase/calc_func.pyx":483
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale <=0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     __pyx_t_66 = ((__pyx_v_tScale <= 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/calc_func.pyx":491
+      /* "fastphase/calc_func.pyx":484
  *             tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale <=0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/calc_func.pyx":490
+      /* "fastphase/calc_func.pyx":483
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale <=0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     }
 
-    /* "fastphase/calc_func.pyx":492
+    /* "fastphase/calc_func.pyx":485
  *         if tScale <=0:
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale             # <<<<<<<<<<<<<<
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_67 = __pyx_v_m;
     if (__pyx_t_67 < 0) __pyx_t_67 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     __pyx_t_68 = (__pyx_v_m - 1);
     if (__pyx_t_68 < 0) __pyx_t_68 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_68, __pyx_pybuffernd_betaScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_67, __pyx_pybuffernd_betaScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-    /* "fastphase/calc_func.pyx":493
+    /* "fastphase/calc_func.pyx":486
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy
  */
     __pyx_t_66 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/calc_func.pyx":494
+      /* "fastphase/calc_func.pyx":487
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             tDoubleSum[m-1]*=dummy
  *             for k1 in range(nK):
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/calc_func.pyx":495
+      /* "fastphase/calc_func.pyx":488
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 tSumk[m-1,k1]*=dummy
  */
       __pyx_t_69 = (__pyx_v_m - 1);
       if (__pyx_t_69 < 0) __pyx_t_69 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_69, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-      /* "fastphase/calc_func.pyx":496
+      /* "fastphase/calc_func.pyx":489
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[m-1,k1]*=dummy
  *                 mBeta[m-1,k1,k1]*=dummy
  */
-      __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 496, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 489, __pyx_L1_error)
       __pyx_t_13 = __pyx_t_12;
       for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_13; __pyx_t_15+=1) {
         __pyx_v_k1 = __pyx_t_15;
 
-        /* "fastphase/calc_func.pyx":497
+        /* "fastphase/calc_func.pyx":490
  *             tDoubleSum[m-1]*=dummy
  *             for k1 in range(nK):
  *                 tSumk[m-1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  */
         __pyx_t_70 = (__pyx_v_m - 1);
         __pyx_t_71 = __pyx_v_k1;
         if (__pyx_t_70 < 0) __pyx_t_70 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_71 < 0) __pyx_t_71 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_70, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_71, __pyx_pybuffernd_tSumk.diminfo[1].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/calc_func.pyx":498
+        /* "fastphase/calc_func.pyx":491
  *             for k1 in range(nK):
  *                 tSumk[m-1,k1]*=dummy
  *                 mBeta[m-1,k1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 for k2 in range(k1+1,nK):
  *                     mBeta[m-1,k1,k2]*=dummy
  */
         __pyx_t_72 = (__pyx_v_m - 1);
         __pyx_t_73 = __pyx_v_k1;
         __pyx_t_74 = __pyx_v_k1;
         if (__pyx_t_72 < 0) __pyx_t_72 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_73 < 0) __pyx_t_73 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_74 < 0) __pyx_t_74 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_72, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_73, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_74, __pyx_pybuffernd_mBeta.diminfo[2].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/calc_func.pyx":499
+        /* "fastphase/calc_func.pyx":492
  *                 tSumk[m-1,k1]*=dummy
  *                 mBeta[m-1,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                     mBeta[m-1,k1,k2]*=dummy
  *                     mBeta[m-1,k2,k1]*=dummy
  */
-        __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 499, __pyx_L1_error)
+        __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 492, __pyx_L1_error)
         __pyx_t_20 = __pyx_t_14;
         for (__pyx_t_21 = (__pyx_v_k1 + 1); __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
           __pyx_v_k2 = __pyx_t_21;
 
-          /* "fastphase/calc_func.pyx":500
+          /* "fastphase/calc_func.pyx":493
  *                 mBeta[m-1,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  *                     mBeta[m-1,k1,k2]*=dummy             # <<<<<<<<<<<<<<
  *                     mBeta[m-1,k2,k1]*=dummy
  *     ##
  */
           __pyx_t_75 = (__pyx_v_m - 1);
           __pyx_t_76 = __pyx_v_k1;
           __pyx_t_77 = __pyx_v_k2;
           if (__pyx_t_75 < 0) __pyx_t_75 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
           if (__pyx_t_76 < 0) __pyx_t_76 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
           if (__pyx_t_77 < 0) __pyx_t_77 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_75, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_76, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_77, __pyx_pybuffernd_mBeta.diminfo[2].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/calc_func.pyx":501
+          /* "fastphase/calc_func.pyx":494
  *                 for k2 in range(k1+1,nK):
  *                     mBeta[m-1,k1,k2]*=dummy
  *                     mBeta[m-1,k2,k1]*=dummy             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute forward probabilities
  */
           __pyx_t_78 = (__pyx_v_m - 1);
@@ -10997,150 +10830,150 @@
           if (__pyx_t_78 < 0) __pyx_t_78 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
           if (__pyx_t_79 < 0) __pyx_t_79 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
           if (__pyx_t_80 < 0) __pyx_t_80 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_78, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_79, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_80, __pyx_pybuffernd_mBeta.diminfo[2].strides) *= __pyx_v_dummy;
         }
       }
 
-      /* "fastphase/calc_func.pyx":493
+      /* "fastphase/calc_func.pyx":486
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy
  */
     }
   }
 
-  /* "fastphase/calc_func.pyx":505
+  /* "fastphase/calc_func.pyx":498
  *     ## compute forward probabilities
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=3] mPhi=np.zeros((nLoc,nK,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     ## at locus 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_nK);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 505, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 498, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 505, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 498, __pyx_L1_error)
   __pyx_t_81 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mPhi.rcbuffer->pybuffer, (PyObject*)__pyx_t_81, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_mPhi = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 505, __pyx_L1_error)
+      __PYX_ERR(0, 498, __pyx_L1_error)
     } else {__pyx_pybuffernd_mPhi.diminfo[0].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mPhi.diminfo[0].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mPhi.diminfo[1].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mPhi.diminfo[1].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_mPhi.diminfo[2].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_mPhi.diminfo[2].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_81 = 0;
   __pyx_v_mPhi = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":506
+  /* "fastphase/calc_func.pyx":499
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=3] mPhi=np.zeros((nLoc,nK,nK),dtype=np.float64)
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     ## at locus 0
  *     for k1 in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_nLoc);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 499, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 506, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 499, __pyx_L1_error)
   __pyx_t_82 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_phiScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_82, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_phiScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 506, __pyx_L1_error)
+      __PYX_ERR(0, 499, __pyx_L1_error)
     } else {__pyx_pybuffernd_phiScale.diminfo[0].strides = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_phiScale.diminfo[0].shape = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_82 = 0;
   __pyx_v_phiScale = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/calc_func.pyx":508
+  /* "fastphase/calc_func.pyx":501
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     ## at locus 0
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(k1,nK):
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 501, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":509
+    /* "fastphase/calc_func.pyx":502
  *     ## at locus 0
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 502, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_k1; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":510
+      /* "fastphase/calc_func.pyx":503
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])             # <<<<<<<<<<<<<<
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]
  *     ## calc the marginal sum at locus 0 (appx A)
  */
       __pyx_t_83 = 0;
@@ -11155,27 +10988,27 @@
       __pyx_t_88 = __pyx_v_k1;
       if (__pyx_t_87 < 0) __pyx_t_87 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_88 < 0) __pyx_t_88 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_89 = 0;
       __pyx_t_90 = __pyx_v_k2;
       if (__pyx_t_89 < 0) __pyx_t_89 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_90 < 0) __pyx_t_90 += __pyx_pybuffernd_theta.diminfo[1].shape;
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 510, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 503, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 510, __pyx_L1_error)
+      if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 503, __pyx_L1_error)
       __pyx_t_91 = 0;
       __pyx_t_92 = __pyx_v_k1;
       __pyx_t_93 = __pyx_v_k2;
       if (__pyx_t_91 < 0) __pyx_t_91 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_92 < 0) __pyx_t_92 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       if (__pyx_t_93 < 0) __pyx_t_93 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
       *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_91, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_92, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_93, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_83, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_84, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_85, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_86, __pyx_pybuffernd_alpha.diminfo[1].strides))) * __pyx_f_9fastphase_9calc_func_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_87, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_88, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_89, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_90, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_6)));
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "fastphase/calc_func.pyx":511
+      /* "fastphase/calc_func.pyx":504
  *         for k2 in range(k1,nK):
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]             # <<<<<<<<<<<<<<
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tDoubleSum[0]=0
  */
       __pyx_t_94 = 0;
@@ -11190,63 +11023,63 @@
       if (__pyx_t_97 < 0) __pyx_t_97 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_98 < 0) __pyx_t_98 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       if (__pyx_t_99 < 0) __pyx_t_99 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
       *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_97, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_98, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_99, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_94, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_95, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_96, __pyx_pybuffernd_mPhi.diminfo[2].strides));
     }
   }
 
-  /* "fastphase/calc_func.pyx":513
+  /* "fastphase/calc_func.pyx":506
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tDoubleSum[0]=0             # <<<<<<<<<<<<<<
  *     for k1 in range(nK):
  *         tSumk[0,k1]=0
  */
   __pyx_t_100 = 0;
   if (__pyx_t_100 < 0) __pyx_t_100 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_100, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) = 0.0;
 
-  /* "fastphase/calc_func.pyx":514
+  /* "fastphase/calc_func.pyx":507
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tDoubleSum[0]=0
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         tSumk[0,k1]=0
  *         for k2 in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 507, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":515
+    /* "fastphase/calc_func.pyx":508
  *     tDoubleSum[0]=0
  *     for k1 in range(nK):
  *         tSumk[0,k1]=0             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  */
     __pyx_t_101 = 0;
     __pyx_t_102 = __pyx_v_k1;
     if (__pyx_t_101 < 0) __pyx_t_101 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
     if (__pyx_t_102 < 0) __pyx_t_102 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_101, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_102, __pyx_pybuffernd_tSumk.diminfo[1].strides) = 0.0;
 
-    /* "fastphase/calc_func.pyx":516
+    /* "fastphase/calc_func.pyx":509
  *     for k1 in range(nK):
  *         tSumk[0,k1]=0
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  *         tDoubleSum[0]+=tSumk[0,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 516, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 509, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":517
+      /* "fastphase/calc_func.pyx":510
  *         tSumk[0,k1]=0
  *         for k2 in range(nK):
  *             tSumk[0,k1]+=mPhi[0,k1,k2]             # <<<<<<<<<<<<<<
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0
  */
       __pyx_t_103 = 0;
@@ -11258,15 +11091,15 @@
       __pyx_t_106 = 0;
       __pyx_t_107 = __pyx_v_k1;
       if (__pyx_t_106 < 0) __pyx_t_106 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
       if (__pyx_t_107 < 0) __pyx_t_107 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_106, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_107, __pyx_pybuffernd_tSumk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_103, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_104, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_105, __pyx_pybuffernd_mPhi.diminfo[2].strides));
     }
 
-    /* "fastphase/calc_func.pyx":518
+    /* "fastphase/calc_func.pyx":511
  *         for k2 in range(nK):
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  *         tDoubleSum[0]+=tSumk[0,k1]             # <<<<<<<<<<<<<<
  *     tScale=0
  *     if tDoubleSum[0] != 0:
  */
     __pyx_t_108 = 0;
@@ -11274,178 +11107,178 @@
     if (__pyx_t_108 < 0) __pyx_t_108 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
     if (__pyx_t_109 < 0) __pyx_t_109 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
     __pyx_t_110 = 0;
     if (__pyx_t_110 < 0) __pyx_t_110 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_110, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_108, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_109, __pyx_pybuffernd_tSumk.diminfo[1].strides));
   }
 
-  /* "fastphase/calc_func.pyx":519
+  /* "fastphase/calc_func.pyx":512
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0             # <<<<<<<<<<<<<<
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  */
   __pyx_v_tScale = 0;
 
-  /* "fastphase/calc_func.pyx":520
+  /* "fastphase/calc_func.pyx":513
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0
  *     if tDoubleSum[0] != 0:             # <<<<<<<<<<<<<<
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:
  */
   __pyx_t_111 = 0;
   if (__pyx_t_111 < 0) __pyx_t_111 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
   __pyx_t_66 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_111, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides)) != 0.0) != 0);
   if (__pyx_t_66) {
 
-    /* "fastphase/calc_func.pyx":521
+    /* "fastphase/calc_func.pyx":514
  *     tScale=0
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))             # <<<<<<<<<<<<<<
  *         if tScale <0:
  *             tScale=0
  */
     __pyx_t_112 = 0;
     if (__pyx_t_112 < 0) __pyx_t_112 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     __pyx_t_16 = (-log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_112, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
     __pyx_t_17 = log(10.0);
     if (unlikely(__pyx_t_17 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 521, __pyx_L1_error)
+      __PYX_ERR(0, 514, __pyx_L1_error)
     }
     __pyx_v_tScale = ((int)(__pyx_t_16 / __pyx_t_17));
 
-    /* "fastphase/calc_func.pyx":522
+    /* "fastphase/calc_func.pyx":515
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[0]=tScale
  */
     __pyx_t_66 = ((__pyx_v_tScale < 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/calc_func.pyx":523
+      /* "fastphase/calc_func.pyx":516
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         phiScale[0]=tScale
  *         if tScale>0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/calc_func.pyx":522
+      /* "fastphase/calc_func.pyx":515
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[0]=tScale
  */
     }
 
-    /* "fastphase/calc_func.pyx":524
+    /* "fastphase/calc_func.pyx":517
  *         if tScale <0:
  *             tScale=0
  *         phiScale[0]=tScale             # <<<<<<<<<<<<<<
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_113 = 0;
     if (__pyx_t_113 < 0) __pyx_t_113 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_113, __pyx_pybuffernd_phiScale.diminfo[0].strides) = __pyx_v_tScale;
 
-    /* "fastphase/calc_func.pyx":525
+    /* "fastphase/calc_func.pyx":518
  *             tScale=0
  *         phiScale[0]=tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):
  */
     __pyx_t_66 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/calc_func.pyx":526
+      /* "fastphase/calc_func.pyx":519
  *         phiScale[0]=tScale
  *         if tScale>0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 tSumk[0,k1]*=dummy
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/calc_func.pyx":527
+      /* "fastphase/calc_func.pyx":520
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[0,k1]*=dummy
  *                 mPhi[0,k1,k1]*=dummy
  */
-      __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 527, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 520, __pyx_L1_error)
       __pyx_t_12 = __pyx_t_11;
       for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
         __pyx_v_k1 = __pyx_t_2;
 
-        /* "fastphase/calc_func.pyx":528
+        /* "fastphase/calc_func.pyx":521
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):
  *                 tSumk[0,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 mPhi[0,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  */
         __pyx_t_114 = 0;
         __pyx_t_115 = __pyx_v_k1;
         if (__pyx_t_114 < 0) __pyx_t_114 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_115 < 0) __pyx_t_115 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_114, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_115, __pyx_pybuffernd_tSumk.diminfo[1].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/calc_func.pyx":529
+        /* "fastphase/calc_func.pyx":522
  *             for k1 in range(nK):
  *                 tSumk[0,k1]*=dummy
  *                 mPhi[0,k1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 for k2 in range(k1+1,nK):
  *                     mPhi[0,k1,k2]*=dummy
  */
         __pyx_t_116 = 0;
         __pyx_t_117 = __pyx_v_k1;
         __pyx_t_118 = __pyx_v_k1;
         if (__pyx_t_116 < 0) __pyx_t_116 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_117 < 0) __pyx_t_117 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_118 < 0) __pyx_t_118 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_116, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_117, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_118, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/calc_func.pyx":530
+        /* "fastphase/calc_func.pyx":523
  *                 tSumk[0,k1]*=dummy
  *                 mPhi[0,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                     mPhi[0,k1,k2]*=dummy
  *                     mPhi[0,k2,k1]*=dummy
  */
-        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 530, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 523, __pyx_L1_error)
         __pyx_t_14 = __pyx_t_13;
         for (__pyx_t_15 = (__pyx_v_k1 + 1); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
           __pyx_v_k2 = __pyx_t_15;
 
-          /* "fastphase/calc_func.pyx":531
+          /* "fastphase/calc_func.pyx":524
  *                 mPhi[0,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  *                     mPhi[0,k1,k2]*=dummy             # <<<<<<<<<<<<<<
  *                     mPhi[0,k2,k1]*=dummy
  *     # do the reccurence
  */
           __pyx_t_119 = 0;
           __pyx_t_120 = __pyx_v_k1;
           __pyx_t_121 = __pyx_v_k2;
           if (__pyx_t_119 < 0) __pyx_t_119 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
           if (__pyx_t_120 < 0) __pyx_t_120 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
           if (__pyx_t_121 < 0) __pyx_t_121 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_119, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_120, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_121, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/calc_func.pyx":532
+          /* "fastphase/calc_func.pyx":525
  *                 for k2 in range(k1+1,nK):
  *                     mPhi[0,k1,k2]*=dummy
  *                     mPhi[0,k2,k1]*=dummy             # <<<<<<<<<<<<<<
  *     # do the reccurence
  *     for m in range(nLoc-1):
  */
           __pyx_t_122 = 0;
@@ -11454,72 +11287,72 @@
           if (__pyx_t_122 < 0) __pyx_t_122 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
           if (__pyx_t_123 < 0) __pyx_t_123 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
           if (__pyx_t_124 < 0) __pyx_t_124 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_122, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_123, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_124, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
         }
       }
 
-      /* "fastphase/calc_func.pyx":525
+      /* "fastphase/calc_func.pyx":518
  *             tScale=0
  *         phiScale[0]=tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):
  */
     }
 
-    /* "fastphase/calc_func.pyx":520
+    /* "fastphase/calc_func.pyx":513
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0
  *     if tDoubleSum[0] != 0:             # <<<<<<<<<<<<<<
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:
  */
   }
 
-  /* "fastphase/calc_func.pyx":534
+  /* "fastphase/calc_func.pyx":527
  *                     mPhi[0,k2,k1]*=dummy
  *     # do the reccurence
  *     for m in range(nLoc-1):             # <<<<<<<<<<<<<<
  *         ## This loop can be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  */
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_6); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 534, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_6); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 527, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":536
+    /* "fastphase/calc_func.pyx":529
  *     for m in range(nLoc-1):
  *         ## This loop can be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 536, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":537
+      /* "fastphase/calc_func.pyx":530
  *         ## This loop can be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 537, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 530, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = __pyx_v_k1; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":538
+        /* "fastphase/calc_func.pyx":531
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]             # <<<<<<<<<<<<<<
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  */
         __pyx_t_125 = (__pyx_v_m + 1);
@@ -11536,28 +11369,28 @@
         if (__pyx_t_130 < 0) __pyx_t_130 += __pyx_pybuffernd_alpha.diminfo[1].shape;
         __pyx_t_131 = __pyx_v_m;
         __pyx_t_132 = __pyx_v_k1;
         if (__pyx_t_131 < 0) __pyx_t_131 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_132 < 0) __pyx_t_132 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_125, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_126, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_127, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_128, __pyx_pybuffernd_tSumk.diminfo[1].strides))) + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_129, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_130, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_131, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_132, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":539
+        /* "fastphase/calc_func.pyx":532
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  */
         __pyx_t_133 = (__pyx_v_m + 1);
         __pyx_t_134 = 0;
         if (__pyx_t_133 < 0) __pyx_t_133 += __pyx_pybuffernd_rho.diminfo[0].shape;
         if (__pyx_t_134 < 0) __pyx_t_134 += __pyx_pybuffernd_rho.diminfo[1].shape;
         __pyx_v_temp = (__pyx_v_temp * (0.5 * __pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_133, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_134, __pyx_pybuffernd_rho.diminfo[1].strides)))));
 
-        /* "fastphase/calc_func.pyx":540
+        /* "fastphase/calc_func.pyx":533
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  */
         __pyx_t_135 = (__pyx_v_m + 1);
@@ -11568,15 +11401,15 @@
         __pyx_t_138 = __pyx_v_k1;
         __pyx_t_139 = __pyx_v_k2;
         if (__pyx_t_137 < 0) __pyx_t_137 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_138 < 0) __pyx_t_138 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_139 < 0) __pyx_t_139 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         __pyx_v_temp = (__pyx_v_temp + (__pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_135, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_136, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_137, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_138, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_139, __pyx_pybuffernd_mPhi.diminfo[2].strides))));
 
-        /* "fastphase/calc_func.pyx":541
+        /* "fastphase/calc_func.pyx":534
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]             # <<<<<<<<<<<<<<
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  */
         __pyx_t_140 = (__pyx_v_m + 1);
@@ -11591,15 +11424,15 @@
         __pyx_t_145 = __pyx_v_k2;
         if (__pyx_t_144 < 0) __pyx_t_144 += __pyx_pybuffernd_alpha.diminfo[0].shape;
         if (__pyx_t_145 < 0) __pyx_t_145 += __pyx_pybuffernd_alpha.diminfo[1].shape;
         __pyx_t_146 = __pyx_v_m;
         if (__pyx_t_146 < 0) __pyx_t_146 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
         __pyx_v_temp = (__pyx_v_temp + (((__pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_140, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_141, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_142, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_143, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_144, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_145, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_146, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
 
-        /* "fastphase/calc_func.pyx":542
+        /* "fastphase/calc_func.pyx":535
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])             # <<<<<<<<<<<<<<
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  *         tDoubleSum[m+1]=0
  */
         __pyx_t_147 = (__pyx_v_m + 1);
@@ -11607,27 +11440,27 @@
         if (__pyx_t_147 < 0) __pyx_t_147 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_148 < 0) __pyx_t_148 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_149 = (__pyx_v_m + 1);
         __pyx_t_150 = __pyx_v_k2;
         if (__pyx_t_149 < 0) __pyx_t_149 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_150 < 0) __pyx_t_150 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_151 = (__pyx_v_m + 1);
-        __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_151, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 542, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_151, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 535, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 542, __pyx_L1_error)
+        if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 535, __pyx_L1_error)
         __pyx_t_152 = (__pyx_v_m + 1);
         __pyx_t_153 = __pyx_v_k1;
         __pyx_t_154 = __pyx_v_k2;
         if (__pyx_t_152 < 0) __pyx_t_152 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_153 < 0) __pyx_t_153 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_154 < 0) __pyx_t_154 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_152, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_153, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_154, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_147, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_148, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_149, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_150, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_6)));
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-        /* "fastphase/calc_func.pyx":543
+        /* "fastphase/calc_func.pyx":536
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]             # <<<<<<<<<<<<<<
  *         tDoubleSum[m+1]=0
  *         for k1 in range(nK):
  */
         __pyx_t_155 = (__pyx_v_m + 1);
@@ -11642,63 +11475,63 @@
         if (__pyx_t_158 < 0) __pyx_t_158 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_159 < 0) __pyx_t_159 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_160 < 0) __pyx_t_160 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_158, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_159, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_160, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_155, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_156, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_157, __pyx_pybuffernd_mPhi.diminfo[2].strides));
       }
     }
 
-    /* "fastphase/calc_func.pyx":544
+    /* "fastphase/calc_func.pyx":537
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  *         tDoubleSum[m+1]=0             # <<<<<<<<<<<<<<
  *         for k1 in range(nK):
  *             tSumk[m+1,k1]=0
  */
     __pyx_t_161 = (__pyx_v_m + 1);
     if (__pyx_t_161 < 0) __pyx_t_161 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_161, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) = 0.0;
 
-    /* "fastphase/calc_func.pyx":545
+    /* "fastphase/calc_func.pyx":538
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  *         tDoubleSum[m+1]=0
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             tSumk[m+1,k1]=0
  *             for k2 in range(nK):
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 545, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 538, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":546
+      /* "fastphase/calc_func.pyx":539
  *         tDoubleSum[m+1]=0
  *         for k1 in range(nK):
  *             tSumk[m+1,k1]=0             # <<<<<<<<<<<<<<
  *             for k2 in range(nK):
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  */
       __pyx_t_162 = (__pyx_v_m + 1);
       __pyx_t_163 = __pyx_v_k1;
       if (__pyx_t_162 < 0) __pyx_t_162 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
       if (__pyx_t_163 < 0) __pyx_t_163 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_162, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_163, __pyx_pybuffernd_tSumk.diminfo[1].strides) = 0.0;
 
-      /* "fastphase/calc_func.pyx":547
+      /* "fastphase/calc_func.pyx":540
  *         for k1 in range(nK):
  *             tSumk[m+1,k1]=0
  *             for k2 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 547, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 540, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":548
+        /* "fastphase/calc_func.pyx":541
  *             tSumk[m+1,k1]=0
  *             for k2 in range(nK):
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]             # <<<<<<<<<<<<<<
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0
  */
         __pyx_t_164 = (__pyx_v_m + 1);
@@ -11710,15 +11543,15 @@
         __pyx_t_167 = (__pyx_v_m + 1);
         __pyx_t_168 = __pyx_v_k1;
         if (__pyx_t_167 < 0) __pyx_t_167 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_168 < 0) __pyx_t_168 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_167, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_168, __pyx_pybuffernd_tSumk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_164, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_165, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_166, __pyx_pybuffernd_mPhi.diminfo[2].strides));
       }
 
-      /* "fastphase/calc_func.pyx":549
+      /* "fastphase/calc_func.pyx":542
  *             for k2 in range(nK):
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]             # <<<<<<<<<<<<<<
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:
  */
       __pyx_t_169 = (__pyx_v_m + 1);
@@ -11726,215 +11559,215 @@
       if (__pyx_t_169 < 0) __pyx_t_169 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
       if (__pyx_t_170 < 0) __pyx_t_170 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
       __pyx_t_171 = (__pyx_v_m + 1);
       if (__pyx_t_171 < 0) __pyx_t_171 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_171, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_169, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_170, __pyx_pybuffernd_tSumk.diminfo[1].strides));
     }
 
-    /* "fastphase/calc_func.pyx":550
+    /* "fastphase/calc_func.pyx":543
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0             # <<<<<<<<<<<<<<
  *         if tDoubleSum[m+1]<=0:
  *             phiScale[m+1]=phiScale[m]
  */
     __pyx_v_tScale = 0;
 
-    /* "fastphase/calc_func.pyx":551
+    /* "fastphase/calc_func.pyx":544
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
     __pyx_t_172 = (__pyx_v_m + 1);
     if (__pyx_t_172 < 0) __pyx_t_172 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     __pyx_t_66 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_172, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides)) <= 0.0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/calc_func.pyx":552
+      /* "fastphase/calc_func.pyx":545
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:
  *             phiScale[m+1]=phiScale[m]             # <<<<<<<<<<<<<<
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  */
       __pyx_t_173 = __pyx_v_m;
       if (__pyx_t_173 < 0) __pyx_t_173 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       __pyx_t_174 = (__pyx_v_m + 1);
       if (__pyx_t_174 < 0) __pyx_t_174 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_174, __pyx_pybuffernd_phiScale.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_173, __pyx_pybuffernd_phiScale.diminfo[0].strides));
 
-      /* "fastphase/calc_func.pyx":551
+      /* "fastphase/calc_func.pyx":544
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
       goto __pyx_L53;
     }
 
-    /* "fastphase/calc_func.pyx":554
+    /* "fastphase/calc_func.pyx":547
  *             phiScale[m+1]=phiScale[m]
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))             # <<<<<<<<<<<<<<
  *             if tScale<0:
  *                 tScale=0
  */
     /*else*/ {
       __pyx_t_175 = (__pyx_v_m + 1);
       if (__pyx_t_175 < 0) __pyx_t_175 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       __pyx_t_17 = (-log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_175, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
       __pyx_t_16 = log(10.0);
       if (unlikely(__pyx_t_16 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 554, __pyx_L1_error)
+        __PYX_ERR(0, 547, __pyx_L1_error)
       }
       __pyx_v_tScale = ((int)(__pyx_t_17 / __pyx_t_16));
 
-      /* "fastphase/calc_func.pyx":555
+      /* "fastphase/calc_func.pyx":548
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  *             if tScale<0:             # <<<<<<<<<<<<<<
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  */
       __pyx_t_66 = ((__pyx_v_tScale < 0) != 0);
       if (__pyx_t_66) {
 
-        /* "fastphase/calc_func.pyx":556
+        /* "fastphase/calc_func.pyx":549
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  *             if tScale<0:
  *                 tScale=0             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:
  */
         __pyx_v_tScale = 0;
 
-        /* "fastphase/calc_func.pyx":555
+        /* "fastphase/calc_func.pyx":548
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  *             if tScale<0:             # <<<<<<<<<<<<<<
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  */
       }
 
-      /* "fastphase/calc_func.pyx":557
+      /* "fastphase/calc_func.pyx":550
  *             if tScale<0:
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale             # <<<<<<<<<<<<<<
  *             if tScale>0:
  *                 dummy=myPow10(tScale)
  */
       __pyx_t_176 = __pyx_v_m;
       if (__pyx_t_176 < 0) __pyx_t_176 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       __pyx_t_177 = (__pyx_v_m + 1);
       if (__pyx_t_177 < 0) __pyx_t_177 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_177, __pyx_pybuffernd_phiScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_176, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-      /* "fastphase/calc_func.pyx":558
+      /* "fastphase/calc_func.pyx":551
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:             # <<<<<<<<<<<<<<
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy
  */
       __pyx_t_66 = ((__pyx_v_tScale > 0) != 0);
       if (__pyx_t_66) {
 
-        /* "fastphase/calc_func.pyx":559
+        /* "fastphase/calc_func.pyx":552
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:
  *                 dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *                 tDoubleSum[m+1]*=dummy
  *                 for k1 in range(nK):
  */
         __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10(__pyx_v_tScale);
 
-        /* "fastphase/calc_func.pyx":560
+        /* "fastphase/calc_func.pyx":553
  *             if tScale>0:
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy             # <<<<<<<<<<<<<<
  *                 for k1 in range(nK):
  *                     tSumk[m+1,k1]*=dummy
  */
         __pyx_t_178 = (__pyx_v_m + 1);
         if (__pyx_t_178 < 0) __pyx_t_178 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
         *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_178, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/calc_func.pyx":561
+        /* "fastphase/calc_func.pyx":554
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy
  *                 for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                     tSumk[m+1,k1]*=dummy
  *                     mPhi[m+1,k1,k1]*=dummy
  */
-        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 554, __pyx_L1_error)
         __pyx_t_14 = __pyx_t_13;
         for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
           __pyx_v_k1 = __pyx_t_15;
 
-          /* "fastphase/calc_func.pyx":562
+          /* "fastphase/calc_func.pyx":555
  *                 tDoubleSum[m+1]*=dummy
  *                 for k1 in range(nK):
  *                     tSumk[m+1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                     mPhi[m+1,k1,k1]*=dummy
  *                     for k2 in range(k1+1,nK):
  */
           __pyx_t_179 = (__pyx_v_m + 1);
           __pyx_t_180 = __pyx_v_k1;
           if (__pyx_t_179 < 0) __pyx_t_179 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
           if (__pyx_t_180 < 0) __pyx_t_180 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_179, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_180, __pyx_pybuffernd_tSumk.diminfo[1].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/calc_func.pyx":563
+          /* "fastphase/calc_func.pyx":556
  *                 for k1 in range(nK):
  *                     tSumk[m+1,k1]*=dummy
  *                     mPhi[m+1,k1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                     for k2 in range(k1+1,nK):
  *                         mPhi[m+1,k1,k2]*=dummy
  */
           __pyx_t_181 = (__pyx_v_m + 1);
           __pyx_t_182 = __pyx_v_k1;
           __pyx_t_183 = __pyx_v_k1;
           if (__pyx_t_181 < 0) __pyx_t_181 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
           if (__pyx_t_182 < 0) __pyx_t_182 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
           if (__pyx_t_183 < 0) __pyx_t_183 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_181, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_182, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_183, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/calc_func.pyx":564
+          /* "fastphase/calc_func.pyx":557
  *                     tSumk[m+1,k1]*=dummy
  *                     mPhi[m+1,k1,k1]*=dummy
  *                     for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                         mPhi[m+1,k1,k2]*=dummy
  *                         mPhi[m+1,k2,k1]*=dummy
  */
-          __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 564, __pyx_L1_error)
+          __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 557, __pyx_L1_error)
           __pyx_t_53 = __pyx_t_20;
           for (__pyx_t_21 = (__pyx_v_k1 + 1); __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
             __pyx_v_k2 = __pyx_t_21;
 
-            /* "fastphase/calc_func.pyx":565
+            /* "fastphase/calc_func.pyx":558
  *                     mPhi[m+1,k1,k1]*=dummy
  *                     for k2 in range(k1+1,nK):
  *                         mPhi[m+1,k1,k2]*=dummy             # <<<<<<<<<<<<<<
  *                         mPhi[m+1,k2,k1]*=dummy
  *     ## end mPhi
  */
             __pyx_t_184 = (__pyx_v_m + 1);
             __pyx_t_185 = __pyx_v_k1;
             __pyx_t_186 = __pyx_v_k2;
             if (__pyx_t_184 < 0) __pyx_t_184 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
             if (__pyx_t_185 < 0) __pyx_t_185 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
             if (__pyx_t_186 < 0) __pyx_t_186 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
             *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_184, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_185, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_186, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-            /* "fastphase/calc_func.pyx":566
+            /* "fastphase/calc_func.pyx":559
  *                     for k2 in range(k1+1,nK):
  *                         mPhi[m+1,k1,k2]*=dummy
  *                         mPhi[m+1,k2,k1]*=dummy             # <<<<<<<<<<<<<<
  *     ## end mPhi
  *     logLikelihood=log(tDoubleSum[nLoc-1])/log(10)-phiScale[nLoc-1]
  */
             __pyx_t_187 = (__pyx_v_m + 1);
@@ -11943,357 +11776,357 @@
             if (__pyx_t_187 < 0) __pyx_t_187 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
             if (__pyx_t_188 < 0) __pyx_t_188 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
             if (__pyx_t_189 < 0) __pyx_t_189 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
             *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_187, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_188, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_189, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
           }
         }
 
-        /* "fastphase/calc_func.pyx":558
+        /* "fastphase/calc_func.pyx":551
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:             # <<<<<<<<<<<<<<
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy
  */
       }
     }
     __pyx_L53:;
   }
 
-  /* "fastphase/calc_func.pyx":568
+  /* "fastphase/calc_func.pyx":561
  *                         mPhi[m+1,k2,k1]*=dummy
  *     ## end mPhi
  *     logLikelihood=log(tDoubleSum[nLoc-1])/log(10)-phiScale[nLoc-1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute Individual Contribution top,bottom,jmk
  */
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_17 = log(__pyx_t_16);
   __pyx_t_16 = log(10.0);
   if (unlikely(__pyx_t_16 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 568, __pyx_L1_error)
+    __PYX_ERR(0, 561, __pyx_L1_error)
   }
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_t_17 / __pyx_t_16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_t_17 / __pyx_t_16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_logLikelihood = __pyx_t_16;
 
-  /* "fastphase/calc_func.pyx":573
+  /* "fastphase/calc_func.pyx":566
  *     ##
  *     # calc ProbZ
  *     cdef np.ndarray[np.float64_t,ndim=3] probZ=mPhi*mBeta             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __pyx_t_6 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 573, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 566, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 573, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 566, __pyx_L1_error)
   __pyx_t_190 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_probZ.rcbuffer->pybuffer, (PyObject*)__pyx_t_190, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_probZ = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 573, __pyx_L1_error)
+      __PYX_ERR(0, 566, __pyx_L1_error)
     } else {__pyx_pybuffernd_probZ.diminfo[0].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_probZ.diminfo[0].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_probZ.diminfo[1].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_probZ.diminfo[1].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_probZ.diminfo[2].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_probZ.diminfo[2].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_190 = 0;
   __pyx_v_probZ = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/calc_func.pyx":574
+  /* "fastphase/calc_func.pyx":567
  *     # calc ProbZ
  *     cdef np.ndarray[np.float64_t,ndim=3] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_int_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_18) < 0) __PYX_ERR(0, 574, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_18) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 574, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_18) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_18, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 574, __pyx_L1_error)
+  if (!(likely(((__pyx_t_18) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_18, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 567, __pyx_L1_error)
   __pyx_t_191 = ((PyArrayObject *)__pyx_t_18);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer, (PyObject*)__pyx_t_191, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_p_g_givX = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 574, __pyx_L1_error)
+      __PYX_ERR(0, 567, __pyx_L1_error)
     } else {__pyx_pybuffernd_p_g_givX.diminfo[0].strides = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_p_g_givX.diminfo[0].shape = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_p_g_givX.diminfo[1].strides = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_p_g_givX.diminfo[1].shape = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_191 = 0;
   __pyx_v_p_g_givX = ((PyArrayObject *)__pyx_t_18);
   __pyx_t_18 = 0;
 
-  /* "fastphase/calc_func.pyx":575
+  /* "fastphase/calc_func.pyx":568
  *     cdef np.ndarray[np.float64_t,ndim=3] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_18);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_18);
   __pyx_t_18 = 0;
-  __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_18, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 575, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_18, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_18); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 575, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_18); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 575, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 568, __pyx_L1_error)
   __pyx_t_192 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_jmk.rcbuffer->pybuffer, (PyObject*)__pyx_t_192, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_jmk = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 575, __pyx_L1_error)
+      __PYX_ERR(0, 568, __pyx_L1_error)
     } else {__pyx_pybuffernd_jmk.diminfo[0].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_jmk.diminfo[0].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_jmk.diminfo[1].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_jmk.diminfo[1].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_192 = 0;
   __pyx_v_jmk = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/calc_func.pyx":576
+  /* "fastphase/calc_func.pyx":569
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  *     ## normalize
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 576, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 576, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 576, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 569, __pyx_L1_error)
   __pyx_t_193 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_top.rcbuffer->pybuffer, (PyObject*)__pyx_t_193, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_top = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_top.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 576, __pyx_L1_error)
+      __PYX_ERR(0, 569, __pyx_L1_error)
     } else {__pyx_pybuffernd_top.diminfo[0].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_top.diminfo[0].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_top.diminfo[1].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_top.diminfo[1].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_193 = 0;
   __pyx_v_top = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":577
+  /* "fastphase/calc_func.pyx":570
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     ## normalize
  *     for m in range(nLoc):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 577, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 577, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 570, __pyx_L1_error)
   __pyx_t_194 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bot.rcbuffer->pybuffer, (PyObject*)__pyx_t_194, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_bot = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 577, __pyx_L1_error)
+      __PYX_ERR(0, 570, __pyx_L1_error)
     } else {__pyx_pybuffernd_bot.diminfo[0].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bot.diminfo[0].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_bot.diminfo[1].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_bot.diminfo[1].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_194 = 0;
   __pyx_v_bot = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/calc_func.pyx":579
+  /* "fastphase/calc_func.pyx":572
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  *     ## normalize
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         normC=0
  *         for k1 in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 579, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 572, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":580
+    /* "fastphase/calc_func.pyx":573
  *     ## normalize
  *     for m in range(nLoc):
  *         normC=0             # <<<<<<<<<<<<<<
  *         for k1 in range(nK):
  *             normC+=probZ[m,k1,k1]
  */
     __pyx_v_normC = 0.0;
 
-    /* "fastphase/calc_func.pyx":581
+    /* "fastphase/calc_func.pyx":574
  *     for m in range(nLoc):
  *         normC=0
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             normC+=probZ[m,k1,k1]
  *             for k2 in range(k1+1,nK):
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 581, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 574, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":582
+      /* "fastphase/calc_func.pyx":575
  *         normC=0
  *         for k1 in range(nK):
  *             normC+=probZ[m,k1,k1]             # <<<<<<<<<<<<<<
  *             for k2 in range(k1+1,nK):
  *                 normC+=2*probZ[m,k1,k2]
  */
       __pyx_t_195 = __pyx_v_m;
       __pyx_t_196 = __pyx_v_k1;
       __pyx_t_197 = __pyx_v_k1;
       if (__pyx_t_195 < 0) __pyx_t_195 += __pyx_pybuffernd_probZ.diminfo[0].shape;
       if (__pyx_t_196 < 0) __pyx_t_196 += __pyx_pybuffernd_probZ.diminfo[1].shape;
       if (__pyx_t_197 < 0) __pyx_t_197 += __pyx_pybuffernd_probZ.diminfo[2].shape;
       __pyx_v_normC = (__pyx_v_normC + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_195, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_196, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_197, __pyx_pybuffernd_probZ.diminfo[2].strides)));
 
-      /* "fastphase/calc_func.pyx":583
+      /* "fastphase/calc_func.pyx":576
  *         for k1 in range(nK):
  *             normC+=probZ[m,k1,k1]
  *             for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                 normC+=2*probZ[m,k1,k2]
  *         probZ[m]/=normC
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 583, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 576, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = (__pyx_v_k1 + 1); __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":584
+        /* "fastphase/calc_func.pyx":577
  *             normC+=probZ[m,k1,k1]
  *             for k2 in range(k1+1,nK):
  *                 normC+=2*probZ[m,k1,k2]             # <<<<<<<<<<<<<<
  *         probZ[m]/=normC
  *     ## Calc P( G| X, pars)
  */
         __pyx_t_198 = __pyx_v_m;
@@ -12302,59 +12135,59 @@
         if (__pyx_t_198 < 0) __pyx_t_198 += __pyx_pybuffernd_probZ.diminfo[0].shape;
         if (__pyx_t_199 < 0) __pyx_t_199 += __pyx_pybuffernd_probZ.diminfo[1].shape;
         if (__pyx_t_200 < 0) __pyx_t_200 += __pyx_pybuffernd_probZ.diminfo[2].shape;
         __pyx_v_normC = (__pyx_v_normC + (2.0 * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_198, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_199, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_200, __pyx_pybuffernd_probZ.diminfo[2].strides))));
       }
     }
 
-    /* "fastphase/calc_func.pyx":585
+    /* "fastphase/calc_func.pyx":578
  *             for k2 in range(k1+1,nK):
  *                 normC+=2*probZ[m,k1,k2]
  *         probZ[m]/=normC             # <<<<<<<<<<<<<<
  *     ## Calc P( G| X, pars)
  *     ## Scheet Stephens, 2008, appendix page 5 P(xim|gi)
  */
     __pyx_t_15 = __pyx_v_m;
-    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 585, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 585, __pyx_L1_error)
+    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 585, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, __pyx_t_4, int, 1, __Pyx_PyInt_From_int, 0, 1, 0) < 0)) __PYX_ERR(0, 585, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, __pyx_t_4, int, 1, __Pyx_PyInt_From_int, 0, 1, 0) < 0)) __PYX_ERR(0, 578, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
 
-  /* "fastphase/calc_func.pyx":589
+  /* "fastphase/calc_func.pyx":582
  *     ## Scheet Stephens, 2008, appendix page 5 P(xim|gi)
  *     ## init at 0
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(k1,nK):
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 589, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 582, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":590
+    /* "fastphase/calc_func.pyx":583
  *     ## init at 0
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 590, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 583, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_k1; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":591
+      /* "fastphase/calc_func.pyx":584
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]             # <<<<<<<<<<<<<<
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  */
       __pyx_t_201 = 0;
@@ -12369,15 +12202,15 @@
       __pyx_t_206 = __pyx_v_k1;
       __pyx_t_207 = __pyx_v_k2;
       if (__pyx_t_205 < 0) __pyx_t_205 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_206 < 0) __pyx_t_206 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       if (__pyx_t_207 < 0) __pyx_t_207 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
       __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_201, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_202, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_203, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_204, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_205, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_206, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_207, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
 
-      /* "fastphase/calc_func.pyx":592
+      /* "fastphase/calc_func.pyx":585
  *         for k2 in range(k1,nK):
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)             # <<<<<<<<<<<<<<
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
  */
       __pyx_t_208 = 0;
@@ -12390,20 +12223,20 @@
       if (__pyx_t_211 < 0) __pyx_t_211 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_212 = 0;
       __pyx_t_213 = 0;
       if (__pyx_t_212 < 0) __pyx_t_212 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
       if (__pyx_t_213 < 0) __pyx_t_213 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_212, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_213, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_208, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_209, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_210, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_211, __pyx_pybuffernd_theta.diminfo[1].strides)), 0));
 
-      /* "fastphase/calc_func.pyx":593
+      /* "fastphase/calc_func.pyx":586
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)             # <<<<<<<<<<<<<<
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
+ *     p_g_givX[0,0] *= lik[0,0]
  */
       __pyx_t_214 = 0;
       __pyx_t_215 = __pyx_v_k1;
       if (__pyx_t_214 < 0) __pyx_t_214 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_215 < 0) __pyx_t_215 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_216 = 0;
       __pyx_t_217 = __pyx_v_k2;
@@ -12411,20 +12244,20 @@
       if (__pyx_t_217 < 0) __pyx_t_217 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_218 = 0;
       __pyx_t_219 = 1;
       if (__pyx_t_218 < 0) __pyx_t_218 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
       if (__pyx_t_219 < 0) __pyx_t_219 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_218, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_219, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_214, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_215, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_216, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_217, __pyx_pybuffernd_theta.diminfo[1].strides)), 1));
 
-      /* "fastphase/calc_func.pyx":594
+      /* "fastphase/calc_func.pyx":587
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)             # <<<<<<<<<<<<<<
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
+ *     p_g_givX[0,0] *= lik[0,0]
+ *     p_g_givX[0,1] *= lik[0,1]
  */
       __pyx_t_220 = 0;
       __pyx_t_221 = __pyx_v_k1;
       if (__pyx_t_220 < 0) __pyx_t_220 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_221 < 0) __pyx_t_221 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_222 = 0;
       __pyx_t_223 = __pyx_v_k2;
@@ -12434,856 +12267,706 @@
       __pyx_t_225 = 2;
       if (__pyx_t_224 < 0) __pyx_t_224 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
       if (__pyx_t_225 < 0) __pyx_t_225 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_224, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_225, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_220, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_221, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_222, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_223, __pyx_pybuffernd_theta.diminfo[1].strides)), 2));
     }
   }
 
-  /* "fastphase/calc_func.pyx":595
+  /* "fastphase/calc_func.pyx":588
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
- *     p_g_givX[0,0] *= np.exp(lik[0,0])             # <<<<<<<<<<<<<<
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+ *     p_g_givX[0,0] *= lik[0,0]             # <<<<<<<<<<<<<<
+ *     p_g_givX[0,1] *= lik[0,1]
+ *     p_g_givX[0,2] *= lik[0,2]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_226 = 0;
   __pyx_t_227 = 0;
   if (__pyx_t_226 < 0) __pyx_t_226 += __pyx_pybuffernd_lik.diminfo[0].shape;
   if (__pyx_t_227 < 0) __pyx_t_227 += __pyx_pybuffernd_lik.diminfo[1].shape;
-  __pyx_t_5 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_226, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_227, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_228 = 0;
   __pyx_t_229 = 0;
-  __pyx_t_230 = 0;
-  if (__pyx_t_229 < 0) __pyx_t_229 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_230 < 0) __pyx_t_230 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_229, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_230, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
+  if (__pyx_t_228 < 0) __pyx_t_228 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_229 < 0) __pyx_t_229 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_228, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_229, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_226, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_227, __pyx_pybuffernd_lik.diminfo[1].strides));
 
-  /* "fastphase/calc_func.pyx":596
+  /* "fastphase/calc_func.pyx":589
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
- *     p_g_givX[0,1] *= np.exp(lik[0,1])             # <<<<<<<<<<<<<<
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+ *     p_g_givX[0,0] *= lik[0,0]
+ *     p_g_givX[0,1] *= lik[0,1]             # <<<<<<<<<<<<<<
+ *     p_g_givX[0,2] *= lik[0,2]
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 596, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_exp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 596, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_231 = 0;
-  __pyx_t_232 = 1;
-  if (__pyx_t_231 < 0) __pyx_t_231 += __pyx_pybuffernd_lik.diminfo[0].shape;
-  if (__pyx_t_232 < 0) __pyx_t_232 += __pyx_pybuffernd_lik.diminfo[1].shape;
-  __pyx_t_6 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_231, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_232, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 596, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 596, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 596, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_233 = 0;
-  __pyx_t_234 = 1;
-  if (__pyx_t_233 < 0) __pyx_t_233 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_234 < 0) __pyx_t_234 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_233, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_234, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-  /* "fastphase/calc_func.pyx":597
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
- *     p_g_givX[0,2] *= np.exp(lik[0,2])             # <<<<<<<<<<<<<<
+  __pyx_t_230 = 0;
+  __pyx_t_231 = 1;
+  if (__pyx_t_230 < 0) __pyx_t_230 += __pyx_pybuffernd_lik.diminfo[0].shape;
+  if (__pyx_t_231 < 0) __pyx_t_231 += __pyx_pybuffernd_lik.diminfo[1].shape;
+  __pyx_t_232 = 0;
+  __pyx_t_233 = 1;
+  if (__pyx_t_232 < 0) __pyx_t_232 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_233 < 0) __pyx_t_233 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_232, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_233, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_230, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_231, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+  /* "fastphase/calc_func.pyx":590
+ *     p_g_givX[0,0] *= lik[0,0]
+ *     p_g_givX[0,1] *= lik[0,1]
+ *     p_g_givX[0,2] *= lik[0,2]             # <<<<<<<<<<<<<<
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
  *     p_g_givX[0]/=normC
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 597, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 597, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_235 = 0;
-  __pyx_t_236 = 2;
-  if (__pyx_t_235 < 0) __pyx_t_235 += __pyx_pybuffernd_lik.diminfo[0].shape;
-  if (__pyx_t_236 < 0) __pyx_t_236 += __pyx_pybuffernd_lik.diminfo[1].shape;
-  __pyx_t_5 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_235, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_236, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 597, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 597, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 597, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_237 = 0;
-  __pyx_t_238 = 2;
-  if (__pyx_t_237 < 0) __pyx_t_237 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_238 < 0) __pyx_t_238 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_237, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_238, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-  /* "fastphase/calc_func.pyx":598
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+  __pyx_t_234 = 0;
+  __pyx_t_235 = 2;
+  if (__pyx_t_234 < 0) __pyx_t_234 += __pyx_pybuffernd_lik.diminfo[0].shape;
+  if (__pyx_t_235 < 0) __pyx_t_235 += __pyx_pybuffernd_lik.diminfo[1].shape;
+  __pyx_t_236 = 0;
+  __pyx_t_237 = 2;
+  if (__pyx_t_236 < 0) __pyx_t_236 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_237 < 0) __pyx_t_237 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_236, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_237, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_234, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_235, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+  /* "fastphase/calc_func.pyx":591
+ *     p_g_givX[0,1] *= lik[0,1]
+ *     p_g_givX[0,2] *= lik[0,2]
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]             # <<<<<<<<<<<<<<
  *     p_g_givX[0]/=normC
  * 
  */
+  __pyx_t_238 = 0;
   __pyx_t_239 = 0;
+  if (__pyx_t_238 < 0) __pyx_t_238 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_239 < 0) __pyx_t_239 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
   __pyx_t_240 = 0;
-  if (__pyx_t_239 < 0) __pyx_t_239 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_240 < 0) __pyx_t_240 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  __pyx_t_241 = 0;
-  __pyx_t_242 = 1;
-  if (__pyx_t_241 < 0) __pyx_t_241 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_242 < 0) __pyx_t_242 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  __pyx_t_243 = 0;
-  __pyx_t_244 = 2;
-  if (__pyx_t_243 < 0) __pyx_t_243 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_244 < 0) __pyx_t_244 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_239, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_240, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_241, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_242, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_243, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_244, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
+  __pyx_t_241 = 1;
+  if (__pyx_t_240 < 0) __pyx_t_240 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_241 < 0) __pyx_t_241 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  __pyx_t_242 = 0;
+  __pyx_t_243 = 2;
+  if (__pyx_t_242 < 0) __pyx_t_242 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_243 < 0) __pyx_t_243 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_238, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_239, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_240, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_241, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_242, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_243, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
 
-  /* "fastphase/calc_func.pyx":599
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+  /* "fastphase/calc_func.pyx":592
+ *     p_g_givX[0,2] *= lik[0,2]
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
  *     p_g_givX[0]/=normC             # <<<<<<<<<<<<<<
  * 
  *     for m in range(nLoc-1):
  */
-  __pyx_t_245 = 0;
-  __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_245, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_244 = 0;
+  __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_244, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 599, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 592, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_245, __pyx_t_5, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0) < 0)) __PYX_ERR(0, 599, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_244, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0) < 0)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "fastphase/calc_func.pyx":601
+  /* "fastphase/calc_func.pyx":594
  *     p_g_givX[0]/=normC
  * 
  *     for m in range(nLoc-1):             # <<<<<<<<<<<<<<
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  */
-  __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 601, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_5); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 601, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 594, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_6); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 594, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":602
+    /* "fastphase/calc_func.pyx":595
  * 
  *     for m in range(nLoc-1):
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 602, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 595, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":603
+      /* "fastphase/calc_func.pyx":596
  *     for m in range(nLoc-1):
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 603, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 596, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = __pyx_v_k1; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":604
+        /* "fastphase/calc_func.pyx":597
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]             # <<<<<<<<<<<<<<
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  */
-        __pyx_t_246 = (__pyx_v_m + 1);
-        __pyx_t_247 = __pyx_v_k1;
-        if (__pyx_t_246 < 0) __pyx_t_246 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_247 < 0) __pyx_t_247 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_248 = __pyx_v_m;
-        __pyx_t_249 = __pyx_v_k2;
-        if (__pyx_t_248 < 0) __pyx_t_248 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
-        if (__pyx_t_249 < 0) __pyx_t_249 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
-        __pyx_t_250 = (__pyx_v_m + 1);
-        __pyx_t_251 = __pyx_v_k2;
-        if (__pyx_t_250 < 0) __pyx_t_250 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_251 < 0) __pyx_t_251 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_252 = __pyx_v_m;
-        __pyx_t_253 = __pyx_v_k1;
-        if (__pyx_t_252 < 0) __pyx_t_252 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
-        if (__pyx_t_253 < 0) __pyx_t_253 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
-        __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_246, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_247, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_248, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_249, __pyx_pybuffernd_tSumk.diminfo[1].strides))) + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_250, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_251, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_252, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_253, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
+        __pyx_t_245 = (__pyx_v_m + 1);
+        __pyx_t_246 = __pyx_v_k1;
+        if (__pyx_t_245 < 0) __pyx_t_245 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_246 < 0) __pyx_t_246 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_247 = __pyx_v_m;
+        __pyx_t_248 = __pyx_v_k2;
+        if (__pyx_t_247 < 0) __pyx_t_247 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
+        if (__pyx_t_248 < 0) __pyx_t_248 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
+        __pyx_t_249 = (__pyx_v_m + 1);
+        __pyx_t_250 = __pyx_v_k2;
+        if (__pyx_t_249 < 0) __pyx_t_249 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_250 < 0) __pyx_t_250 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_251 = __pyx_v_m;
+        __pyx_t_252 = __pyx_v_k1;
+        if (__pyx_t_251 < 0) __pyx_t_251 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
+        if (__pyx_t_252 < 0) __pyx_t_252 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
+        __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_245, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_246, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_247, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_248, __pyx_pybuffernd_tSumk.diminfo[1].strides))) + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_249, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_250, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_251, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_252, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":605
+        /* "fastphase/calc_func.pyx":598
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  */
-        __pyx_t_254 = (__pyx_v_m + 1);
-        __pyx_t_255 = 0;
-        if (__pyx_t_254 < 0) __pyx_t_254 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_255 < 0) __pyx_t_255 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_v_temp = (__pyx_v_temp * (0.5 * __pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_254, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_255, __pyx_pybuffernd_rho.diminfo[1].strides)))));
+        __pyx_t_253 = (__pyx_v_m + 1);
+        __pyx_t_254 = 0;
+        if (__pyx_t_253 < 0) __pyx_t_253 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_254 < 0) __pyx_t_254 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_v_temp = (__pyx_v_temp * (0.5 * __pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_253, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_254, __pyx_pybuffernd_rho.diminfo[1].strides)))));
 
-        /* "fastphase/calc_func.pyx":606
+        /* "fastphase/calc_func.pyx":599
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 temp*=mBeta[m+1,k1,k2]
  */
-        __pyx_t_256 = (__pyx_v_m + 1);
-        __pyx_t_257 = 0;
-        if (__pyx_t_256 < 0) __pyx_t_256 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_257 < 0) __pyx_t_257 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_t_258 = __pyx_v_m;
-        __pyx_t_259 = __pyx_v_k1;
-        __pyx_t_260 = __pyx_v_k2;
-        if (__pyx_t_258 < 0) __pyx_t_258 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
-        if (__pyx_t_259 < 0) __pyx_t_259 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
-        if (__pyx_t_260 < 0) __pyx_t_260 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
-        __pyx_v_temp = (__pyx_v_temp + (__pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_256, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_257, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_258, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_259, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_260, __pyx_pybuffernd_mPhi.diminfo[2].strides))));
+        __pyx_t_255 = (__pyx_v_m + 1);
+        __pyx_t_256 = 0;
+        if (__pyx_t_255 < 0) __pyx_t_255 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_256 < 0) __pyx_t_256 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_t_257 = __pyx_v_m;
+        __pyx_t_258 = __pyx_v_k1;
+        __pyx_t_259 = __pyx_v_k2;
+        if (__pyx_t_257 < 0) __pyx_t_257 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
+        if (__pyx_t_258 < 0) __pyx_t_258 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
+        if (__pyx_t_259 < 0) __pyx_t_259 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
+        __pyx_v_temp = (__pyx_v_temp + (__pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_255, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_256, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_257, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_258, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_259, __pyx_pybuffernd_mPhi.diminfo[2].strides))));
 
-        /* "fastphase/calc_func.pyx":607
+        /* "fastphase/calc_func.pyx":600
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]             # <<<<<<<<<<<<<<
  *                 temp*=mBeta[m+1,k1,k2]
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  */
-        __pyx_t_261 = (__pyx_v_m + 1);
-        __pyx_t_262 = 0;
-        if (__pyx_t_261 < 0) __pyx_t_261 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_262 < 0) __pyx_t_262 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_t_263 = (__pyx_v_m + 1);
-        __pyx_t_264 = __pyx_v_k1;
-        if (__pyx_t_263 < 0) __pyx_t_263 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_264 < 0) __pyx_t_264 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_265 = (__pyx_v_m + 1);
-        __pyx_t_266 = __pyx_v_k2;
-        if (__pyx_t_265 < 0) __pyx_t_265 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_266 < 0) __pyx_t_266 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_267 = __pyx_v_m;
-        if (__pyx_t_267 < 0) __pyx_t_267 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
-        __pyx_v_temp = (__pyx_v_temp + (((__pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_261, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_262, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_263, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_264, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_265, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_266, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_267, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
+        __pyx_t_260 = (__pyx_v_m + 1);
+        __pyx_t_261 = 0;
+        if (__pyx_t_260 < 0) __pyx_t_260 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_261 < 0) __pyx_t_261 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_t_262 = (__pyx_v_m + 1);
+        __pyx_t_263 = __pyx_v_k1;
+        if (__pyx_t_262 < 0) __pyx_t_262 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_263 < 0) __pyx_t_263 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_264 = (__pyx_v_m + 1);
+        __pyx_t_265 = __pyx_v_k2;
+        if (__pyx_t_264 < 0) __pyx_t_264 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_265 < 0) __pyx_t_265 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_266 = __pyx_v_m;
+        if (__pyx_t_266 < 0) __pyx_t_266 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
+        __pyx_v_temp = (__pyx_v_temp + (((__pyx_f_9fastphase_9calc_func_probJ((__pyx_v_m + 1), 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_260, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_261, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_262, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_263, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_264, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_265, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_266, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
 
-        /* "fastphase/calc_func.pyx":608
+        /* "fastphase/calc_func.pyx":601
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 temp*=mBeta[m+1,k1,k2]             # <<<<<<<<<<<<<<
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  */
-        __pyx_t_268 = (__pyx_v_m + 1);
-        __pyx_t_269 = __pyx_v_k1;
-        __pyx_t_270 = __pyx_v_k2;
-        if (__pyx_t_268 < 0) __pyx_t_268 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
-        if (__pyx_t_269 < 0) __pyx_t_269 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
-        if (__pyx_t_270 < 0) __pyx_t_270 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
-        __pyx_v_temp = (__pyx_v_temp * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_268, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_269, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_270, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
+        __pyx_t_267 = (__pyx_v_m + 1);
+        __pyx_t_268 = __pyx_v_k1;
+        __pyx_t_269 = __pyx_v_k2;
+        if (__pyx_t_267 < 0) __pyx_t_267 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
+        if (__pyx_t_268 < 0) __pyx_t_268 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
+        if (__pyx_t_269 < 0) __pyx_t_269 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
+        __pyx_v_temp = (__pyx_v_temp * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_267, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_268, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_269, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
 
-        /* "fastphase/calc_func.pyx":609
+        /* "fastphase/calc_func.pyx":602
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 temp*=mBeta[m+1,k1,k2]
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)             # <<<<<<<<<<<<<<
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
  */
-        __pyx_t_271 = (__pyx_v_m + 1);
-        __pyx_t_272 = __pyx_v_k1;
-        if (__pyx_t_271 < 0) __pyx_t_271 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_272 < 0) __pyx_t_272 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_273 = (__pyx_v_m + 1);
-        __pyx_t_274 = __pyx_v_k2;
-        if (__pyx_t_273 < 0) __pyx_t_273 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_274 < 0) __pyx_t_274 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_275 = (__pyx_v_m + 1);
-        __pyx_t_276 = 0;
-        if (__pyx_t_275 < 0) __pyx_t_275 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-        if (__pyx_t_276 < 0) __pyx_t_276 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_275, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_276, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_271, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_272, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_273, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_274, __pyx_pybuffernd_theta.diminfo[1].strides)), 0));
+        __pyx_t_270 = (__pyx_v_m + 1);
+        __pyx_t_271 = __pyx_v_k1;
+        if (__pyx_t_270 < 0) __pyx_t_270 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_271 < 0) __pyx_t_271 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_272 = (__pyx_v_m + 1);
+        __pyx_t_273 = __pyx_v_k2;
+        if (__pyx_t_272 < 0) __pyx_t_272 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_273 < 0) __pyx_t_273 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_274 = (__pyx_v_m + 1);
+        __pyx_t_275 = 0;
+        if (__pyx_t_274 < 0) __pyx_t_274 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+        if (__pyx_t_275 < 0) __pyx_t_275 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_274, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_275, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_270, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_271, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_272, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_273, __pyx_pybuffernd_theta.diminfo[1].strides)), 0));
 
-        /* "fastphase/calc_func.pyx":610
+        /* "fastphase/calc_func.pyx":603
  *                 temp*=mBeta[m+1,k1,k2]
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)             # <<<<<<<<<<<<<<
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
  */
-        __pyx_t_277 = (__pyx_v_m + 1);
-        __pyx_t_278 = __pyx_v_k1;
-        if (__pyx_t_277 < 0) __pyx_t_277 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_278 < 0) __pyx_t_278 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_279 = (__pyx_v_m + 1);
-        __pyx_t_280 = __pyx_v_k2;
-        if (__pyx_t_279 < 0) __pyx_t_279 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_280 < 0) __pyx_t_280 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_281 = (__pyx_v_m + 1);
-        __pyx_t_282 = 1;
-        if (__pyx_t_281 < 0) __pyx_t_281 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-        if (__pyx_t_282 < 0) __pyx_t_282 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_281, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_282, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_277, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_278, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_279, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_280, __pyx_pybuffernd_theta.diminfo[1].strides)), 1));
+        __pyx_t_276 = (__pyx_v_m + 1);
+        __pyx_t_277 = __pyx_v_k1;
+        if (__pyx_t_276 < 0) __pyx_t_276 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_277 < 0) __pyx_t_277 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_278 = (__pyx_v_m + 1);
+        __pyx_t_279 = __pyx_v_k2;
+        if (__pyx_t_278 < 0) __pyx_t_278 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_279 < 0) __pyx_t_279 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_280 = (__pyx_v_m + 1);
+        __pyx_t_281 = 1;
+        if (__pyx_t_280 < 0) __pyx_t_280 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+        if (__pyx_t_281 < 0) __pyx_t_281 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_280, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_281, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_276, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_277, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_278, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_279, __pyx_pybuffernd_theta.diminfo[1].strides)), 1));
 
-        /* "fastphase/calc_func.pyx":611
+        /* "fastphase/calc_func.pyx":604
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)             # <<<<<<<<<<<<<<
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
  */
-        __pyx_t_283 = (__pyx_v_m + 1);
-        __pyx_t_284 = __pyx_v_k1;
-        if (__pyx_t_283 < 0) __pyx_t_283 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_284 < 0) __pyx_t_284 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_285 = (__pyx_v_m + 1);
-        __pyx_t_286 = __pyx_v_k2;
-        if (__pyx_t_285 < 0) __pyx_t_285 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_286 < 0) __pyx_t_286 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_287 = (__pyx_v_m + 1);
-        __pyx_t_288 = 2;
-        if (__pyx_t_287 < 0) __pyx_t_287 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-        if (__pyx_t_288 < 0) __pyx_t_288 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_287, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_288, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_283, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_284, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_285, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_286, __pyx_pybuffernd_theta.diminfo[1].strides)), 2));
+        __pyx_t_282 = (__pyx_v_m + 1);
+        __pyx_t_283 = __pyx_v_k1;
+        if (__pyx_t_282 < 0) __pyx_t_282 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_283 < 0) __pyx_t_283 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_284 = (__pyx_v_m + 1);
+        __pyx_t_285 = __pyx_v_k2;
+        if (__pyx_t_284 < 0) __pyx_t_284 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_285 < 0) __pyx_t_285 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_286 = (__pyx_v_m + 1);
+        __pyx_t_287 = 2;
+        if (__pyx_t_286 < 0) __pyx_t_286 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+        if (__pyx_t_287 < 0) __pyx_t_287 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_286, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_287, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_282, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_283, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_284, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_285, __pyx_pybuffernd_theta.diminfo[1].strides)), 2));
       }
     }
 
-    /* "fastphase/calc_func.pyx":612
+    /* "fastphase/calc_func.pyx":605
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])             # <<<<<<<<<<<<<<
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 612, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_exp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_289 = (__pyx_v_m + 1);
-    __pyx_t_290 = 0;
-    if (__pyx_t_289 < 0) __pyx_t_289 += __pyx_pybuffernd_lik.diminfo[0].shape;
-    if (__pyx_t_290 < 0) __pyx_t_290 += __pyx_pybuffernd_lik.diminfo[1].shape;
-    __pyx_t_6 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_289, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_290, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 612, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 612, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 612, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_291 = (__pyx_v_m + 1);
-    __pyx_t_292 = 0;
-    if (__pyx_t_291 < 0) __pyx_t_291 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_292 < 0) __pyx_t_292 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_291, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_292, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
+ *         p_g_givX[m+1,0] *= lik[m+1,0]             # <<<<<<<<<<<<<<
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
+ */
+    __pyx_t_288 = (__pyx_v_m + 1);
+    __pyx_t_289 = 0;
+    if (__pyx_t_288 < 0) __pyx_t_288 += __pyx_pybuffernd_lik.diminfo[0].shape;
+    if (__pyx_t_289 < 0) __pyx_t_289 += __pyx_pybuffernd_lik.diminfo[1].shape;
+    __pyx_t_290 = (__pyx_v_m + 1);
+    __pyx_t_291 = 0;
+    if (__pyx_t_290 < 0) __pyx_t_290 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_291 < 0) __pyx_t_291 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_290, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_291, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_288, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_289, __pyx_pybuffernd_lik.diminfo[1].strides));
 
-    /* "fastphase/calc_func.pyx":613
+    /* "fastphase/calc_func.pyx":606
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])             # <<<<<<<<<<<<<<
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
+ *         p_g_givX[m+1,1] *= lik[m+1,1]             # <<<<<<<<<<<<<<
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 613, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_293 = (__pyx_v_m + 1);
-    __pyx_t_294 = 1;
-    if (__pyx_t_293 < 0) __pyx_t_293 += __pyx_pybuffernd_lik.diminfo[0].shape;
-    if (__pyx_t_294 < 0) __pyx_t_294 += __pyx_pybuffernd_lik.diminfo[1].shape;
-    __pyx_t_4 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_293, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_294, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 613, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 613, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 613, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_295 = (__pyx_v_m + 1);
-    __pyx_t_296 = 1;
-    if (__pyx_t_295 < 0) __pyx_t_295 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_296 < 0) __pyx_t_296 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_295, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_296, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-    /* "fastphase/calc_func.pyx":614
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])             # <<<<<<<<<<<<<<
+    __pyx_t_292 = (__pyx_v_m + 1);
+    __pyx_t_293 = 1;
+    if (__pyx_t_292 < 0) __pyx_t_292 += __pyx_pybuffernd_lik.diminfo[0].shape;
+    if (__pyx_t_293 < 0) __pyx_t_293 += __pyx_pybuffernd_lik.diminfo[1].shape;
+    __pyx_t_294 = (__pyx_v_m + 1);
+    __pyx_t_295 = 1;
+    if (__pyx_t_294 < 0) __pyx_t_294 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_295 < 0) __pyx_t_295 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_294, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_295, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_292, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_293, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+    /* "fastphase/calc_func.pyx":607
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
+ *         p_g_givX[m+1,2] *= lik[m+1,2]             # <<<<<<<<<<<<<<
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
  *         p_g_givX[m+1]/=normC
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 614, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_exp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_297 = (__pyx_v_m + 1);
-    __pyx_t_298 = 2;
-    if (__pyx_t_297 < 0) __pyx_t_297 += __pyx_pybuffernd_lik.diminfo[0].shape;
-    if (__pyx_t_298 < 0) __pyx_t_298 += __pyx_pybuffernd_lik.diminfo[1].shape;
-    __pyx_t_6 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_297, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_298, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 614, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 614, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_299 = (__pyx_v_m + 1);
-    __pyx_t_300 = 2;
-    if (__pyx_t_299 < 0) __pyx_t_299 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_300 < 0) __pyx_t_300 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_299, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_300, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-    /* "fastphase/calc_func.pyx":615
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+    __pyx_t_296 = (__pyx_v_m + 1);
+    __pyx_t_297 = 2;
+    if (__pyx_t_296 < 0) __pyx_t_296 += __pyx_pybuffernd_lik.diminfo[0].shape;
+    if (__pyx_t_297 < 0) __pyx_t_297 += __pyx_pybuffernd_lik.diminfo[1].shape;
+    __pyx_t_298 = (__pyx_v_m + 1);
+    __pyx_t_299 = 2;
+    if (__pyx_t_298 < 0) __pyx_t_298 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_299 < 0) __pyx_t_299 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_298, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_299, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_296, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_297, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+    /* "fastphase/calc_func.pyx":608
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]             # <<<<<<<<<<<<<<
  *         p_g_givX[m+1]/=normC
  * 
  */
-    __pyx_t_301 = (__pyx_v_m + 1);
-    __pyx_t_302 = 0;
-    if (__pyx_t_301 < 0) __pyx_t_301 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_302 < 0) __pyx_t_302 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    __pyx_t_303 = (__pyx_v_m + 1);
-    __pyx_t_304 = 1;
-    if (__pyx_t_303 < 0) __pyx_t_303 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_304 < 0) __pyx_t_304 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    __pyx_t_305 = (__pyx_v_m + 1);
-    __pyx_t_306 = 2;
-    if (__pyx_t_305 < 0) __pyx_t_305 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_306 < 0) __pyx_t_306 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_301, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_302, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_303, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_304, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_305, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_306, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
+    __pyx_t_300 = (__pyx_v_m + 1);
+    __pyx_t_301 = 0;
+    if (__pyx_t_300 < 0) __pyx_t_300 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_301 < 0) __pyx_t_301 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    __pyx_t_302 = (__pyx_v_m + 1);
+    __pyx_t_303 = 1;
+    if (__pyx_t_302 < 0) __pyx_t_302 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_303 < 0) __pyx_t_303 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    __pyx_t_304 = (__pyx_v_m + 1);
+    __pyx_t_305 = 2;
+    if (__pyx_t_304 < 0) __pyx_t_304 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_305 < 0) __pyx_t_305 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_300, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_301, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_302, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_303, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_304, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_305, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
 
-    /* "fastphase/calc_func.pyx":616
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+    /* "fastphase/calc_func.pyx":609
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
  *         p_g_givX[m+1]/=normC             # <<<<<<<<<<<<<<
  * 
  *     if up2pz>0:
  */
     __pyx_t_13 = (__pyx_v_m + 1);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 609, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 616, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 616, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 0) < 0)) __PYX_ERR(0, 609, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 0) < 0)) __PYX_ERR(0, 616, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "fastphase/calc_func.pyx":618
+  /* "fastphase/calc_func.pyx":611
  *         p_g_givX[m+1]/=normC
  * 
  *     if up2pz>0:             # <<<<<<<<<<<<<<
  *         return probZ,p_g_givX
  *     # calc jmk
  */
   __pyx_t_66 = ((__pyx_v_up2pz > 0) != 0);
   if (__pyx_t_66) {
 
-    /* "fastphase/calc_func.pyx":619
+    /* "fastphase/calc_func.pyx":612
  * 
  *     if up2pz>0:
  *         return probZ,p_g_givX             # <<<<<<<<<<<<<<
  *     # calc jmk
  *     for k1 in range(nK):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 619, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(((PyObject *)__pyx_v_probZ));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_probZ));
-    PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)__pyx_v_probZ));
+    PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_probZ));
     __Pyx_INCREF(((PyObject *)__pyx_v_p_g_givX));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_p_g_givX));
-    PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_p_g_givX));
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_p_g_givX));
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "fastphase/calc_func.pyx":618
+    /* "fastphase/calc_func.pyx":611
  *         p_g_givX[m+1]/=normC
  * 
  *     if up2pz>0:             # <<<<<<<<<<<<<<
  *         return probZ,p_g_givX
  *     # calc jmk
  */
   }
 
-  /* "fastphase/calc_func.pyx":621
+  /* "fastphase/calc_func.pyx":614
  *         return probZ,p_g_givX
  *     # calc jmk
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         ##jmk[0,k1]=2*alpha[0,k1]
  *         jmk[0, k1] = probZ[0,k1,k1]
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":623
+    /* "fastphase/calc_func.pyx":616
  *     for k1 in range(nK):
  *         ##jmk[0,k1]=2*alpha[0,k1]
  *         jmk[0, k1] = probZ[0,k1,k1]             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             jmk[0, k1] += probZ[0, k2, k1]
  */
-    __pyx_t_307 = 0;
+    __pyx_t_306 = 0;
+    __pyx_t_307 = __pyx_v_k1;
     __pyx_t_308 = __pyx_v_k1;
-    __pyx_t_309 = __pyx_v_k1;
-    if (__pyx_t_307 < 0) __pyx_t_307 += __pyx_pybuffernd_probZ.diminfo[0].shape;
-    if (__pyx_t_308 < 0) __pyx_t_308 += __pyx_pybuffernd_probZ.diminfo[1].shape;
-    if (__pyx_t_309 < 0) __pyx_t_309 += __pyx_pybuffernd_probZ.diminfo[2].shape;
-    __pyx_t_310 = 0;
-    __pyx_t_311 = __pyx_v_k1;
-    if (__pyx_t_310 < 0) __pyx_t_310 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-    if (__pyx_t_311 < 0) __pyx_t_311 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_310, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_311, __pyx_pybuffernd_jmk.diminfo[1].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_307, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_308, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_309, __pyx_pybuffernd_probZ.diminfo[2].strides));
+    if (__pyx_t_306 < 0) __pyx_t_306 += __pyx_pybuffernd_probZ.diminfo[0].shape;
+    if (__pyx_t_307 < 0) __pyx_t_307 += __pyx_pybuffernd_probZ.diminfo[1].shape;
+    if (__pyx_t_308 < 0) __pyx_t_308 += __pyx_pybuffernd_probZ.diminfo[2].shape;
+    __pyx_t_309 = 0;
+    __pyx_t_310 = __pyx_v_k1;
+    if (__pyx_t_309 < 0) __pyx_t_309 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+    if (__pyx_t_310 < 0) __pyx_t_310 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_309, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_310, __pyx_pybuffernd_jmk.diminfo[1].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_306, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_307, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_308, __pyx_pybuffernd_probZ.diminfo[2].strides));
 
-    /* "fastphase/calc_func.pyx":624
+    /* "fastphase/calc_func.pyx":617
  *         ##jmk[0,k1]=2*alpha[0,k1]
  *         jmk[0, k1] = probZ[0,k1,k1]
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             jmk[0, k1] += probZ[0, k2, k1]
  * 
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 624, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 617, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":625
+      /* "fastphase/calc_func.pyx":618
  *         jmk[0, k1] = probZ[0,k1,k1]
  *         for k2 in range(nK):
  *             jmk[0, k1] += probZ[0, k2, k1]             # <<<<<<<<<<<<<<
  * 
  *     for m in range(1,nLoc):
  */
-      __pyx_t_312 = 0;
-      __pyx_t_313 = __pyx_v_k2;
-      __pyx_t_314 = __pyx_v_k1;
-      if (__pyx_t_312 < 0) __pyx_t_312 += __pyx_pybuffernd_probZ.diminfo[0].shape;
-      if (__pyx_t_313 < 0) __pyx_t_313 += __pyx_pybuffernd_probZ.diminfo[1].shape;
-      if (__pyx_t_314 < 0) __pyx_t_314 += __pyx_pybuffernd_probZ.diminfo[2].shape;
-      __pyx_t_315 = 0;
-      __pyx_t_316 = __pyx_v_k1;
-      if (__pyx_t_315 < 0) __pyx_t_315 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-      if (__pyx_t_316 < 0) __pyx_t_316 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_315, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_316, __pyx_pybuffernd_jmk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_312, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_313, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_314, __pyx_pybuffernd_probZ.diminfo[2].strides));
+      __pyx_t_311 = 0;
+      __pyx_t_312 = __pyx_v_k2;
+      __pyx_t_313 = __pyx_v_k1;
+      if (__pyx_t_311 < 0) __pyx_t_311 += __pyx_pybuffernd_probZ.diminfo[0].shape;
+      if (__pyx_t_312 < 0) __pyx_t_312 += __pyx_pybuffernd_probZ.diminfo[1].shape;
+      if (__pyx_t_313 < 0) __pyx_t_313 += __pyx_pybuffernd_probZ.diminfo[2].shape;
+      __pyx_t_314 = 0;
+      __pyx_t_315 = __pyx_v_k1;
+      if (__pyx_t_314 < 0) __pyx_t_314 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+      if (__pyx_t_315 < 0) __pyx_t_315 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_314, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_315, __pyx_pybuffernd_jmk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_311, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_312, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_313, __pyx_pybuffernd_probZ.diminfo[2].strides));
     }
   }
 
-  /* "fastphase/calc_func.pyx":627
+  /* "fastphase/calc_func.pyx":620
  *             jmk[0, k1] += probZ[0, k2, k1]
  * 
  *     for m in range(1,nLoc):             # <<<<<<<<<<<<<<
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 620, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 1; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":628
+    /* "fastphase/calc_func.pyx":621
  * 
  *     for m in range(1,nLoc):
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             for k1 in range(nK):
  */
-    __pyx_t_317 = (__pyx_v_m - 1);
-    if (__pyx_t_317 < 0) __pyx_t_317 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
-    __pyx_t_318 = __pyx_v_m;
-    if (__pyx_t_318 < 0) __pyx_t_318 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
-    __pyx_t_6 = __Pyx_PyInt_From_npy_long(((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_317, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_318, __pyx_pybuffernd_betaScale.diminfo[0].strides)))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 628, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
+    __pyx_t_316 = (__pyx_v_m - 1);
+    if (__pyx_t_316 < 0) __pyx_t_316 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
+    __pyx_t_317 = __pyx_v_m;
+    if (__pyx_t_317 < 0) __pyx_t_317 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
+    __pyx_t_4 = __Pyx_PyInt_From_npy_long(((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_316, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_317, __pyx_pybuffernd_betaScale.diminfo[0].strides)))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 628, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 621, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyNumber_Subtract(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Subtract(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 628, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_15 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_15 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 621, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_15 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_15 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 628, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10(__pyx_t_15);
 
-    /* "fastphase/calc_func.pyx":629
+    /* "fastphase/calc_func.pyx":622
  *     for m in range(1,nLoc):
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 629, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 622, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":630
+      /* "fastphase/calc_func.pyx":623
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 623, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k1 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":631
+        /* "fastphase/calc_func.pyx":624
  *         for k in range(nK):
  *             for k1 in range(nK):
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])             # <<<<<<<<<<<<<<
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  */
-        __pyx_t_319 = (__pyx_v_m - 1);
-        __pyx_t_320 = __pyx_v_k1;
-        if (__pyx_t_319 < 0) __pyx_t_319 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
-        if (__pyx_t_320 < 0) __pyx_t_320 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
-        __pyx_t_321 = __pyx_v_m;
-        __pyx_t_322 = 0;
-        if (__pyx_t_321 < 0) __pyx_t_321 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_322 < 0) __pyx_t_322 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_v_temp = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_319, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_320, __pyx_pybuffernd_tSumk.diminfo[1].strides)) * __pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_321, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_322, __pyx_pybuffernd_rho.diminfo[1].strides))));
+        __pyx_t_318 = (__pyx_v_m - 1);
+        __pyx_t_319 = __pyx_v_k1;
+        if (__pyx_t_318 < 0) __pyx_t_318 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
+        if (__pyx_t_319 < 0) __pyx_t_319 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
+        __pyx_t_320 = __pyx_v_m;
+        __pyx_t_321 = 0;
+        if (__pyx_t_320 < 0) __pyx_t_320 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_321 < 0) __pyx_t_321 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_v_temp = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_318, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_319, __pyx_pybuffernd_tSumk.diminfo[1].strides)) * __pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_320, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_321, __pyx_pybuffernd_rho.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":632
+        /* "fastphase/calc_func.pyx":625
  *             for k1 in range(nK):
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]             # <<<<<<<<<<<<<<
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  *             jmk[m,k] *= alpha[m,k]
  */
-        __pyx_t_323 = __pyx_v_m;
-        __pyx_t_324 = 0;
-        if (__pyx_t_323 < 0) __pyx_t_323 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_324 < 0) __pyx_t_324 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_t_325 = (__pyx_v_m - 1);
-        if (__pyx_t_325 < 0) __pyx_t_325 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
-        __pyx_t_326 = __pyx_v_m;
-        __pyx_t_327 = __pyx_v_k1;
-        if (__pyx_t_326 < 0) __pyx_t_326 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_327 < 0) __pyx_t_327 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_v_temp = (__pyx_v_temp + (((2.0 * __pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_323, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_324, __pyx_pybuffernd_rho.diminfo[1].strides)))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_325, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_326, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_327, __pyx_pybuffernd_alpha.diminfo[1].strides))));
+        __pyx_t_322 = __pyx_v_m;
+        __pyx_t_323 = 0;
+        if (__pyx_t_322 < 0) __pyx_t_322 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_323 < 0) __pyx_t_323 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_t_324 = (__pyx_v_m - 1);
+        if (__pyx_t_324 < 0) __pyx_t_324 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
+        __pyx_t_325 = __pyx_v_m;
+        __pyx_t_326 = __pyx_v_k1;
+        if (__pyx_t_325 < 0) __pyx_t_325 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_326 < 0) __pyx_t_326 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_v_temp = (__pyx_v_temp + (((2.0 * __pyx_f_9fastphase_9calc_func_probJ(__pyx_v_m, 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_322, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_323, __pyx_pybuffernd_rho.diminfo[1].strides)))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_324, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_325, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_326, __pyx_pybuffernd_alpha.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":633
+        /* "fastphase/calc_func.pyx":626
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]             # <<<<<<<<<<<<<<
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tDoubleSum[nLoc-1]
  */
-        __pyx_t_328 = __pyx_v_m;
-        __pyx_t_329 = __pyx_v_k;
-        if (__pyx_t_328 < 0) __pyx_t_328 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_329 < 0) __pyx_t_329 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_330 = __pyx_v_m;
-        __pyx_t_331 = __pyx_v_k1;
-        if (__pyx_t_330 < 0) __pyx_t_330 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_331 < 0) __pyx_t_331 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 633, __pyx_L1_error)
-        __pyx_t_332 = __pyx_v_m;
-        __pyx_t_333 = __pyx_v_k;
-        __pyx_t_334 = __pyx_v_k1;
-        if (__pyx_t_332 < 0) __pyx_t_332 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
-        if (__pyx_t_333 < 0) __pyx_t_333 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
-        if (__pyx_t_334 < 0) __pyx_t_334 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
-        __pyx_t_335 = __pyx_v_m;
-        __pyx_t_336 = __pyx_v_k;
-        if (__pyx_t_335 < 0) __pyx_t_335 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-        if (__pyx_t_336 < 0) __pyx_t_336 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_335, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_336, __pyx_pybuffernd_jmk.diminfo[1].strides) += ((__pyx_v_temp * __pyx_f_9fastphase_9calc_func_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_328, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_329, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_330, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_331, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_4))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_332, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_333, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_334, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_327 = __pyx_v_m;
+        __pyx_t_328 = __pyx_v_k;
+        if (__pyx_t_327 < 0) __pyx_t_327 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_328 < 0) __pyx_t_328 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_329 = __pyx_v_m;
+        __pyx_t_330 = __pyx_v_k1;
+        if (__pyx_t_329 < 0) __pyx_t_329 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_330 < 0) __pyx_t_330 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 626, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 626, __pyx_L1_error)
+        __pyx_t_331 = __pyx_v_m;
+        __pyx_t_332 = __pyx_v_k;
+        __pyx_t_333 = __pyx_v_k1;
+        if (__pyx_t_331 < 0) __pyx_t_331 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
+        if (__pyx_t_332 < 0) __pyx_t_332 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
+        if (__pyx_t_333 < 0) __pyx_t_333 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
+        __pyx_t_334 = __pyx_v_m;
+        __pyx_t_335 = __pyx_v_k;
+        if (__pyx_t_334 < 0) __pyx_t_334 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+        if (__pyx_t_335 < 0) __pyx_t_335 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_334, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_335, __pyx_pybuffernd_jmk.diminfo[1].strides) += ((__pyx_v_temp * __pyx_f_9fastphase_9calc_func_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_327, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_328, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_329, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_330, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_5))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_331, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_332, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_333, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
 
-      /* "fastphase/calc_func.pyx":634
+      /* "fastphase/calc_func.pyx":627
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  *             jmk[m,k] *= alpha[m,k]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= tDoubleSum[nLoc-1]
  *             jmk[m,k] /= dummy
  */
-      __pyx_t_337 = __pyx_v_m;
-      __pyx_t_338 = __pyx_v_k;
-      if (__pyx_t_337 < 0) __pyx_t_337 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-      if (__pyx_t_338 < 0) __pyx_t_338 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-      __pyx_t_339 = __pyx_v_m;
-      __pyx_t_340 = __pyx_v_k;
-      if (__pyx_t_339 < 0) __pyx_t_339 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-      if (__pyx_t_340 < 0) __pyx_t_340 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_339, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_340, __pyx_pybuffernd_jmk.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_337, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_338, __pyx_pybuffernd_alpha.diminfo[1].strides));
+      __pyx_t_336 = __pyx_v_m;
+      __pyx_t_337 = __pyx_v_k;
+      if (__pyx_t_336 < 0) __pyx_t_336 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+      if (__pyx_t_337 < 0) __pyx_t_337 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+      __pyx_t_338 = __pyx_v_m;
+      __pyx_t_339 = __pyx_v_k;
+      if (__pyx_t_338 < 0) __pyx_t_338 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+      if (__pyx_t_339 < 0) __pyx_t_339 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_338, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_339, __pyx_pybuffernd_jmk.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_336, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_337, __pyx_pybuffernd_alpha.diminfo[1].strides));
 
-      /* "fastphase/calc_func.pyx":635
+      /* "fastphase/calc_func.pyx":628
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tDoubleSum[nLoc-1]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= dummy
  *     # calc top,bottom
  */
-      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 635, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 635, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 628, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 635, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 628, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_340 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_340 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 628, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_341 = __pyx_v_m;
       __pyx_t_342 = __pyx_v_k;
       if (__pyx_t_341 < 0) __pyx_t_341 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_342 < 0) __pyx_t_342 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_341, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_342, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_t_228;
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_341, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_342, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_t_340;
 
-      /* "fastphase/calc_func.pyx":636
+      /* "fastphase/calc_func.pyx":629
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tDoubleSum[nLoc-1]
  *             jmk[m,k] /= dummy             # <<<<<<<<<<<<<<
  *     # calc top,bottom
  *     for m in range(nLoc):
  */
       __pyx_t_343 = __pyx_v_m;
       __pyx_t_344 = __pyx_v_k;
       if (__pyx_t_343 < 0) __pyx_t_343 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_344 < 0) __pyx_t_344 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_343, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_344, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_v_dummy;
     }
   }
 
-  /* "fastphase/calc_func.pyx":638
+  /* "fastphase/calc_func.pyx":631
  *             jmk[m,k] /= dummy
  *     # calc top,bottom
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         ## bottom
  *         for k in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 631, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":640
+    /* "fastphase/calc_func.pyx":633
  *     for m in range(nLoc):
  *         ## bottom
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             bot[m,k]+=probZ[m,k,k]
  *             for k1 in range(nK):
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 640, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 633, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":641
+      /* "fastphase/calc_func.pyx":634
  *         ## bottom
  *         for k in range(nK):
  *             bot[m,k]+=probZ[m,k,k]             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 bot[m,k]+=probZ[m,k1,k]
  */
       __pyx_t_345 = __pyx_v_m;
@@ -13294,27 +12977,27 @@
       if (__pyx_t_347 < 0) __pyx_t_347 += __pyx_pybuffernd_probZ.diminfo[2].shape;
       __pyx_t_348 = __pyx_v_m;
       __pyx_t_349 = __pyx_v_k;
       if (__pyx_t_348 < 0) __pyx_t_348 += __pyx_pybuffernd_bot.diminfo[0].shape;
       if (__pyx_t_349 < 0) __pyx_t_349 += __pyx_pybuffernd_bot.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_348, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_349, __pyx_pybuffernd_bot.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_345, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_346, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_347, __pyx_pybuffernd_probZ.diminfo[2].strides));
 
-      /* "fastphase/calc_func.pyx":642
+      /* "fastphase/calc_func.pyx":635
  *         for k in range(nK):
  *             bot[m,k]+=probZ[m,k,k]
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 bot[m,k]+=probZ[m,k1,k]
  *         # ## top
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 642, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 635, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k1 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":643
+        /* "fastphase/calc_func.pyx":636
  *             bot[m,k]+=probZ[m,k,k]
  *             for k1 in range(nK):
  *                 bot[m,k]+=probZ[m,k1,k]             # <<<<<<<<<<<<<<
  *         # ## top
  *         for k in range(nK):
  */
         __pyx_t_350 = __pyx_v_m;
@@ -13327,39 +13010,39 @@
         __pyx_t_354 = __pyx_v_k;
         if (__pyx_t_353 < 0) __pyx_t_353 += __pyx_pybuffernd_bot.diminfo[0].shape;
         if (__pyx_t_354 < 0) __pyx_t_354 += __pyx_pybuffernd_bot.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_353, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_354, __pyx_pybuffernd_bot.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_350, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_351, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_352, __pyx_pybuffernd_probZ.diminfo[2].strides));
       }
     }
 
-    /* "fastphase/calc_func.pyx":645
+    /* "fastphase/calc_func.pyx":638
  *                 bot[m,k]+=probZ[m,k1,k]
  *         # ## top
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 t1=theta[m,k]*(1-theta[m,k1])
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 638, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "fastphase/calc_func.pyx":646
+      /* "fastphase/calc_func.pyx":639
  *         # ## top
  *         for k in range(nK):
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 t1=theta[m,k]*(1-theta[m,k1])
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 646, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 639, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k1 = __pyx_t_21;
 
-        /* "fastphase/calc_func.pyx":647
+        /* "fastphase/calc_func.pyx":640
  *         for k in range(nK):
  *             for k1 in range(nK):
  *                 t1=theta[m,k]*(1-theta[m,k1])             # <<<<<<<<<<<<<<
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  */
         __pyx_t_355 = __pyx_v_m;
@@ -13368,15 +13051,15 @@
         if (__pyx_t_356 < 0) __pyx_t_356 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_357 = __pyx_v_m;
         __pyx_t_358 = __pyx_v_k1;
         if (__pyx_t_357 < 0) __pyx_t_357 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_358 < 0) __pyx_t_358 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_v_t1 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_355, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_356, __pyx_pybuffernd_theta.diminfo[1].strides)) * (1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_357, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_358, __pyx_pybuffernd_theta.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":648
+        /* "fastphase/calc_func.pyx":641
  *             for k1 in range(nK):
  *                 t1=theta[m,k]*(1-theta[m,k1])
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])             # <<<<<<<<<<<<<<
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):
  */
         __pyx_t_359 = __pyx_v_m;
@@ -13385,75 +13068,75 @@
         if (__pyx_t_360 < 0) __pyx_t_360 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_361 = __pyx_v_m;
         __pyx_t_362 = __pyx_v_k;
         if (__pyx_t_361 < 0) __pyx_t_361 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_362 < 0) __pyx_t_362 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_v_t2 = (__pyx_v_t1 + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_359, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_360, __pyx_pybuffernd_theta.diminfo[1].strides)) * (1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_361, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_362, __pyx_pybuffernd_theta.diminfo[1].strides)))));
 
-        /* "fastphase/calc_func.pyx":649
+        /* "fastphase/calc_func.pyx":642
  *                 t1=theta[m,k]*(1-theta[m,k1])
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])             # <<<<<<<<<<<<<<
  *                 if (k == k1):
  *                     top[m,k] += 2*temp
  */
         __pyx_t_363 = __pyx_v_m;
         __pyx_t_364 = __pyx_v_k;
         __pyx_t_365 = __pyx_v_k1;
         if (__pyx_t_363 < 0) __pyx_t_363 += __pyx_pybuffernd_probZ.diminfo[0].shape;
         if (__pyx_t_364 < 0) __pyx_t_364 += __pyx_pybuffernd_probZ.diminfo[1].shape;
         if (__pyx_t_365 < 0) __pyx_t_365 += __pyx_pybuffernd_probZ.diminfo[2].shape;
         if (unlikely(__pyx_v_t2 == 0)) {
           PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-          __PYX_ERR(0, 649, __pyx_L1_error)
+          __PYX_ERR(0, 642, __pyx_L1_error)
         }
         __pyx_t_366 = __pyx_v_m;
         __pyx_t_367 = 1;
         if (__pyx_t_366 < 0) __pyx_t_366 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
         if (__pyx_t_367 < 0) __pyx_t_367 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
         __pyx_t_368 = __pyx_v_m;
         __pyx_t_369 = 2;
         if (__pyx_t_368 < 0) __pyx_t_368 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
         if (__pyx_t_369 < 0) __pyx_t_369 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
         __pyx_v_temp = ((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_363, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_364, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_365, __pyx_pybuffernd_probZ.diminfo[2].strides)) * (((__pyx_v_t1 / __pyx_v_t2) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_366, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_367, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_368, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_369, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":650
+        /* "fastphase/calc_func.pyx":643
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):             # <<<<<<<<<<<<<<
  *                     top[m,k] += 2*temp
  *                 else:
  */
         __pyx_t_66 = ((__pyx_v_k == __pyx_v_k1) != 0);
         if (__pyx_t_66) {
 
-          /* "fastphase/calc_func.pyx":651
+          /* "fastphase/calc_func.pyx":644
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):
  *                     top[m,k] += 2*temp             # <<<<<<<<<<<<<<
  *                 else:
  *                     top[m,k] += temp
  */
           __pyx_t_370 = __pyx_v_m;
           __pyx_t_371 = __pyx_v_k;
           if (__pyx_t_370 < 0) __pyx_t_370 += __pyx_pybuffernd_top.diminfo[0].shape;
           if (__pyx_t_371 < 0) __pyx_t_371 += __pyx_pybuffernd_top.diminfo[1].shape;
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_top.rcbuffer->pybuffer.buf, __pyx_t_370, __pyx_pybuffernd_top.diminfo[0].strides, __pyx_t_371, __pyx_pybuffernd_top.diminfo[1].strides) += (2.0 * __pyx_v_temp);
 
-          /* "fastphase/calc_func.pyx":650
+          /* "fastphase/calc_func.pyx":643
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):             # <<<<<<<<<<<<<<
  *                     top[m,k] += 2*temp
  *                 else:
  */
           goto __pyx_L97;
         }
 
-        /* "fastphase/calc_func.pyx":653
+        /* "fastphase/calc_func.pyx":646
  *                     top[m,k] += 2*temp
  *                 else:
  *                     top[m,k] += temp             # <<<<<<<<<<<<<<
  *     return logLikelihood,top,bot,jmk
  * 
  */
         /*else*/ {
@@ -13464,44 +13147,44 @@
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_top.rcbuffer->pybuffer.buf, __pyx_t_372, __pyx_pybuffernd_top.diminfo[0].strides, __pyx_t_373, __pyx_pybuffernd_top.diminfo[1].strides) += __pyx_v_temp;
         }
         __pyx_L97:;
       }
     }
   }
 
-  /* "fastphase/calc_func.pyx":654
+  /* "fastphase/calc_func.pyx":647
  *                 else:
  *                     top[m,k] += temp
  *     return logLikelihood,top,bot,jmk             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 647, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 654, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
   __Pyx_INCREF(((PyObject *)__pyx_v_top));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_top));
-  PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_top));
+  PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_top));
   __Pyx_INCREF(((PyObject *)__pyx_v_bot));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_bot));
-  PyTuple_SET_ITEM(__pyx_t_4, 2, ((PyObject *)__pyx_v_bot));
+  PyTuple_SET_ITEM(__pyx_t_5, 2, ((PyObject *)__pyx_v_bot));
   __Pyx_INCREF(((PyObject *)__pyx_v_jmk));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_jmk));
-  PyTuple_SET_ITEM(__pyx_t_4, 3, ((PyObject *)__pyx_v_jmk));
+  PyTuple_SET_ITEM(__pyx_t_5, 3, ((PyObject *)__pyx_v_jmk));
+  __pyx_t_6 = 0;
+  __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
-  __pyx_r = __pyx_t_4;
-  __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "fastphase/calc_func.pyx":435
- *     return rez
+  /* "fastphase/calc_func.pyx":428
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
 
   /* function exit code */
@@ -13613,37 +13296,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aa)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 1); __PYX_ERR(0, 435, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 1); __PYX_ERR(0, 428, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 2); __PYX_ERR(0, 435, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 2); __PYX_ERR(0, 428, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ll)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 3); __PYX_ERR(0, 435, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 3); __PYX_ERR(0, 428, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u2p)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 4); __PYX_ERR(0, 435, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 4); __PYX_ERR(0, 428, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "likCalc") < 0)) __PYX_ERR(0, 435, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "likCalc") < 0)) __PYX_ERR(0, 428, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -13654,15 +13337,15 @@
     __pyx_v_tt = values[1];
     __pyx_v_rr = values[2];
     __pyx_v_ll = values[3];
     __pyx_v_u2p = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 435, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 428, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastphase.calc_func.likCalc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9fastphase_9calc_func_12likCalc(__pyx_self, __pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_ll, __pyx_v_u2p);
 
@@ -13673,15 +13356,15 @@
 
 static PyObject *__pyx_pf_9fastphase_9calc_func_12likCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_aa, PyObject *__pyx_v_tt, PyObject *__pyx_v_rr, PyObject *__pyx_v_ll, PyObject *__pyx_v_u2p) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("likCalc", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9fastphase_9calc_func_likCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_ll, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9fastphase_9calc_func_likCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_ll, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13690,104 +13373,104 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/calc_func.pyx":659
+/* "fastphase/calc_func.pyx":652
  * #### Haplotype Calculations
  * 
  * cdef double happrG(double t,int s):             # <<<<<<<<<<<<<<
  *     if s==0:
  *         return 1-t
  */
 
 static double __pyx_f_9fastphase_9calc_func_happrG(double __pyx_v_t, int __pyx_v_s) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("happrG", 0);
 
-  /* "fastphase/calc_func.pyx":660
+  /* "fastphase/calc_func.pyx":653
  * 
  * cdef double happrG(double t,int s):
  *     if s==0:             # <<<<<<<<<<<<<<
  *         return 1-t
  *     elif s==1:
  */
   switch (__pyx_v_s) {
     case 0:
 
-    /* "fastphase/calc_func.pyx":661
+    /* "fastphase/calc_func.pyx":654
  * cdef double happrG(double t,int s):
  *     if s==0:
  *         return 1-t             # <<<<<<<<<<<<<<
  *     elif s==1:
  *         return t
  */
     __pyx_r = (1.0 - __pyx_v_t);
     goto __pyx_L0;
 
-    /* "fastphase/calc_func.pyx":660
+    /* "fastphase/calc_func.pyx":653
  * 
  * cdef double happrG(double t,int s):
  *     if s==0:             # <<<<<<<<<<<<<<
  *         return 1-t
  *     elif s==1:
  */
     break;
     case 1:
 
-    /* "fastphase/calc_func.pyx":663
+    /* "fastphase/calc_func.pyx":656
  *         return 1-t
  *     elif s==1:
  *         return t             # <<<<<<<<<<<<<<
  *     else:
  *         return 1
  */
     __pyx_r = __pyx_v_t;
     goto __pyx_L0;
 
-    /* "fastphase/calc_func.pyx":662
+    /* "fastphase/calc_func.pyx":655
  *     if s==0:
  *         return 1-t
  *     elif s==1:             # <<<<<<<<<<<<<<
  *         return t
  *     else:
  */
     break;
     default:
 
-    /* "fastphase/calc_func.pyx":665
+    /* "fastphase/calc_func.pyx":658
  *         return t
  *     else:
  *         return 1             # <<<<<<<<<<<<<<
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):
  */
     __pyx_r = 1.0;
     goto __pyx_L0;
     break;
   }
 
-  /* "fastphase/calc_func.pyx":659
+  /* "fastphase/calc_func.pyx":652
  * #### Haplotype Calculations
  * 
  * cdef double happrG(double t,int s):             # <<<<<<<<<<<<<<
  *     if s==0:
  *         return 1-t
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/calc_func.pyx":667
+/* "fastphase/calc_func.pyx":660
  *         return 1
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -13910,337 +13593,337 @@
   __pyx_pybuffernd_soluce.data = NULL;
   __pyx_pybuffernd_soluce.rcbuffer = &__pyx_pybuffer_soluce;
   __pyx_pybuffer_tempVal.pybuffer.buf = NULL;
   __pyx_pybuffer_tempVal.refcount = 0;
   __pyx_pybuffernd_tempVal.data = NULL;
   __pyx_pybuffernd_tempVal.rcbuffer = &__pyx_pybuffer_tempVal;
 
-  /* "fastphase/calc_func.pyx":668
+  /* "fastphase/calc_func.pyx":661
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  */
-  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 668, __pyx_L1_error)
+  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 661, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_aa;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alpha.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_alpha = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 668, __pyx_L1_error)
+      __PYX_ERR(0, 661, __pyx_L1_error)
     } else {__pyx_pybuffernd_alpha.diminfo[0].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alpha.diminfo[0].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_alpha.diminfo[1].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_alpha.diminfo[1].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_alpha = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":669
+  /* "fastphase/calc_func.pyx":662
  * cpdef hapViterbi( aa, tt, rr, hh):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  */
-  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 669, __pyx_L1_error)
+  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 662, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_tt;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_theta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 669, __pyx_L1_error)
+      __PYX_ERR(0, 662, __pyx_L1_error)
     } else {__pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_theta = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":670
+  /* "fastphase/calc_func.pyx":663
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  * 
  */
-  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 670, __pyx_L1_error)
+  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 663, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_rr;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rho.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_rho = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 670, __pyx_L1_error)
+      __PYX_ERR(0, 663, __pyx_L1_error)
     } else {__pyx_pybuffernd_rho.diminfo[0].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rho.diminfo[0].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_rho.diminfo[1].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_rho.diminfo[1].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_rho = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":671
+  /* "fastphase/calc_func.pyx":664
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh             # <<<<<<<<<<<<<<
  * 
  *     ## cython declarations
  */
-  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 671, __pyx_L1_error)
+  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 664, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_hh;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_hap.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_hap = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 671, __pyx_L1_error)
+      __PYX_ERR(0, 664, __pyx_L1_error)
     } else {__pyx_pybuffernd_hap.diminfo[0].strides = __pyx_pybuffernd_hap.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_hap.diminfo[0].shape = __pyx_pybuffernd_hap.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_v_hap = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":677
+  /* "fastphase/calc_func.pyx":670
  *     cdef int k, prev_k, best_k, m
  *     cdef double best_v
  *     nLoc = alpha.shape[0]             # <<<<<<<<<<<<<<
  *     nK = alpha.shape[1]
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  */
   __pyx_v_nLoc = (__pyx_v_alpha->dimensions[0]);
 
-  /* "fastphase/calc_func.pyx":678
+  /* "fastphase/calc_func.pyx":671
  *     cdef double best_v
  *     nLoc = alpha.shape[0]
  *     nK = alpha.shape[1]             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  */
   __pyx_v_nK = (__pyx_v_alpha->dimensions[1]);
 
-  /* "fastphase/calc_func.pyx":679
+  /* "fastphase/calc_func.pyx":672
  *     nLoc = alpha.shape[0]
  *     nK = alpha.shape[1]
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 679, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 672, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 679, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 672, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_delta.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_delta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 679, __pyx_L1_error)
+      __PYX_ERR(0, 672, __pyx_L1_error)
     } else {__pyx_pybuffernd_delta.diminfo[0].strides = __pyx_pybuffernd_delta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_delta.diminfo[0].shape = __pyx_pybuffernd_delta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_delta.diminfo[1].strides = __pyx_pybuffernd_delta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_delta.diminfo[1].shape = __pyx_pybuffernd_delta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_delta = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":680
+  /* "fastphase/calc_func.pyx":673
  *     nK = alpha.shape[1]
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)
  *     cdef np.ndarray[ np.float64_t, ndim = 1] tempVal = np.zeros( nK, dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_5 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 680, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 680, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 673, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 680, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 673, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psi.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_psi = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_psi.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 680, __pyx_L1_error)
+      __PYX_ERR(0, 673, __pyx_L1_error)
     } else {__pyx_pybuffernd_psi.diminfo[0].strides = __pyx_pybuffernd_psi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_psi.diminfo[0].shape = __pyx_pybuffernd_psi.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_psi.diminfo[1].strides = __pyx_pybuffernd_psi.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_psi.diminfo[1].shape = __pyx_pybuffernd_psi.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_psi = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":681
+  /* "fastphase/calc_func.pyx":674
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.float64_t, ndim = 1] tempVal = np.zeros( nK, dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 681, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 681, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 681, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 674, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_soluce.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_soluce = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_soluce.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 681, __pyx_L1_error)
+      __PYX_ERR(0, 674, __pyx_L1_error)
     } else {__pyx_pybuffernd_soluce.diminfo[0].strides = __pyx_pybuffernd_soluce.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_soluce.diminfo[0].shape = __pyx_pybuffernd_soluce.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_soluce = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":682
+  /* "fastphase/calc_func.pyx":675
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)
  *     cdef np.ndarray[ np.float64_t, ndim = 1] tempVal = np.zeros( nK, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     ## initialization
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 682, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 682, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 675, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tempVal.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_tempVal = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 682, __pyx_L1_error)
+      __PYX_ERR(0, 675, __pyx_L1_error)
     } else {__pyx_pybuffernd_tempVal.diminfo[0].strides = __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tempVal.diminfo[0].shape = __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_tempVal = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "fastphase/calc_func.pyx":685
+  /* "fastphase/calc_func.pyx":678
  * 
  *     ## initialization
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         delta[k,0] = log(alpha[ 0, k]) + log(happrG( theta[ 0, k], hap[0]))
  * 
  */
   __pyx_t_10 = __pyx_v_nK;
   __pyx_t_11 = __pyx_t_10;
   for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_k = __pyx_t_12;
 
-    /* "fastphase/calc_func.pyx":686
+    /* "fastphase/calc_func.pyx":679
  *     ## initialization
  *     for k in range(nK):
  *         delta[k,0] = log(alpha[ 0, k]) + log(happrG( theta[ 0, k], hap[0]))             # <<<<<<<<<<<<<<
  * 
  *     ## recursion
  */
     __pyx_t_13 = 0;
@@ -14256,51 +13939,51 @@
     __pyx_t_18 = __pyx_v_k;
     __pyx_t_19 = 0;
     if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_delta.diminfo[0].shape;
     if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_delta.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_delta.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_delta.diminfo[1].strides) = (log((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_14, __pyx_pybuffernd_alpha.diminfo[1].strides))) + log(__pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_hap.diminfo[0].strides)))));
   }
 
-  /* "fastphase/calc_func.pyx":689
+  /* "fastphase/calc_func.pyx":682
  * 
  *     ## recursion
  *     for m in range(1, nLoc):             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             for prev_k in range(nK):
  */
   __pyx_t_10 = __pyx_v_nLoc;
   __pyx_t_11 = __pyx_t_10;
   for (__pyx_t_12 = 1; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_m = __pyx_t_12;
 
-    /* "fastphase/calc_func.pyx":690
+    /* "fastphase/calc_func.pyx":683
  *     ## recursion
  *     for m in range(1, nLoc):
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             for prev_k in range(nK):
  *                 ## jump
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_21 = __pyx_t_20;
     for (__pyx_t_22 = 0; __pyx_t_22 < __pyx_t_21; __pyx_t_22+=1) {
       __pyx_v_k = __pyx_t_22;
 
-      /* "fastphase/calc_func.pyx":691
+      /* "fastphase/calc_func.pyx":684
  *     for m in range(1, nLoc):
  *         for k in range(nK):
  *             for prev_k in range(nK):             # <<<<<<<<<<<<<<
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])
  */
       __pyx_t_23 = __pyx_v_nK;
       __pyx_t_24 = __pyx_t_23;
       for (__pyx_t_25 = 0; __pyx_t_25 < __pyx_t_24; __pyx_t_25+=1) {
         __pyx_v_prev_k = __pyx_t_25;
 
-        /* "fastphase/calc_func.pyx":693
+        /* "fastphase/calc_func.pyx":686
  *             for prev_k in range(nK):
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])             # <<<<<<<<<<<<<<
  *                 if k == prev_k:
  *                     ## no jump
  */
         __pyx_t_26 = __pyx_v_m;
@@ -14311,25 +13994,25 @@
         __pyx_t_29 = __pyx_v_k;
         if (__pyx_t_28 < 0) __pyx_t_28 += __pyx_pybuffernd_alpha.diminfo[0].shape;
         if (__pyx_t_29 < 0) __pyx_t_29 += __pyx_pybuffernd_alpha.diminfo[1].shape;
         __pyx_t_30 = __pyx_v_prev_k;
         if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_pybuffernd_tempVal.diminfo[0].shape;
         *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_tempVal.diminfo[0].strides) = (log((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_rho.diminfo[1].strides))) + log((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_alpha.diminfo[1].strides))));
 
-        /* "fastphase/calc_func.pyx":694
+        /* "fastphase/calc_func.pyx":687
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])
  *                 if k == prev_k:             # <<<<<<<<<<<<<<
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  */
         __pyx_t_31 = ((__pyx_v_k == __pyx_v_prev_k) != 0);
         if (__pyx_t_31) {
 
-          /* "fastphase/calc_func.pyx":696
+          /* "fastphase/calc_func.pyx":689
  *                 if k == prev_k:
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))             # <<<<<<<<<<<<<<
  *                 tempVal[ prev_k] += delta[prev_k, m-1]
  *                 psi[ k, m] = argmax(tempVal, nK)
  */
           __pyx_t_32 = __pyx_v_m;
@@ -14344,52 +14027,52 @@
           __pyx_t_37 = 0;
           if (__pyx_t_36 < 0) __pyx_t_36 += __pyx_pybuffernd_rho.diminfo[0].shape;
           if (__pyx_t_37 < 0) __pyx_t_37 += __pyx_pybuffernd_rho.diminfo[1].shape;
           __pyx_t_38 = __pyx_v_prev_k;
           if (__pyx_t_38 < 0) __pyx_t_38 += __pyx_pybuffernd_tempVal.diminfo[0].shape;
           *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_tempVal.diminfo[0].strides) = log((((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_rho.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_alpha.diminfo[1].strides))) + (1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_rho.diminfo[1].strides)))));
 
-          /* "fastphase/calc_func.pyx":694
+          /* "fastphase/calc_func.pyx":687
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])
  *                 if k == prev_k:             # <<<<<<<<<<<<<<
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  */
         }
 
-        /* "fastphase/calc_func.pyx":697
+        /* "fastphase/calc_func.pyx":690
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  *                 tempVal[ prev_k] += delta[prev_k, m-1]             # <<<<<<<<<<<<<<
  *                 psi[ k, m] = argmax(tempVal, nK)
  *                 delta[ k, m] = tempVal[ psi[ k, m]] +log( happrG( theta[ m, k], hap[ m]))
  */
         __pyx_t_39 = __pyx_v_prev_k;
         __pyx_t_40 = (__pyx_v_m - 1);
         if (__pyx_t_39 < 0) __pyx_t_39 += __pyx_pybuffernd_delta.diminfo[0].shape;
         if (__pyx_t_40 < 0) __pyx_t_40 += __pyx_pybuffernd_delta.diminfo[1].shape;
         __pyx_t_41 = __pyx_v_prev_k;
         if (__pyx_t_41 < 0) __pyx_t_41 += __pyx_pybuffernd_tempVal.diminfo[0].shape;
         *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_41, __pyx_pybuffernd_tempVal.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_delta.diminfo[0].strides, __pyx_t_40, __pyx_pybuffernd_delta.diminfo[1].strides));
 
-        /* "fastphase/calc_func.pyx":698
+        /* "fastphase/calc_func.pyx":691
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  *                 tempVal[ prev_k] += delta[prev_k, m-1]
  *                 psi[ k, m] = argmax(tempVal, nK)             # <<<<<<<<<<<<<<
  *                 delta[ k, m] = tempVal[ psi[ k, m]] +log( happrG( theta[ m, k], hap[ m]))
  * 
  */
         __pyx_t_42 = __pyx_v_k;
         __pyx_t_43 = __pyx_v_m;
         if (__pyx_t_42 < 0) __pyx_t_42 += __pyx_pybuffernd_psi.diminfo[0].shape;
         if (__pyx_t_43 < 0) __pyx_t_43 += __pyx_pybuffernd_psi.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_psi.rcbuffer->pybuffer.buf, __pyx_t_42, __pyx_pybuffernd_psi.diminfo[0].strides, __pyx_t_43, __pyx_pybuffernd_psi.diminfo[1].strides) = __pyx_f_9fastphase_9calc_func_argmax(((PyArrayObject *)__pyx_v_tempVal), __pyx_v_nK);
 
-        /* "fastphase/calc_func.pyx":699
+        /* "fastphase/calc_func.pyx":692
  *                 tempVal[ prev_k] += delta[prev_k, m-1]
  *                 psi[ k, m] = argmax(tempVal, nK)
  *                 delta[ k, m] = tempVal[ psi[ k, m]] +log( happrG( theta[ m, k], hap[ m]))             # <<<<<<<<<<<<<<
  * 
  *     ## termination
  */
         __pyx_t_44 = __pyx_v_k;
@@ -14409,51 +14092,51 @@
         if (__pyx_t_50 < 0) __pyx_t_50 += __pyx_pybuffernd_delta.diminfo[0].shape;
         if (__pyx_t_51 < 0) __pyx_t_51 += __pyx_pybuffernd_delta.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf, __pyx_t_50, __pyx_pybuffernd_delta.diminfo[0].strides, __pyx_t_51, __pyx_pybuffernd_delta.diminfo[1].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_tempVal.diminfo[0].strides)) + log(__pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_47, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_48, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_49, __pyx_pybuffernd_hap.diminfo[0].strides)))));
       }
     }
   }
 
-  /* "fastphase/calc_func.pyx":702
+  /* "fastphase/calc_func.pyx":695
  * 
  *     ## termination
  *     soluce[ nLoc - 1 ] = argmax( delta[ :, nLoc-1], nK)             # <<<<<<<<<<<<<<
  *     for m in range( nLoc - 2, -1, -1):
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]
  */
-  __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_nLoc - 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 702, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_nLoc - 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 702, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_slice_);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_delta), __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 702, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_delta), __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 695, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 702, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 695, __pyx_L1_error)
   __pyx_t_52 = (__pyx_v_nLoc - 1);
   if (__pyx_t_52 < 0) __pyx_t_52 += __pyx_pybuffernd_soluce.diminfo[0].shape;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_soluce.rcbuffer->pybuffer.buf, __pyx_t_52, __pyx_pybuffernd_soluce.diminfo[0].strides) = __pyx_f_9fastphase_9calc_func_argmax(((PyArrayObject *)__pyx_t_4), __pyx_v_nK);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastphase/calc_func.pyx":703
+  /* "fastphase/calc_func.pyx":696
  *     ## termination
  *     soluce[ nLoc - 1 ] = argmax( delta[ :, nLoc-1], nK)
  *     for m in range( nLoc - 2, -1, -1):             # <<<<<<<<<<<<<<
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]
  *     return soluce
  */
   for (__pyx_t_10 = (__pyx_v_nLoc - 2); __pyx_t_10 > -1; __pyx_t_10-=1) {
     __pyx_v_m = __pyx_t_10;
 
-    /* "fastphase/calc_func.pyx":704
+    /* "fastphase/calc_func.pyx":697
  *     soluce[ nLoc - 1 ] = argmax( delta[ :, nLoc-1], nK)
  *     for m in range( nLoc - 2, -1, -1):
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]             # <<<<<<<<<<<<<<
  *     return soluce
  * 
  */
     __pyx_t_53 = (__pyx_v_m + 1);
@@ -14463,27 +14146,27 @@
     if (__pyx_t_54 < 0) __pyx_t_54 += __pyx_pybuffernd_psi.diminfo[0].shape;
     if (__pyx_t_55 < 0) __pyx_t_55 += __pyx_pybuffernd_psi.diminfo[1].shape;
     __pyx_t_56 = __pyx_v_m;
     if (__pyx_t_56 < 0) __pyx_t_56 += __pyx_pybuffernd_soluce.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_soluce.rcbuffer->pybuffer.buf, __pyx_t_56, __pyx_pybuffernd_soluce.diminfo[0].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_psi.rcbuffer->pybuffer.buf, __pyx_t_54, __pyx_pybuffernd_psi.diminfo[0].strides, __pyx_t_55, __pyx_pybuffernd_psi.diminfo[1].strides));
   }
 
-  /* "fastphase/calc_func.pyx":705
+  /* "fastphase/calc_func.pyx":698
  *     for m in range( nLoc - 2, -1, -1):
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]
  *     return soluce             # <<<<<<<<<<<<<<
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_soluce));
   __pyx_r = ((PyObject *)__pyx_v_soluce);
   goto __pyx_L0;
 
-  /* "fastphase/calc_func.pyx":667
+  /* "fastphase/calc_func.pyx":660
  *         return 1
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -14568,31 +14251,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aa)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 1); __PYX_ERR(0, 667, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 1); __PYX_ERR(0, 660, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 2); __PYX_ERR(0, 667, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 2); __PYX_ERR(0, 660, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hh)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 3); __PYX_ERR(0, 667, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 3); __PYX_ERR(0, 660, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapViterbi") < 0)) __PYX_ERR(0, 667, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapViterbi") < 0)) __PYX_ERR(0, 660, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -14601,15 +14284,15 @@
     __pyx_v_aa = values[0];
     __pyx_v_tt = values[1];
     __pyx_v_rr = values[2];
     __pyx_v_hh = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 667, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 660, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastphase.calc_func.hapViterbi", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9fastphase_9calc_func_14hapViterbi(__pyx_self, __pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh);
 
@@ -14620,15 +14303,15 @@
 
 static PyObject *__pyx_pf_9fastphase_9calc_func_14hapViterbi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_aa, PyObject *__pyx_v_tt, PyObject *__pyx_v_rr, PyObject *__pyx_v_hh) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("hapViterbi", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9fastphase_9calc_func_hapViterbi(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9fastphase_9calc_func_hapViterbi(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14637,15 +14320,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/calc_func.pyx":707
+/* "fastphase/calc_func.pyx":700
  *     return soluce
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -14897,316 +14580,316 @@
   __pyx_pybuffernd_top.data = NULL;
   __pyx_pybuffernd_top.rcbuffer = &__pyx_pybuffer_top;
   __pyx_pybuffer_bot.pybuffer.buf = NULL;
   __pyx_pybuffer_bot.refcount = 0;
   __pyx_pybuffernd_bot.data = NULL;
   __pyx_pybuffernd_bot.rcbuffer = &__pyx_pybuffer_bot;
 
-  /* "fastphase/calc_func.pyx":708
+  /* "fastphase/calc_func.pyx":701
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  */
-  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 708, __pyx_L1_error)
+  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 701, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_aa;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alpha.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_alpha = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 708, __pyx_L1_error)
+      __PYX_ERR(0, 701, __pyx_L1_error)
     } else {__pyx_pybuffernd_alpha.diminfo[0].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alpha.diminfo[0].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_alpha.diminfo[1].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_alpha.diminfo[1].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_alpha = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":709
+  /* "fastphase/calc_func.pyx":702
  * cpdef hapCalc(aa,tt,rr,hh,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  */
-  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 709, __pyx_L1_error)
+  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 702, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_tt;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_theta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 709, __pyx_L1_error)
+      __PYX_ERR(0, 702, __pyx_L1_error)
     } else {__pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_theta = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":710
+  /* "fastphase/calc_func.pyx":703
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  *     cdef int up2pz=u2p
  */
-  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 710, __pyx_L1_error)
+  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 703, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_rr;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rho.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_rho = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 710, __pyx_L1_error)
+      __PYX_ERR(0, 703, __pyx_L1_error)
     } else {__pyx_pybuffernd_rho.diminfo[0].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rho.diminfo[0].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_rho.diminfo[1].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_rho.diminfo[1].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_rho = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":711
+  /* "fastphase/calc_func.pyx":704
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh             # <<<<<<<<<<<<<<
  *     cdef int up2pz=u2p
  *     ## cython declarations
  */
-  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 711, __pyx_L1_error)
+  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 704, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_hh;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_hap.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_hap = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 711, __pyx_L1_error)
+      __PYX_ERR(0, 704, __pyx_L1_error)
     } else {__pyx_pybuffernd_hap.diminfo[0].strides = __pyx_pybuffernd_hap.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_hap.diminfo[0].shape = __pyx_pybuffernd_hap.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_v_hap = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":712
+  /* "fastphase/calc_func.pyx":705
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  *     cdef int up2pz=u2p             # <<<<<<<<<<<<<<
  *     ## cython declarations
  *     cdef int nLoc,nK,tScale
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 705, __pyx_L1_error)
   __pyx_v_up2pz = __pyx_t_2;
 
-  /* "fastphase/calc_func.pyx":720
+  /* "fastphase/calc_func.pyx":713
  *     cdef double logLikelihood
  *     ## end cython declarations
  *     nLoc=alpha.shape[0]             # <<<<<<<<<<<<<<
  *     nK=alpha.shape[1]
  *     ##
  */
   __pyx_v_nLoc = (__pyx_v_alpha->dimensions[0]);
 
-  /* "fastphase/calc_func.pyx":721
+  /* "fastphase/calc_func.pyx":714
  *     ## end cython declarations
  *     nLoc=alpha.shape[0]
  *     nK=alpha.shape[1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute backward probabilities
  */
   __pyx_v_nK = (__pyx_v_alpha->dimensions[1]);
 
-  /* "fastphase/calc_func.pyx":725
+  /* "fastphase/calc_func.pyx":718
  *     ## compute backward probabilities
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=1] tSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 725, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 725, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 725, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 718, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_betaScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_betaScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 725, __pyx_L1_error)
+      __PYX_ERR(0, 718, __pyx_L1_error)
     } else {__pyx_pybuffernd_betaScale.diminfo[0].strides = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_betaScale.diminfo[0].shape = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_betaScale = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/calc_func.pyx":726
+  /* "fastphase/calc_func.pyx":719
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=1] tSum=np.zeros(nLoc,dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 726, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 726, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 726, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 719, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tSum.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_tSum = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 726, __pyx_L1_error)
+      __PYX_ERR(0, 719, __pyx_L1_error)
     } else {__pyx_pybuffernd_tSum.diminfo[0].strides = __pyx_pybuffernd_tSum.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tSum.diminfo[0].shape = __pyx_pybuffernd_tSum.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_tSum = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":727
+  /* "fastphase/calc_func.pyx":720
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=1] tSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for k in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_5 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 727, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 720, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 727, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 720, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mBeta.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_mBeta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 727, __pyx_L1_error)
+      __PYX_ERR(0, 720, __pyx_L1_error)
     } else {__pyx_pybuffernd_mBeta.diminfo[0].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mBeta.diminfo[0].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mBeta.diminfo[1].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mBeta.diminfo[1].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_mBeta = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/calc_func.pyx":729
+  /* "fastphase/calc_func.pyx":722
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         mBeta[nLoc-1,k]=1
  * 
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":730
+    /* "fastphase/calc_func.pyx":723
  * 
  *     for k in range(nK):
  *         mBeta[nLoc-1,k]=1             # <<<<<<<<<<<<<<
  * 
  *     for k in range(nK):
  */
     __pyx_t_12 = (__pyx_v_nLoc - 1);
     __pyx_t_13 = __pyx_v_k;
     if (__pyx_t_12 < 0) __pyx_t_12 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
     if (__pyx_t_13 < 0) __pyx_t_13 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_13, __pyx_pybuffernd_mBeta.diminfo[1].strides) = 1.0;
   }
 
-  /* "fastphase/calc_func.pyx":732
+  /* "fastphase/calc_func.pyx":725
  *         mBeta[nLoc-1,k]=1
  * 
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]
  *     for m in range(nLoc-1,0,-1):
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":733
+    /* "fastphase/calc_func.pyx":726
  * 
  *     for k in range(nK):
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]             # <<<<<<<<<<<<<<
  *     for m in range(nLoc-1,0,-1):
  *         tScaleTemp=0
  */
     __pyx_t_14 = (__pyx_v_nLoc - 1);
@@ -15220,46 +14903,46 @@
     if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_alpha.diminfo[0].shape;
     if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_alpha.diminfo[1].shape;
     __pyx_t_19 = (__pyx_v_nLoc - 1);
     if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_tSum.diminfo[0].strides) += (__pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_hap.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_alpha.diminfo[1].strides)));
   }
 
-  /* "fastphase/calc_func.pyx":734
+  /* "fastphase/calc_func.pyx":727
  *     for k in range(nK):
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]
  *     for m in range(nLoc-1,0,-1):             # <<<<<<<<<<<<<<
  *         tScaleTemp=0
  *         ## this loop can be parallelized across clusters #CUDA
  */
   for (__pyx_t_2 = (__pyx_v_nLoc - 1); __pyx_t_2 > 0; __pyx_t_2-=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":735
+    /* "fastphase/calc_func.pyx":728
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]
  *     for m in range(nLoc-1,0,-1):
  *         tScaleTemp=0             # <<<<<<<<<<<<<<
  *         ## this loop can be parallelized across clusters #CUDA
  *         for k in range(nK):
  */
     __pyx_v_tScaleTemp = 0.0;
 
-    /* "fastphase/calc_func.pyx":737
+    /* "fastphase/calc_func.pyx":730
  *         tScaleTemp=0
  *         ## this loop can be parallelized across clusters #CUDA
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  */
     __pyx_t_10 = __pyx_v_nK;
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
       __pyx_v_k = __pyx_t_20;
 
-      /* "fastphase/calc_func.pyx":738
+      /* "fastphase/calc_func.pyx":731
  *         ## this loop can be parallelized across clusters #CUDA
  *         for k in range(nK):
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]             # <<<<<<<<<<<<<<
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]
  */
       __pyx_t_21 = __pyx_v_m;
@@ -15274,15 +14957,15 @@
       if (__pyx_t_25 < 0) __pyx_t_25 += __pyx_pybuffernd_hap.diminfo[0].shape;
       __pyx_t_26 = __pyx_v_m;
       __pyx_t_27 = __pyx_v_k;
       if (__pyx_t_26 < 0) __pyx_t_26 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_27 < 0) __pyx_t_27 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       __pyx_v_temp = (((1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_rho.diminfo[1].strides))) * __pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_24, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_25, __pyx_pybuffernd_hap.diminfo[0].strides)))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_mBeta.diminfo[1].strides)));
 
-      /* "fastphase/calc_func.pyx":739
+      /* "fastphase/calc_func.pyx":732
  *         for k in range(nK):
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]             # <<<<<<<<<<<<<<
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]
  *             tScaleTemp+=mBeta[m-1,k]
  */
       __pyx_t_28 = __pyx_v_m;
@@ -15293,15 +14976,15 @@
       if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_t_31 = (__pyx_v_m - 1);
       __pyx_t_32 = __pyx_v_k;
       if (__pyx_t_31 < 0) __pyx_t_31 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_32 < 0) __pyx_t_32 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_31, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_32, __pyx_pybuffernd_mBeta.diminfo[1].strides) = (__pyx_v_temp + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_rho.diminfo[1].strides)) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_tSum.diminfo[0].strides))));
 
-      /* "fastphase/calc_func.pyx":740
+      /* "fastphase/calc_func.pyx":733
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]             # <<<<<<<<<<<<<<
  *             tScaleTemp+=mBeta[m-1,k]
  *         # if np.isnan(tScaleTemp):
  */
       __pyx_t_33 = (__pyx_v_m - 1);
@@ -15318,267 +15001,267 @@
       __pyx_t_39 = __pyx_v_k;
       if (__pyx_t_38 < 0) __pyx_t_38 += __pyx_pybuffernd_alpha.diminfo[0].shape;
       if (__pyx_t_39 < 0) __pyx_t_39 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_40 = (__pyx_v_m - 1);
       if (__pyx_t_40 < 0) __pyx_t_40 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_40, __pyx_pybuffernd_tSum.diminfo[0].strides) += ((__pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_hap.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_mBeta.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_39, __pyx_pybuffernd_alpha.diminfo[1].strides)));
 
-      /* "fastphase/calc_func.pyx":741
+      /* "fastphase/calc_func.pyx":734
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]
  *             tScaleTemp+=mBeta[m-1,k]             # <<<<<<<<<<<<<<
  *         # if np.isnan(tScaleTemp):
  *         #     print mBeta[m-1]
  */
       __pyx_t_41 = (__pyx_v_m - 1);
       __pyx_t_42 = __pyx_v_k;
       if (__pyx_t_41 < 0) __pyx_t_41 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_42 < 0) __pyx_t_42 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       __pyx_v_tScaleTemp = (__pyx_v_tScaleTemp + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_41, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_42, __pyx_pybuffernd_mBeta.diminfo[1].strides)));
     }
 
-    /* "fastphase/calc_func.pyx":750
+    /* "fastphase/calc_func.pyx":743
  *         #     print hap[m]
  *         #     print 'BLA'
  *         tScale=int(-log(tScaleTemp)/log(10))             # <<<<<<<<<<<<<<
  *         if tScale<0:
  *             tScale=0
  */
     __pyx_t_43 = (-log(__pyx_v_tScaleTemp));
     __pyx_t_44 = log(10.0);
     if (unlikely(__pyx_t_44 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 750, __pyx_L1_error)
+      __PYX_ERR(0, 743, __pyx_L1_error)
     }
     __pyx_v_tScale = ((int)(__pyx_t_43 / __pyx_t_44));
 
-    /* "fastphase/calc_func.pyx":751
+    /* "fastphase/calc_func.pyx":744
  *         #     print 'BLA'
  *         tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale<0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     __pyx_t_45 = ((__pyx_v_tScale < 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":752
+      /* "fastphase/calc_func.pyx":745
  *         tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale<0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/calc_func.pyx":751
+      /* "fastphase/calc_func.pyx":744
  *         #     print 'BLA'
  *         tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale<0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     }
 
-    /* "fastphase/calc_func.pyx":753
+    /* "fastphase/calc_func.pyx":746
  *         if tScale<0:
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale             # <<<<<<<<<<<<<<
  *         if tScale >0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_46 = __pyx_v_m;
     if (__pyx_t_46 < 0) __pyx_t_46 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     __pyx_t_47 = (__pyx_v_m - 1);
     if (__pyx_t_47 < 0) __pyx_t_47 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_47, __pyx_pybuffernd_betaScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_betaScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-    /* "fastphase/calc_func.pyx":754
+    /* "fastphase/calc_func.pyx":747
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy
  */
     __pyx_t_45 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":755
+      /* "fastphase/calc_func.pyx":748
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             tSum[m-1]*=dummy
  *             for k in range(nK):
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/calc_func.pyx":756
+      /* "fastphase/calc_func.pyx":749
  *         if tScale >0:
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 mBeta[m-1,k]*=dummy
  */
       __pyx_t_48 = (__pyx_v_m - 1);
       if (__pyx_t_48 < 0) __pyx_t_48 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_48, __pyx_pybuffernd_tSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-      /* "fastphase/calc_func.pyx":757
+      /* "fastphase/calc_func.pyx":750
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k]*=dummy
  *     ##
  */
       __pyx_t_10 = __pyx_v_nK;
       __pyx_t_11 = __pyx_t_10;
       for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
         __pyx_v_k = __pyx_t_20;
 
-        /* "fastphase/calc_func.pyx":758
+        /* "fastphase/calc_func.pyx":751
  *             tSum[m-1]*=dummy
  *             for k in range(nK):
  *                 mBeta[m-1,k]*=dummy             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute forward probabilities
  */
         __pyx_t_49 = (__pyx_v_m - 1);
         __pyx_t_50 = __pyx_v_k;
         if (__pyx_t_49 < 0) __pyx_t_49 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_50 < 0) __pyx_t_50 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_49, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_50, __pyx_pybuffernd_mBeta.diminfo[1].strides) *= __pyx_v_dummy;
       }
 
-      /* "fastphase/calc_func.pyx":754
+      /* "fastphase/calc_func.pyx":747
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy
  */
     }
   }
 
-  /* "fastphase/calc_func.pyx":762
+  /* "fastphase/calc_func.pyx":755
  *     ## compute forward probabilities
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=2] mPhi=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     for k in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 762, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 755, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 762, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 755, __pyx_L1_error)
   __pyx_t_51 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mPhi.rcbuffer->pybuffer, (PyObject*)__pyx_t_51, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_mPhi = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 762, __pyx_L1_error)
+      __PYX_ERR(0, 755, __pyx_L1_error)
     } else {__pyx_pybuffernd_mPhi.diminfo[0].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mPhi.diminfo[0].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mPhi.diminfo[1].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mPhi.diminfo[1].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_51 = 0;
   __pyx_v_mPhi = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/calc_func.pyx":763
+  /* "fastphase/calc_func.pyx":756
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=2] mPhi=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     for k in range(nK):
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 763, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 763, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 763, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 756, __pyx_L1_error)
   __pyx_t_52 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_phiScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_52, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_phiScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 763, __pyx_L1_error)
+      __PYX_ERR(0, 756, __pyx_L1_error)
     } else {__pyx_pybuffernd_phiScale.diminfo[0].strides = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_phiScale.diminfo[0].shape = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_52 = 0;
   __pyx_v_phiScale = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/calc_func.pyx":764
+  /* "fastphase/calc_func.pyx":757
  *     cdef np.ndarray[np.float64_t,ndim=2] mPhi=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])
  *     ## calc the marginal sum at locus 0 (appx A)
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":765
+    /* "fastphase/calc_func.pyx":758
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     for k in range(nK):
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])             # <<<<<<<<<<<<<<
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tSum[0]=0
  */
     __pyx_t_53 = 0;
@@ -15594,38 +15277,38 @@
     __pyx_t_58 = 0;
     __pyx_t_59 = __pyx_v_k;
     if (__pyx_t_58 < 0) __pyx_t_58 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
     if (__pyx_t_59 < 0) __pyx_t_59 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_58, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_59, __pyx_pybuffernd_mPhi.diminfo[1].strides) = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_53, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_54, __pyx_pybuffernd_alpha.diminfo[1].strides)) * __pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_55, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_56, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_57, __pyx_pybuffernd_hap.diminfo[0].strides))));
   }
 
-  /* "fastphase/calc_func.pyx":767
+  /* "fastphase/calc_func.pyx":760
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tSum[0]=0             # <<<<<<<<<<<<<<
  *     for k in range(nK):
  *         tSum[0]+=mPhi[0,k]
  */
   __pyx_t_60 = 0;
   if (__pyx_t_60 < 0) __pyx_t_60 += __pyx_pybuffernd_tSum.diminfo[0].shape;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_60, __pyx_pybuffernd_tSum.diminfo[0].strides) = 0.0;
 
-  /* "fastphase/calc_func.pyx":768
+  /* "fastphase/calc_func.pyx":761
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tSum[0]=0
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         tSum[0]+=mPhi[0,k]
  *     ## calc Phi
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":769
+    /* "fastphase/calc_func.pyx":762
  *     tSum[0]=0
  *     for k in range(nK):
  *         tSum[0]+=mPhi[0,k]             # <<<<<<<<<<<<<<
  *     ## calc Phi
  *     for m in range(nLoc-1):
  */
     __pyx_t_61 = 0;
@@ -15633,50 +15316,50 @@
     if (__pyx_t_61 < 0) __pyx_t_61 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
     if (__pyx_t_62 < 0) __pyx_t_62 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
     __pyx_t_63 = 0;
     if (__pyx_t_63 < 0) __pyx_t_63 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_63, __pyx_pybuffernd_tSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_61, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_62, __pyx_pybuffernd_mPhi.diminfo[1].strides));
   }
 
-  /* "fastphase/calc_func.pyx":771
+  /* "fastphase/calc_func.pyx":764
  *         tSum[0]+=mPhi[0,k]
  *     ## calc Phi
  *     for m in range(nLoc-1):             # <<<<<<<<<<<<<<
  *         tSum[m+1]=0
  *         ## this loop could be parallelized across clusters #CUDA
  */
   __pyx_t_64 = (__pyx_v_nLoc - 1);
   __pyx_t_65 = __pyx_t_64;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_65; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/calc_func.pyx":772
+    /* "fastphase/calc_func.pyx":765
  *     ## calc Phi
  *     for m in range(nLoc-1):
  *         tSum[m+1]=0             # <<<<<<<<<<<<<<
  *         ## this loop could be parallelized across clusters #CUDA
  *         for k in range(nK):
  */
     __pyx_t_66 = (__pyx_v_m + 1);
     if (__pyx_t_66 < 0) __pyx_t_66 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_66, __pyx_pybuffernd_tSum.diminfo[0].strides) = 0.0;
 
-    /* "fastphase/calc_func.pyx":774
+    /* "fastphase/calc_func.pyx":767
  *         tSum[m+1]=0
  *         ## this loop could be parallelized across clusters #CUDA
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  */
     __pyx_t_10 = __pyx_v_nK;
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
       __pyx_v_k = __pyx_t_20;
 
-      /* "fastphase/calc_func.pyx":775
+      /* "fastphase/calc_func.pyx":768
  *         ## this loop could be parallelized across clusters #CUDA
  *         for k in range(nK):
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]             # <<<<<<<<<<<<<<
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  *             tSum[m+1]+=mPhi[m+1,k]
  */
       __pyx_t_67 = (__pyx_v_m + 1);
@@ -15695,15 +15378,15 @@
       __pyx_t_74 = __pyx_v_k;
       if (__pyx_t_73 < 0) __pyx_t_73 += __pyx_pybuffernd_alpha.diminfo[0].shape;
       if (__pyx_t_74 < 0) __pyx_t_74 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_75 = __pyx_v_m;
       if (__pyx_t_75 < 0) __pyx_t_75 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_v_temp = (((1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_67, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_68, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_69, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_70, __pyx_pybuffernd_mPhi.diminfo[1].strides))) + (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_71, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_72, __pyx_pybuffernd_rho.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_73, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_74, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_75, __pyx_pybuffernd_tSum.diminfo[0].strides))));
 
-      /* "fastphase/calc_func.pyx":776
+      /* "fastphase/calc_func.pyx":769
  *         for k in range(nK):
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])             # <<<<<<<<<<<<<<
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0
  */
       __pyx_t_76 = (__pyx_v_m + 1);
@@ -15714,15 +15397,15 @@
       if (__pyx_t_78 < 0) __pyx_t_78 += __pyx_pybuffernd_hap.diminfo[0].shape;
       __pyx_t_79 = (__pyx_v_m + 1);
       __pyx_t_80 = __pyx_v_k;
       if (__pyx_t_79 < 0) __pyx_t_79 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_80 < 0) __pyx_t_80 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_79, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_80, __pyx_pybuffernd_mPhi.diminfo[1].strides) = (__pyx_v_temp * __pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_76, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_77, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_78, __pyx_pybuffernd_hap.diminfo[0].strides))));
 
-      /* "fastphase/calc_func.pyx":777
+      /* "fastphase/calc_func.pyx":770
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  *             tSum[m+1]+=mPhi[m+1,k]             # <<<<<<<<<<<<<<
  *         tScale=0
  *         if tSum[m+1] < 0:
  */
       __pyx_t_81 = (__pyx_v_m + 1);
@@ -15730,516 +15413,516 @@
       if (__pyx_t_81 < 0) __pyx_t_81 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_82 < 0) __pyx_t_82 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       __pyx_t_83 = (__pyx_v_m + 1);
       if (__pyx_t_83 < 0) __pyx_t_83 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_83, __pyx_pybuffernd_tSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_81, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_82, __pyx_pybuffernd_mPhi.diminfo[1].strides));
     }
 
-    /* "fastphase/calc_func.pyx":778
+    /* "fastphase/calc_func.pyx":771
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0             # <<<<<<<<<<<<<<
  *         if tSum[m+1] < 0:
  *             phiScale[m+1]=phiScale[m]
  */
     __pyx_v_tScale = 0;
 
-    /* "fastphase/calc_func.pyx":779
+    /* "fastphase/calc_func.pyx":772
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0
  *         if tSum[m+1] < 0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
     __pyx_t_84 = (__pyx_v_m + 1);
     if (__pyx_t_84 < 0) __pyx_t_84 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     __pyx_t_45 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_84, __pyx_pybuffernd_tSum.diminfo[0].strides)) < 0.0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":780
+      /* "fastphase/calc_func.pyx":773
  *         tScale=0
  *         if tSum[m+1] < 0:
  *             phiScale[m+1]=phiScale[m]             # <<<<<<<<<<<<<<
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))
  */
       __pyx_t_85 = __pyx_v_m;
       if (__pyx_t_85 < 0) __pyx_t_85 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       __pyx_t_86 = (__pyx_v_m + 1);
       if (__pyx_t_86 < 0) __pyx_t_86 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_86, __pyx_pybuffernd_phiScale.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_85, __pyx_pybuffernd_phiScale.diminfo[0].strides));
 
-      /* "fastphase/calc_func.pyx":779
+      /* "fastphase/calc_func.pyx":772
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0
  *         if tSum[m+1] < 0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
       goto __pyx_L23;
     }
 
-    /* "fastphase/calc_func.pyx":782
+    /* "fastphase/calc_func.pyx":775
  *             phiScale[m+1]=phiScale[m]
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))             # <<<<<<<<<<<<<<
  *         if tScale < 0:
  *             tScale=0
  */
     /*else*/ {
       __pyx_t_87 = (__pyx_v_m + 1);
       if (__pyx_t_87 < 0) __pyx_t_87 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_t_44 = (-log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_87, __pyx_pybuffernd_tSum.diminfo[0].strides))));
       __pyx_t_43 = log(10.0);
       if (unlikely(__pyx_t_43 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 782, __pyx_L1_error)
+        __PYX_ERR(0, 775, __pyx_L1_error)
       }
       __pyx_v_tScale = ((int)(__pyx_t_44 / __pyx_t_43));
     }
     __pyx_L23:;
 
-    /* "fastphase/calc_func.pyx":783
+    /* "fastphase/calc_func.pyx":776
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))
  *         if tScale < 0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  */
     __pyx_t_45 = ((__pyx_v_tScale < 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":784
+      /* "fastphase/calc_func.pyx":777
  *             tScale=int(-log(tSum[m+1])/log(10))
  *         if tScale < 0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/calc_func.pyx":783
+      /* "fastphase/calc_func.pyx":776
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))
  *         if tScale < 0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  */
     }
 
-    /* "fastphase/calc_func.pyx":785
+    /* "fastphase/calc_func.pyx":778
  *         if tScale < 0:
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale             # <<<<<<<<<<<<<<
  *         if tScale > 0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_88 = __pyx_v_m;
     if (__pyx_t_88 < 0) __pyx_t_88 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     __pyx_t_89 = (__pyx_v_m + 1);
     if (__pyx_t_89 < 0) __pyx_t_89 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_89, __pyx_pybuffernd_phiScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_88, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-    /* "fastphase/calc_func.pyx":786
+    /* "fastphase/calc_func.pyx":779
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy
  */
     __pyx_t_45 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":787
+      /* "fastphase/calc_func.pyx":780
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             tSum[m+1]*=dummy
  *             for k in range(nK):
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/calc_func.pyx":788
+      /* "fastphase/calc_func.pyx":781
  *         if tScale > 0:
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 mPhi[m+1,k]*=dummy
  */
       __pyx_t_90 = (__pyx_v_m + 1);
       if (__pyx_t_90 < 0) __pyx_t_90 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_90, __pyx_pybuffernd_tSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-      /* "fastphase/calc_func.pyx":789
+      /* "fastphase/calc_func.pyx":782
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 mPhi[m+1,k]*=dummy
  *     ## end calc Phi
  */
       __pyx_t_10 = __pyx_v_nK;
       __pyx_t_11 = __pyx_t_10;
       for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
         __pyx_v_k = __pyx_t_20;
 
-        /* "fastphase/calc_func.pyx":790
+        /* "fastphase/calc_func.pyx":783
  *             tSum[m+1]*=dummy
  *             for k in range(nK):
  *                 mPhi[m+1,k]*=dummy             # <<<<<<<<<<<<<<
  *     ## end calc Phi
  *     logLikelihood=log(tSum[nLoc-1])/log(10)-phiScale[nLoc-1]
  */
         __pyx_t_91 = (__pyx_v_m + 1);
         __pyx_t_92 = __pyx_v_k;
         if (__pyx_t_91 < 0) __pyx_t_91 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_92 < 0) __pyx_t_92 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_91, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_92, __pyx_pybuffernd_mPhi.diminfo[1].strides) *= __pyx_v_dummy;
       }
 
-      /* "fastphase/calc_func.pyx":786
+      /* "fastphase/calc_func.pyx":779
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy
  */
     }
   }
 
-  /* "fastphase/calc_func.pyx":792
+  /* "fastphase/calc_func.pyx":785
  *                 mPhi[m+1,k]*=dummy
  *     ## end calc Phi
  *     logLikelihood=log(tSum[nLoc-1])/log(10)-phiScale[nLoc-1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute individual contributions top,bottom,jmk
  */
   __pyx_t_93 = (__pyx_v_nLoc - 1);
   if (__pyx_t_93 < 0) __pyx_t_93 += __pyx_pybuffernd_tSum.diminfo[0].shape;
   __pyx_t_43 = log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_93, __pyx_pybuffernd_tSum.diminfo[0].strides)));
   __pyx_t_44 = log(10.0);
   if (unlikely(__pyx_t_44 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 792, __pyx_L1_error)
+    __PYX_ERR(0, 785, __pyx_L1_error)
   }
   __pyx_t_94 = (__pyx_v_nLoc - 1);
   if (__pyx_t_94 < 0) __pyx_t_94 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
   __pyx_v_logLikelihood = ((__pyx_t_43 / __pyx_t_44) - (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_94, __pyx_pybuffernd_phiScale.diminfo[0].strides)));
 
-  /* "fastphase/calc_func.pyx":797
+  /* "fastphase/calc_func.pyx":790
  *     ##
  *     # compute probZ see appx A at the end
  *     cdef np.ndarray[np.float64_t,ndim=2] probZ=mPhi*mBeta             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __pyx_t_3 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 797, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 797, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 790, __pyx_L1_error)
   __pyx_t_95 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_probZ.rcbuffer->pybuffer, (PyObject*)__pyx_t_95, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_probZ = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 797, __pyx_L1_error)
+      __PYX_ERR(0, 790, __pyx_L1_error)
     } else {__pyx_pybuffernd_probZ.diminfo[0].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_probZ.diminfo[0].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_probZ.diminfo[1].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_probZ.diminfo[1].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_95 = 0;
   __pyx_v_probZ = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/calc_func.pyx":798
+  /* "fastphase/calc_func.pyx":791
  *     # compute probZ see appx A at the end
  *     cdef np.ndarray[np.float64_t,ndim=2] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 798, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 798, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 791, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 798, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 791, __pyx_L1_error)
   __pyx_t_96 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_jmk.rcbuffer->pybuffer, (PyObject*)__pyx_t_96, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_jmk = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 798, __pyx_L1_error)
+      __PYX_ERR(0, 791, __pyx_L1_error)
     } else {__pyx_pybuffernd_jmk.diminfo[0].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_jmk.diminfo[0].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_jmk.diminfo[1].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_jmk.diminfo[1].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_96 = 0;
   __pyx_v_jmk = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":799
+  /* "fastphase/calc_func.pyx":792
  *     cdef np.ndarray[np.float64_t,ndim=2] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 799, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 799, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 792, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 799, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 792, __pyx_L1_error)
   __pyx_t_97 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_top.rcbuffer->pybuffer, (PyObject*)__pyx_t_97, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_top = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_top.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 799, __pyx_L1_error)
+      __PYX_ERR(0, 792, __pyx_L1_error)
     } else {__pyx_pybuffernd_top.diminfo[0].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_top.diminfo[0].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_top.diminfo[1].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_top.diminfo[1].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_97 = 0;
   __pyx_v_top = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/calc_func.pyx":800
+  /* "fastphase/calc_func.pyx":793
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for m in range(nLoc):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 800, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 800, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 793, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 800, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 793, __pyx_L1_error)
   __pyx_t_98 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bot.rcbuffer->pybuffer, (PyObject*)__pyx_t_98, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_bot = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 800, __pyx_L1_error)
+      __PYX_ERR(0, 793, __pyx_L1_error)
     } else {__pyx_pybuffernd_bot.diminfo[0].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bot.diminfo[0].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_bot.diminfo[1].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_bot.diminfo[1].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_98 = 0;
   __pyx_v_bot = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":802
+  /* "fastphase/calc_func.pyx":795
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         normC=0
  *         for k in range(nK):
  */
   __pyx_t_2 = __pyx_v_nLoc;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_m = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":803
+    /* "fastphase/calc_func.pyx":796
  * 
  *     for m in range(nLoc):
  *         normC=0             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             normC+=probZ[m,k]
  */
     __pyx_v_normC = 0.0;
 
-    /* "fastphase/calc_func.pyx":804
+    /* "fastphase/calc_func.pyx":797
  *     for m in range(nLoc):
  *         normC=0
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             normC+=probZ[m,k]
  *         for k in range(nK):
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_99 = __pyx_t_20;
     for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
       __pyx_v_k = __pyx_t_100;
 
-      /* "fastphase/calc_func.pyx":805
+      /* "fastphase/calc_func.pyx":798
  *         normC=0
  *         for k in range(nK):
  *             normC+=probZ[m,k]             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             probZ[m,k]/=normC
  */
       __pyx_t_101 = __pyx_v_m;
       __pyx_t_102 = __pyx_v_k;
       if (__pyx_t_101 < 0) __pyx_t_101 += __pyx_pybuffernd_probZ.diminfo[0].shape;
       if (__pyx_t_102 < 0) __pyx_t_102 += __pyx_pybuffernd_probZ.diminfo[1].shape;
       __pyx_v_normC = (__pyx_v_normC + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_101, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_102, __pyx_pybuffernd_probZ.diminfo[1].strides)));
     }
 
-    /* "fastphase/calc_func.pyx":806
+    /* "fastphase/calc_func.pyx":799
  *         for k in range(nK):
  *             normC+=probZ[m,k]
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             probZ[m,k]/=normC
  *     if up2pz:
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_99 = __pyx_t_20;
     for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
       __pyx_v_k = __pyx_t_100;
 
-      /* "fastphase/calc_func.pyx":807
+      /* "fastphase/calc_func.pyx":800
  *             normC+=probZ[m,k]
  *         for k in range(nK):
  *             probZ[m,k]/=normC             # <<<<<<<<<<<<<<
  *     if up2pz:
  *         return probZ
  */
       __pyx_t_103 = __pyx_v_m;
       __pyx_t_104 = __pyx_v_k;
       if (__pyx_t_103 < 0) __pyx_t_103 += __pyx_pybuffernd_probZ.diminfo[0].shape;
       if (__pyx_t_104 < 0) __pyx_t_104 += __pyx_pybuffernd_probZ.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_103, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_104, __pyx_pybuffernd_probZ.diminfo[1].strides) /= __pyx_v_normC;
     }
   }
 
-  /* "fastphase/calc_func.pyx":808
+  /* "fastphase/calc_func.pyx":801
  *         for k in range(nK):
  *             probZ[m,k]/=normC
  *     if up2pz:             # <<<<<<<<<<<<<<
  *         return probZ
  *     ## compute expected jum prob for each interval (appx C)
  */
   __pyx_t_45 = (__pyx_v_up2pz != 0);
   if (__pyx_t_45) {
 
-    /* "fastphase/calc_func.pyx":809
+    /* "fastphase/calc_func.pyx":802
  *             probZ[m,k]/=normC
  *     if up2pz:
  *         return probZ             # <<<<<<<<<<<<<<
  *     ## compute expected jum prob for each interval (appx C)
  *     # locus 0
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_probZ));
     __pyx_r = ((PyObject *)__pyx_v_probZ);
     goto __pyx_L0;
 
-    /* "fastphase/calc_func.pyx":808
+    /* "fastphase/calc_func.pyx":801
  *         for k in range(nK):
  *             probZ[m,k]/=normC
  *     if up2pz:             # <<<<<<<<<<<<<<
  *         return probZ
  *     ## compute expected jum prob for each interval (appx C)
  */
   }
 
-  /* "fastphase/calc_func.pyx":812
+  /* "fastphase/calc_func.pyx":805
  *     ## compute expected jum prob for each interval (appx C)
  *     # locus 0
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         ##jmk[0,k]=alpha[0,k]
  *         jmk[0, k] = probZ[ 0, k]
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":814
+    /* "fastphase/calc_func.pyx":807
  *     for k in range(nK):
  *         ##jmk[0,k]=alpha[0,k]
  *         jmk[0, k] = probZ[ 0, k]             # <<<<<<<<<<<<<<
  *     for m in range(1,nLoc):
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  */
     __pyx_t_105 = 0;
@@ -16249,54 +15932,54 @@
     __pyx_t_107 = 0;
     __pyx_t_108 = __pyx_v_k;
     if (__pyx_t_107 < 0) __pyx_t_107 += __pyx_pybuffernd_jmk.diminfo[0].shape;
     if (__pyx_t_108 < 0) __pyx_t_108 += __pyx_pybuffernd_jmk.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_107, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_108, __pyx_pybuffernd_jmk.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_105, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_106, __pyx_pybuffernd_probZ.diminfo[1].strides));
   }
 
-  /* "fastphase/calc_func.pyx":815
+  /* "fastphase/calc_func.pyx":808
  *         ##jmk[0,k]=alpha[0,k]
  *         jmk[0, k] = probZ[ 0, k]
  *     for m in range(1,nLoc):             # <<<<<<<<<<<<<<
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  */
   __pyx_t_2 = __pyx_v_nLoc;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 1; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_m = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":816
+    /* "fastphase/calc_func.pyx":809
  *         jmk[0, k] = probZ[ 0, k]
  *     for m in range(1,nLoc):
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  */
     __pyx_t_109 = (__pyx_v_m - 1);
     if (__pyx_t_109 < 0) __pyx_t_109 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     __pyx_t_110 = __pyx_v_m;
     if (__pyx_t_110 < 0) __pyx_t_110 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     __pyx_t_111 = (__pyx_v_nLoc - 1);
     if (__pyx_t_111 < 0) __pyx_t_111 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     __pyx_v_dummy = __pyx_f_9fastphase_9calc_func_myPow10((((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_109, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_110, __pyx_pybuffernd_betaScale.diminfo[0].strides))) - (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_111, __pyx_pybuffernd_phiScale.diminfo[0].strides))));
 
-    /* "fastphase/calc_func.pyx":817
+    /* "fastphase/calc_func.pyx":810
  *     for m in range(1,nLoc):
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             jmk[m,k] *= alpha[m,k]
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_99 = __pyx_t_20;
     for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
       __pyx_v_k = __pyx_t_100;
 
-      /* "fastphase/calc_func.pyx":818
+      /* "fastphase/calc_func.pyx":811
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]             # <<<<<<<<<<<<<<
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tSum[nLoc-1]
  */
       __pyx_t_112 = (__pyx_v_m - 1);
@@ -16317,15 +16000,15 @@
       if (__pyx_t_119 < 0) __pyx_t_119 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       __pyx_t_120 = __pyx_v_m;
       __pyx_t_121 = __pyx_v_k;
       if (__pyx_t_120 < 0) __pyx_t_120 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_121 < 0) __pyx_t_121 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_120, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_121, __pyx_pybuffernd_jmk.diminfo[1].strides) = ((((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_112, __pyx_pybuffernd_tSum.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_113, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_114, __pyx_pybuffernd_rho.diminfo[1].strides))) * __pyx_f_9fastphase_9calc_func_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_115, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_116, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_117, __pyx_pybuffernd_hap.diminfo[0].strides)))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_118, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_119, __pyx_pybuffernd_mBeta.diminfo[1].strides)));
 
-      /* "fastphase/calc_func.pyx":819
+      /* "fastphase/calc_func.pyx":812
  *         for k in range(nK):
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             jmk[m,k] *= alpha[m,k]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= tSum[nLoc-1]
  *             jmk[m,k] /= dummy
  */
       __pyx_t_122 = __pyx_v_m;
@@ -16334,81 +16017,81 @@
       if (__pyx_t_123 < 0) __pyx_t_123 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_124 = __pyx_v_m;
       __pyx_t_125 = __pyx_v_k;
       if (__pyx_t_124 < 0) __pyx_t_124 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_125 < 0) __pyx_t_125 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_124, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_125, __pyx_pybuffernd_jmk.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_122, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_123, __pyx_pybuffernd_alpha.diminfo[1].strides));
 
-      /* "fastphase/calc_func.pyx":820
+      /* "fastphase/calc_func.pyx":813
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tSum[nLoc-1]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= dummy
  *             # if not np.isfinite(jmk[m,k]):
  */
       __pyx_t_126 = (__pyx_v_nLoc - 1);
       if (__pyx_t_126 < 0) __pyx_t_126 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_t_127 = __pyx_v_m;
       __pyx_t_128 = __pyx_v_k;
       if (__pyx_t_127 < 0) __pyx_t_127 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_128 < 0) __pyx_t_128 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_127, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_128, __pyx_pybuffernd_jmk.diminfo[1].strides) /= (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_126, __pyx_pybuffernd_tSum.diminfo[0].strides));
 
-      /* "fastphase/calc_func.pyx":821
+      /* "fastphase/calc_func.pyx":814
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tSum[nLoc-1]
  *             jmk[m,k] /= dummy             # <<<<<<<<<<<<<<
  *             # if not np.isfinite(jmk[m,k]):
  *             #     print tSum[m-1],rho[m,0],theta[m,k],hap[m],mBeta[m,k]
  */
       __pyx_t_129 = __pyx_v_m;
       __pyx_t_130 = __pyx_v_k;
       if (__pyx_t_129 < 0) __pyx_t_129 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_130 < 0) __pyx_t_130 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_129, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_130, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_v_dummy;
     }
   }
 
-  /* "fastphase/calc_func.pyx":829
+  /* "fastphase/calc_func.pyx":822
  *             #     raise ValueError
  *     # calc thetablock and its inner product with probZ (appx C.)
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         if hap[m] == 0:
  *             for k in range(nK):
  */
   __pyx_t_2 = __pyx_v_nLoc;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_m = __pyx_t_11;
 
-    /* "fastphase/calc_func.pyx":830
+    /* "fastphase/calc_func.pyx":823
  *     # calc thetablock and its inner product with probZ (appx C.)
  *     for m in range(nLoc):
  *         if hap[m] == 0:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  */
     __pyx_t_131 = __pyx_v_m;
     if (__pyx_t_131 < 0) __pyx_t_131 += __pyx_pybuffernd_hap.diminfo[0].shape;
     __pyx_t_45 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_131, __pyx_pybuffernd_hap.diminfo[0].strides)) == 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":831
+      /* "fastphase/calc_func.pyx":824
  *     for m in range(nLoc):
  *         if hap[m] == 0:
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:
  */
       __pyx_t_20 = __pyx_v_nK;
       __pyx_t_99 = __pyx_t_20;
       for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
         __pyx_v_k = __pyx_t_100;
 
-        /* "fastphase/calc_func.pyx":832
+        /* "fastphase/calc_func.pyx":825
  *         if hap[m] == 0:
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]             # <<<<<<<<<<<<<<
  *         elif hap[m]==1:
  *             for k in range(nK):
  */
         __pyx_t_132 = __pyx_v_m;
@@ -16418,49 +16101,49 @@
         __pyx_t_134 = __pyx_v_m;
         __pyx_t_135 = __pyx_v_k;
         if (__pyx_t_134 < 0) __pyx_t_134 += __pyx_pybuffernd_bot.diminfo[0].shape;
         if (__pyx_t_135 < 0) __pyx_t_135 += __pyx_pybuffernd_bot.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_134, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_135, __pyx_pybuffernd_bot.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_132, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_133, __pyx_pybuffernd_probZ.diminfo[1].strides));
       }
 
-      /* "fastphase/calc_func.pyx":830
+      /* "fastphase/calc_func.pyx":823
  *     # calc thetablock and its inner product with probZ (appx C.)
  *     for m in range(nLoc):
  *         if hap[m] == 0:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  */
       goto __pyx_L43;
     }
 
-    /* "fastphase/calc_func.pyx":833
+    /* "fastphase/calc_func.pyx":826
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]
  */
     __pyx_t_136 = __pyx_v_m;
     if (__pyx_t_136 < 0) __pyx_t_136 += __pyx_pybuffernd_hap.diminfo[0].shape;
     __pyx_t_45 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_136, __pyx_pybuffernd_hap.diminfo[0].strides)) == 1) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/calc_func.pyx":834
+      /* "fastphase/calc_func.pyx":827
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 top[m,k]=probZ[m,k]
  *                 bot[m,k]=probZ[m,k]
  */
       __pyx_t_20 = __pyx_v_nK;
       __pyx_t_99 = __pyx_t_20;
       for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
         __pyx_v_k = __pyx_t_100;
 
-        /* "fastphase/calc_func.pyx":835
+        /* "fastphase/calc_func.pyx":828
  *         elif hap[m]==1:
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]             # <<<<<<<<<<<<<<
  *                 bot[m,k]=probZ[m,k]
  *     return logLikelihood,top,bot,jmk
  */
         __pyx_t_137 = __pyx_v_m;
@@ -16469,15 +16152,15 @@
         if (__pyx_t_138 < 0) __pyx_t_138 += __pyx_pybuffernd_probZ.diminfo[1].shape;
         __pyx_t_139 = __pyx_v_m;
         __pyx_t_140 = __pyx_v_k;
         if (__pyx_t_139 < 0) __pyx_t_139 += __pyx_pybuffernd_top.diminfo[0].shape;
         if (__pyx_t_140 < 0) __pyx_t_140 += __pyx_pybuffernd_top.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_top.rcbuffer->pybuffer.buf, __pyx_t_139, __pyx_pybuffernd_top.diminfo[0].strides, __pyx_t_140, __pyx_pybuffernd_top.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_137, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_138, __pyx_pybuffernd_probZ.diminfo[1].strides));
 
-        /* "fastphase/calc_func.pyx":836
+        /* "fastphase/calc_func.pyx":829
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]
  *                 bot[m,k]=probZ[m,k]             # <<<<<<<<<<<<<<
  *     return logLikelihood,top,bot,jmk
  * 
  */
         __pyx_t_141 = __pyx_v_m;
@@ -16487,36 +16170,36 @@
         __pyx_t_143 = __pyx_v_m;
         __pyx_t_144 = __pyx_v_k;
         if (__pyx_t_143 < 0) __pyx_t_143 += __pyx_pybuffernd_bot.diminfo[0].shape;
         if (__pyx_t_144 < 0) __pyx_t_144 += __pyx_pybuffernd_bot.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_143, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_144, __pyx_pybuffernd_bot.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_141, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_142, __pyx_pybuffernd_probZ.diminfo[1].strides));
       }
 
-      /* "fastphase/calc_func.pyx":833
+      /* "fastphase/calc_func.pyx":826
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]
  */
     }
     __pyx_L43:;
   }
 
-  /* "fastphase/calc_func.pyx":837
+  /* "fastphase/calc_func.pyx":830
  *                 top[m,k]=probZ[m,k]
  *                 bot[m,k]=probZ[m,k]
  *     return logLikelihood,top,bot,jmk             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 830, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 830, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_v_top));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_top));
   PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_top));
   __Pyx_INCREF(((PyObject *)__pyx_v_bot));
@@ -16526,15 +16209,15 @@
   __Pyx_GIVEREF(((PyObject *)__pyx_v_jmk));
   PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject *)__pyx_v_jmk));
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "fastphase/calc_func.pyx":707
+  /* "fastphase/calc_func.pyx":700
  *     return soluce
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -16637,37 +16320,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aa)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 1); __PYX_ERR(0, 707, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 1); __PYX_ERR(0, 700, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 2); __PYX_ERR(0, 707, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 2); __PYX_ERR(0, 700, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hh)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 3); __PYX_ERR(0, 707, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 3); __PYX_ERR(0, 700, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u2p)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 4); __PYX_ERR(0, 707, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 4); __PYX_ERR(0, 700, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapCalc") < 0)) __PYX_ERR(0, 707, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapCalc") < 0)) __PYX_ERR(0, 700, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -16678,15 +16361,15 @@
     __pyx_v_tt = values[1];
     __pyx_v_rr = values[2];
     __pyx_v_hh = values[3];
     __pyx_v_u2p = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 707, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 700, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastphase.calc_func.hapCalc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9fastphase_9calc_func_16hapCalc(__pyx_self, __pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, __pyx_v_u2p);
 
@@ -16697,15 +16380,15 @@
 
 static PyObject *__pyx_pf_9fastphase_9calc_func_16hapCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_aa, PyObject *__pyx_v_tt, PyObject *__pyx_v_rr, PyObject *__pyx_v_hh, PyObject *__pyx_v_u2p) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("hapCalc", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9fastphase_9calc_func_hapCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9fastphase_9calc_func_hapCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19194,15 +18877,14 @@
   {&__pyx_n_s_calc_cost_matrix_geno_tot, __pyx_k_calc_cost_matrix_geno_tot, sizeof(__pyx_k_calc_cost_matrix_geno_tot), 0, 0, 1, 1},
   {&__pyx_n_s_calc_cost_matrix_haplo, __pyx_k_calc_cost_matrix_haplo, sizeof(__pyx_k_calc_cost_matrix_haplo), 0, 0, 1, 1},
   {&__pyx_n_s_calc_cost_matrix_haplo_tot, __pyx_k_calc_cost_matrix_haplo_tot, sizeof(__pyx_k_calc_cost_matrix_haplo_tot), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_cost_mat, __pyx_k_cost_mat, sizeof(__pyx_k_cost_mat), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
-  {&__pyx_n_s_exp, __pyx_k_exp, sizeof(__pyx_k_exp), 0, 0, 1, 1},
   {&__pyx_n_s_fastphase_calc_func, __pyx_k_fastphase_calc_func, sizeof(__pyx_k_fastphase_calc_func), 0, 0, 1, 1},
   {&__pyx_kp_s_fastphase_calc_func_pyx, __pyx_k_fastphase_calc_func_pyx, sizeof(__pyx_k_fastphase_calc_func_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
   {&__pyx_n_s_genCalc, __pyx_k_genCalc, sizeof(__pyx_k_genCalc), 0, 0, 1, 1},
   {&__pyx_n_s_genViterbi, __pyx_k_genViterbi, sizeof(__pyx_k_genViterbi), 0, 0, 1, 1},
   {&__pyx_n_s_gg, __pyx_k_gg, sizeof(__pyx_k_gg), 0, 0, 1, 1},
   {&__pyx_n_s_hapCalc, __pyx_k_hapCalc, sizeof(__pyx_k_hapCalc), 0, 0, 1, 1},
@@ -19408,49 +19090,49 @@
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
   __pyx_tuple__19 = PyTuple_Pack(5, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_gg, __pyx_n_s_u2p); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
   __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_genCalc, 220, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 220, __pyx_L1_error)
 
-  /* "fastphase/calc_func.pyx":435
- *     return rez
+  /* "fastphase/calc_func.pyx":428
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
-  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_ll, __pyx_n_s_u2p); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(5, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_ll, __pyx_n_s_u2p); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_likCalc, 435, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_likCalc, 428, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 428, __pyx_L1_error)
 
-  /* "fastphase/calc_func.pyx":667
+  /* "fastphase/calc_func.pyx":660
  *         return 1
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
-  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_hh); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_hh); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_hapViterbi, 667, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(4, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_hapViterbi, 660, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 660, __pyx_L1_error)
 
-  /* "fastphase/calc_func.pyx":707
+  /* "fastphase/calc_func.pyx":700
  *     return soluce
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
-  __pyx_tuple__25 = PyTuple_Pack(5, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_hh, __pyx_n_s_u2p); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(5, __pyx_n_s_aa, __pyx_n_s_tt, __pyx_n_s_rr, __pyx_n_s_hh, __pyx_n_s_u2p); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_hapCalc, 707, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(5, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_fastphase_calc_func_pyx, __pyx_n_s_hapCalc, 700, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 700, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -19844,48 +19526,48 @@
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
   __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_11genCalc, 0, __pyx_n_s_genCalc, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_genCalc, __pyx_t_1) < 0) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":435
- *     return rez
+  /* "fastphase/calc_func.pyx":428
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_13likCalc, 0, __pyx_n_s_likCalc, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_13likCalc, 0, __pyx_n_s_likCalc, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__22)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_likCalc, __pyx_t_1) < 0) __PYX_ERR(0, 435, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_likCalc, __pyx_t_1) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":667
+  /* "fastphase/calc_func.pyx":660
  *         return 1
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_15hapViterbi, 0, __pyx_n_s_hapViterbi, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_15hapViterbi, 0, __pyx_n_s_hapViterbi, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_hapViterbi, __pyx_t_1) < 0) __PYX_ERR(0, 667, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_hapViterbi, __pyx_t_1) < 0) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "fastphase/calc_func.pyx":707
+  /* "fastphase/calc_func.pyx":700
  *     return soluce
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
-  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_17hapCalc, 0, __pyx_n_s_hapCalc, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9calc_func_17hapCalc, 0, __pyx_n_s_hapCalc, NULL, __pyx_n_s_fastphase_calc_func, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 700, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_hapCalc, __pyx_t_1) < 0) __PYX_ERR(0, 707, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_hapCalc, __pyx_t_1) < 0) __PYX_ERR(0, 700, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "fastphase/calc_func.pyx":1
  * #!python             # <<<<<<<<<<<<<<
  * #cython: language_level=3, boundscheck=False, embedsignature=True, binding=True
  * 
  */
```

### Comparing `fastphase-2.0.dev2/fastphase/calc_func.pyx` & `fastphase-2.0.dev3/fastphase/calc_func.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -417,24 +417,17 @@
             for k in range(nK):
                 top[m,k]=0
                 bot[m,k]=0
     return logLikelihood,top,bot,jmk
 
 
 ########################################### Genotype likelihood Calculations #####################################################
-cdef double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):
-    cdef double rez
-    cdef int i
-    
-    rez = 0.0
-    ## g = 0
-    rez = np.exp(gl[0])*(1-t1)*(1-t2)
-    rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
-    rez += np.exp(gl[2])*t1*t2
-    return rez
+
+cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):
+    return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
 
 cpdef likCalc(aa,tt,rr,ll,u2p):
     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
     cdef int up2pz=u2p
@@ -588,34 +581,34 @@
     ## init at 0
     for k1 in range(nK):
         for k2 in range(k1,nK):
             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0) 
             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1) 
             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
-    p_g_givX[0,0] *= np.exp(lik[0,0])
-    p_g_givX[0,1] *= np.exp(lik[0,1])
-    p_g_givX[0,2] *= np.exp(lik[0,2])
+    p_g_givX[0,0] *= lik[0,0]
+    p_g_givX[0,1] *= lik[0,1]
+    p_g_givX[0,2] *= lik[0,2]
     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
     p_g_givX[0]/=normC
             
     for m in range(nLoc-1):
         for k1 in range(nK):
             for k2 in range(k1,nK):
                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
                 temp*=mBeta[m+1,k1,k2]
                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
-        p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
-        p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
-        p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+        p_g_givX[m+1,0] *= lik[m+1,0]
+        p_g_givX[m+1,1] *= lik[m+1,1]
+        p_g_givX[m+1,2] *= lik[m+1,2]
         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
         p_g_givX[m+1]/=normC
                 
     if up2pz>0:
         return probZ,p_g_givX
     # calc jmk
     for k1 in range(nK):
```

### Comparing `fastphase-2.0.dev2/fastphase/fastphase.c` & `fastphase-2.0.dev3/fastphase/fastphase.c`

 * *Files 0% similar despite different names*

```diff
@@ -2342,15 +2342,15 @@
 static int __pyx_f_9fastphase_9fastphase_argmax(PyArrayObject *, int); /*proto*/
 static int __pyx_f_9fastphase_9fastphase_pair2idx(int, int, int); /*proto*/
 static __pyx_ctuple_int__and_int __pyx_f_9fastphase_9fastphase_idx2pair(int, int); /*proto*/
 static double __pyx_f_9fastphase_9fastphase_genprG(double, double, int); /*proto*/
 static double __pyx_f_9fastphase_9fastphase_probJ(int, int, double); /*proto*/
 static PyObject *__pyx_f_9fastphase_9fastphase_genViterbi(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9fastphase_9fastphase_genCalc(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
-static double __pyx_f_9fastphase_9fastphase_likprG(double, double, PyArrayObject *); /*proto*/
+static CYTHON_INLINE double __pyx_f_9fastphase_9fastphase_likprG(double, double, PyArrayObject *); /*proto*/
 static PyObject *__pyx_f_9fastphase_9fastphase_likCalc(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static double __pyx_f_9fastphase_9fastphase_happrG(double, int); /*proto*/
 static PyObject *__pyx_f_9fastphase_9fastphase_hapViterbi(PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9fastphase_9fastphase_hapCalc(PyObject *, PyObject *, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch); /*proto*/
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int32_t = { "int32_t", NULL, sizeof(__pyx_t_5numpy_int32_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int32_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int32_t), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t = { "float64_t", NULL, sizeof(__pyx_t_5numpy_float64_t), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_nn___pyx_t_5numpy_int_t = { "int_t", NULL, sizeof(__pyx_t_5numpy_int_t), { 0 }, 0, IS_UNSIGNED(__pyx_t_5numpy_int_t) ? 'U' : 'I', IS_UNSIGNED(__pyx_t_5numpy_int_t), 0 };
@@ -5304,15 +5304,15 @@
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
       /* "fastphase/fastphase.pyx":198
  *         except AssertionError:
  *             print("Wrong Array Size:", lik.shape,"is not",(self.nLoci,3))
  *             raise             # <<<<<<<<<<<<<<
  *         lik = np.array(lik)
- *         self.genolik[ID] = lik - np.max(lik, axis=1,keepdims=True)
+ *         self.genolik[ID] = np.exp(lik - np.max(lik, axis=1,keepdims=True))
  */
       __Pyx_GIVEREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_ErrRestoreWithState(__pyx_t_5, __pyx_t_6, __pyx_t_4);
       __pyx_t_5 = 0; __pyx_t_6 = 0; __pyx_t_4 = 0; 
       __PYX_ERR(0, 198, __pyx_L5_except_error)
@@ -5335,15 +5335,15 @@
     __pyx_L8_try_end:;
   }
 
   /* "fastphase/fastphase.pyx":199
  *             print("Wrong Array Size:", lik.shape,"is not",(self.nLoci,3))
  *             raise
  *         lik = np.array(lik)             # <<<<<<<<<<<<<<
- *         self.genolik[ID] = lik - np.max(lik, axis=1,keepdims=True)
+ *         self.genolik[ID] = np.exp(lik - np.max(lik, axis=1,keepdims=True))
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_array); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
@@ -5364,45 +5364,66 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF_SET(__pyx_v_lik, __pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "fastphase/fastphase.pyx":200
  *             raise
  *         lik = np.array(lik)
- *         self.genolik[ID] = lik - np.max(lik, axis=1,keepdims=True)             # <<<<<<<<<<<<<<
+ *         self.genolik[ID] = np.exp(lik - np.max(lik, axis=1,keepdims=True))             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_max); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_INCREF(__pyx_v_lik);
-  __Pyx_GIVEREF(__pyx_v_lik);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_lik);
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_keepdims, Py_True) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_max); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_INCREF(__pyx_v_lik);
+  __Pyx_GIVEREF(__pyx_v_lik);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_lik);
+  __pyx_t_10 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_axis, __pyx_int_1) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_keepdims, Py_True) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_5, __pyx_t_10); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_10 = PyNumber_Subtract(__pyx_v_lik, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_9 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
+    __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
+    if (likely(__pyx_t_9)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_9);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_6, function);
+    }
+  }
+  __pyx_t_4 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_9, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Subtract(__pyx_v_lik, __pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_genolik); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_genolik); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_11);
-  if (unlikely(PyObject_SetItem(__pyx_t_11, __pyx_v_ID, __pyx_t_6) < 0)) __PYX_ERR(0, 200, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  if (unlikely(PyObject_SetItem(__pyx_t_6, __pyx_v_ID, __pyx_t_4) < 0)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "fastphase/fastphase.pyx":188
  *             print("Wrong Genotype Size:",gen.shape[0],"is not",self.nLoci)
  *             raise
  *     def addGenotypeLikelihood(self, ID, lik):             # <<<<<<<<<<<<<<
  *         '''
  *         Add a matrix of genotype likelihoods to the model observations.
@@ -21866,229 +21887,64 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "fastphase/fastphase.pyx":911
  * 
  * ########################################### Genotype likelihood Calculations #####################################################
- * cdef double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
- *     cdef double rez
- *     cdef int i
+ * cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
+ * 
  */
 
-static double __pyx_f_9fastphase_9fastphase_likprG(double __pyx_v_t1, double __pyx_v_t2, PyArrayObject *__pyx_v_gl) {
-  double __pyx_v_rez;
+static CYTHON_INLINE double __pyx_f_9fastphase_9fastphase_likprG(double __pyx_v_t1, double __pyx_v_t2, PyArrayObject *__pyx_v_gl) {
   __Pyx_LocalBuf_ND __pyx_pybuffernd_gl;
   __Pyx_Buffer __pyx_pybuffer_gl;
   double __pyx_r;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  Py_ssize_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  double __pyx_t_6;
-  Py_ssize_t __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
-  Py_ssize_t __pyx_t_9;
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
   __Pyx_RefNannySetupContext("likprG", 0);
   __pyx_pybuffer_gl.pybuffer.buf = NULL;
   __pyx_pybuffer_gl.refcount = 0;
   __pyx_pybuffernd_gl.data = NULL;
   __pyx_pybuffernd_gl.rcbuffer = &__pyx_pybuffer_gl;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_gl.rcbuffer->pybuffer, (PyObject*)__pyx_v_gl, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 911, __pyx_L1_error)
   }
   __pyx_pybuffernd_gl.diminfo[0].strides = __pyx_pybuffernd_gl.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_gl.diminfo[0].shape = __pyx_pybuffernd_gl.rcbuffer->pybuffer.shape[0];
 
-  /* "fastphase/fastphase.pyx":915
- *     cdef int i
- * 
- *     rez = 0.0             # <<<<<<<<<<<<<<
- *     ## g = 0
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)
- */
-  __pyx_v_rez = 0.0;
-
-  /* "fastphase/fastphase.pyx":917
- *     rez = 0.0
- *     ## g = 0
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)             # <<<<<<<<<<<<<<
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
- *     rez += np.exp(gl[2])*t1*t2
- */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_exp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = 0;
-  if (__pyx_t_4 < 0) __pyx_t_4 += __pyx_pybuffernd_gl.diminfo[0].shape;
-  __pyx_t_2 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_4, __pyx_pybuffernd_gl.diminfo[0].strides))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble((1.0 - __pyx_v_t1)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble((1.0 - __pyx_v_t2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 917, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_rez = __pyx_t_6;
-
-  /* "fastphase/fastphase.pyx":918
- *     ## g = 0
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)             # <<<<<<<<<<<<<<
- *     rez += np.exp(gl[2])*t1*t2
- *     return rez
- */
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_rez); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_exp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = 1;
-  if (__pyx_t_7 < 0) __pyx_t_7 += __pyx_pybuffernd_gl.diminfo[0].shape;
-  __pyx_t_2 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_7, __pyx_pybuffernd_gl.diminfo[0].strides))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-    }
-  }
-  __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyFloat_FromDouble(((__pyx_v_t1 * (1.0 - __pyx_v_t2)) + ((1.0 - __pyx_v_t1) * __pyx_v_t2))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 918, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_v_rez = __pyx_t_6;
-
-  /* "fastphase/fastphase.pyx":919
- *     rez = np.exp(gl[0])*(1-t1)*(1-t2)
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
- *     rez += np.exp(gl[2])*t1*t2             # <<<<<<<<<<<<<<
- *     return rez
- * 
- */
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_rez); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_exp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_9 = 2;
-  if (__pyx_t_9 < 0) __pyx_t_9 += __pyx_pybuffernd_gl.diminfo[0].shape;
-  __pyx_t_1 = PyFloat_FromDouble((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_9, __pyx_pybuffernd_gl.diminfo[0].strides))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_8)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_8);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-    }
-  }
-  __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_8, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_t1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyNumber_Multiply(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_t2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyNumber_Multiply(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_6 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_rez = __pyx_t_6;
-
-  /* "fastphase/fastphase.pyx":920
- *     rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
- *     rez += np.exp(gl[2])*t1*t2
- *     return rez             # <<<<<<<<<<<<<<
+  /* "fastphase/fastphase.pyx":912
+ * ########################################### Genotype likelihood Calculations #####################################################
+ * cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2             # <<<<<<<<<<<<<<
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):
  */
-  __pyx_r = __pyx_v_rez;
+  __pyx_t_1 = 0;
+  if (__pyx_t_1 < 0) __pyx_t_1 += __pyx_pybuffernd_gl.diminfo[0].shape;
+  __pyx_t_2 = 1;
+  if (__pyx_t_2 < 0) __pyx_t_2 += __pyx_pybuffernd_gl.diminfo[0].shape;
+  __pyx_t_3 = 2;
+  if (__pyx_t_3 < 0) __pyx_t_3 += __pyx_pybuffernd_gl.diminfo[0].shape;
+  __pyx_r = (((((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_1, __pyx_pybuffernd_gl.diminfo[0].strides)) * (1.0 - __pyx_v_t1)) * (1.0 - __pyx_v_t2)) + ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_2, __pyx_pybuffernd_gl.diminfo[0].strides)) * ((__pyx_v_t1 * (1.0 - __pyx_v_t2)) + ((1.0 - __pyx_v_t1) * __pyx_v_t2)))) + (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_gl.rcbuffer->pybuffer.buf, __pyx_t_3, __pyx_pybuffernd_gl.diminfo[0].strides)) * __pyx_v_t1) * __pyx_v_t2));
   goto __pyx_L0;
 
   /* "fastphase/fastphase.pyx":911
  * 
  * ########################################### Genotype likelihood Calculations #####################################################
- * cdef double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
- *     cdef double rez
- *     cdef int i
+ * cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):             # <<<<<<<<<<<<<<
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
+ * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_8);
   { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_gl.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
   __Pyx_WriteUnraisable("fastphase.fastphase.likprG", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
@@ -22097,16 +21953,16 @@
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_gl.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/fastphase.pyx":922
- *     return rez
+/* "fastphase/fastphase.pyx":914
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
 
 static PyObject *__pyx_pw_9fastphase_9fastphase_21likCalc(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
@@ -22396,15 +22252,15 @@
   Py_ssize_t __pyx_t_221;
   Py_ssize_t __pyx_t_222;
   Py_ssize_t __pyx_t_223;
   Py_ssize_t __pyx_t_224;
   Py_ssize_t __pyx_t_225;
   Py_ssize_t __pyx_t_226;
   Py_ssize_t __pyx_t_227;
-  __pyx_t_5numpy_float64_t __pyx_t_228;
+  Py_ssize_t __pyx_t_228;
   Py_ssize_t __pyx_t_229;
   Py_ssize_t __pyx_t_230;
   Py_ssize_t __pyx_t_231;
   Py_ssize_t __pyx_t_232;
   Py_ssize_t __pyx_t_233;
   Py_ssize_t __pyx_t_234;
   Py_ssize_t __pyx_t_235;
@@ -22508,15 +22364,15 @@
   Py_ssize_t __pyx_t_333;
   Py_ssize_t __pyx_t_334;
   Py_ssize_t __pyx_t_335;
   Py_ssize_t __pyx_t_336;
   Py_ssize_t __pyx_t_337;
   Py_ssize_t __pyx_t_338;
   Py_ssize_t __pyx_t_339;
-  Py_ssize_t __pyx_t_340;
+  __pyx_t_5numpy_float64_t __pyx_t_340;
   Py_ssize_t __pyx_t_341;
   Py_ssize_t __pyx_t_342;
   Py_ssize_t __pyx_t_343;
   Py_ssize_t __pyx_t_344;
   Py_ssize_t __pyx_t_345;
   Py_ssize_t __pyx_t_346;
   Py_ssize_t __pyx_t_347;
@@ -22604,617 +22460,617 @@
   __pyx_pybuffernd_top.data = NULL;
   __pyx_pybuffernd_top.rcbuffer = &__pyx_pybuffer_top;
   __pyx_pybuffer_bot.pybuffer.buf = NULL;
   __pyx_pybuffer_bot.refcount = 0;
   __pyx_pybuffernd_bot.data = NULL;
   __pyx_pybuffernd_bot.rcbuffer = &__pyx_pybuffer_bot;
 
-  /* "fastphase/fastphase.pyx":923
+  /* "fastphase/fastphase.pyx":915
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  */
-  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 923, __pyx_L1_error)
+  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 915, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_aa;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alpha.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_alpha = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 923, __pyx_L1_error)
+      __PYX_ERR(0, 915, __pyx_L1_error)
     } else {__pyx_pybuffernd_alpha.diminfo[0].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alpha.diminfo[0].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_alpha.diminfo[1].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_alpha.diminfo[1].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_alpha = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":924
+  /* "fastphase/fastphase.pyx":916
  * cpdef likCalc(aa,tt,rr,ll,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
  */
-  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 924, __pyx_L1_error)
+  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 916, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_tt;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_theta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 924, __pyx_L1_error)
+      __PYX_ERR(0, 916, __pyx_L1_error)
     } else {__pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_theta = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":925
+  /* "fastphase/fastphase.pyx":917
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
  *     cdef int up2pz=u2p
  */
-  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 925, __pyx_L1_error)
+  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 917, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_rr;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rho.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_rho = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 925, __pyx_L1_error)
+      __PYX_ERR(0, 917, __pyx_L1_error)
     } else {__pyx_pybuffernd_rho.diminfo[0].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rho.diminfo[0].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_rho.diminfo[1].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_rho.diminfo[1].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_rho = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":926
+  /* "fastphase/fastphase.pyx":918
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll             # <<<<<<<<<<<<<<
  *     cdef int up2pz=u2p
  * 
  */
-  if (!(likely(((__pyx_v_ll) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_ll, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 926, __pyx_L1_error)
+  if (!(likely(((__pyx_v_ll) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_ll, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 918, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_ll;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_lik.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_lik = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 926, __pyx_L1_error)
+      __PYX_ERR(0, 918, __pyx_L1_error)
     } else {__pyx_pybuffernd_lik.diminfo[0].strides = __pyx_pybuffernd_lik.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_lik.diminfo[0].shape = __pyx_pybuffernd_lik.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_lik.diminfo[1].strides = __pyx_pybuffernd_lik.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_lik.diminfo[1].shape = __pyx_pybuffernd_lik.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_lik = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":927
+  /* "fastphase/fastphase.pyx":919
  *     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
  *     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
  *     cdef int up2pz=u2p             # <<<<<<<<<<<<<<
  * 
  *     ## cython declarations
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 927, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 919, __pyx_L1_error)
   __pyx_v_up2pz = __pyx_t_2;
 
-  /* "fastphase/fastphase.pyx":939
+  /* "fastphase/fastphase.pyx":931
  *     ## end cython declarations
  * 
  *     nLoc=alpha.shape[0]             # <<<<<<<<<<<<<<
  *     nK=alpha.shape[1]
  *     ##
  */
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_nLoc = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":940
+  /* "fastphase/fastphase.pyx":932
  * 
  *     nLoc=alpha.shape[0]
  *     nK=alpha.shape[1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute backward probabilities
  */
-  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_Py_intptr_t((__pyx_v_alpha->dimensions[1])); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_nK = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":944
+  /* "fastphase/fastphase.pyx":936
  *     ## compute backward probabilities
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_nLoc);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 944, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 944, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 944, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 936, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_betaScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_betaScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 944, __pyx_L1_error)
+      __PYX_ERR(0, 936, __pyx_L1_error)
     } else {__pyx_pybuffernd_betaScale.diminfo[0].strides = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_betaScale.diminfo[0].shape = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_betaScale = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/fastphase.pyx":945
+  /* "fastphase/fastphase.pyx":937
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_nK);
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 945, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_1, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 945, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 937, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tSumk.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_tSumk = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 945, __pyx_L1_error)
+      __PYX_ERR(0, 937, __pyx_L1_error)
     } else {__pyx_pybuffernd_tSumk.diminfo[0].strides = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tSumk.diminfo[0].shape = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_tSumk.diminfo[1].strides = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_tSumk.diminfo[1].shape = __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_tSumk = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":946
+  /* "fastphase/fastphase.pyx":938
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_nLoc);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 946, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 938, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 946, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 938, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_tDoubleSum = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 946, __pyx_L1_error)
+      __PYX_ERR(0, 938, __pyx_L1_error)
     } else {__pyx_pybuffernd_tDoubleSum.diminfo[0].strides = __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tDoubleSum.diminfo[0].shape = __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_tDoubleSum = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/fastphase.pyx":947
+  /* "fastphase/fastphase.pyx":939
  *     cdef np.ndarray[np.float64_t,ndim=2] tSumk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=1] tDoubleSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for k1 in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_nK);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_nK);
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 947, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 947, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 939, __pyx_L1_error)
   __pyx_t_10 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mBeta.rcbuffer->pybuffer, (PyObject*)__pyx_t_10, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_mBeta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 947, __pyx_L1_error)
+      __PYX_ERR(0, 939, __pyx_L1_error)
     } else {__pyx_pybuffernd_mBeta.diminfo[0].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mBeta.diminfo[0].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mBeta.diminfo[1].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mBeta.diminfo[1].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_mBeta.diminfo[2].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_mBeta.diminfo[2].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_10 = 0;
   __pyx_v_mBeta = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "fastphase/fastphase.pyx":949
+  /* "fastphase/fastphase.pyx":941
  *     cdef np.ndarray[np.float64_t,ndim=3] mBeta=np.zeros((nLoc,nK,nK),dtype=np.float64)
  * 
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             mBeta[nLoc-1,k1,k2]=1
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 949, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 941, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":950
+    /* "fastphase/fastphase.pyx":942
  * 
  *     for k1 in range(nK):
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             mBeta[nLoc-1,k1,k2]=1
  *     ## calc the marginal sum at locus M as in appendix A
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 950, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 942, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":951
+      /* "fastphase/fastphase.pyx":943
  *     for k1 in range(nK):
  *         for k2 in range(nK):
  *             mBeta[nLoc-1,k1,k2]=1             # <<<<<<<<<<<<<<
  *     ## calc the marginal sum at locus M as in appendix A
  *     for k1 in range(nK):
  */
-      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 951, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 951, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 951, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 951, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_3);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_5);
       __pyx_t_4 = 0;
       __pyx_t_3 = 0;
       __pyx_t_5 = 0;
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_1, __pyx_int_1) < 0)) __PYX_ERR(0, 951, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_1, __pyx_int_1) < 0)) __PYX_ERR(0, 943, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
   }
 
-  /* "fastphase/fastphase.pyx":953
+  /* "fastphase/fastphase.pyx":945
  *             mBeta[nLoc-1,k1,k2]=1
  *     ## calc the marginal sum at locus M as in appendix A
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 953, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":954
+    /* "fastphase/fastphase.pyx":946
  *     ## calc the marginal sum at locus M as in appendix A
  *     for k1 in range(nK):
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 954, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 946, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":955
+      /* "fastphase/fastphase.pyx":947
  *     for k1 in range(nK):
  *         for k2 in range(nK):
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]             # <<<<<<<<<<<<<<
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]
  *     ## recurrent calculations backward
  */
-      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5);
       __pyx_t_1 = 0;
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
       __pyx_t_1 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
       __pyx_t_4 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_theta), __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_lik), __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_lik), __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 955, __pyx_L1_error)
-      __pyx_t_6 = PyFloat_FromDouble(__pyx_f_9fastphase_9fastphase_likprG(__pyx_t_16, __pyx_t_17, ((PyArrayObject *)__pyx_t_1))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 947, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble(__pyx_f_9fastphase_9fastphase_likprG(__pyx_t_16, __pyx_t_17, ((PyArrayObject *)__pyx_t_1))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_18 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_19 = PyTuple_New(3); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_1);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_18);
       PyTuple_SET_ITEM(__pyx_t_19, 2, __pyx_t_18);
       __pyx_t_1 = 0;
       __pyx_t_4 = 0;
       __pyx_t_18 = 0;
-      __pyx_t_18 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_mBeta), __pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-      __pyx_t_19 = PyNumber_Multiply(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_19 = PyNumber_Multiply(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-      __pyx_t_18 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_18);
-      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_k2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_18);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_18);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_6);
       __pyx_t_18 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = PyNumber_Multiply(__pyx_t_19, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_4 = PyNumber_Multiply(__pyx_t_19, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 955, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceAdd(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3, __pyx_t_6) < 0)) __PYX_ERR(0, 955, __pyx_L1_error)
+      if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_3, __pyx_t_6) < 0)) __PYX_ERR(0, 947, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
 
-    /* "fastphase/fastphase.pyx":956
+    /* "fastphase/fastphase.pyx":948
  *         for k2 in range(nK):
  *             tSumk[nLoc-1,k1] += likprG(theta[nLoc-1,k1],theta[nLoc-1,k2],lik[nLoc-1])*mBeta[nLoc-1,k1,k2]*alpha[nLoc-1,k2]
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]             # <<<<<<<<<<<<<<
  *     ## recurrent calculations backward
  *     for m in range(nLoc-1,0,-1):
  */
-    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_19 = PyTuple_New(2); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_19, 0, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_19, 1, __pyx_t_5);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_19); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tSumk), __pyx_t_19); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
-    __pyx_t_19 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_19);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_k1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_GIVEREF(__pyx_t_19);
     PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_t_19);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_4);
     __pyx_t_19 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_alpha), __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-    __pyx_t_18 = PyNumber_Multiply(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_18 = PyNumber_Multiply(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 956, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_InPlaceAdd(__pyx_t_6, __pyx_t_18); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3, __pyx_t_4) < 0)) __PYX_ERR(0, 956, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_3, __pyx_t_4) < 0)) __PYX_ERR(0, 948, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
 
-  /* "fastphase/fastphase.pyx":958
+  /* "fastphase/fastphase.pyx":950
  *         tDoubleSum[nLoc-1]+=tSumk[nLoc-1,k1]*alpha[nLoc-1,k1]
  *     ## recurrent calculations backward
  *     for m in range(nLoc-1,0,-1):             # <<<<<<<<<<<<<<
  *         ## these loops could be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  */
-  __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 958, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 958, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_3); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (__pyx_t_2 = __pyx_t_11; __pyx_t_2 > 0; __pyx_t_2-=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":960
+    /* "fastphase/fastphase.pyx":952
  *     for m in range(nLoc-1,0,-1):
  *         ## these loops could be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(k1,nK):
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  */
-    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 960, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 952, __pyx_L1_error)
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_13; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":961
+      /* "fastphase/fastphase.pyx":953
  *         ## these loops could be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  */
-      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 961, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 953, __pyx_L1_error)
       __pyx_t_20 = __pyx_t_14;
       for (__pyx_t_21 = __pyx_v_k1; __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":962
+        /* "fastphase/fastphase.pyx":954
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]
  */
         __pyx_t_22 = __pyx_v_m;
@@ -23227,15 +23083,15 @@
         if (__pyx_t_25 < 0) __pyx_t_25 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         __pyx_t_26 = __pyx_v_m;
         __pyx_t_27 = __pyx_v_k2;
         if (__pyx_t_26 < 0) __pyx_t_26 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_27 < 0) __pyx_t_27 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         __pyx_v_temp = ((0.5 * __pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_22, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_23, __pyx_pybuffernd_rho.diminfo[1].strides)))) * ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_24, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_25, __pyx_pybuffernd_tSumk.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":963
+        /* "fastphase/fastphase.pyx":955
  *             for k2 in range(k1,nK):
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]
  */
         __pyx_t_28 = __pyx_v_m;
@@ -23246,27 +23102,27 @@
         __pyx_t_31 = __pyx_v_k1;
         if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_31 < 0) __pyx_t_31 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_32 = __pyx_v_m;
         __pyx_t_33 = __pyx_v_k2;
         if (__pyx_t_32 < 0) __pyx_t_32 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_33 < 0) __pyx_t_33 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 963, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 955, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 963, __pyx_L1_error)
+        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 955, __pyx_L1_error)
         __pyx_t_34 = __pyx_v_m;
         __pyx_t_35 = __pyx_v_k1;
         __pyx_t_36 = __pyx_v_k2;
         if (__pyx_t_34 < 0) __pyx_t_34 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_35 < 0) __pyx_t_35 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_36 < 0) __pyx_t_36 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         __pyx_v_temp = (__pyx_v_temp + ((__pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_rho.diminfo[1].strides))) * __pyx_f_9fastphase_9fastphase_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_31, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_3))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_36, __pyx_pybuffernd_mBeta.diminfo[2].strides))));
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "fastphase/fastphase.pyx":964
+        /* "fastphase/fastphase.pyx":956
  *                 temp=0.5*probJ(m,1,rho[m,0])*(tSumk[m,k1]+tSumk[m,k2])
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]
  *         ## marginal sum and real sum for loc m-1
  */
         __pyx_t_37 = __pyx_v_m;
@@ -23279,15 +23135,15 @@
         __pyx_t_41 = __pyx_v_k1;
         __pyx_t_42 = __pyx_v_k2;
         if (__pyx_t_40 < 0) __pyx_t_40 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_41 < 0) __pyx_t_41 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_42 < 0) __pyx_t_42 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_40, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_41, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_42, __pyx_pybuffernd_mBeta.diminfo[2].strides) = (__pyx_v_temp + (__pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_37, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_38, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
 
-        /* "fastphase/fastphase.pyx":965
+        /* "fastphase/fastphase.pyx":957
  *                 temp+=probJ(m,0,rho[m,0])*likprG(theta[m,k1],theta[m,k2],lik[m])*mBeta[m,k1,k2]
  *                 mBeta[m-1,k1,k2]=temp+probJ(m,2,rho[m,0])*tDoubleSum[m]
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]             # <<<<<<<<<<<<<<
  *         ## marginal sum and real sum for loc m-1
  *         for k1 in range(nK):
  */
         __pyx_t_43 = (__pyx_v_m - 1);
@@ -23302,39 +23158,39 @@
         if (__pyx_t_46 < 0) __pyx_t_46 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_47 < 0) __pyx_t_47 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_48 < 0) __pyx_t_48 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_47, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_48, __pyx_pybuffernd_mBeta.diminfo[2].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_43, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_44, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_45, __pyx_pybuffernd_mBeta.diminfo[2].strides));
       }
     }
 
-    /* "fastphase/fastphase.pyx":967
+    /* "fastphase/fastphase.pyx":959
  *                 mBeta[m-1,k2,k1]=mBeta[m-1,k1,k2]
  *         ## marginal sum and real sum for loc m-1
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(nK):
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  */
-    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 967, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 959, __pyx_L1_error)
     __pyx_t_13 = __pyx_t_12;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_13; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":968
+      /* "fastphase/fastphase.pyx":960
  *         ## marginal sum and real sum for loc m-1
  *         for k1 in range(nK):
  *             for k2 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]
  */
-      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 968, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 960, __pyx_L1_error)
       __pyx_t_20 = __pyx_t_14;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":969
+        /* "fastphase/fastphase.pyx":961
  *         for k1 in range(nK):
  *             for k2 in range(nK):
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]             # <<<<<<<<<<<<<<
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]
  *         tScaleTemp=np.sum(mBeta[m-1])
  */
         __pyx_t_49 = (__pyx_v_m - 1);
@@ -23342,17 +23198,17 @@
         if (__pyx_t_49 < 0) __pyx_t_49 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_50 < 0) __pyx_t_50 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_51 = (__pyx_v_m - 1);
         __pyx_t_52 = __pyx_v_k2;
         if (__pyx_t_51 < 0) __pyx_t_51 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_52 < 0) __pyx_t_52 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_53 = (__pyx_v_m - 1);
-        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_53, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_53, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 961, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 969, __pyx_L1_error)
+        if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 961, __pyx_L1_error)
         __pyx_t_54 = (__pyx_v_m - 1);
         __pyx_t_55 = __pyx_v_k1;
         __pyx_t_56 = __pyx_v_k2;
         if (__pyx_t_54 < 0) __pyx_t_54 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_55 < 0) __pyx_t_55 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_56 < 0) __pyx_t_56 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         __pyx_t_57 = (__pyx_v_m - 1);
@@ -23363,15 +23219,15 @@
         __pyx_t_60 = __pyx_v_k1;
         if (__pyx_t_59 < 0) __pyx_t_59 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_60 < 0) __pyx_t_60 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_59, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_60, __pyx_pybuffernd_tSumk.diminfo[1].strides) += ((__pyx_f_9fastphase_9fastphase_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_49, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_50, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_51, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_52, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_3)) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_54, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_55, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_56, __pyx_pybuffernd_mBeta.diminfo[2].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_57, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_58, __pyx_pybuffernd_alpha.diminfo[1].strides)));
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
 
-      /* "fastphase/fastphase.pyx":970
+      /* "fastphase/fastphase.pyx":962
  *             for k2 in range(nK):
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]             # <<<<<<<<<<<<<<
  *         tScaleTemp=np.sum(mBeta[m-1])
  *         ## tScaleTemp=0 a gerer <---
  */
       __pyx_t_61 = (__pyx_v_m - 1);
@@ -23383,235 +23239,235 @@
       if (__pyx_t_63 < 0) __pyx_t_63 += __pyx_pybuffernd_alpha.diminfo[0].shape;
       if (__pyx_t_64 < 0) __pyx_t_64 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_65 = (__pyx_v_m - 1);
       if (__pyx_t_65 < 0) __pyx_t_65 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_65, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) += ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_61, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_62, __pyx_pybuffernd_tSumk.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_63, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_64, __pyx_pybuffernd_alpha.diminfo[1].strides)));
     }
 
-    /* "fastphase/fastphase.pyx":971
+    /* "fastphase/fastphase.pyx":963
  *                 tSumk[m-1,k1]+=likprG(theta[m-1,k1],theta[m-1,k2],lik[m-1])*mBeta[m-1,k1,k2]*alpha[m-1,k2]
  *             tDoubleSum[m-1]+=tSumk[m-1,k1]*alpha[m-1,k1]
  *         tScaleTemp=np.sum(mBeta[m-1])             # <<<<<<<<<<<<<<
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 971, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_sum); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 971, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_sum); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_12 = (__pyx_v_m - 1);
-    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_mBeta), __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 971, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_mBeta), __pyx_t_12, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_18))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_18);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_18);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_18, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_18, __pyx_t_6, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_18, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 971, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-    __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 971, __pyx_L1_error)
+    __pyx_t_17 = __pyx_PyFloat_AsDouble(__pyx_t_3); if (unlikely((__pyx_t_17 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 963, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_tScaleTemp = __pyx_t_17;
 
-    /* "fastphase/fastphase.pyx":973
+    /* "fastphase/fastphase.pyx":965
  *         tScaleTemp=np.sum(mBeta[m-1])
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:             # <<<<<<<<<<<<<<
  *             tScale=20
  *         else:
  */
     __pyx_t_66 = ((__pyx_v_tScaleTemp < 1e-20) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/fastphase.pyx":974
+      /* "fastphase/fastphase.pyx":966
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:
  *             tScale=20             # <<<<<<<<<<<<<<
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))
  */
       __pyx_v_tScale = 20;
 
-      /* "fastphase/fastphase.pyx":973
+      /* "fastphase/fastphase.pyx":965
  *         tScaleTemp=np.sum(mBeta[m-1])
  *         ## tScaleTemp=0 a gerer <---
  *         if tScaleTemp<1e-20:             # <<<<<<<<<<<<<<
  *             tScale=20
  *         else:
  */
       goto __pyx_L21;
     }
 
-    /* "fastphase/fastphase.pyx":976
+    /* "fastphase/fastphase.pyx":968
  *             tScale=20
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))             # <<<<<<<<<<<<<<
  *         if tScale <=0:
  *             tScale=0
  */
     /*else*/ {
       __pyx_t_17 = (-log(__pyx_v_tScaleTemp));
       __pyx_t_16 = log(10.0);
       if (unlikely(__pyx_t_16 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 976, __pyx_L1_error)
+        __PYX_ERR(0, 968, __pyx_L1_error)
       }
       __pyx_v_tScale = ((int)(__pyx_t_17 / __pyx_t_16));
     }
     __pyx_L21:;
 
-    /* "fastphase/fastphase.pyx":977
+    /* "fastphase/fastphase.pyx":969
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale <=0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     __pyx_t_66 = ((__pyx_v_tScale <= 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/fastphase.pyx":978
+      /* "fastphase/fastphase.pyx":970
  *             tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale <=0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/fastphase.pyx":977
+      /* "fastphase/fastphase.pyx":969
  *         else:
  *             tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale <=0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     }
 
-    /* "fastphase/fastphase.pyx":979
+    /* "fastphase/fastphase.pyx":971
  *         if tScale <=0:
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale             # <<<<<<<<<<<<<<
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_67 = __pyx_v_m;
     if (__pyx_t_67 < 0) __pyx_t_67 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     __pyx_t_68 = (__pyx_v_m - 1);
     if (__pyx_t_68 < 0) __pyx_t_68 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_68, __pyx_pybuffernd_betaScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_67, __pyx_pybuffernd_betaScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-    /* "fastphase/fastphase.pyx":980
+    /* "fastphase/fastphase.pyx":972
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy
  */
     __pyx_t_66 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/fastphase.pyx":981
+      /* "fastphase/fastphase.pyx":973
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             tDoubleSum[m-1]*=dummy
  *             for k1 in range(nK):
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/fastphase.pyx":982
+      /* "fastphase/fastphase.pyx":974
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 tSumk[m-1,k1]*=dummy
  */
       __pyx_t_69 = (__pyx_v_m - 1);
       if (__pyx_t_69 < 0) __pyx_t_69 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_69, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-      /* "fastphase/fastphase.pyx":983
+      /* "fastphase/fastphase.pyx":975
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[m-1,k1]*=dummy
  *                 mBeta[m-1,k1,k1]*=dummy
  */
-      __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 983, __pyx_L1_error)
+      __pyx_t_12 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_12 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 975, __pyx_L1_error)
       __pyx_t_13 = __pyx_t_12;
       for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_13; __pyx_t_15+=1) {
         __pyx_v_k1 = __pyx_t_15;
 
-        /* "fastphase/fastphase.pyx":984
+        /* "fastphase/fastphase.pyx":976
  *             tDoubleSum[m-1]*=dummy
  *             for k1 in range(nK):
  *                 tSumk[m-1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  */
         __pyx_t_70 = (__pyx_v_m - 1);
         __pyx_t_71 = __pyx_v_k1;
         if (__pyx_t_70 < 0) __pyx_t_70 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_71 < 0) __pyx_t_71 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_70, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_71, __pyx_pybuffernd_tSumk.diminfo[1].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/fastphase.pyx":985
+        /* "fastphase/fastphase.pyx":977
  *             for k1 in range(nK):
  *                 tSumk[m-1,k1]*=dummy
  *                 mBeta[m-1,k1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 for k2 in range(k1+1,nK):
  *                     mBeta[m-1,k1,k2]*=dummy
  */
         __pyx_t_72 = (__pyx_v_m - 1);
         __pyx_t_73 = __pyx_v_k1;
         __pyx_t_74 = __pyx_v_k1;
         if (__pyx_t_72 < 0) __pyx_t_72 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_73 < 0) __pyx_t_73 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         if (__pyx_t_74 < 0) __pyx_t_74 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_72, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_73, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_74, __pyx_pybuffernd_mBeta.diminfo[2].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/fastphase.pyx":986
+        /* "fastphase/fastphase.pyx":978
  *                 tSumk[m-1,k1]*=dummy
  *                 mBeta[m-1,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                     mBeta[m-1,k1,k2]*=dummy
  *                     mBeta[m-1,k2,k1]*=dummy
  */
-        __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 986, __pyx_L1_error)
+        __pyx_t_14 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_14 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 978, __pyx_L1_error)
         __pyx_t_20 = __pyx_t_14;
         for (__pyx_t_21 = (__pyx_v_k1 + 1); __pyx_t_21 < __pyx_t_20; __pyx_t_21+=1) {
           __pyx_v_k2 = __pyx_t_21;
 
-          /* "fastphase/fastphase.pyx":987
+          /* "fastphase/fastphase.pyx":979
  *                 mBeta[m-1,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  *                     mBeta[m-1,k1,k2]*=dummy             # <<<<<<<<<<<<<<
  *                     mBeta[m-1,k2,k1]*=dummy
  *     ##
  */
           __pyx_t_75 = (__pyx_v_m - 1);
           __pyx_t_76 = __pyx_v_k1;
           __pyx_t_77 = __pyx_v_k2;
           if (__pyx_t_75 < 0) __pyx_t_75 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
           if (__pyx_t_76 < 0) __pyx_t_76 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
           if (__pyx_t_77 < 0) __pyx_t_77 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_75, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_76, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_77, __pyx_pybuffernd_mBeta.diminfo[2].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/fastphase.pyx":988
+          /* "fastphase/fastphase.pyx":980
  *                 for k2 in range(k1+1,nK):
  *                     mBeta[m-1,k1,k2]*=dummy
  *                     mBeta[m-1,k2,k1]*=dummy             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute forward probabilities
  */
           __pyx_t_78 = (__pyx_v_m - 1);
@@ -23620,150 +23476,150 @@
           if (__pyx_t_78 < 0) __pyx_t_78 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
           if (__pyx_t_79 < 0) __pyx_t_79 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
           if (__pyx_t_80 < 0) __pyx_t_80 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_78, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_79, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_80, __pyx_pybuffernd_mBeta.diminfo[2].strides) *= __pyx_v_dummy;
         }
       }
 
-      /* "fastphase/fastphase.pyx":980
+      /* "fastphase/fastphase.pyx":972
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tDoubleSum[m-1]*=dummy
  */
     }
   }
 
-  /* "fastphase/fastphase.pyx":992
+  /* "fastphase/fastphase.pyx":984
  *     ## compute forward probabilities
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=3] mPhi=np.zeros((nLoc,nK,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     ## at locus 0
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_nK);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 992, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 992, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 992, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 984, __pyx_L1_error)
   __pyx_t_81 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mPhi.rcbuffer->pybuffer, (PyObject*)__pyx_t_81, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_mPhi = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 992, __pyx_L1_error)
+      __PYX_ERR(0, 984, __pyx_L1_error)
     } else {__pyx_pybuffernd_mPhi.diminfo[0].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mPhi.diminfo[0].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mPhi.diminfo[1].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mPhi.diminfo[1].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_mPhi.diminfo[2].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_mPhi.diminfo[2].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_81 = 0;
   __pyx_v_mPhi = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":993
+  /* "fastphase/fastphase.pyx":985
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=3] mPhi=np.zeros((nLoc,nK,nK),dtype=np.float64)
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     ## at locus 0
  *     for k1 in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_nLoc);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 993, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 985, __pyx_L1_error)
   __pyx_t_82 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_phiScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_82, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_phiScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 993, __pyx_L1_error)
+      __PYX_ERR(0, 985, __pyx_L1_error)
     } else {__pyx_pybuffernd_phiScale.diminfo[0].strides = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_phiScale.diminfo[0].shape = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_82 = 0;
   __pyx_v_phiScale = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/fastphase.pyx":995
+  /* "fastphase/fastphase.pyx":987
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     ## at locus 0
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(k1,nK):
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 995, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 987, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":996
+    /* "fastphase/fastphase.pyx":988
  *     ## at locus 0
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 996, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 988, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_k1; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":997
+      /* "fastphase/fastphase.pyx":989
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])             # <<<<<<<<<<<<<<
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]
  *     ## calc the marginal sum at locus 0 (appx A)
  */
       __pyx_t_83 = 0;
@@ -23778,27 +23634,27 @@
       __pyx_t_88 = __pyx_v_k1;
       if (__pyx_t_87 < 0) __pyx_t_87 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_88 < 0) __pyx_t_88 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_89 = 0;
       __pyx_t_90 = __pyx_v_k2;
       if (__pyx_t_89 < 0) __pyx_t_89 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_90 < 0) __pyx_t_90 += __pyx_pybuffernd_theta.diminfo[1].shape;
-      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 997, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 989, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 997, __pyx_L1_error)
+      if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 989, __pyx_L1_error)
       __pyx_t_91 = 0;
       __pyx_t_92 = __pyx_v_k1;
       __pyx_t_93 = __pyx_v_k2;
       if (__pyx_t_91 < 0) __pyx_t_91 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_92 < 0) __pyx_t_92 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       if (__pyx_t_93 < 0) __pyx_t_93 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
       *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_91, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_92, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_93, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_83, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_84, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_85, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_86, __pyx_pybuffernd_alpha.diminfo[1].strides))) * __pyx_f_9fastphase_9fastphase_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_87, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_88, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_89, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_90, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_6)));
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "fastphase/fastphase.pyx":998
+      /* "fastphase/fastphase.pyx":990
  *         for k2 in range(k1,nK):
  *             mPhi[0,k1,k2]=alpha[0,k1]*alpha[0,k2]*likprG(theta[0,k1],theta[0,k2],lik[0])
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]             # <<<<<<<<<<<<<<
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tDoubleSum[0]=0
  */
       __pyx_t_94 = 0;
@@ -23813,63 +23669,63 @@
       if (__pyx_t_97 < 0) __pyx_t_97 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_98 < 0) __pyx_t_98 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       if (__pyx_t_99 < 0) __pyx_t_99 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
       *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_97, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_98, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_99, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_94, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_95, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_96, __pyx_pybuffernd_mPhi.diminfo[2].strides));
     }
   }
 
-  /* "fastphase/fastphase.pyx":1000
+  /* "fastphase/fastphase.pyx":992
  *             mPhi[0,k2,k1]=mPhi[0,k1,k2]
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tDoubleSum[0]=0             # <<<<<<<<<<<<<<
  *     for k1 in range(nK):
  *         tSumk[0,k1]=0
  */
   __pyx_t_100 = 0;
   if (__pyx_t_100 < 0) __pyx_t_100 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_100, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) = 0.0;
 
-  /* "fastphase/fastphase.pyx":1001
+  /* "fastphase/fastphase.pyx":993
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tDoubleSum[0]=0
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         tSumk[0,k1]=0
  *         for k2 in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 993, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1002
+    /* "fastphase/fastphase.pyx":994
  *     tDoubleSum[0]=0
  *     for k1 in range(nK):
  *         tSumk[0,k1]=0             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  */
     __pyx_t_101 = 0;
     __pyx_t_102 = __pyx_v_k1;
     if (__pyx_t_101 < 0) __pyx_t_101 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
     if (__pyx_t_102 < 0) __pyx_t_102 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_101, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_102, __pyx_pybuffernd_tSumk.diminfo[1].strides) = 0.0;
 
-    /* "fastphase/fastphase.pyx":1003
+    /* "fastphase/fastphase.pyx":995
  *     for k1 in range(nK):
  *         tSumk[0,k1]=0
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  *         tDoubleSum[0]+=tSumk[0,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1003, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 995, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1004
+      /* "fastphase/fastphase.pyx":996
  *         tSumk[0,k1]=0
  *         for k2 in range(nK):
  *             tSumk[0,k1]+=mPhi[0,k1,k2]             # <<<<<<<<<<<<<<
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0
  */
       __pyx_t_103 = 0;
@@ -23881,15 +23737,15 @@
       __pyx_t_106 = 0;
       __pyx_t_107 = __pyx_v_k1;
       if (__pyx_t_106 < 0) __pyx_t_106 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
       if (__pyx_t_107 < 0) __pyx_t_107 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_106, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_107, __pyx_pybuffernd_tSumk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_103, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_104, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_105, __pyx_pybuffernd_mPhi.diminfo[2].strides));
     }
 
-    /* "fastphase/fastphase.pyx":1005
+    /* "fastphase/fastphase.pyx":997
  *         for k2 in range(nK):
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  *         tDoubleSum[0]+=tSumk[0,k1]             # <<<<<<<<<<<<<<
  *     tScale=0
  *     if tDoubleSum[0] != 0:
  */
     __pyx_t_108 = 0;
@@ -23897,178 +23753,178 @@
     if (__pyx_t_108 < 0) __pyx_t_108 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
     if (__pyx_t_109 < 0) __pyx_t_109 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
     __pyx_t_110 = 0;
     if (__pyx_t_110 < 0) __pyx_t_110 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_110, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_108, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_109, __pyx_pybuffernd_tSumk.diminfo[1].strides));
   }
 
-  /* "fastphase/fastphase.pyx":1006
+  /* "fastphase/fastphase.pyx":998
  *             tSumk[0,k1]+=mPhi[0,k1,k2]
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0             # <<<<<<<<<<<<<<
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  */
   __pyx_v_tScale = 0;
 
-  /* "fastphase/fastphase.pyx":1007
+  /* "fastphase/fastphase.pyx":999
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0
  *     if tDoubleSum[0] != 0:             # <<<<<<<<<<<<<<
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:
  */
   __pyx_t_111 = 0;
   if (__pyx_t_111 < 0) __pyx_t_111 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
   __pyx_t_66 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_111, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides)) != 0.0) != 0);
   if (__pyx_t_66) {
 
-    /* "fastphase/fastphase.pyx":1008
+    /* "fastphase/fastphase.pyx":1000
  *     tScale=0
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))             # <<<<<<<<<<<<<<
  *         if tScale <0:
  *             tScale=0
  */
     __pyx_t_112 = 0;
     if (__pyx_t_112 < 0) __pyx_t_112 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     __pyx_t_16 = (-log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_112, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
     __pyx_t_17 = log(10.0);
     if (unlikely(__pyx_t_17 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 1008, __pyx_L1_error)
+      __PYX_ERR(0, 1000, __pyx_L1_error)
     }
     __pyx_v_tScale = ((int)(__pyx_t_16 / __pyx_t_17));
 
-    /* "fastphase/fastphase.pyx":1009
+    /* "fastphase/fastphase.pyx":1001
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[0]=tScale
  */
     __pyx_t_66 = ((__pyx_v_tScale < 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/fastphase.pyx":1010
+      /* "fastphase/fastphase.pyx":1002
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         phiScale[0]=tScale
  *         if tScale>0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/fastphase.pyx":1009
+      /* "fastphase/fastphase.pyx":1001
  *     if tDoubleSum[0] != 0:
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[0]=tScale
  */
     }
 
-    /* "fastphase/fastphase.pyx":1011
+    /* "fastphase/fastphase.pyx":1003
  *         if tScale <0:
  *             tScale=0
  *         phiScale[0]=tScale             # <<<<<<<<<<<<<<
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_113 = 0;
     if (__pyx_t_113 < 0) __pyx_t_113 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_113, __pyx_pybuffernd_phiScale.diminfo[0].strides) = __pyx_v_tScale;
 
-    /* "fastphase/fastphase.pyx":1012
+    /* "fastphase/fastphase.pyx":1004
  *             tScale=0
  *         phiScale[0]=tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):
  */
     __pyx_t_66 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/fastphase.pyx":1013
+      /* "fastphase/fastphase.pyx":1005
  *         phiScale[0]=tScale
  *         if tScale>0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 tSumk[0,k1]*=dummy
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/fastphase.pyx":1014
+      /* "fastphase/fastphase.pyx":1006
  *         if tScale>0:
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[0,k1]*=dummy
  *                 mPhi[0,k1,k1]*=dummy
  */
-      __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1014, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1006, __pyx_L1_error)
       __pyx_t_12 = __pyx_t_11;
       for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
         __pyx_v_k1 = __pyx_t_2;
 
-        /* "fastphase/fastphase.pyx":1015
+        /* "fastphase/fastphase.pyx":1007
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):
  *                 tSumk[0,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 mPhi[0,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  */
         __pyx_t_114 = 0;
         __pyx_t_115 = __pyx_v_k1;
         if (__pyx_t_114 < 0) __pyx_t_114 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_115 < 0) __pyx_t_115 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_114, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_115, __pyx_pybuffernd_tSumk.diminfo[1].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/fastphase.pyx":1016
+        /* "fastphase/fastphase.pyx":1008
  *             for k1 in range(nK):
  *                 tSumk[0,k1]*=dummy
  *                 mPhi[0,k1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                 for k2 in range(k1+1,nK):
  *                     mPhi[0,k1,k2]*=dummy
  */
         __pyx_t_116 = 0;
         __pyx_t_117 = __pyx_v_k1;
         __pyx_t_118 = __pyx_v_k1;
         if (__pyx_t_116 < 0) __pyx_t_116 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_117 < 0) __pyx_t_117 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_118 < 0) __pyx_t_118 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_116, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_117, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_118, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/fastphase.pyx":1017
+        /* "fastphase/fastphase.pyx":1009
  *                 tSumk[0,k1]*=dummy
  *                 mPhi[0,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                     mPhi[0,k1,k2]*=dummy
  *                     mPhi[0,k2,k1]*=dummy
  */
-        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1017, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1009, __pyx_L1_error)
         __pyx_t_14 = __pyx_t_13;
         for (__pyx_t_15 = (__pyx_v_k1 + 1); __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
           __pyx_v_k2 = __pyx_t_15;
 
-          /* "fastphase/fastphase.pyx":1018
+          /* "fastphase/fastphase.pyx":1010
  *                 mPhi[0,k1,k1]*=dummy
  *                 for k2 in range(k1+1,nK):
  *                     mPhi[0,k1,k2]*=dummy             # <<<<<<<<<<<<<<
  *                     mPhi[0,k2,k1]*=dummy
  *     # do the reccurence
  */
           __pyx_t_119 = 0;
           __pyx_t_120 = __pyx_v_k1;
           __pyx_t_121 = __pyx_v_k2;
           if (__pyx_t_119 < 0) __pyx_t_119 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
           if (__pyx_t_120 < 0) __pyx_t_120 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
           if (__pyx_t_121 < 0) __pyx_t_121 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_119, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_120, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_121, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/fastphase.pyx":1019
+          /* "fastphase/fastphase.pyx":1011
  *                 for k2 in range(k1+1,nK):
  *                     mPhi[0,k1,k2]*=dummy
  *                     mPhi[0,k2,k1]*=dummy             # <<<<<<<<<<<<<<
  *     # do the reccurence
  *     for m in range(nLoc-1):
  */
           __pyx_t_122 = 0;
@@ -24077,72 +23933,72 @@
           if (__pyx_t_122 < 0) __pyx_t_122 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
           if (__pyx_t_123 < 0) __pyx_t_123 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
           if (__pyx_t_124 < 0) __pyx_t_124 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_122, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_123, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_124, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
         }
       }
 
-      /* "fastphase/fastphase.pyx":1012
+      /* "fastphase/fastphase.pyx":1004
  *             tScale=0
  *         phiScale[0]=tScale
  *         if tScale>0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             for k1 in range(nK):
  */
     }
 
-    /* "fastphase/fastphase.pyx":1007
+    /* "fastphase/fastphase.pyx":999
  *         tDoubleSum[0]+=tSumk[0,k1]
  *     tScale=0
  *     if tDoubleSum[0] != 0:             # <<<<<<<<<<<<<<
  *         tScale=int(-log(tDoubleSum[0])/log(10))
  *         if tScale <0:
  */
   }
 
-  /* "fastphase/fastphase.pyx":1021
+  /* "fastphase/fastphase.pyx":1013
  *                     mPhi[0,k2,k1]*=dummy
  *     # do the reccurence
  *     for m in range(nLoc-1):             # <<<<<<<<<<<<<<
  *         ## This loop can be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  */
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1021, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_6); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1021, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_6); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1013, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1023
+    /* "fastphase/fastphase.pyx":1015
  *     for m in range(nLoc-1):
  *         ## This loop can be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1023, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1015, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1024
+      /* "fastphase/fastphase.pyx":1016
  *         ## This loop can be parallelized across cluster pairs #CUDA
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1024, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1016, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = __pyx_v_k1; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1025
+        /* "fastphase/fastphase.pyx":1017
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]             # <<<<<<<<<<<<<<
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  */
         __pyx_t_125 = (__pyx_v_m + 1);
@@ -24159,28 +24015,28 @@
         if (__pyx_t_130 < 0) __pyx_t_130 += __pyx_pybuffernd_alpha.diminfo[1].shape;
         __pyx_t_131 = __pyx_v_m;
         __pyx_t_132 = __pyx_v_k1;
         if (__pyx_t_131 < 0) __pyx_t_131 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_132 < 0) __pyx_t_132 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_125, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_126, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_127, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_128, __pyx_pybuffernd_tSumk.diminfo[1].strides))) + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_129, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_130, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_131, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_132, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1026
+        /* "fastphase/fastphase.pyx":1018
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  */
         __pyx_t_133 = (__pyx_v_m + 1);
         __pyx_t_134 = 0;
         if (__pyx_t_133 < 0) __pyx_t_133 += __pyx_pybuffernd_rho.diminfo[0].shape;
         if (__pyx_t_134 < 0) __pyx_t_134 += __pyx_pybuffernd_rho.diminfo[1].shape;
         __pyx_v_temp = (__pyx_v_temp * (0.5 * __pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_133, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_134, __pyx_pybuffernd_rho.diminfo[1].strides)))));
 
-        /* "fastphase/fastphase.pyx":1027
+        /* "fastphase/fastphase.pyx":1019
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  */
         __pyx_t_135 = (__pyx_v_m + 1);
@@ -24191,15 +24047,15 @@
         __pyx_t_138 = __pyx_v_k1;
         __pyx_t_139 = __pyx_v_k2;
         if (__pyx_t_137 < 0) __pyx_t_137 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_138 < 0) __pyx_t_138 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_139 < 0) __pyx_t_139 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         __pyx_v_temp = (__pyx_v_temp + (__pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_135, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_136, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_137, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_138, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_139, __pyx_pybuffernd_mPhi.diminfo[2].strides))));
 
-        /* "fastphase/fastphase.pyx":1028
+        /* "fastphase/fastphase.pyx":1020
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]             # <<<<<<<<<<<<<<
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  */
         __pyx_t_140 = (__pyx_v_m + 1);
@@ -24214,15 +24070,15 @@
         __pyx_t_145 = __pyx_v_k2;
         if (__pyx_t_144 < 0) __pyx_t_144 += __pyx_pybuffernd_alpha.diminfo[0].shape;
         if (__pyx_t_145 < 0) __pyx_t_145 += __pyx_pybuffernd_alpha.diminfo[1].shape;
         __pyx_t_146 = __pyx_v_m;
         if (__pyx_t_146 < 0) __pyx_t_146 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
         __pyx_v_temp = (__pyx_v_temp + (((__pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_140, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_141, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_142, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_143, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_144, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_145, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_146, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
 
-        /* "fastphase/fastphase.pyx":1029
+        /* "fastphase/fastphase.pyx":1021
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])             # <<<<<<<<<<<<<<
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  *         tDoubleSum[m+1]=0
  */
         __pyx_t_147 = (__pyx_v_m + 1);
@@ -24230,27 +24086,27 @@
         if (__pyx_t_147 < 0) __pyx_t_147 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_148 < 0) __pyx_t_148 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_149 = (__pyx_v_m + 1);
         __pyx_t_150 = __pyx_v_k2;
         if (__pyx_t_149 < 0) __pyx_t_149 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_150 < 0) __pyx_t_150 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_151 = (__pyx_v_m + 1);
-        __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_151, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1029, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_t_151, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1021, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1029, __pyx_L1_error)
+        if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1021, __pyx_L1_error)
         __pyx_t_152 = (__pyx_v_m + 1);
         __pyx_t_153 = __pyx_v_k1;
         __pyx_t_154 = __pyx_v_k2;
         if (__pyx_t_152 < 0) __pyx_t_152 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_153 < 0) __pyx_t_153 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_154 < 0) __pyx_t_154 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_152, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_153, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_154, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_147, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_148, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_149, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_150, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_6)));
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-        /* "fastphase/fastphase.pyx":1030
+        /* "fastphase/fastphase.pyx":1022
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]             # <<<<<<<<<<<<<<
  *         tDoubleSum[m+1]=0
  *         for k1 in range(nK):
  */
         __pyx_t_155 = (__pyx_v_m + 1);
@@ -24265,63 +24121,63 @@
         if (__pyx_t_158 < 0) __pyx_t_158 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_159 < 0) __pyx_t_159 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         if (__pyx_t_160 < 0) __pyx_t_160 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
         *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_158, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_159, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_160, __pyx_pybuffernd_mPhi.diminfo[2].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_155, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_156, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_157, __pyx_pybuffernd_mPhi.diminfo[2].strides));
       }
     }
 
-    /* "fastphase/fastphase.pyx":1031
+    /* "fastphase/fastphase.pyx":1023
  *                 mPhi[m+1,k1,k2]=temp*likprG(theta[m+1,k1],theta[m+1,k2],lik[m+1])
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  *         tDoubleSum[m+1]=0             # <<<<<<<<<<<<<<
  *         for k1 in range(nK):
  *             tSumk[m+1,k1]=0
  */
     __pyx_t_161 = (__pyx_v_m + 1);
     if (__pyx_t_161 < 0) __pyx_t_161 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_161, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) = 0.0;
 
-    /* "fastphase/fastphase.pyx":1032
+    /* "fastphase/fastphase.pyx":1024
  *                 mPhi[m+1,k2,k1]=mPhi[m+1,k1,k2]
  *         tDoubleSum[m+1]=0
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             tSumk[m+1,k1]=0
  *             for k2 in range(nK):
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1032, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1024, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1033
+      /* "fastphase/fastphase.pyx":1025
  *         tDoubleSum[m+1]=0
  *         for k1 in range(nK):
  *             tSumk[m+1,k1]=0             # <<<<<<<<<<<<<<
  *             for k2 in range(nK):
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  */
       __pyx_t_162 = (__pyx_v_m + 1);
       __pyx_t_163 = __pyx_v_k1;
       if (__pyx_t_162 < 0) __pyx_t_162 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
       if (__pyx_t_163 < 0) __pyx_t_163 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_162, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_163, __pyx_pybuffernd_tSumk.diminfo[1].strides) = 0.0;
 
-      /* "fastphase/fastphase.pyx":1034
+      /* "fastphase/fastphase.pyx":1026
  *         for k1 in range(nK):
  *             tSumk[m+1,k1]=0
  *             for k2 in range(nK):             # <<<<<<<<<<<<<<
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1034, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1026, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1035
+        /* "fastphase/fastphase.pyx":1027
  *             tSumk[m+1,k1]=0
  *             for k2 in range(nK):
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]             # <<<<<<<<<<<<<<
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0
  */
         __pyx_t_164 = (__pyx_v_m + 1);
@@ -24333,15 +24189,15 @@
         __pyx_t_167 = (__pyx_v_m + 1);
         __pyx_t_168 = __pyx_v_k1;
         if (__pyx_t_167 < 0) __pyx_t_167 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
         if (__pyx_t_168 < 0) __pyx_t_168 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_167, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_168, __pyx_pybuffernd_tSumk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_164, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_165, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_166, __pyx_pybuffernd_mPhi.diminfo[2].strides));
       }
 
-      /* "fastphase/fastphase.pyx":1036
+      /* "fastphase/fastphase.pyx":1028
  *             for k2 in range(nK):
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]             # <<<<<<<<<<<<<<
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:
  */
       __pyx_t_169 = (__pyx_v_m + 1);
@@ -24349,215 +24205,215 @@
       if (__pyx_t_169 < 0) __pyx_t_169 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
       if (__pyx_t_170 < 0) __pyx_t_170 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
       __pyx_t_171 = (__pyx_v_m + 1);
       if (__pyx_t_171 < 0) __pyx_t_171 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_171, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_169, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_170, __pyx_pybuffernd_tSumk.diminfo[1].strides));
     }
 
-    /* "fastphase/fastphase.pyx":1037
+    /* "fastphase/fastphase.pyx":1029
  *                 tSumk[m+1,k1]+=mPhi[m+1,k1,k2]
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0             # <<<<<<<<<<<<<<
  *         if tDoubleSum[m+1]<=0:
  *             phiScale[m+1]=phiScale[m]
  */
     __pyx_v_tScale = 0;
 
-    /* "fastphase/fastphase.pyx":1038
+    /* "fastphase/fastphase.pyx":1030
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
     __pyx_t_172 = (__pyx_v_m + 1);
     if (__pyx_t_172 < 0) __pyx_t_172 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
     __pyx_t_66 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_172, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides)) <= 0.0) != 0);
     if (__pyx_t_66) {
 
-      /* "fastphase/fastphase.pyx":1039
+      /* "fastphase/fastphase.pyx":1031
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:
  *             phiScale[m+1]=phiScale[m]             # <<<<<<<<<<<<<<
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  */
       __pyx_t_173 = __pyx_v_m;
       if (__pyx_t_173 < 0) __pyx_t_173 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       __pyx_t_174 = (__pyx_v_m + 1);
       if (__pyx_t_174 < 0) __pyx_t_174 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_174, __pyx_pybuffernd_phiScale.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_173, __pyx_pybuffernd_phiScale.diminfo[0].strides));
 
-      /* "fastphase/fastphase.pyx":1038
+      /* "fastphase/fastphase.pyx":1030
  *             tDoubleSum[m+1]+=tSumk[m+1,k1]
  *         tScale=0
  *         if tDoubleSum[m+1]<=0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
       goto __pyx_L53;
     }
 
-    /* "fastphase/fastphase.pyx":1041
+    /* "fastphase/fastphase.pyx":1033
  *             phiScale[m+1]=phiScale[m]
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))             # <<<<<<<<<<<<<<
  *             if tScale<0:
  *                 tScale=0
  */
     /*else*/ {
       __pyx_t_175 = (__pyx_v_m + 1);
       if (__pyx_t_175 < 0) __pyx_t_175 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
       __pyx_t_17 = (-log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_175, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
       __pyx_t_16 = log(10.0);
       if (unlikely(__pyx_t_16 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 1041, __pyx_L1_error)
+        __PYX_ERR(0, 1033, __pyx_L1_error)
       }
       __pyx_v_tScale = ((int)(__pyx_t_17 / __pyx_t_16));
 
-      /* "fastphase/fastphase.pyx":1042
+      /* "fastphase/fastphase.pyx":1034
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  *             if tScale<0:             # <<<<<<<<<<<<<<
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  */
       __pyx_t_66 = ((__pyx_v_tScale < 0) != 0);
       if (__pyx_t_66) {
 
-        /* "fastphase/fastphase.pyx":1043
+        /* "fastphase/fastphase.pyx":1035
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  *             if tScale<0:
  *                 tScale=0             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:
  */
         __pyx_v_tScale = 0;
 
-        /* "fastphase/fastphase.pyx":1042
+        /* "fastphase/fastphase.pyx":1034
  *         else:
  *             tScale=int(-log(tDoubleSum[m+1])/log(10))
  *             if tScale<0:             # <<<<<<<<<<<<<<
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  */
       }
 
-      /* "fastphase/fastphase.pyx":1044
+      /* "fastphase/fastphase.pyx":1036
  *             if tScale<0:
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale             # <<<<<<<<<<<<<<
  *             if tScale>0:
  *                 dummy=myPow10(tScale)
  */
       __pyx_t_176 = __pyx_v_m;
       if (__pyx_t_176 < 0) __pyx_t_176 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       __pyx_t_177 = (__pyx_v_m + 1);
       if (__pyx_t_177 < 0) __pyx_t_177 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_177, __pyx_pybuffernd_phiScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_176, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-      /* "fastphase/fastphase.pyx":1045
+      /* "fastphase/fastphase.pyx":1037
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:             # <<<<<<<<<<<<<<
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy
  */
       __pyx_t_66 = ((__pyx_v_tScale > 0) != 0);
       if (__pyx_t_66) {
 
-        /* "fastphase/fastphase.pyx":1046
+        /* "fastphase/fastphase.pyx":1038
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:
  *                 dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *                 tDoubleSum[m+1]*=dummy
  *                 for k1 in range(nK):
  */
         __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10(__pyx_v_tScale);
 
-        /* "fastphase/fastphase.pyx":1047
+        /* "fastphase/fastphase.pyx":1039
  *             if tScale>0:
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy             # <<<<<<<<<<<<<<
  *                 for k1 in range(nK):
  *                     tSumk[m+1,k1]*=dummy
  */
         __pyx_t_178 = (__pyx_v_m + 1);
         if (__pyx_t_178 < 0) __pyx_t_178 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
         *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_178, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-        /* "fastphase/fastphase.pyx":1048
+        /* "fastphase/fastphase.pyx":1040
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy
  *                 for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                     tSumk[m+1,k1]*=dummy
  *                     mPhi[m+1,k1,k1]*=dummy
  */
-        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1048, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1040, __pyx_L1_error)
         __pyx_t_14 = __pyx_t_13;
         for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
           __pyx_v_k1 = __pyx_t_15;
 
-          /* "fastphase/fastphase.pyx":1049
+          /* "fastphase/fastphase.pyx":1041
  *                 tDoubleSum[m+1]*=dummy
  *                 for k1 in range(nK):
  *                     tSumk[m+1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                     mPhi[m+1,k1,k1]*=dummy
  *                     for k2 in range(k1+1,nK):
  */
           __pyx_t_179 = (__pyx_v_m + 1);
           __pyx_t_180 = __pyx_v_k1;
           if (__pyx_t_179 < 0) __pyx_t_179 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
           if (__pyx_t_180 < 0) __pyx_t_180 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_179, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_180, __pyx_pybuffernd_tSumk.diminfo[1].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/fastphase.pyx":1050
+          /* "fastphase/fastphase.pyx":1042
  *                 for k1 in range(nK):
  *                     tSumk[m+1,k1]*=dummy
  *                     mPhi[m+1,k1,k1]*=dummy             # <<<<<<<<<<<<<<
  *                     for k2 in range(k1+1,nK):
  *                         mPhi[m+1,k1,k2]*=dummy
  */
           __pyx_t_181 = (__pyx_v_m + 1);
           __pyx_t_182 = __pyx_v_k1;
           __pyx_t_183 = __pyx_v_k1;
           if (__pyx_t_181 < 0) __pyx_t_181 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
           if (__pyx_t_182 < 0) __pyx_t_182 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
           if (__pyx_t_183 < 0) __pyx_t_183 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
           *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_181, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_182, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_183, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-          /* "fastphase/fastphase.pyx":1051
+          /* "fastphase/fastphase.pyx":1043
  *                     tSumk[m+1,k1]*=dummy
  *                     mPhi[m+1,k1,k1]*=dummy
  *                     for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                         mPhi[m+1,k1,k2]*=dummy
  *                         mPhi[m+1,k2,k1]*=dummy
  */
-          __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1051, __pyx_L1_error)
+          __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1043, __pyx_L1_error)
           __pyx_t_53 = __pyx_t_20;
           for (__pyx_t_21 = (__pyx_v_k1 + 1); __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
             __pyx_v_k2 = __pyx_t_21;
 
-            /* "fastphase/fastphase.pyx":1052
+            /* "fastphase/fastphase.pyx":1044
  *                     mPhi[m+1,k1,k1]*=dummy
  *                     for k2 in range(k1+1,nK):
  *                         mPhi[m+1,k1,k2]*=dummy             # <<<<<<<<<<<<<<
  *                         mPhi[m+1,k2,k1]*=dummy
  *     ## end mPhi
  */
             __pyx_t_184 = (__pyx_v_m + 1);
             __pyx_t_185 = __pyx_v_k1;
             __pyx_t_186 = __pyx_v_k2;
             if (__pyx_t_184 < 0) __pyx_t_184 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
             if (__pyx_t_185 < 0) __pyx_t_185 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
             if (__pyx_t_186 < 0) __pyx_t_186 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
             *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_184, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_185, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_186, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
 
-            /* "fastphase/fastphase.pyx":1053
+            /* "fastphase/fastphase.pyx":1045
  *                     for k2 in range(k1+1,nK):
  *                         mPhi[m+1,k1,k2]*=dummy
  *                         mPhi[m+1,k2,k1]*=dummy             # <<<<<<<<<<<<<<
  *     ## end mPhi
  *     logLikelihood=log(tDoubleSum[nLoc-1])/log(10)-phiScale[nLoc-1]
  */
             __pyx_t_187 = (__pyx_v_m + 1);
@@ -24566,357 +24422,357 @@
             if (__pyx_t_187 < 0) __pyx_t_187 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
             if (__pyx_t_188 < 0) __pyx_t_188 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
             if (__pyx_t_189 < 0) __pyx_t_189 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
             *__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_187, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_188, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_189, __pyx_pybuffernd_mPhi.diminfo[2].strides) *= __pyx_v_dummy;
           }
         }
 
-        /* "fastphase/fastphase.pyx":1045
+        /* "fastphase/fastphase.pyx":1037
  *                 tScale=0
  *             phiScale[m+1]=phiScale[m]+tScale
  *             if tScale>0:             # <<<<<<<<<<<<<<
  *                 dummy=myPow10(tScale)
  *                 tDoubleSum[m+1]*=dummy
  */
       }
     }
     __pyx_L53:;
   }
 
-  /* "fastphase/fastphase.pyx":1055
+  /* "fastphase/fastphase.pyx":1047
  *                         mPhi[m+1,k2,k1]*=dummy
  *     ## end mPhi
  *     logLikelihood=log(tDoubleSum[nLoc-1])/log(10)-phiScale[nLoc-1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute Individual Contribution top,bottom,jmk
  */
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_17 = log(__pyx_t_16);
   __pyx_t_16 = log(10.0);
   if (unlikely(__pyx_t_16 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 1055, __pyx_L1_error)
+    __PYX_ERR(0, 1047, __pyx_L1_error)
   }
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_t_17 / __pyx_t_16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_t_17 / __pyx_t_16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Subtract(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1055, __pyx_L1_error)
+  __pyx_t_16 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_16 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1047, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_logLikelihood = __pyx_t_16;
 
-  /* "fastphase/fastphase.pyx":1060
+  /* "fastphase/fastphase.pyx":1052
  *     ##
  *     # calc ProbZ
  *     cdef np.ndarray[np.float64_t,ndim=3] probZ=mPhi*mBeta             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __pyx_t_6 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1060, __pyx_L1_error)
+  __pyx_t_6 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1052, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1060, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1052, __pyx_L1_error)
   __pyx_t_190 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_probZ.rcbuffer->pybuffer, (PyObject*)__pyx_t_190, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 3, 0, __pyx_stack) == -1)) {
       __pyx_v_probZ = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1060, __pyx_L1_error)
+      __PYX_ERR(0, 1052, __pyx_L1_error)
     } else {__pyx_pybuffernd_probZ.diminfo[0].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_probZ.diminfo[0].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_probZ.diminfo[1].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_probZ.diminfo[1].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[1]; __pyx_pybuffernd_probZ.diminfo[2].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[2]; __pyx_pybuffernd_probZ.diminfo[2].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[2];
     }
   }
   __pyx_t_190 = 0;
   __pyx_v_probZ = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/fastphase.pyx":1061
+  /* "fastphase/fastphase.pyx":1053
  *     # calc ProbZ
  *     cdef np.ndarray[np.float64_t,ndim=3] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_int_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_18) < 0) __PYX_ERR(0, 1061, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_18) < 0) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1061, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_18) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_18, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1061, __pyx_L1_error)
+  if (!(likely(((__pyx_t_18) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_18, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1053, __pyx_L1_error)
   __pyx_t_191 = ((PyArrayObject *)__pyx_t_18);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer, (PyObject*)__pyx_t_191, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_p_g_givX = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1061, __pyx_L1_error)
+      __PYX_ERR(0, 1053, __pyx_L1_error)
     } else {__pyx_pybuffernd_p_g_givX.diminfo[0].strides = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_p_g_givX.diminfo[0].shape = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_p_g_givX.diminfo[1].strides = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_p_g_givX.diminfo[1].shape = __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_191 = 0;
   __pyx_v_p_g_givX = ((PyArrayObject *)__pyx_t_18);
   __pyx_t_18 = 0;
 
-  /* "fastphase/fastphase.pyx":1062
+  /* "fastphase/fastphase.pyx":1054
  *     cdef np.ndarray[np.float64_t,ndim=3] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_18);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_18);
   __pyx_t_18 = 0;
-  __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_18, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1062, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_18, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_18); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1062, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_18); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1062, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1054, __pyx_L1_error)
   __pyx_t_192 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_jmk.rcbuffer->pybuffer, (PyObject*)__pyx_t_192, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_jmk = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1062, __pyx_L1_error)
+      __PYX_ERR(0, 1054, __pyx_L1_error)
     } else {__pyx_pybuffernd_jmk.diminfo[0].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_jmk.diminfo[0].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_jmk.diminfo[1].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_jmk.diminfo[1].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_192 = 0;
   __pyx_v_jmk = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/fastphase.pyx":1063
+  /* "fastphase/fastphase.pyx":1055
  *     cdef np.ndarray[np.float64_t,ndim=2] p_g_givX=np.zeros((nLoc,3),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  *     ## normalize
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1063, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1063, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_18, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1055, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1063, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1055, __pyx_L1_error)
   __pyx_t_193 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_top.rcbuffer->pybuffer, (PyObject*)__pyx_t_193, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_top = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_top.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1063, __pyx_L1_error)
+      __PYX_ERR(0, 1055, __pyx_L1_error)
     } else {__pyx_pybuffernd_top.diminfo[0].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_top.diminfo[0].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_top.diminfo[1].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_top.diminfo[1].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_193 = 0;
   __pyx_v_top = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":1064
+  /* "fastphase/fastphase.pyx":1056
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     ## normalize
  *     for m in range(nLoc):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_nLoc);
   __Pyx_GIVEREF(__pyx_v_nLoc);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_nLoc);
   __Pyx_INCREF(__pyx_v_nK);
   __Pyx_GIVEREF(__pyx_v_nK);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_v_nK);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_np); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_18, __pyx_n_s_float64); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 1064, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1064, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1056, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1064, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1056, __pyx_L1_error)
   __pyx_t_194 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bot.rcbuffer->pybuffer, (PyObject*)__pyx_t_194, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_bot = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1064, __pyx_L1_error)
+      __PYX_ERR(0, 1056, __pyx_L1_error)
     } else {__pyx_pybuffernd_bot.diminfo[0].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bot.diminfo[0].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_bot.diminfo[1].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_bot.diminfo[1].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_194 = 0;
   __pyx_v_bot = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/fastphase.pyx":1066
+  /* "fastphase/fastphase.pyx":1058
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  *     ## normalize
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         normC=0
  *         for k1 in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1066, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1058, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1067
+    /* "fastphase/fastphase.pyx":1059
  *     ## normalize
  *     for m in range(nLoc):
  *         normC=0             # <<<<<<<<<<<<<<
  *         for k1 in range(nK):
  *             normC+=probZ[m,k1,k1]
  */
     __pyx_v_normC = 0.0;
 
-    /* "fastphase/fastphase.pyx":1068
+    /* "fastphase/fastphase.pyx":1060
  *     for m in range(nLoc):
  *         normC=0
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             normC+=probZ[m,k1,k1]
  *             for k2 in range(k1+1,nK):
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1068, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1060, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1069
+      /* "fastphase/fastphase.pyx":1061
  *         normC=0
  *         for k1 in range(nK):
  *             normC+=probZ[m,k1,k1]             # <<<<<<<<<<<<<<
  *             for k2 in range(k1+1,nK):
  *                 normC+=2*probZ[m,k1,k2]
  */
       __pyx_t_195 = __pyx_v_m;
       __pyx_t_196 = __pyx_v_k1;
       __pyx_t_197 = __pyx_v_k1;
       if (__pyx_t_195 < 0) __pyx_t_195 += __pyx_pybuffernd_probZ.diminfo[0].shape;
       if (__pyx_t_196 < 0) __pyx_t_196 += __pyx_pybuffernd_probZ.diminfo[1].shape;
       if (__pyx_t_197 < 0) __pyx_t_197 += __pyx_pybuffernd_probZ.diminfo[2].shape;
       __pyx_v_normC = (__pyx_v_normC + (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_195, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_196, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_197, __pyx_pybuffernd_probZ.diminfo[2].strides)));
 
-      /* "fastphase/fastphase.pyx":1070
+      /* "fastphase/fastphase.pyx":1062
  *         for k1 in range(nK):
  *             normC+=probZ[m,k1,k1]
  *             for k2 in range(k1+1,nK):             # <<<<<<<<<<<<<<
  *                 normC+=2*probZ[m,k1,k2]
  *         probZ[m]/=normC
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1070, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1062, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = (__pyx_v_k1 + 1); __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1071
+        /* "fastphase/fastphase.pyx":1063
  *             normC+=probZ[m,k1,k1]
  *             for k2 in range(k1+1,nK):
  *                 normC+=2*probZ[m,k1,k2]             # <<<<<<<<<<<<<<
  *         probZ[m]/=normC
  *     ## Calc P( G| X, pars)
  */
         __pyx_t_198 = __pyx_v_m;
@@ -24925,59 +24781,59 @@
         if (__pyx_t_198 < 0) __pyx_t_198 += __pyx_pybuffernd_probZ.diminfo[0].shape;
         if (__pyx_t_199 < 0) __pyx_t_199 += __pyx_pybuffernd_probZ.diminfo[1].shape;
         if (__pyx_t_200 < 0) __pyx_t_200 += __pyx_pybuffernd_probZ.diminfo[2].shape;
         __pyx_v_normC = (__pyx_v_normC + (2.0 * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_198, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_199, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_200, __pyx_pybuffernd_probZ.diminfo[2].strides))));
       }
     }
 
-    /* "fastphase/fastphase.pyx":1072
+    /* "fastphase/fastphase.pyx":1064
  *             for k2 in range(k1+1,nK):
  *                 normC+=2*probZ[m,k1,k2]
  *         probZ[m]/=normC             # <<<<<<<<<<<<<<
  *     ## Calc P( G| X, pars)
  *     ## Scheet Stephens, 2008, appendix page 5 P(xim|gi)
  */
     __pyx_t_15 = __pyx_v_m;
-    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1072, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1064, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1072, __pyx_L1_error)
+    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1064, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1072, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1064, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, __pyx_t_4, int, 1, __Pyx_PyInt_From_int, 0, 1, 0) < 0)) __PYX_ERR(0, 1072, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_probZ), __pyx_t_15, __pyx_t_4, int, 1, __Pyx_PyInt_From_int, 0, 1, 0) < 0)) __PYX_ERR(0, 1064, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
 
-  /* "fastphase/fastphase.pyx":1076
+  /* "fastphase/fastphase.pyx":1068
  *     ## Scheet Stephens, 2008, appendix page 5 P(xim|gi)
  *     ## init at 0
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         for k2 in range(k1,nK):
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1076, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1068, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1077
+    /* "fastphase/fastphase.pyx":1069
  *     ## init at 0
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1077, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1069, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = __pyx_v_k1; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1078
+      /* "fastphase/fastphase.pyx":1070
  *     for k1 in range(nK):
  *         for k2 in range(k1,nK):
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]             # <<<<<<<<<<<<<<
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  */
       __pyx_t_201 = 0;
@@ -24992,15 +24848,15 @@
       __pyx_t_206 = __pyx_v_k1;
       __pyx_t_207 = __pyx_v_k2;
       if (__pyx_t_205 < 0) __pyx_t_205 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_206 < 0) __pyx_t_206 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       if (__pyx_t_207 < 0) __pyx_t_207 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
       __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_201, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_202, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_203, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_204, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_205, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_206, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_207, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
 
-      /* "fastphase/fastphase.pyx":1079
+      /* "fastphase/fastphase.pyx":1071
  *         for k2 in range(k1,nK):
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)             # <<<<<<<<<<<<<<
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
  */
       __pyx_t_208 = 0;
@@ -25013,20 +24869,20 @@
       if (__pyx_t_211 < 0) __pyx_t_211 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_212 = 0;
       __pyx_t_213 = 0;
       if (__pyx_t_212 < 0) __pyx_t_212 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
       if (__pyx_t_213 < 0) __pyx_t_213 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_212, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_213, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_208, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_209, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_210, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_211, __pyx_pybuffernd_theta.diminfo[1].strides)), 0));
 
-      /* "fastphase/fastphase.pyx":1080
+      /* "fastphase/fastphase.pyx":1072
  *             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)             # <<<<<<<<<<<<<<
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
+ *     p_g_givX[0,0] *= lik[0,0]
  */
       __pyx_t_214 = 0;
       __pyx_t_215 = __pyx_v_k1;
       if (__pyx_t_214 < 0) __pyx_t_214 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_215 < 0) __pyx_t_215 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_216 = 0;
       __pyx_t_217 = __pyx_v_k2;
@@ -25034,20 +24890,20 @@
       if (__pyx_t_217 < 0) __pyx_t_217 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_218 = 0;
       __pyx_t_219 = 1;
       if (__pyx_t_218 < 0) __pyx_t_218 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
       if (__pyx_t_219 < 0) __pyx_t_219 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_218, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_219, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_214, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_215, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_216, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_217, __pyx_pybuffernd_theta.diminfo[1].strides)), 1));
 
-      /* "fastphase/fastphase.pyx":1081
+      /* "fastphase/fastphase.pyx":1073
  *             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0)
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)             # <<<<<<<<<<<<<<
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
+ *     p_g_givX[0,0] *= lik[0,0]
+ *     p_g_givX[0,1] *= lik[0,1]
  */
       __pyx_t_220 = 0;
       __pyx_t_221 = __pyx_v_k1;
       if (__pyx_t_220 < 0) __pyx_t_220 += __pyx_pybuffernd_theta.diminfo[0].shape;
       if (__pyx_t_221 < 0) __pyx_t_221 += __pyx_pybuffernd_theta.diminfo[1].shape;
       __pyx_t_222 = 0;
       __pyx_t_223 = __pyx_v_k2;
@@ -25057,856 +24913,706 @@
       __pyx_t_225 = 2;
       if (__pyx_t_224 < 0) __pyx_t_224 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
       if (__pyx_t_225 < 0) __pyx_t_225 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_224, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_225, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_220, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_221, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_222, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_223, __pyx_pybuffernd_theta.diminfo[1].strides)), 2));
     }
   }
 
-  /* "fastphase/fastphase.pyx":1082
+  /* "fastphase/fastphase.pyx":1074
  *             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1)
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
- *     p_g_givX[0,0] *= np.exp(lik[0,0])             # <<<<<<<<<<<<<<
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+ *     p_g_givX[0,0] *= lik[0,0]             # <<<<<<<<<<<<<<
+ *     p_g_givX[0,1] *= lik[0,1]
+ *     p_g_givX[0,2] *= lik[0,2]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1082, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1082, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_226 = 0;
   __pyx_t_227 = 0;
   if (__pyx_t_226 < 0) __pyx_t_226 += __pyx_pybuffernd_lik.diminfo[0].shape;
   if (__pyx_t_227 < 0) __pyx_t_227 += __pyx_pybuffernd_lik.diminfo[1].shape;
-  __pyx_t_5 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_226, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_227, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1082, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1082, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1082, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_228 = 0;
   __pyx_t_229 = 0;
-  __pyx_t_230 = 0;
-  if (__pyx_t_229 < 0) __pyx_t_229 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_230 < 0) __pyx_t_230 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_229, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_230, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
+  if (__pyx_t_228 < 0) __pyx_t_228 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_229 < 0) __pyx_t_229 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_228, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_229, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_226, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_227, __pyx_pybuffernd_lik.diminfo[1].strides));
 
-  /* "fastphase/fastphase.pyx":1083
+  /* "fastphase/fastphase.pyx":1075
  *             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
- *     p_g_givX[0,1] *= np.exp(lik[0,1])             # <<<<<<<<<<<<<<
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+ *     p_g_givX[0,0] *= lik[0,0]
+ *     p_g_givX[0,1] *= lik[0,1]             # <<<<<<<<<<<<<<
+ *     p_g_givX[0,2] *= lik[0,2]
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1083, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_exp); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1083, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_231 = 0;
-  __pyx_t_232 = 1;
-  if (__pyx_t_231 < 0) __pyx_t_231 += __pyx_pybuffernd_lik.diminfo[0].shape;
-  if (__pyx_t_232 < 0) __pyx_t_232 += __pyx_pybuffernd_lik.diminfo[1].shape;
-  __pyx_t_6 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_231, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_232, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1083, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_5, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1083, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1083, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_233 = 0;
-  __pyx_t_234 = 1;
-  if (__pyx_t_233 < 0) __pyx_t_233 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_234 < 0) __pyx_t_234 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_233, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_234, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-  /* "fastphase/fastphase.pyx":1084
- *     p_g_givX[0,0] *= np.exp(lik[0,0])
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
- *     p_g_givX[0,2] *= np.exp(lik[0,2])             # <<<<<<<<<<<<<<
+  __pyx_t_230 = 0;
+  __pyx_t_231 = 1;
+  if (__pyx_t_230 < 0) __pyx_t_230 += __pyx_pybuffernd_lik.diminfo[0].shape;
+  if (__pyx_t_231 < 0) __pyx_t_231 += __pyx_pybuffernd_lik.diminfo[1].shape;
+  __pyx_t_232 = 0;
+  __pyx_t_233 = 1;
+  if (__pyx_t_232 < 0) __pyx_t_232 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_233 < 0) __pyx_t_233 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_232, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_233, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_230, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_231, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+  /* "fastphase/fastphase.pyx":1076
+ *     p_g_givX[0,0] *= lik[0,0]
+ *     p_g_givX[0,1] *= lik[0,1]
+ *     p_g_givX[0,2] *= lik[0,2]             # <<<<<<<<<<<<<<
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
  *     p_g_givX[0]/=normC
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1084, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1084, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_235 = 0;
-  __pyx_t_236 = 2;
-  if (__pyx_t_235 < 0) __pyx_t_235 += __pyx_pybuffernd_lik.diminfo[0].shape;
-  if (__pyx_t_236 < 0) __pyx_t_236 += __pyx_pybuffernd_lik.diminfo[1].shape;
-  __pyx_t_5 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_235, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_236, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1084, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_6, function);
-    }
-  }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1084, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_4); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1084, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_237 = 0;
-  __pyx_t_238 = 2;
-  if (__pyx_t_237 < 0) __pyx_t_237 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_238 < 0) __pyx_t_238 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_237, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_238, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-  /* "fastphase/fastphase.pyx":1085
- *     p_g_givX[0,1] *= np.exp(lik[0,1])
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+  __pyx_t_234 = 0;
+  __pyx_t_235 = 2;
+  if (__pyx_t_234 < 0) __pyx_t_234 += __pyx_pybuffernd_lik.diminfo[0].shape;
+  if (__pyx_t_235 < 0) __pyx_t_235 += __pyx_pybuffernd_lik.diminfo[1].shape;
+  __pyx_t_236 = 0;
+  __pyx_t_237 = 2;
+  if (__pyx_t_236 < 0) __pyx_t_236 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_237 < 0) __pyx_t_237 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_236, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_237, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_234, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_235, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+  /* "fastphase/fastphase.pyx":1077
+ *     p_g_givX[0,1] *= lik[0,1]
+ *     p_g_givX[0,2] *= lik[0,2]
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]             # <<<<<<<<<<<<<<
  *     p_g_givX[0]/=normC
  * 
  */
+  __pyx_t_238 = 0;
   __pyx_t_239 = 0;
+  if (__pyx_t_238 < 0) __pyx_t_238 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_239 < 0) __pyx_t_239 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
   __pyx_t_240 = 0;
-  if (__pyx_t_239 < 0) __pyx_t_239 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_240 < 0) __pyx_t_240 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  __pyx_t_241 = 0;
-  __pyx_t_242 = 1;
-  if (__pyx_t_241 < 0) __pyx_t_241 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_242 < 0) __pyx_t_242 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  __pyx_t_243 = 0;
-  __pyx_t_244 = 2;
-  if (__pyx_t_243 < 0) __pyx_t_243 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-  if (__pyx_t_244 < 0) __pyx_t_244 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-  __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_239, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_240, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_241, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_242, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_243, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_244, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
+  __pyx_t_241 = 1;
+  if (__pyx_t_240 < 0) __pyx_t_240 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_241 < 0) __pyx_t_241 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  __pyx_t_242 = 0;
+  __pyx_t_243 = 2;
+  if (__pyx_t_242 < 0) __pyx_t_242 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+  if (__pyx_t_243 < 0) __pyx_t_243 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+  __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_238, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_239, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_240, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_241, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_242, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_243, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
 
-  /* "fastphase/fastphase.pyx":1086
- *     p_g_givX[0,2] *= np.exp(lik[0,2])
+  /* "fastphase/fastphase.pyx":1078
+ *     p_g_givX[0,2] *= lik[0,2]
  *     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
  *     p_g_givX[0]/=normC             # <<<<<<<<<<<<<<
  * 
  *     for m in range(nLoc-1):
  */
-  __pyx_t_245 = 0;
-  __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_245, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1086, __pyx_L1_error)
+  __pyx_t_244 = 0;
+  __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_244, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1078, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1086, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1086, __pyx_L1_error)
+  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1078, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1078, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_245, __pyx_t_5, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0) < 0)) __PYX_ERR(0, 1086, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_244, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 0) < 0)) __PYX_ERR(0, 1078, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "fastphase/fastphase.pyx":1088
+  /* "fastphase/fastphase.pyx":1080
  *     p_g_givX[0]/=normC
  * 
  *     for m in range(nLoc-1):             # <<<<<<<<<<<<<<
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  */
-  __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1088, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_5); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1088, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_6 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1080, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_t_6); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1080, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1089
+    /* "fastphase/fastphase.pyx":1081
  * 
  *     for m in range(nLoc-1):
  *         for k1 in range(nK):             # <<<<<<<<<<<<<<
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1089, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1081, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k1 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1090
+      /* "fastphase/fastphase.pyx":1082
  *     for m in range(nLoc-1):
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):             # <<<<<<<<<<<<<<
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1090, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1082, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = __pyx_v_k1; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k2 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1091
+        /* "fastphase/fastphase.pyx":1083
  *         for k1 in range(nK):
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]             # <<<<<<<<<<<<<<
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  */
-        __pyx_t_246 = (__pyx_v_m + 1);
-        __pyx_t_247 = __pyx_v_k1;
-        if (__pyx_t_246 < 0) __pyx_t_246 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_247 < 0) __pyx_t_247 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_248 = __pyx_v_m;
-        __pyx_t_249 = __pyx_v_k2;
-        if (__pyx_t_248 < 0) __pyx_t_248 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
-        if (__pyx_t_249 < 0) __pyx_t_249 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
-        __pyx_t_250 = (__pyx_v_m + 1);
-        __pyx_t_251 = __pyx_v_k2;
-        if (__pyx_t_250 < 0) __pyx_t_250 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_251 < 0) __pyx_t_251 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_252 = __pyx_v_m;
-        __pyx_t_253 = __pyx_v_k1;
-        if (__pyx_t_252 < 0) __pyx_t_252 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
-        if (__pyx_t_253 < 0) __pyx_t_253 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
-        __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_246, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_247, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_248, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_249, __pyx_pybuffernd_tSumk.diminfo[1].strides))) + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_250, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_251, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_252, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_253, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
+        __pyx_t_245 = (__pyx_v_m + 1);
+        __pyx_t_246 = __pyx_v_k1;
+        if (__pyx_t_245 < 0) __pyx_t_245 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_246 < 0) __pyx_t_246 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_247 = __pyx_v_m;
+        __pyx_t_248 = __pyx_v_k2;
+        if (__pyx_t_247 < 0) __pyx_t_247 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
+        if (__pyx_t_248 < 0) __pyx_t_248 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
+        __pyx_t_249 = (__pyx_v_m + 1);
+        __pyx_t_250 = __pyx_v_k2;
+        if (__pyx_t_249 < 0) __pyx_t_249 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_250 < 0) __pyx_t_250 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_251 = __pyx_v_m;
+        __pyx_t_252 = __pyx_v_k1;
+        if (__pyx_t_251 < 0) __pyx_t_251 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
+        if (__pyx_t_252 < 0) __pyx_t_252 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
+        __pyx_v_temp = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_245, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_246, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_247, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_248, __pyx_pybuffernd_tSumk.diminfo[1].strides))) + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_249, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_250, __pyx_pybuffernd_alpha.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_251, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_252, __pyx_pybuffernd_tSumk.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1092
+        /* "fastphase/fastphase.pyx":1084
  *             for k2 in range(k1,nK):
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  */
-        __pyx_t_254 = (__pyx_v_m + 1);
-        __pyx_t_255 = 0;
-        if (__pyx_t_254 < 0) __pyx_t_254 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_255 < 0) __pyx_t_255 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_v_temp = (__pyx_v_temp * (0.5 * __pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_254, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_255, __pyx_pybuffernd_rho.diminfo[1].strides)))));
+        __pyx_t_253 = (__pyx_v_m + 1);
+        __pyx_t_254 = 0;
+        if (__pyx_t_253 < 0) __pyx_t_253 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_254 < 0) __pyx_t_254 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_v_temp = (__pyx_v_temp * (0.5 * __pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_253, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_254, __pyx_pybuffernd_rho.diminfo[1].strides)))));
 
-        /* "fastphase/fastphase.pyx":1093
+        /* "fastphase/fastphase.pyx":1085
  *                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]             # <<<<<<<<<<<<<<
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 temp*=mBeta[m+1,k1,k2]
  */
-        __pyx_t_256 = (__pyx_v_m + 1);
-        __pyx_t_257 = 0;
-        if (__pyx_t_256 < 0) __pyx_t_256 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_257 < 0) __pyx_t_257 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_t_258 = __pyx_v_m;
-        __pyx_t_259 = __pyx_v_k1;
-        __pyx_t_260 = __pyx_v_k2;
-        if (__pyx_t_258 < 0) __pyx_t_258 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
-        if (__pyx_t_259 < 0) __pyx_t_259 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
-        if (__pyx_t_260 < 0) __pyx_t_260 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
-        __pyx_v_temp = (__pyx_v_temp + (__pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_256, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_257, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_258, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_259, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_260, __pyx_pybuffernd_mPhi.diminfo[2].strides))));
+        __pyx_t_255 = (__pyx_v_m + 1);
+        __pyx_t_256 = 0;
+        if (__pyx_t_255 < 0) __pyx_t_255 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_256 < 0) __pyx_t_256 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_t_257 = __pyx_v_m;
+        __pyx_t_258 = __pyx_v_k1;
+        __pyx_t_259 = __pyx_v_k2;
+        if (__pyx_t_257 < 0) __pyx_t_257 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
+        if (__pyx_t_258 < 0) __pyx_t_258 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
+        if (__pyx_t_259 < 0) __pyx_t_259 += __pyx_pybuffernd_mPhi.diminfo[2].shape;
+        __pyx_v_temp = (__pyx_v_temp + (__pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 0, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_255, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_256, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_257, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_258, __pyx_pybuffernd_mPhi.diminfo[1].strides, __pyx_t_259, __pyx_pybuffernd_mPhi.diminfo[2].strides))));
 
-        /* "fastphase/fastphase.pyx":1094
+        /* "fastphase/fastphase.pyx":1086
  *                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]             # <<<<<<<<<<<<<<
  *                 temp*=mBeta[m+1,k1,k2]
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  */
-        __pyx_t_261 = (__pyx_v_m + 1);
-        __pyx_t_262 = 0;
-        if (__pyx_t_261 < 0) __pyx_t_261 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_262 < 0) __pyx_t_262 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_t_263 = (__pyx_v_m + 1);
-        __pyx_t_264 = __pyx_v_k1;
-        if (__pyx_t_263 < 0) __pyx_t_263 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_264 < 0) __pyx_t_264 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_265 = (__pyx_v_m + 1);
-        __pyx_t_266 = __pyx_v_k2;
-        if (__pyx_t_265 < 0) __pyx_t_265 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_266 < 0) __pyx_t_266 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_t_267 = __pyx_v_m;
-        if (__pyx_t_267 < 0) __pyx_t_267 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
-        __pyx_v_temp = (__pyx_v_temp + (((__pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_261, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_262, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_263, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_264, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_265, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_266, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_267, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
+        __pyx_t_260 = (__pyx_v_m + 1);
+        __pyx_t_261 = 0;
+        if (__pyx_t_260 < 0) __pyx_t_260 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_261 < 0) __pyx_t_261 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_t_262 = (__pyx_v_m + 1);
+        __pyx_t_263 = __pyx_v_k1;
+        if (__pyx_t_262 < 0) __pyx_t_262 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_263 < 0) __pyx_t_263 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_264 = (__pyx_v_m + 1);
+        __pyx_t_265 = __pyx_v_k2;
+        if (__pyx_t_264 < 0) __pyx_t_264 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_265 < 0) __pyx_t_265 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_t_266 = __pyx_v_m;
+        if (__pyx_t_266 < 0) __pyx_t_266 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
+        __pyx_v_temp = (__pyx_v_temp + (((__pyx_f_9fastphase_9fastphase_probJ((__pyx_v_m + 1), 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_260, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_261, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_262, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_263, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_264, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_265, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_266, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))));
 
-        /* "fastphase/fastphase.pyx":1095
+        /* "fastphase/fastphase.pyx":1087
  *                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 temp*=mBeta[m+1,k1,k2]             # <<<<<<<<<<<<<<
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  */
-        __pyx_t_268 = (__pyx_v_m + 1);
-        __pyx_t_269 = __pyx_v_k1;
-        __pyx_t_270 = __pyx_v_k2;
-        if (__pyx_t_268 < 0) __pyx_t_268 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
-        if (__pyx_t_269 < 0) __pyx_t_269 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
-        if (__pyx_t_270 < 0) __pyx_t_270 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
-        __pyx_v_temp = (__pyx_v_temp * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_268, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_269, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_270, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
+        __pyx_t_267 = (__pyx_v_m + 1);
+        __pyx_t_268 = __pyx_v_k1;
+        __pyx_t_269 = __pyx_v_k2;
+        if (__pyx_t_267 < 0) __pyx_t_267 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
+        if (__pyx_t_268 < 0) __pyx_t_268 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
+        if (__pyx_t_269 < 0) __pyx_t_269 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
+        __pyx_v_temp = (__pyx_v_temp * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_267, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_268, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_269, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
 
-        /* "fastphase/fastphase.pyx":1096
+        /* "fastphase/fastphase.pyx":1088
  *                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
  *                 temp*=mBeta[m+1,k1,k2]
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)             # <<<<<<<<<<<<<<
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
  */
-        __pyx_t_271 = (__pyx_v_m + 1);
-        __pyx_t_272 = __pyx_v_k1;
-        if (__pyx_t_271 < 0) __pyx_t_271 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_272 < 0) __pyx_t_272 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_273 = (__pyx_v_m + 1);
-        __pyx_t_274 = __pyx_v_k2;
-        if (__pyx_t_273 < 0) __pyx_t_273 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_274 < 0) __pyx_t_274 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_275 = (__pyx_v_m + 1);
-        __pyx_t_276 = 0;
-        if (__pyx_t_275 < 0) __pyx_t_275 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-        if (__pyx_t_276 < 0) __pyx_t_276 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_275, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_276, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_271, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_272, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_273, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_274, __pyx_pybuffernd_theta.diminfo[1].strides)), 0));
+        __pyx_t_270 = (__pyx_v_m + 1);
+        __pyx_t_271 = __pyx_v_k1;
+        if (__pyx_t_270 < 0) __pyx_t_270 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_271 < 0) __pyx_t_271 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_272 = (__pyx_v_m + 1);
+        __pyx_t_273 = __pyx_v_k2;
+        if (__pyx_t_272 < 0) __pyx_t_272 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_273 < 0) __pyx_t_273 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_274 = (__pyx_v_m + 1);
+        __pyx_t_275 = 0;
+        if (__pyx_t_274 < 0) __pyx_t_274 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+        if (__pyx_t_275 < 0) __pyx_t_275 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_274, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_275, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_270, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_271, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_272, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_273, __pyx_pybuffernd_theta.diminfo[1].strides)), 0));
 
-        /* "fastphase/fastphase.pyx":1097
+        /* "fastphase/fastphase.pyx":1089
  *                 temp*=mBeta[m+1,k1,k2]
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)             # <<<<<<<<<<<<<<
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
  */
-        __pyx_t_277 = (__pyx_v_m + 1);
-        __pyx_t_278 = __pyx_v_k1;
-        if (__pyx_t_277 < 0) __pyx_t_277 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_278 < 0) __pyx_t_278 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_279 = (__pyx_v_m + 1);
-        __pyx_t_280 = __pyx_v_k2;
-        if (__pyx_t_279 < 0) __pyx_t_279 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_280 < 0) __pyx_t_280 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_281 = (__pyx_v_m + 1);
-        __pyx_t_282 = 1;
-        if (__pyx_t_281 < 0) __pyx_t_281 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-        if (__pyx_t_282 < 0) __pyx_t_282 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_281, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_282, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_277, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_278, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_279, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_280, __pyx_pybuffernd_theta.diminfo[1].strides)), 1));
+        __pyx_t_276 = (__pyx_v_m + 1);
+        __pyx_t_277 = __pyx_v_k1;
+        if (__pyx_t_276 < 0) __pyx_t_276 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_277 < 0) __pyx_t_277 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_278 = (__pyx_v_m + 1);
+        __pyx_t_279 = __pyx_v_k2;
+        if (__pyx_t_278 < 0) __pyx_t_278 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_279 < 0) __pyx_t_279 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_280 = (__pyx_v_m + 1);
+        __pyx_t_281 = 1;
+        if (__pyx_t_280 < 0) __pyx_t_280 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+        if (__pyx_t_281 < 0) __pyx_t_281 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_280, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_281, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_276, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_277, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_278, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_279, __pyx_pybuffernd_theta.diminfo[1].strides)), 1));
 
-        /* "fastphase/fastphase.pyx":1098
+        /* "fastphase/fastphase.pyx":1090
  *                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)             # <<<<<<<<<<<<<<
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
  */
-        __pyx_t_283 = (__pyx_v_m + 1);
-        __pyx_t_284 = __pyx_v_k1;
-        if (__pyx_t_283 < 0) __pyx_t_283 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_284 < 0) __pyx_t_284 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_285 = (__pyx_v_m + 1);
-        __pyx_t_286 = __pyx_v_k2;
-        if (__pyx_t_285 < 0) __pyx_t_285 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_286 < 0) __pyx_t_286 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_287 = (__pyx_v_m + 1);
-        __pyx_t_288 = 2;
-        if (__pyx_t_287 < 0) __pyx_t_287 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-        if (__pyx_t_288 < 0) __pyx_t_288 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_287, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_288, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_283, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_284, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_285, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_286, __pyx_pybuffernd_theta.diminfo[1].strides)), 2));
+        __pyx_t_282 = (__pyx_v_m + 1);
+        __pyx_t_283 = __pyx_v_k1;
+        if (__pyx_t_282 < 0) __pyx_t_282 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_283 < 0) __pyx_t_283 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_284 = (__pyx_v_m + 1);
+        __pyx_t_285 = __pyx_v_k2;
+        if (__pyx_t_284 < 0) __pyx_t_284 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_285 < 0) __pyx_t_285 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_286 = (__pyx_v_m + 1);
+        __pyx_t_287 = 2;
+        if (__pyx_t_286 < 0) __pyx_t_286 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+        if (__pyx_t_287 < 0) __pyx_t_287 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_286, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_287, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) += (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_genprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_282, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_283, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_284, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_285, __pyx_pybuffernd_theta.diminfo[1].strides)), 2));
       }
     }
 
-    /* "fastphase/fastphase.pyx":1099
+    /* "fastphase/fastphase.pyx":1091
  *                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])             # <<<<<<<<<<<<<<
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
- */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1099, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_exp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1099, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_289 = (__pyx_v_m + 1);
-    __pyx_t_290 = 0;
-    if (__pyx_t_289 < 0) __pyx_t_289 += __pyx_pybuffernd_lik.diminfo[0].shape;
-    if (__pyx_t_290 < 0) __pyx_t_290 += __pyx_pybuffernd_lik.diminfo[1].shape;
-    __pyx_t_6 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_289, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_290, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1099, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1099, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1099, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_291 = (__pyx_v_m + 1);
-    __pyx_t_292 = 0;
-    if (__pyx_t_291 < 0) __pyx_t_291 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_292 < 0) __pyx_t_292 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_291, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_292, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
+ *         p_g_givX[m+1,0] *= lik[m+1,0]             # <<<<<<<<<<<<<<
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
+ */
+    __pyx_t_288 = (__pyx_v_m + 1);
+    __pyx_t_289 = 0;
+    if (__pyx_t_288 < 0) __pyx_t_288 += __pyx_pybuffernd_lik.diminfo[0].shape;
+    if (__pyx_t_289 < 0) __pyx_t_289 += __pyx_pybuffernd_lik.diminfo[1].shape;
+    __pyx_t_290 = (__pyx_v_m + 1);
+    __pyx_t_291 = 0;
+    if (__pyx_t_290 < 0) __pyx_t_290 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_291 < 0) __pyx_t_291 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_290, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_291, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_288, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_289, __pyx_pybuffernd_lik.diminfo[1].strides));
 
-    /* "fastphase/fastphase.pyx":1100
+    /* "fastphase/fastphase.pyx":1092
  *                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])             # <<<<<<<<<<<<<<
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
+ *         p_g_givX[m+1,1] *= lik[m+1,1]             # <<<<<<<<<<<<<<
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1100, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_exp); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1100, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_293 = (__pyx_v_m + 1);
-    __pyx_t_294 = 1;
-    if (__pyx_t_293 < 0) __pyx_t_293 += __pyx_pybuffernd_lik.diminfo[0].shape;
-    if (__pyx_t_294 < 0) __pyx_t_294 += __pyx_pybuffernd_lik.diminfo[1].shape;
-    __pyx_t_4 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_293, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_294, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1100, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1100, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1100, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_295 = (__pyx_v_m + 1);
-    __pyx_t_296 = 1;
-    if (__pyx_t_295 < 0) __pyx_t_295 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_296 < 0) __pyx_t_296 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_295, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_296, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-    /* "fastphase/fastphase.pyx":1101
- *         p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])             # <<<<<<<<<<<<<<
+    __pyx_t_292 = (__pyx_v_m + 1);
+    __pyx_t_293 = 1;
+    if (__pyx_t_292 < 0) __pyx_t_292 += __pyx_pybuffernd_lik.diminfo[0].shape;
+    if (__pyx_t_293 < 0) __pyx_t_293 += __pyx_pybuffernd_lik.diminfo[1].shape;
+    __pyx_t_294 = (__pyx_v_m + 1);
+    __pyx_t_295 = 1;
+    if (__pyx_t_294 < 0) __pyx_t_294 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_295 < 0) __pyx_t_295 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_294, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_295, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_292, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_293, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+    /* "fastphase/fastphase.pyx":1093
+ *         p_g_givX[m+1,0] *= lik[m+1,0]
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
+ *         p_g_givX[m+1,2] *= lik[m+1,2]             # <<<<<<<<<<<<<<
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
  *         p_g_givX[m+1]/=normC
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1101, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_exp); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1101, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_297 = (__pyx_v_m + 1);
-    __pyx_t_298 = 2;
-    if (__pyx_t_297 < 0) __pyx_t_297 += __pyx_pybuffernd_lik.diminfo[0].shape;
-    if (__pyx_t_298 < 0) __pyx_t_298 += __pyx_pybuffernd_lik.diminfo[1].shape;
-    __pyx_t_6 = PyFloat_FromDouble((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_297, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_298, __pyx_pybuffernd_lik.diminfo[1].strides))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1101, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_3)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_3);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-      }
-    }
-    __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_6);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1101, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1101, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_299 = (__pyx_v_m + 1);
-    __pyx_t_300 = 2;
-    if (__pyx_t_299 < 0) __pyx_t_299 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_300 < 0) __pyx_t_300 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_299, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_300, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= __pyx_t_228;
-
-    /* "fastphase/fastphase.pyx":1102
- *         p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+    __pyx_t_296 = (__pyx_v_m + 1);
+    __pyx_t_297 = 2;
+    if (__pyx_t_296 < 0) __pyx_t_296 += __pyx_pybuffernd_lik.diminfo[0].shape;
+    if (__pyx_t_297 < 0) __pyx_t_297 += __pyx_pybuffernd_lik.diminfo[1].shape;
+    __pyx_t_298 = (__pyx_v_m + 1);
+    __pyx_t_299 = 2;
+    if (__pyx_t_298 < 0) __pyx_t_298 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_299 < 0) __pyx_t_299 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_298, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_299, __pyx_pybuffernd_p_g_givX.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_lik.rcbuffer->pybuffer.buf, __pyx_t_296, __pyx_pybuffernd_lik.diminfo[0].strides, __pyx_t_297, __pyx_pybuffernd_lik.diminfo[1].strides));
+
+    /* "fastphase/fastphase.pyx":1094
+ *         p_g_givX[m+1,1] *= lik[m+1,1]
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]             # <<<<<<<<<<<<<<
  *         p_g_givX[m+1]/=normC
  * 
  */
-    __pyx_t_301 = (__pyx_v_m + 1);
-    __pyx_t_302 = 0;
-    if (__pyx_t_301 < 0) __pyx_t_301 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_302 < 0) __pyx_t_302 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    __pyx_t_303 = (__pyx_v_m + 1);
-    __pyx_t_304 = 1;
-    if (__pyx_t_303 < 0) __pyx_t_303 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_304 < 0) __pyx_t_304 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    __pyx_t_305 = (__pyx_v_m + 1);
-    __pyx_t_306 = 2;
-    if (__pyx_t_305 < 0) __pyx_t_305 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
-    if (__pyx_t_306 < 0) __pyx_t_306 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
-    __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_301, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_302, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_303, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_304, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_305, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_306, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
+    __pyx_t_300 = (__pyx_v_m + 1);
+    __pyx_t_301 = 0;
+    if (__pyx_t_300 < 0) __pyx_t_300 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_301 < 0) __pyx_t_301 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    __pyx_t_302 = (__pyx_v_m + 1);
+    __pyx_t_303 = 1;
+    if (__pyx_t_302 < 0) __pyx_t_302 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_303 < 0) __pyx_t_303 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    __pyx_t_304 = (__pyx_v_m + 1);
+    __pyx_t_305 = 2;
+    if (__pyx_t_304 < 0) __pyx_t_304 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
+    if (__pyx_t_305 < 0) __pyx_t_305 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
+    __pyx_v_normC = (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_300, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_301, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_302, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_303, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_304, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_305, __pyx_pybuffernd_p_g_givX.diminfo[1].strides)));
 
-    /* "fastphase/fastphase.pyx":1103
- *         p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+    /* "fastphase/fastphase.pyx":1095
+ *         p_g_givX[m+1,2] *= lik[m+1,2]
  *         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
  *         p_g_givX[m+1]/=normC             # <<<<<<<<<<<<<<
  * 
  *     if up2pz>0:
  */
     __pyx_t_13 = (__pyx_v_m + 1);
-    __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1103, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, long, 1, __Pyx_PyInt_From_long, 0, 1, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1095, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1095, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_normC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1103, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1095, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyNumber_InPlaceDivide(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1103, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 0) < 0)) __PYX_ERR(0, 1095, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_p_g_givX), __pyx_t_13, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 0) < 0)) __PYX_ERR(0, 1103, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
 
-  /* "fastphase/fastphase.pyx":1105
+  /* "fastphase/fastphase.pyx":1097
  *         p_g_givX[m+1]/=normC
  * 
  *     if up2pz>0:             # <<<<<<<<<<<<<<
  *         return probZ,p_g_givX
  *     # calc jmk
  */
   __pyx_t_66 = ((__pyx_v_up2pz > 0) != 0);
   if (__pyx_t_66) {
 
-    /* "fastphase/fastphase.pyx":1106
+    /* "fastphase/fastphase.pyx":1098
  * 
  *     if up2pz>0:
  *         return probZ,p_g_givX             # <<<<<<<<<<<<<<
  *     # calc jmk
  *     for k1 in range(nK):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1106, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1098, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(((PyObject *)__pyx_v_probZ));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_probZ));
-    PyTuple_SET_ITEM(__pyx_t_6, 0, ((PyObject *)__pyx_v_probZ));
+    PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_probZ));
     __Pyx_INCREF(((PyObject *)__pyx_v_p_g_givX));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_p_g_givX));
-    PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_p_g_givX));
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_p_g_givX));
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "fastphase/fastphase.pyx":1105
+    /* "fastphase/fastphase.pyx":1097
  *         p_g_givX[m+1]/=normC
  * 
  *     if up2pz>0:             # <<<<<<<<<<<<<<
  *         return probZ,p_g_givX
  *     # calc jmk
  */
   }
 
-  /* "fastphase/fastphase.pyx":1108
+  /* "fastphase/fastphase.pyx":1100
  *         return probZ,p_g_givX
  *     # calc jmk
  *     for k1 in range(nK):             # <<<<<<<<<<<<<<
  *         ##jmk[0,k1]=2*alpha[0,k1]
  *         jmk[0, k1] = probZ[0,k1,k1]
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1108, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1100, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_k1 = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1110
+    /* "fastphase/fastphase.pyx":1102
  *     for k1 in range(nK):
  *         ##jmk[0,k1]=2*alpha[0,k1]
  *         jmk[0, k1] = probZ[0,k1,k1]             # <<<<<<<<<<<<<<
  *         for k2 in range(nK):
  *             jmk[0, k1] += probZ[0, k2, k1]
  */
-    __pyx_t_307 = 0;
+    __pyx_t_306 = 0;
+    __pyx_t_307 = __pyx_v_k1;
     __pyx_t_308 = __pyx_v_k1;
-    __pyx_t_309 = __pyx_v_k1;
-    if (__pyx_t_307 < 0) __pyx_t_307 += __pyx_pybuffernd_probZ.diminfo[0].shape;
-    if (__pyx_t_308 < 0) __pyx_t_308 += __pyx_pybuffernd_probZ.diminfo[1].shape;
-    if (__pyx_t_309 < 0) __pyx_t_309 += __pyx_pybuffernd_probZ.diminfo[2].shape;
-    __pyx_t_310 = 0;
-    __pyx_t_311 = __pyx_v_k1;
-    if (__pyx_t_310 < 0) __pyx_t_310 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-    if (__pyx_t_311 < 0) __pyx_t_311 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_310, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_311, __pyx_pybuffernd_jmk.diminfo[1].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_307, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_308, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_309, __pyx_pybuffernd_probZ.diminfo[2].strides));
+    if (__pyx_t_306 < 0) __pyx_t_306 += __pyx_pybuffernd_probZ.diminfo[0].shape;
+    if (__pyx_t_307 < 0) __pyx_t_307 += __pyx_pybuffernd_probZ.diminfo[1].shape;
+    if (__pyx_t_308 < 0) __pyx_t_308 += __pyx_pybuffernd_probZ.diminfo[2].shape;
+    __pyx_t_309 = 0;
+    __pyx_t_310 = __pyx_v_k1;
+    if (__pyx_t_309 < 0) __pyx_t_309 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+    if (__pyx_t_310 < 0) __pyx_t_310 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+    *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_309, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_310, __pyx_pybuffernd_jmk.diminfo[1].strides) = (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_306, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_307, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_308, __pyx_pybuffernd_probZ.diminfo[2].strides));
 
-    /* "fastphase/fastphase.pyx":1111
+    /* "fastphase/fastphase.pyx":1103
  *         ##jmk[0,k1]=2*alpha[0,k1]
  *         jmk[0, k1] = probZ[0,k1,k1]
  *         for k2 in range(nK):             # <<<<<<<<<<<<<<
  *             jmk[0, k1] += probZ[0, k2, k1]
  * 
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1111, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1103, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k2 = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1112
+      /* "fastphase/fastphase.pyx":1104
  *         jmk[0, k1] = probZ[0,k1,k1]
  *         for k2 in range(nK):
  *             jmk[0, k1] += probZ[0, k2, k1]             # <<<<<<<<<<<<<<
  * 
  *     for m in range(1,nLoc):
  */
-      __pyx_t_312 = 0;
-      __pyx_t_313 = __pyx_v_k2;
-      __pyx_t_314 = __pyx_v_k1;
-      if (__pyx_t_312 < 0) __pyx_t_312 += __pyx_pybuffernd_probZ.diminfo[0].shape;
-      if (__pyx_t_313 < 0) __pyx_t_313 += __pyx_pybuffernd_probZ.diminfo[1].shape;
-      if (__pyx_t_314 < 0) __pyx_t_314 += __pyx_pybuffernd_probZ.diminfo[2].shape;
-      __pyx_t_315 = 0;
-      __pyx_t_316 = __pyx_v_k1;
-      if (__pyx_t_315 < 0) __pyx_t_315 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-      if (__pyx_t_316 < 0) __pyx_t_316 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_315, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_316, __pyx_pybuffernd_jmk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_312, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_313, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_314, __pyx_pybuffernd_probZ.diminfo[2].strides));
+      __pyx_t_311 = 0;
+      __pyx_t_312 = __pyx_v_k2;
+      __pyx_t_313 = __pyx_v_k1;
+      if (__pyx_t_311 < 0) __pyx_t_311 += __pyx_pybuffernd_probZ.diminfo[0].shape;
+      if (__pyx_t_312 < 0) __pyx_t_312 += __pyx_pybuffernd_probZ.diminfo[1].shape;
+      if (__pyx_t_313 < 0) __pyx_t_313 += __pyx_pybuffernd_probZ.diminfo[2].shape;
+      __pyx_t_314 = 0;
+      __pyx_t_315 = __pyx_v_k1;
+      if (__pyx_t_314 < 0) __pyx_t_314 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+      if (__pyx_t_315 < 0) __pyx_t_315 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_314, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_315, __pyx_pybuffernd_jmk.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_311, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_312, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_313, __pyx_pybuffernd_probZ.diminfo[2].strides));
     }
   }
 
-  /* "fastphase/fastphase.pyx":1114
+  /* "fastphase/fastphase.pyx":1106
  *             jmk[0, k1] += probZ[0, k2, k1]
  * 
  *     for m in range(1,nLoc):             # <<<<<<<<<<<<<<
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1114, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1106, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 1; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1115
+    /* "fastphase/fastphase.pyx":1107
  * 
  *     for m in range(1,nLoc):
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             for k1 in range(nK):
  */
-    __pyx_t_317 = (__pyx_v_m - 1);
-    if (__pyx_t_317 < 0) __pyx_t_317 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
-    __pyx_t_318 = __pyx_v_m;
-    if (__pyx_t_318 < 0) __pyx_t_318 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
-    __pyx_t_6 = __Pyx_PyInt_From_npy_long(((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_317, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_318, __pyx_pybuffernd_betaScale.diminfo[0].strides)))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1115, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1115, __pyx_L1_error)
+    __pyx_t_316 = (__pyx_v_m - 1);
+    if (__pyx_t_316 < 0) __pyx_t_316 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
+    __pyx_t_317 = __pyx_v_m;
+    if (__pyx_t_317 < 0) __pyx_t_317 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
+    __pyx_t_4 = __Pyx_PyInt_From_npy_long(((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_316, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_317, __pyx_pybuffernd_betaScale.diminfo[0].strides)))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1115, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1107, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_phiScale), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1107, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyNumber_Subtract(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyNumber_Subtract(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1115, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_15 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_15 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1107, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_15 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_15 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1115, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10(__pyx_t_15);
 
-    /* "fastphase/fastphase.pyx":1116
+    /* "fastphase/fastphase.pyx":1108
  *     for m in range(1,nLoc):
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1116, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1108, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1117
+      /* "fastphase/fastphase.pyx":1109
  *         dummy = myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1117, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1109, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k1 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1118
+        /* "fastphase/fastphase.pyx":1110
  *         for k in range(nK):
  *             for k1 in range(nK):
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])             # <<<<<<<<<<<<<<
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  */
-        __pyx_t_319 = (__pyx_v_m - 1);
-        __pyx_t_320 = __pyx_v_k1;
-        if (__pyx_t_319 < 0) __pyx_t_319 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
-        if (__pyx_t_320 < 0) __pyx_t_320 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
-        __pyx_t_321 = __pyx_v_m;
-        __pyx_t_322 = 0;
-        if (__pyx_t_321 < 0) __pyx_t_321 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_322 < 0) __pyx_t_322 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_v_temp = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_319, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_320, __pyx_pybuffernd_tSumk.diminfo[1].strides)) * __pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_321, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_322, __pyx_pybuffernd_rho.diminfo[1].strides))));
+        __pyx_t_318 = (__pyx_v_m - 1);
+        __pyx_t_319 = __pyx_v_k1;
+        if (__pyx_t_318 < 0) __pyx_t_318 += __pyx_pybuffernd_tSumk.diminfo[0].shape;
+        if (__pyx_t_319 < 0) __pyx_t_319 += __pyx_pybuffernd_tSumk.diminfo[1].shape;
+        __pyx_t_320 = __pyx_v_m;
+        __pyx_t_321 = 0;
+        if (__pyx_t_320 < 0) __pyx_t_320 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_321 < 0) __pyx_t_321 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_v_temp = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSumk.rcbuffer->pybuffer.buf, __pyx_t_318, __pyx_pybuffernd_tSumk.diminfo[0].strides, __pyx_t_319, __pyx_pybuffernd_tSumk.diminfo[1].strides)) * __pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 1, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_320, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_321, __pyx_pybuffernd_rho.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1119
+        /* "fastphase/fastphase.pyx":1111
  *             for k1 in range(nK):
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]             # <<<<<<<<<<<<<<
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  *             jmk[m,k] *= alpha[m,k]
  */
-        __pyx_t_323 = __pyx_v_m;
-        __pyx_t_324 = 0;
-        if (__pyx_t_323 < 0) __pyx_t_323 += __pyx_pybuffernd_rho.diminfo[0].shape;
-        if (__pyx_t_324 < 0) __pyx_t_324 += __pyx_pybuffernd_rho.diminfo[1].shape;
-        __pyx_t_325 = (__pyx_v_m - 1);
-        if (__pyx_t_325 < 0) __pyx_t_325 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
-        __pyx_t_326 = __pyx_v_m;
-        __pyx_t_327 = __pyx_v_k1;
-        if (__pyx_t_326 < 0) __pyx_t_326 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-        if (__pyx_t_327 < 0) __pyx_t_327 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-        __pyx_v_temp = (__pyx_v_temp + (((2.0 * __pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_323, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_324, __pyx_pybuffernd_rho.diminfo[1].strides)))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_325, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_326, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_327, __pyx_pybuffernd_alpha.diminfo[1].strides))));
+        __pyx_t_322 = __pyx_v_m;
+        __pyx_t_323 = 0;
+        if (__pyx_t_322 < 0) __pyx_t_322 += __pyx_pybuffernd_rho.diminfo[0].shape;
+        if (__pyx_t_323 < 0) __pyx_t_323 += __pyx_pybuffernd_rho.diminfo[1].shape;
+        __pyx_t_324 = (__pyx_v_m - 1);
+        if (__pyx_t_324 < 0) __pyx_t_324 += __pyx_pybuffernd_tDoubleSum.diminfo[0].shape;
+        __pyx_t_325 = __pyx_v_m;
+        __pyx_t_326 = __pyx_v_k1;
+        if (__pyx_t_325 < 0) __pyx_t_325 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+        if (__pyx_t_326 < 0) __pyx_t_326 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+        __pyx_v_temp = (__pyx_v_temp + (((2.0 * __pyx_f_9fastphase_9fastphase_probJ(__pyx_v_m, 2, (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_322, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_323, __pyx_pybuffernd_rho.diminfo[1].strides)))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tDoubleSum.rcbuffer->pybuffer.buf, __pyx_t_324, __pyx_pybuffernd_tDoubleSum.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_325, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_326, __pyx_pybuffernd_alpha.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1120
+        /* "fastphase/fastphase.pyx":1112
  *                 temp = tSumk[ m-1, k1] * probJ(m,1,rho[m,0])
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]             # <<<<<<<<<<<<<<
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tDoubleSum[nLoc-1]
  */
-        __pyx_t_328 = __pyx_v_m;
-        __pyx_t_329 = __pyx_v_k;
-        if (__pyx_t_328 < 0) __pyx_t_328 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_329 < 0) __pyx_t_329 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_330 = __pyx_v_m;
-        __pyx_t_331 = __pyx_v_k1;
-        if (__pyx_t_330 < 0) __pyx_t_330 += __pyx_pybuffernd_theta.diminfo[0].shape;
-        if (__pyx_t_331 < 0) __pyx_t_331 += __pyx_pybuffernd_theta.diminfo[1].shape;
-        __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1120, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1120, __pyx_L1_error)
-        __pyx_t_332 = __pyx_v_m;
-        __pyx_t_333 = __pyx_v_k;
-        __pyx_t_334 = __pyx_v_k1;
-        if (__pyx_t_332 < 0) __pyx_t_332 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
-        if (__pyx_t_333 < 0) __pyx_t_333 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
-        if (__pyx_t_334 < 0) __pyx_t_334 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
-        __pyx_t_335 = __pyx_v_m;
-        __pyx_t_336 = __pyx_v_k;
-        if (__pyx_t_335 < 0) __pyx_t_335 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-        if (__pyx_t_336 < 0) __pyx_t_336 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_335, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_336, __pyx_pybuffernd_jmk.diminfo[1].strides) += ((__pyx_v_temp * __pyx_f_9fastphase_9fastphase_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_328, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_329, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_330, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_331, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_4))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_332, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_333, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_334, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_327 = __pyx_v_m;
+        __pyx_t_328 = __pyx_v_k;
+        if (__pyx_t_327 < 0) __pyx_t_327 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_328 < 0) __pyx_t_328 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_329 = __pyx_v_m;
+        __pyx_t_330 = __pyx_v_k1;
+        if (__pyx_t_329 < 0) __pyx_t_329 += __pyx_pybuffernd_theta.diminfo[0].shape;
+        if (__pyx_t_330 < 0) __pyx_t_330 += __pyx_pybuffernd_theta.diminfo[1].shape;
+        __pyx_t_5 = __Pyx_GetItemInt(((PyObject *)__pyx_v_lik), __pyx_v_m, int, 1, __Pyx_PyInt_From_int, 0, 1, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1112, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1112, __pyx_L1_error)
+        __pyx_t_331 = __pyx_v_m;
+        __pyx_t_332 = __pyx_v_k;
+        __pyx_t_333 = __pyx_v_k1;
+        if (__pyx_t_331 < 0) __pyx_t_331 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
+        if (__pyx_t_332 < 0) __pyx_t_332 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
+        if (__pyx_t_333 < 0) __pyx_t_333 += __pyx_pybuffernd_mBeta.diminfo[2].shape;
+        __pyx_t_334 = __pyx_v_m;
+        __pyx_t_335 = __pyx_v_k;
+        if (__pyx_t_334 < 0) __pyx_t_334 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+        if (__pyx_t_335 < 0) __pyx_t_335 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+        *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_334, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_335, __pyx_pybuffernd_jmk.diminfo[1].strides) += ((__pyx_v_temp * __pyx_f_9fastphase_9fastphase_likprG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_327, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_328, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_329, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_330, __pyx_pybuffernd_theta.diminfo[1].strides)), ((PyArrayObject *)__pyx_t_5))) * (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_331, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_332, __pyx_pybuffernd_mBeta.diminfo[1].strides, __pyx_t_333, __pyx_pybuffernd_mBeta.diminfo[2].strides)));
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
 
-      /* "fastphase/fastphase.pyx":1121
+      /* "fastphase/fastphase.pyx":1113
  *                 temp += 2 * probJ( m, 2, rho[m,0]) * tDoubleSum[m-1] * alpha[m,k1]
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  *             jmk[m,k] *= alpha[m,k]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= tDoubleSum[nLoc-1]
  *             jmk[m,k] /= dummy
  */
-      __pyx_t_337 = __pyx_v_m;
-      __pyx_t_338 = __pyx_v_k;
-      if (__pyx_t_337 < 0) __pyx_t_337 += __pyx_pybuffernd_alpha.diminfo[0].shape;
-      if (__pyx_t_338 < 0) __pyx_t_338 += __pyx_pybuffernd_alpha.diminfo[1].shape;
-      __pyx_t_339 = __pyx_v_m;
-      __pyx_t_340 = __pyx_v_k;
-      if (__pyx_t_339 < 0) __pyx_t_339 += __pyx_pybuffernd_jmk.diminfo[0].shape;
-      if (__pyx_t_340 < 0) __pyx_t_340 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_339, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_340, __pyx_pybuffernd_jmk.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_337, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_338, __pyx_pybuffernd_alpha.diminfo[1].strides));
+      __pyx_t_336 = __pyx_v_m;
+      __pyx_t_337 = __pyx_v_k;
+      if (__pyx_t_336 < 0) __pyx_t_336 += __pyx_pybuffernd_alpha.diminfo[0].shape;
+      if (__pyx_t_337 < 0) __pyx_t_337 += __pyx_pybuffernd_alpha.diminfo[1].shape;
+      __pyx_t_338 = __pyx_v_m;
+      __pyx_t_339 = __pyx_v_k;
+      if (__pyx_t_338 < 0) __pyx_t_338 += __pyx_pybuffernd_jmk.diminfo[0].shape;
+      if (__pyx_t_339 < 0) __pyx_t_339 += __pyx_pybuffernd_jmk.diminfo[1].shape;
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_338, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_339, __pyx_pybuffernd_jmk.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_336, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_337, __pyx_pybuffernd_alpha.diminfo[1].strides));
 
-      /* "fastphase/fastphase.pyx":1122
+      /* "fastphase/fastphase.pyx":1114
  *                 jmk[m,k] += temp * likprG( theta[m,k], theta[m,k1], lik[m]) * mBeta[m,k,k1]
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tDoubleSum[nLoc-1]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= dummy
  *     # calc top,bottom
  */
-      __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1122, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1122, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_SubtractObjC(__pyx_v_nLoc, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_228 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_228 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1122, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_tDoubleSum), __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1114, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_340 = __pyx_PyFloat_AsDouble(__pyx_t_6); if (unlikely((__pyx_t_340 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 1114, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_341 = __pyx_v_m;
       __pyx_t_342 = __pyx_v_k;
       if (__pyx_t_341 < 0) __pyx_t_341 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_342 < 0) __pyx_t_342 += __pyx_pybuffernd_jmk.diminfo[1].shape;
-      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_341, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_342, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_t_228;
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_341, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_342, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_t_340;
 
-      /* "fastphase/fastphase.pyx":1123
+      /* "fastphase/fastphase.pyx":1115
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tDoubleSum[nLoc-1]
  *             jmk[m,k] /= dummy             # <<<<<<<<<<<<<<
  *     # calc top,bottom
  *     for m in range(nLoc):
  */
       __pyx_t_343 = __pyx_v_m;
       __pyx_t_344 = __pyx_v_k;
       if (__pyx_t_343 < 0) __pyx_t_343 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_344 < 0) __pyx_t_344 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_343, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_344, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_v_dummy;
     }
   }
 
-  /* "fastphase/fastphase.pyx":1125
+  /* "fastphase/fastphase.pyx":1117
  *             jmk[m,k] /= dummy
  *     # calc top,bottom
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         ## bottom
  *         for k in range(nK):
  */
-  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1125, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_long(__pyx_v_nLoc); if (unlikely((__pyx_t_11 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1117, __pyx_L1_error)
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_12; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1127
+    /* "fastphase/fastphase.pyx":1119
  *     for m in range(nLoc):
  *         ## bottom
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             bot[m,k]+=probZ[m,k,k]
  *             for k1 in range(nK):
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1127, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1119, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1128
+      /* "fastphase/fastphase.pyx":1120
  *         ## bottom
  *         for k in range(nK):
  *             bot[m,k]+=probZ[m,k,k]             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 bot[m,k]+=probZ[m,k1,k]
  */
       __pyx_t_345 = __pyx_v_m;
@@ -25917,27 +25623,27 @@
       if (__pyx_t_347 < 0) __pyx_t_347 += __pyx_pybuffernd_probZ.diminfo[2].shape;
       __pyx_t_348 = __pyx_v_m;
       __pyx_t_349 = __pyx_v_k;
       if (__pyx_t_348 < 0) __pyx_t_348 += __pyx_pybuffernd_bot.diminfo[0].shape;
       if (__pyx_t_349 < 0) __pyx_t_349 += __pyx_pybuffernd_bot.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_348, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_349, __pyx_pybuffernd_bot.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_345, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_346, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_347, __pyx_pybuffernd_probZ.diminfo[2].strides));
 
-      /* "fastphase/fastphase.pyx":1129
+      /* "fastphase/fastphase.pyx":1121
  *         for k in range(nK):
  *             bot[m,k]+=probZ[m,k,k]
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 bot[m,k]+=probZ[m,k1,k]
  *         # ## top
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1129, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1121, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k1 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1130
+        /* "fastphase/fastphase.pyx":1122
  *             bot[m,k]+=probZ[m,k,k]
  *             for k1 in range(nK):
  *                 bot[m,k]+=probZ[m,k1,k]             # <<<<<<<<<<<<<<
  *         # ## top
  *         for k in range(nK):
  */
         __pyx_t_350 = __pyx_v_m;
@@ -25950,39 +25656,39 @@
         __pyx_t_354 = __pyx_v_k;
         if (__pyx_t_353 < 0) __pyx_t_353 += __pyx_pybuffernd_bot.diminfo[0].shape;
         if (__pyx_t_354 < 0) __pyx_t_354 += __pyx_pybuffernd_bot.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_353, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_354, __pyx_pybuffernd_bot.diminfo[1].strides) += (*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_350, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_351, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_352, __pyx_pybuffernd_probZ.diminfo[2].strides));
       }
     }
 
-    /* "fastphase/fastphase.pyx":1132
+    /* "fastphase/fastphase.pyx":1124
  *                 bot[m,k]+=probZ[m,k1,k]
  *         # ## top
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             for k1 in range(nK):
  *                 t1=theta[m,k]*(1-theta[m,k1])
  */
-    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1132, __pyx_L1_error)
+    __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1124, __pyx_L1_error)
     __pyx_t_14 = __pyx_t_13;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
       __pyx_v_k = __pyx_t_15;
 
-      /* "fastphase/fastphase.pyx":1133
+      /* "fastphase/fastphase.pyx":1125
  *         # ## top
  *         for k in range(nK):
  *             for k1 in range(nK):             # <<<<<<<<<<<<<<
  *                 t1=theta[m,k]*(1-theta[m,k1])
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  */
-      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1133, __pyx_L1_error)
+      __pyx_t_20 = __Pyx_PyInt_As_long(__pyx_v_nK); if (unlikely((__pyx_t_20 == (long)-1) && PyErr_Occurred())) __PYX_ERR(0, 1125, __pyx_L1_error)
       __pyx_t_53 = __pyx_t_20;
       for (__pyx_t_21 = 0; __pyx_t_21 < __pyx_t_53; __pyx_t_21+=1) {
         __pyx_v_k1 = __pyx_t_21;
 
-        /* "fastphase/fastphase.pyx":1134
+        /* "fastphase/fastphase.pyx":1126
  *         for k in range(nK):
  *             for k1 in range(nK):
  *                 t1=theta[m,k]*(1-theta[m,k1])             # <<<<<<<<<<<<<<
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  */
         __pyx_t_355 = __pyx_v_m;
@@ -25991,15 +25697,15 @@
         if (__pyx_t_356 < 0) __pyx_t_356 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_357 = __pyx_v_m;
         __pyx_t_358 = __pyx_v_k1;
         if (__pyx_t_357 < 0) __pyx_t_357 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_358 < 0) __pyx_t_358 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_v_t1 = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_355, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_356, __pyx_pybuffernd_theta.diminfo[1].strides)) * (1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_357, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_358, __pyx_pybuffernd_theta.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1135
+        /* "fastphase/fastphase.pyx":1127
  *             for k1 in range(nK):
  *                 t1=theta[m,k]*(1-theta[m,k1])
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])             # <<<<<<<<<<<<<<
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):
  */
         __pyx_t_359 = __pyx_v_m;
@@ -26008,75 +25714,75 @@
         if (__pyx_t_360 < 0) __pyx_t_360 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_t_361 = __pyx_v_m;
         __pyx_t_362 = __pyx_v_k;
         if (__pyx_t_361 < 0) __pyx_t_361 += __pyx_pybuffernd_theta.diminfo[0].shape;
         if (__pyx_t_362 < 0) __pyx_t_362 += __pyx_pybuffernd_theta.diminfo[1].shape;
         __pyx_v_t2 = (__pyx_v_t1 + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_359, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_360, __pyx_pybuffernd_theta.diminfo[1].strides)) * (1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_361, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_362, __pyx_pybuffernd_theta.diminfo[1].strides)))));
 
-        /* "fastphase/fastphase.pyx":1136
+        /* "fastphase/fastphase.pyx":1128
  *                 t1=theta[m,k]*(1-theta[m,k1])
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])             # <<<<<<<<<<<<<<
  *                 if (k == k1):
  *                     top[m,k] += 2*temp
  */
         __pyx_t_363 = __pyx_v_m;
         __pyx_t_364 = __pyx_v_k;
         __pyx_t_365 = __pyx_v_k1;
         if (__pyx_t_363 < 0) __pyx_t_363 += __pyx_pybuffernd_probZ.diminfo[0].shape;
         if (__pyx_t_364 < 0) __pyx_t_364 += __pyx_pybuffernd_probZ.diminfo[1].shape;
         if (__pyx_t_365 < 0) __pyx_t_365 += __pyx_pybuffernd_probZ.diminfo[2].shape;
         if (unlikely(__pyx_v_t2 == 0)) {
           PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-          __PYX_ERR(0, 1136, __pyx_L1_error)
+          __PYX_ERR(0, 1128, __pyx_L1_error)
         }
         __pyx_t_366 = __pyx_v_m;
         __pyx_t_367 = 1;
         if (__pyx_t_366 < 0) __pyx_t_366 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
         if (__pyx_t_367 < 0) __pyx_t_367 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
         __pyx_t_368 = __pyx_v_m;
         __pyx_t_369 = 2;
         if (__pyx_t_368 < 0) __pyx_t_368 += __pyx_pybuffernd_p_g_givX.diminfo[0].shape;
         if (__pyx_t_369 < 0) __pyx_t_369 += __pyx_pybuffernd_p_g_givX.diminfo[1].shape;
         __pyx_v_temp = ((*__Pyx_BufPtrStrided3d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_363, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_364, __pyx_pybuffernd_probZ.diminfo[1].strides, __pyx_t_365, __pyx_pybuffernd_probZ.diminfo[2].strides)) * (((__pyx_v_t1 / __pyx_v_t2) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_366, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_367, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))) + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_p_g_givX.rcbuffer->pybuffer.buf, __pyx_t_368, __pyx_pybuffernd_p_g_givX.diminfo[0].strides, __pyx_t_369, __pyx_pybuffernd_p_g_givX.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1137
+        /* "fastphase/fastphase.pyx":1129
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):             # <<<<<<<<<<<<<<
  *                     top[m,k] += 2*temp
  *                 else:
  */
         __pyx_t_66 = ((__pyx_v_k == __pyx_v_k1) != 0);
         if (__pyx_t_66) {
 
-          /* "fastphase/fastphase.pyx":1138
+          /* "fastphase/fastphase.pyx":1130
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):
  *                     top[m,k] += 2*temp             # <<<<<<<<<<<<<<
  *                 else:
  *                     top[m,k] += temp
  */
           __pyx_t_370 = __pyx_v_m;
           __pyx_t_371 = __pyx_v_k;
           if (__pyx_t_370 < 0) __pyx_t_370 += __pyx_pybuffernd_top.diminfo[0].shape;
           if (__pyx_t_371 < 0) __pyx_t_371 += __pyx_pybuffernd_top.diminfo[1].shape;
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_top.rcbuffer->pybuffer.buf, __pyx_t_370, __pyx_pybuffernd_top.diminfo[0].strides, __pyx_t_371, __pyx_pybuffernd_top.diminfo[1].strides) += (2.0 * __pyx_v_temp);
 
-          /* "fastphase/fastphase.pyx":1137
+          /* "fastphase/fastphase.pyx":1129
  *                 t2=t1+theta[m,k1]*(1-theta[m,k])
  *                 temp = probZ[m,k,k1]*((t1/t2)*p_g_givX[m,1] + p_g_givX[m,2])
  *                 if (k == k1):             # <<<<<<<<<<<<<<
  *                     top[m,k] += 2*temp
  *                 else:
  */
           goto __pyx_L97;
         }
 
-        /* "fastphase/fastphase.pyx":1140
+        /* "fastphase/fastphase.pyx":1132
  *                     top[m,k] += 2*temp
  *                 else:
  *                     top[m,k] += temp             # <<<<<<<<<<<<<<
  *     return logLikelihood,top,bot,jmk
  * 
  */
         /*else*/ {
@@ -26087,44 +25793,44 @@
           *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_top.rcbuffer->pybuffer.buf, __pyx_t_372, __pyx_pybuffernd_top.diminfo[0].strides, __pyx_t_373, __pyx_pybuffernd_top.diminfo[1].strides) += __pyx_v_temp;
         }
         __pyx_L97:;
       }
     }
   }
 
-  /* "fastphase/fastphase.pyx":1141
+  /* "fastphase/fastphase.pyx":1133
  *                 else:
  *                     top[m,k] += temp
  *     return logLikelihood,top,bot,jmk             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1141, __pyx_L1_error)
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1141, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
   __Pyx_INCREF(((PyObject *)__pyx_v_top));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_top));
-  PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_top));
+  PyTuple_SET_ITEM(__pyx_t_5, 1, ((PyObject *)__pyx_v_top));
   __Pyx_INCREF(((PyObject *)__pyx_v_bot));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_bot));
-  PyTuple_SET_ITEM(__pyx_t_4, 2, ((PyObject *)__pyx_v_bot));
+  PyTuple_SET_ITEM(__pyx_t_5, 2, ((PyObject *)__pyx_v_bot));
   __Pyx_INCREF(((PyObject *)__pyx_v_jmk));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_jmk));
-  PyTuple_SET_ITEM(__pyx_t_4, 3, ((PyObject *)__pyx_v_jmk));
+  PyTuple_SET_ITEM(__pyx_t_5, 3, ((PyObject *)__pyx_v_jmk));
+  __pyx_t_6 = 0;
+  __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
-  __pyx_r = __pyx_t_4;
-  __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "fastphase/fastphase.pyx":922
- *     return rez
+  /* "fastphase/fastphase.pyx":914
+ *     return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
  * 
  * cpdef likCalc(aa,tt,rr,ll,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
  */
 
   /* function exit code */
@@ -26234,37 +25940,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aa)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 1); __PYX_ERR(0, 922, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 1); __PYX_ERR(0, 914, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 2); __PYX_ERR(0, 922, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 2); __PYX_ERR(0, 914, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ll)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 3); __PYX_ERR(0, 922, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 3); __PYX_ERR(0, 914, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u2p)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 4); __PYX_ERR(0, 922, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, 4); __PYX_ERR(0, 914, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "likCalc") < 0)) __PYX_ERR(0, 922, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "likCalc") < 0)) __PYX_ERR(0, 914, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -26275,15 +25981,15 @@
     __pyx_v_tt = values[1];
     __pyx_v_rr = values[2];
     __pyx_v_ll = values[3];
     __pyx_v_u2p = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 922, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("likCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 914, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastphase.fastphase.likCalc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9fastphase_9fastphase_20likCalc(__pyx_self, __pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_ll, __pyx_v_u2p);
 
@@ -26294,15 +26000,15 @@
 
 static PyObject *__pyx_pf_9fastphase_9fastphase_20likCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_aa, PyObject *__pyx_v_tt, PyObject *__pyx_v_rr, PyObject *__pyx_v_ll, PyObject *__pyx_v_u2p) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("likCalc", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9fastphase_9fastphase_likCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_ll, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 922, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9fastphase_9fastphase_likCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_ll, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 914, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -26311,104 +26017,104 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/fastphase.pyx":1146
+/* "fastphase/fastphase.pyx":1138
  * #### Haplotype Calculations
  * 
  * cdef double happrG(double t,int s):             # <<<<<<<<<<<<<<
  *     if s==0:
  *         return 1-t
  */
 
 static double __pyx_f_9fastphase_9fastphase_happrG(double __pyx_v_t, int __pyx_v_s) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("happrG", 0);
 
-  /* "fastphase/fastphase.pyx":1147
+  /* "fastphase/fastphase.pyx":1139
  * 
  * cdef double happrG(double t,int s):
  *     if s==0:             # <<<<<<<<<<<<<<
  *         return 1-t
  *     elif s==1:
  */
   switch (__pyx_v_s) {
     case 0:
 
-    /* "fastphase/fastphase.pyx":1148
+    /* "fastphase/fastphase.pyx":1140
  * cdef double happrG(double t,int s):
  *     if s==0:
  *         return 1-t             # <<<<<<<<<<<<<<
  *     elif s==1:
  *         return t
  */
     __pyx_r = (1.0 - __pyx_v_t);
     goto __pyx_L0;
 
-    /* "fastphase/fastphase.pyx":1147
+    /* "fastphase/fastphase.pyx":1139
  * 
  * cdef double happrG(double t,int s):
  *     if s==0:             # <<<<<<<<<<<<<<
  *         return 1-t
  *     elif s==1:
  */
     break;
     case 1:
 
-    /* "fastphase/fastphase.pyx":1150
+    /* "fastphase/fastphase.pyx":1142
  *         return 1-t
  *     elif s==1:
  *         return t             # <<<<<<<<<<<<<<
  *     else:
  *         return 1
  */
     __pyx_r = __pyx_v_t;
     goto __pyx_L0;
 
-    /* "fastphase/fastphase.pyx":1149
+    /* "fastphase/fastphase.pyx":1141
  *     if s==0:
  *         return 1-t
  *     elif s==1:             # <<<<<<<<<<<<<<
  *         return t
  *     else:
  */
     break;
     default:
 
-    /* "fastphase/fastphase.pyx":1152
+    /* "fastphase/fastphase.pyx":1144
  *         return t
  *     else:
  *         return 1             # <<<<<<<<<<<<<<
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):
  */
     __pyx_r = 1.0;
     goto __pyx_L0;
     break;
   }
 
-  /* "fastphase/fastphase.pyx":1146
+  /* "fastphase/fastphase.pyx":1138
  * #### Haplotype Calculations
  * 
  * cdef double happrG(double t,int s):             # <<<<<<<<<<<<<<
  *     if s==0:
  *         return 1-t
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/fastphase.pyx":1154
+/* "fastphase/fastphase.pyx":1146
  *         return 1
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -26531,337 +26237,337 @@
   __pyx_pybuffernd_soluce.data = NULL;
   __pyx_pybuffernd_soluce.rcbuffer = &__pyx_pybuffer_soluce;
   __pyx_pybuffer_tempVal.pybuffer.buf = NULL;
   __pyx_pybuffer_tempVal.refcount = 0;
   __pyx_pybuffernd_tempVal.data = NULL;
   __pyx_pybuffernd_tempVal.rcbuffer = &__pyx_pybuffer_tempVal;
 
-  /* "fastphase/fastphase.pyx":1155
+  /* "fastphase/fastphase.pyx":1147
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  */
-  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1155, __pyx_L1_error)
+  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1147, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_aa;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alpha.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_alpha = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1155, __pyx_L1_error)
+      __PYX_ERR(0, 1147, __pyx_L1_error)
     } else {__pyx_pybuffernd_alpha.diminfo[0].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alpha.diminfo[0].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_alpha.diminfo[1].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_alpha.diminfo[1].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_alpha = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1156
+  /* "fastphase/fastphase.pyx":1148
  * cpdef hapViterbi( aa, tt, rr, hh):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  */
-  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1156, __pyx_L1_error)
+  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1148, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_tt;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_theta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1156, __pyx_L1_error)
+      __PYX_ERR(0, 1148, __pyx_L1_error)
     } else {__pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_theta = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1157
+  /* "fastphase/fastphase.pyx":1149
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  * 
  */
-  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1157, __pyx_L1_error)
+  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1149, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_rr;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rho.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_rho = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1157, __pyx_L1_error)
+      __PYX_ERR(0, 1149, __pyx_L1_error)
     } else {__pyx_pybuffernd_rho.diminfo[0].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rho.diminfo[0].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_rho.diminfo[1].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_rho.diminfo[1].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_rho = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1158
+  /* "fastphase/fastphase.pyx":1150
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh             # <<<<<<<<<<<<<<
  * 
  *     ## cython declarations
  */
-  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1158, __pyx_L1_error)
+  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1150, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_hh;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_hap.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_hap = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1158, __pyx_L1_error)
+      __PYX_ERR(0, 1150, __pyx_L1_error)
     } else {__pyx_pybuffernd_hap.diminfo[0].strides = __pyx_pybuffernd_hap.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_hap.diminfo[0].shape = __pyx_pybuffernd_hap.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_v_hap = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1164
+  /* "fastphase/fastphase.pyx":1156
  *     cdef int k, prev_k, best_k, m
  *     cdef double best_v
  *     nLoc = alpha.shape[0]             # <<<<<<<<<<<<<<
  *     nK = alpha.shape[1]
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  */
   __pyx_v_nLoc = (__pyx_v_alpha->dimensions[0]);
 
-  /* "fastphase/fastphase.pyx":1165
+  /* "fastphase/fastphase.pyx":1157
  *     cdef double best_v
  *     nLoc = alpha.shape[0]
  *     nK = alpha.shape[1]             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  */
   __pyx_v_nK = (__pyx_v_alpha->dimensions[1]);
 
-  /* "fastphase/fastphase.pyx":1166
+  /* "fastphase/fastphase.pyx":1158
  *     nLoc = alpha.shape[0]
  *     nK = alpha.shape[1]
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1166, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1166, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1166, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1158, __pyx_L1_error)
   __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_delta.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_delta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1166, __pyx_L1_error)
+      __PYX_ERR(0, 1158, __pyx_L1_error)
     } else {__pyx_pybuffernd_delta.diminfo[0].strides = __pyx_pybuffernd_delta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_delta.diminfo[0].shape = __pyx_pybuffernd_delta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_delta.diminfo[1].strides = __pyx_pybuffernd_delta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_delta.diminfo[1].shape = __pyx_pybuffernd_delta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_6 = 0;
   __pyx_v_delta = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":1167
+  /* "fastphase/fastphase.pyx":1159
  *     nK = alpha.shape[1]
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)
  *     cdef np.ndarray[ np.float64_t, ndim = 1] tempVal = np.zeros( nK, dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_5 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1167, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1167, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1167, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1159, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_psi.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_psi = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_psi.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1167, __pyx_L1_error)
+      __PYX_ERR(0, 1159, __pyx_L1_error)
     } else {__pyx_pybuffernd_psi.diminfo[0].strides = __pyx_pybuffernd_psi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_psi.diminfo[0].shape = __pyx_pybuffernd_psi.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_psi.diminfo[1].strides = __pyx_pybuffernd_psi.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_psi.diminfo[1].shape = __pyx_pybuffernd_psi.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_psi = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1168
+  /* "fastphase/fastphase.pyx":1160
  *     cdef np.ndarray[ np.float64_t, ndim = 2 ] delta = np.zeros((nK, nLoc), dtype=np.float64)
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[ np.float64_t, ndim = 1] tempVal = np.zeros( nK, dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1168, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1168, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1168, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1160, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_soluce.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_soluce = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_soluce.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1168, __pyx_L1_error)
+      __PYX_ERR(0, 1160, __pyx_L1_error)
     } else {__pyx_pybuffernd_soluce.diminfo[0].strides = __pyx_pybuffernd_soluce.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_soluce.diminfo[0].shape = __pyx_pybuffernd_soluce.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_soluce = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":1169
+  /* "fastphase/fastphase.pyx":1161
  *     cdef np.ndarray[ np.int_t, ndim = 2 ] psi = np.zeros((nK, nLoc), dtype=np.int)
  *     cdef np.ndarray[ np.int_t, ndim = 1] soluce = np.empty(nLoc, dtype= np.int)
  *     cdef np.ndarray[ np.float64_t, ndim = 1] tempVal = np.zeros( nK, dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     ## initialization
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float64); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 1169, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1169, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1161, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1169, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1161, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_4);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tempVal.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_tempVal = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1169, __pyx_L1_error)
+      __PYX_ERR(0, 1161, __pyx_L1_error)
     } else {__pyx_pybuffernd_tempVal.diminfo[0].strides = __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tempVal.diminfo[0].shape = __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_tempVal = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "fastphase/fastphase.pyx":1172
+  /* "fastphase/fastphase.pyx":1164
  * 
  *     ## initialization
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         delta[k,0] = log(alpha[ 0, k]) + log(happrG( theta[ 0, k], hap[0]))
  * 
  */
   __pyx_t_10 = __pyx_v_nK;
   __pyx_t_11 = __pyx_t_10;
   for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_k = __pyx_t_12;
 
-    /* "fastphase/fastphase.pyx":1173
+    /* "fastphase/fastphase.pyx":1165
  *     ## initialization
  *     for k in range(nK):
  *         delta[k,0] = log(alpha[ 0, k]) + log(happrG( theta[ 0, k], hap[0]))             # <<<<<<<<<<<<<<
  * 
  *     ## recursion
  */
     __pyx_t_13 = 0;
@@ -26877,51 +26583,51 @@
     __pyx_t_18 = __pyx_v_k;
     __pyx_t_19 = 0;
     if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_delta.diminfo[0].shape;
     if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_delta.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf, __pyx_t_18, __pyx_pybuffernd_delta.diminfo[0].strides, __pyx_t_19, __pyx_pybuffernd_delta.diminfo[1].strides) = (log((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_13, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_14, __pyx_pybuffernd_alpha.diminfo[1].strides))) + log(__pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_hap.diminfo[0].strides)))));
   }
 
-  /* "fastphase/fastphase.pyx":1176
+  /* "fastphase/fastphase.pyx":1168
  * 
  *     ## recursion
  *     for m in range(1, nLoc):             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             for prev_k in range(nK):
  */
   __pyx_t_10 = __pyx_v_nLoc;
   __pyx_t_11 = __pyx_t_10;
   for (__pyx_t_12 = 1; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_m = __pyx_t_12;
 
-    /* "fastphase/fastphase.pyx":1177
+    /* "fastphase/fastphase.pyx":1169
  *     ## recursion
  *     for m in range(1, nLoc):
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             for prev_k in range(nK):
  *                 ## jump
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_21 = __pyx_t_20;
     for (__pyx_t_22 = 0; __pyx_t_22 < __pyx_t_21; __pyx_t_22+=1) {
       __pyx_v_k = __pyx_t_22;
 
-      /* "fastphase/fastphase.pyx":1178
+      /* "fastphase/fastphase.pyx":1170
  *     for m in range(1, nLoc):
  *         for k in range(nK):
  *             for prev_k in range(nK):             # <<<<<<<<<<<<<<
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])
  */
       __pyx_t_23 = __pyx_v_nK;
       __pyx_t_24 = __pyx_t_23;
       for (__pyx_t_25 = 0; __pyx_t_25 < __pyx_t_24; __pyx_t_25+=1) {
         __pyx_v_prev_k = __pyx_t_25;
 
-        /* "fastphase/fastphase.pyx":1180
+        /* "fastphase/fastphase.pyx":1172
  *             for prev_k in range(nK):
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])             # <<<<<<<<<<<<<<
  *                 if k == prev_k:
  *                     ## no jump
  */
         __pyx_t_26 = __pyx_v_m;
@@ -26932,25 +26638,25 @@
         __pyx_t_29 = __pyx_v_k;
         if (__pyx_t_28 < 0) __pyx_t_28 += __pyx_pybuffernd_alpha.diminfo[0].shape;
         if (__pyx_t_29 < 0) __pyx_t_29 += __pyx_pybuffernd_alpha.diminfo[1].shape;
         __pyx_t_30 = __pyx_v_prev_k;
         if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_pybuffernd_tempVal.diminfo[0].shape;
         *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_tempVal.diminfo[0].strides) = (log((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_rho.diminfo[1].strides))) + log((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_alpha.diminfo[1].strides))));
 
-        /* "fastphase/fastphase.pyx":1181
+        /* "fastphase/fastphase.pyx":1173
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])
  *                 if k == prev_k:             # <<<<<<<<<<<<<<
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  */
         __pyx_t_31 = ((__pyx_v_k == __pyx_v_prev_k) != 0);
         if (__pyx_t_31) {
 
-          /* "fastphase/fastphase.pyx":1183
+          /* "fastphase/fastphase.pyx":1175
  *                 if k == prev_k:
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))             # <<<<<<<<<<<<<<
  *                 tempVal[ prev_k] +=  delta[prev_k, m-1]
  *                 psi[ k, m] = argmax(tempVal, nK)
  */
           __pyx_t_32 = __pyx_v_m;
@@ -26965,52 +26671,52 @@
           __pyx_t_37 = 0;
           if (__pyx_t_36 < 0) __pyx_t_36 += __pyx_pybuffernd_rho.diminfo[0].shape;
           if (__pyx_t_37 < 0) __pyx_t_37 += __pyx_pybuffernd_rho.diminfo[1].shape;
           __pyx_t_38 = __pyx_v_prev_k;
           if (__pyx_t_38 < 0) __pyx_t_38 += __pyx_pybuffernd_tempVal.diminfo[0].shape;
           *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_tempVal.diminfo[0].strides) = log((((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_32, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_33, __pyx_pybuffernd_rho.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_34, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_35, __pyx_pybuffernd_alpha.diminfo[1].strides))) + (1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_rho.diminfo[1].strides)))));
 
-          /* "fastphase/fastphase.pyx":1181
+          /* "fastphase/fastphase.pyx":1173
  *                 ## jump
  *                 tempVal[ prev_k] = log(rho[ m, 0])+log( alpha[ m, k])
  *                 if k == prev_k:             # <<<<<<<<<<<<<<
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  */
         }
 
-        /* "fastphase/fastphase.pyx":1184
+        /* "fastphase/fastphase.pyx":1176
  *                     ## no jump
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  *                 tempVal[ prev_k] +=  delta[prev_k, m-1]             # <<<<<<<<<<<<<<
  *                 psi[ k, m] = argmax(tempVal, nK)
  *                 delta[ k, m] = tempVal[ psi[ k, m]] +log( happrG( theta[ m, k], hap[ m]))
  */
         __pyx_t_39 = __pyx_v_prev_k;
         __pyx_t_40 = (__pyx_v_m - 1);
         if (__pyx_t_39 < 0) __pyx_t_39 += __pyx_pybuffernd_delta.diminfo[0].shape;
         if (__pyx_t_40 < 0) __pyx_t_40 += __pyx_pybuffernd_delta.diminfo[1].shape;
         __pyx_t_41 = __pyx_v_prev_k;
         if (__pyx_t_41 < 0) __pyx_t_41 += __pyx_pybuffernd_tempVal.diminfo[0].shape;
         *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_41, __pyx_pybuffernd_tempVal.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf, __pyx_t_39, __pyx_pybuffernd_delta.diminfo[0].strides, __pyx_t_40, __pyx_pybuffernd_delta.diminfo[1].strides));
 
-        /* "fastphase/fastphase.pyx":1185
+        /* "fastphase/fastphase.pyx":1177
  *                     tempVal[ prev_k] = log( rho[ m, 0]*alpha[ m, k] + (1 - rho[ m, 0]))
  *                 tempVal[ prev_k] +=  delta[prev_k, m-1]
  *                 psi[ k, m] = argmax(tempVal, nK)             # <<<<<<<<<<<<<<
  *                 delta[ k, m] = tempVal[ psi[ k, m]] +log( happrG( theta[ m, k], hap[ m]))
  * 
  */
         __pyx_t_42 = __pyx_v_k;
         __pyx_t_43 = __pyx_v_m;
         if (__pyx_t_42 < 0) __pyx_t_42 += __pyx_pybuffernd_psi.diminfo[0].shape;
         if (__pyx_t_43 < 0) __pyx_t_43 += __pyx_pybuffernd_psi.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_psi.rcbuffer->pybuffer.buf, __pyx_t_42, __pyx_pybuffernd_psi.diminfo[0].strides, __pyx_t_43, __pyx_pybuffernd_psi.diminfo[1].strides) = __pyx_f_9fastphase_9fastphase_argmax(((PyArrayObject *)__pyx_v_tempVal), __pyx_v_nK);
 
-        /* "fastphase/fastphase.pyx":1186
+        /* "fastphase/fastphase.pyx":1178
  *                 tempVal[ prev_k] +=  delta[prev_k, m-1]
  *                 psi[ k, m] = argmax(tempVal, nK)
  *                 delta[ k, m] = tempVal[ psi[ k, m]] +log( happrG( theta[ m, k], hap[ m]))             # <<<<<<<<<<<<<<
  * 
  *     ## termination
  */
         __pyx_t_44 = __pyx_v_k;
@@ -27030,51 +26736,51 @@
         if (__pyx_t_50 < 0) __pyx_t_50 += __pyx_pybuffernd_delta.diminfo[0].shape;
         if (__pyx_t_51 < 0) __pyx_t_51 += __pyx_pybuffernd_delta.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_delta.rcbuffer->pybuffer.buf, __pyx_t_50, __pyx_pybuffernd_delta.diminfo[0].strides, __pyx_t_51, __pyx_pybuffernd_delta.diminfo[1].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tempVal.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_tempVal.diminfo[0].strides)) + log(__pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_47, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_48, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_49, __pyx_pybuffernd_hap.diminfo[0].strides)))));
       }
     }
   }
 
-  /* "fastphase/fastphase.pyx":1189
+  /* "fastphase/fastphase.pyx":1181
  * 
  *     ## termination
  *     soluce[ nLoc - 1 ] = argmax( delta[ :, nLoc-1], nK)             # <<<<<<<<<<<<<<
  *     for m in range( nLoc - 2, -1, -1):
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]
  */
-  __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_nLoc - 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_long((__pyx_v_nLoc - 1)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_slice__9);
   __Pyx_GIVEREF(__pyx_slice__9);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_slice__9);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_delta), __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1189, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_delta), __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1189, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1181, __pyx_L1_error)
   __pyx_t_52 = (__pyx_v_nLoc - 1);
   if (__pyx_t_52 < 0) __pyx_t_52 += __pyx_pybuffernd_soluce.diminfo[0].shape;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_soluce.rcbuffer->pybuffer.buf, __pyx_t_52, __pyx_pybuffernd_soluce.diminfo[0].strides) = __pyx_f_9fastphase_9fastphase_argmax(((PyArrayObject *)__pyx_t_4), __pyx_v_nK);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "fastphase/fastphase.pyx":1190
+  /* "fastphase/fastphase.pyx":1182
  *     ## termination
  *     soluce[ nLoc - 1 ] = argmax( delta[ :, nLoc-1], nK)
  *     for m in range( nLoc - 2, -1, -1):             # <<<<<<<<<<<<<<
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]
  *     return soluce
  */
   for (__pyx_t_10 = (__pyx_v_nLoc - 2); __pyx_t_10 > -1; __pyx_t_10-=1) {
     __pyx_v_m = __pyx_t_10;
 
-    /* "fastphase/fastphase.pyx":1191
+    /* "fastphase/fastphase.pyx":1183
  *     soluce[ nLoc - 1 ] = argmax( delta[ :, nLoc-1], nK)
  *     for m in range( nLoc - 2, -1, -1):
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]             # <<<<<<<<<<<<<<
  *     return soluce
  * 
  */
     __pyx_t_53 = (__pyx_v_m + 1);
@@ -27084,27 +26790,27 @@
     if (__pyx_t_54 < 0) __pyx_t_54 += __pyx_pybuffernd_psi.diminfo[0].shape;
     if (__pyx_t_55 < 0) __pyx_t_55 += __pyx_pybuffernd_psi.diminfo[1].shape;
     __pyx_t_56 = __pyx_v_m;
     if (__pyx_t_56 < 0) __pyx_t_56 += __pyx_pybuffernd_soluce.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_soluce.rcbuffer->pybuffer.buf, __pyx_t_56, __pyx_pybuffernd_soluce.diminfo[0].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_psi.rcbuffer->pybuffer.buf, __pyx_t_54, __pyx_pybuffernd_psi.diminfo[0].strides, __pyx_t_55, __pyx_pybuffernd_psi.diminfo[1].strides));
   }
 
-  /* "fastphase/fastphase.pyx":1192
+  /* "fastphase/fastphase.pyx":1184
  *     for m in range( nLoc - 2, -1, -1):
  *         soluce[ m ] = psi[ soluce[ m+1 ], m+1]
  *     return soluce             # <<<<<<<<<<<<<<
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_soluce));
   __pyx_r = ((PyObject *)__pyx_v_soluce);
   goto __pyx_L0;
 
-  /* "fastphase/fastphase.pyx":1154
+  /* "fastphase/fastphase.pyx":1146
  *         return 1
  * 
  * cpdef hapViterbi( aa, tt, rr, hh):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -27187,31 +26893,31 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aa)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 1); __PYX_ERR(0, 1154, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 1); __PYX_ERR(0, 1146, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 2); __PYX_ERR(0, 1154, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 2); __PYX_ERR(0, 1146, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hh)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 3); __PYX_ERR(0, 1154, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, 3); __PYX_ERR(0, 1146, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapViterbi") < 0)) __PYX_ERR(0, 1154, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapViterbi") < 0)) __PYX_ERR(0, 1146, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -27220,15 +26926,15 @@
     __pyx_v_aa = values[0];
     __pyx_v_tt = values[1];
     __pyx_v_rr = values[2];
     __pyx_v_hh = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1154, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("hapViterbi", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1146, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastphase.fastphase.hapViterbi", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9fastphase_9fastphase_22hapViterbi(__pyx_self, __pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh);
 
@@ -27239,15 +26945,15 @@
 
 static PyObject *__pyx_pf_9fastphase_9fastphase_22hapViterbi(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_aa, PyObject *__pyx_v_tt, PyObject *__pyx_v_rr, PyObject *__pyx_v_hh) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("hapViterbi", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9fastphase_9fastphase_hapViterbi(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1154, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9fastphase_9fastphase_hapViterbi(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -27256,15 +26962,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "fastphase/fastphase.pyx":1194
+/* "fastphase/fastphase.pyx":1186
  *     return soluce
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -27516,316 +27222,316 @@
   __pyx_pybuffernd_top.data = NULL;
   __pyx_pybuffernd_top.rcbuffer = &__pyx_pybuffer_top;
   __pyx_pybuffer_bot.pybuffer.buf = NULL;
   __pyx_pybuffer_bot.refcount = 0;
   __pyx_pybuffernd_bot.data = NULL;
   __pyx_pybuffernd_bot.rcbuffer = &__pyx_pybuffer_bot;
 
-  /* "fastphase/fastphase.pyx":1195
+  /* "fastphase/fastphase.pyx":1187
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  */
-  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1195, __pyx_L1_error)
+  if (!(likely(((__pyx_v_aa) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_aa, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1187, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_aa;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alpha.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_alpha = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1195, __pyx_L1_error)
+      __PYX_ERR(0, 1187, __pyx_L1_error)
     } else {__pyx_pybuffernd_alpha.diminfo[0].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alpha.diminfo[0].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_alpha.diminfo[1].strides = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_alpha.diminfo[1].shape = __pyx_pybuffernd_alpha.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_alpha = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1196
+  /* "fastphase/fastphase.pyx":1188
  * cpdef hapCalc(aa,tt,rr,hh,u2p):
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  */
-  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1196, __pyx_L1_error)
+  if (!(likely(((__pyx_v_tt) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_tt, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1188, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_tt;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_theta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1196, __pyx_L1_error)
+      __PYX_ERR(0, 1188, __pyx_L1_error)
     } else {__pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_theta = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1197
+  /* "fastphase/fastphase.pyx":1189
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  *     cdef int up2pz=u2p
  */
-  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1197, __pyx_L1_error)
+  if (!(likely(((__pyx_v_rr) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_rr, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1189, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_rr;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_rho.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_rho = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1197, __pyx_L1_error)
+      __PYX_ERR(0, 1189, __pyx_L1_error)
     } else {__pyx_pybuffernd_rho.diminfo[0].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_rho.diminfo[0].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_rho.diminfo[1].strides = __pyx_pybuffernd_rho.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_rho.diminfo[1].shape = __pyx_pybuffernd_rho.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_v_rho = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1198
+  /* "fastphase/fastphase.pyx":1190
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh             # <<<<<<<<<<<<<<
  *     cdef int up2pz=u2p
  *     ## cython declarations
  */
-  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1198, __pyx_L1_error)
+  if (!(likely(((__pyx_v_hh) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_hh, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1190, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_hh;
   __Pyx_INCREF(__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_hap.rcbuffer->pybuffer, (PyObject*)((PyArrayObject *)__pyx_t_1), &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_hap = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1198, __pyx_L1_error)
+      __PYX_ERR(0, 1190, __pyx_L1_error)
     } else {__pyx_pybuffernd_hap.diminfo[0].strides = __pyx_pybuffernd_hap.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_hap.diminfo[0].shape = __pyx_pybuffernd_hap.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_v_hap = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1199
+  /* "fastphase/fastphase.pyx":1191
  *     cdef np.ndarray[np.float64_t, ndim=2] rho = rr
  *     cdef np.ndarray[np.int_t, ndim=1] hap = hh
  *     cdef int up2pz=u2p             # <<<<<<<<<<<<<<
  *     ## cython declarations
  *     cdef int nLoc,nK,tScale
  */
-  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_u2p); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 1191, __pyx_L1_error)
   __pyx_v_up2pz = __pyx_t_2;
 
-  /* "fastphase/fastphase.pyx":1207
+  /* "fastphase/fastphase.pyx":1199
  *     cdef double logLikelihood
  *     ## end cython declarations
  *     nLoc=alpha.shape[0]             # <<<<<<<<<<<<<<
  *     nK=alpha.shape[1]
  *     ##
  */
   __pyx_v_nLoc = (__pyx_v_alpha->dimensions[0]);
 
-  /* "fastphase/fastphase.pyx":1208
+  /* "fastphase/fastphase.pyx":1200
  *     ## end cython declarations
  *     nLoc=alpha.shape[0]
  *     nK=alpha.shape[1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute backward probabilities
  */
   __pyx_v_nK = (__pyx_v_alpha->dimensions[1]);
 
-  /* "fastphase/fastphase.pyx":1212
+  /* "fastphase/fastphase.pyx":1204
  *     ## compute backward probabilities
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=1] tSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_int); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 1212, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1212, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1212, __pyx_L1_error)
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1204, __pyx_L1_error)
   __pyx_t_7 = ((PyArrayObject *)__pyx_t_6);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_betaScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_7, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_betaScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1212, __pyx_L1_error)
+      __PYX_ERR(0, 1204, __pyx_L1_error)
     } else {__pyx_pybuffernd_betaScale.diminfo[0].strides = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_betaScale.diminfo[0].shape = __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_7 = 0;
   __pyx_v_betaScale = ((PyArrayObject *)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "fastphase/fastphase.pyx":1213
+  /* "fastphase/fastphase.pyx":1205
  *     ##
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=1] tSum=np.zeros(nLoc,dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1213, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1213, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1205, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1213, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1205, __pyx_L1_error)
   __pyx_t_8 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_tSum.rcbuffer->pybuffer, (PyObject*)__pyx_t_8, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_tSum = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1213, __pyx_L1_error)
+      __PYX_ERR(0, 1205, __pyx_L1_error)
     } else {__pyx_pybuffernd_tSum.diminfo[0].strides = __pyx_pybuffernd_tSum.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_tSum.diminfo[0].shape = __pyx_pybuffernd_tSum.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_8 = 0;
   __pyx_v_tSum = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":1214
+  /* "fastphase/fastphase.pyx":1206
  *     cdef np.ndarray[np.int_t,ndim=1] betaScale=np.zeros(nLoc,dtype=np.int)
  *     cdef np.ndarray[np.float64_t,ndim=1] tSum=np.zeros(nLoc,dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for k in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_5 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1214, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1214, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1206, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1214, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1206, __pyx_L1_error)
   __pyx_t_9 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mBeta.rcbuffer->pybuffer, (PyObject*)__pyx_t_9, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_mBeta = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1214, __pyx_L1_error)
+      __PYX_ERR(0, 1206, __pyx_L1_error)
     } else {__pyx_pybuffernd_mBeta.diminfo[0].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mBeta.diminfo[0].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mBeta.diminfo[1].strides = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mBeta.diminfo[1].shape = __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_9 = 0;
   __pyx_v_mBeta = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/fastphase.pyx":1216
+  /* "fastphase/fastphase.pyx":1208
  *     cdef np.ndarray[np.float64_t,ndim=2] mBeta=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         mBeta[nLoc-1,k]=1
  * 
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1217
+    /* "fastphase/fastphase.pyx":1209
  * 
  *     for k in range(nK):
  *         mBeta[nLoc-1,k]=1             # <<<<<<<<<<<<<<
  * 
  *     for k in range(nK):
  */
     __pyx_t_12 = (__pyx_v_nLoc - 1);
     __pyx_t_13 = __pyx_v_k;
     if (__pyx_t_12 < 0) __pyx_t_12 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
     if (__pyx_t_13 < 0) __pyx_t_13 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_12, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_13, __pyx_pybuffernd_mBeta.diminfo[1].strides) = 1.0;
   }
 
-  /* "fastphase/fastphase.pyx":1219
+  /* "fastphase/fastphase.pyx":1211
  *         mBeta[nLoc-1,k]=1
  * 
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]
  *     for m in range(nLoc-1,0,-1):
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1220
+    /* "fastphase/fastphase.pyx":1212
  * 
  *     for k in range(nK):
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]             # <<<<<<<<<<<<<<
  *     for m in range(nLoc-1,0,-1):
  *         tScaleTemp=0
  */
     __pyx_t_14 = (__pyx_v_nLoc - 1);
@@ -27839,46 +27545,46 @@
     if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_pybuffernd_alpha.diminfo[0].shape;
     if (__pyx_t_18 < 0) __pyx_t_18 += __pyx_pybuffernd_alpha.diminfo[1].shape;
     __pyx_t_19 = (__pyx_v_nLoc - 1);
     if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_19, __pyx_pybuffernd_tSum.diminfo[0].strides) += (__pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_14, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_15, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_16, __pyx_pybuffernd_hap.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_17, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_18, __pyx_pybuffernd_alpha.diminfo[1].strides)));
   }
 
-  /* "fastphase/fastphase.pyx":1221
+  /* "fastphase/fastphase.pyx":1213
  *     for k in range(nK):
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]
  *     for m in range(nLoc-1,0,-1):             # <<<<<<<<<<<<<<
  *         tScaleTemp=0
  *         ## this loop can be parallelized across clusters #CUDA
  */
   for (__pyx_t_2 = (__pyx_v_nLoc - 1); __pyx_t_2 > 0; __pyx_t_2-=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1222
+    /* "fastphase/fastphase.pyx":1214
  *         tSum[nLoc-1] += happrG(theta[nLoc-1,k],hap[nLoc-1])*alpha[nLoc-1,k]
  *     for m in range(nLoc-1,0,-1):
  *         tScaleTemp=0             # <<<<<<<<<<<<<<
  *         ## this loop can be parallelized across clusters #CUDA
  *         for k in range(nK):
  */
     __pyx_v_tScaleTemp = 0.0;
 
-    /* "fastphase/fastphase.pyx":1224
+    /* "fastphase/fastphase.pyx":1216
  *         tScaleTemp=0
  *         ## this loop can be parallelized across clusters #CUDA
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  */
     __pyx_t_10 = __pyx_v_nK;
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
       __pyx_v_k = __pyx_t_20;
 
-      /* "fastphase/fastphase.pyx":1225
+      /* "fastphase/fastphase.pyx":1217
  *         ## this loop can be parallelized across clusters #CUDA
  *         for k in range(nK):
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]             # <<<<<<<<<<<<<<
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]
  */
       __pyx_t_21 = __pyx_v_m;
@@ -27893,15 +27599,15 @@
       if (__pyx_t_25 < 0) __pyx_t_25 += __pyx_pybuffernd_hap.diminfo[0].shape;
       __pyx_t_26 = __pyx_v_m;
       __pyx_t_27 = __pyx_v_k;
       if (__pyx_t_26 < 0) __pyx_t_26 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_27 < 0) __pyx_t_27 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       __pyx_v_temp = (((1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_21, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_22, __pyx_pybuffernd_rho.diminfo[1].strides))) * __pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_23, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_24, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_25, __pyx_pybuffernd_hap.diminfo[0].strides)))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_26, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_27, __pyx_pybuffernd_mBeta.diminfo[1].strides)));
 
-      /* "fastphase/fastphase.pyx":1226
+      /* "fastphase/fastphase.pyx":1218
  *         for k in range(nK):
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]             # <<<<<<<<<<<<<<
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]
  *             tScaleTemp+=mBeta[m-1,k]
  */
       __pyx_t_28 = __pyx_v_m;
@@ -27912,15 +27618,15 @@
       if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_t_31 = (__pyx_v_m - 1);
       __pyx_t_32 = __pyx_v_k;
       if (__pyx_t_31 < 0) __pyx_t_31 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_32 < 0) __pyx_t_32 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_31, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_32, __pyx_pybuffernd_mBeta.diminfo[1].strides) = (__pyx_v_temp + ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_28, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_29, __pyx_pybuffernd_rho.diminfo[1].strides)) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_30, __pyx_pybuffernd_tSum.diminfo[0].strides))));
 
-      /* "fastphase/fastphase.pyx":1227
+      /* "fastphase/fastphase.pyx":1219
  *             temp=(1.0-rho[m,0])*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]             # <<<<<<<<<<<<<<
  *             tScaleTemp+=mBeta[m-1,k]
  *         # if np.isnan(tScaleTemp):
  */
       __pyx_t_33 = (__pyx_v_m - 1);
@@ -27937,267 +27643,267 @@
       __pyx_t_39 = __pyx_v_k;
       if (__pyx_t_38 < 0) __pyx_t_38 += __pyx_pybuffernd_alpha.diminfo[0].shape;
       if (__pyx_t_39 < 0) __pyx_t_39 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_40 = (__pyx_v_m - 1);
       if (__pyx_t_40 < 0) __pyx_t_40 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_40, __pyx_pybuffernd_tSum.diminfo[0].strides) += ((__pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_34, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_hap.diminfo[0].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_36, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_37, __pyx_pybuffernd_mBeta.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_38, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_39, __pyx_pybuffernd_alpha.diminfo[1].strides)));
 
-      /* "fastphase/fastphase.pyx":1228
+      /* "fastphase/fastphase.pyx":1220
  *             mBeta[m-1,k]=temp+rho[m,0]*tSum[m]
  *             tSum[m-1]+=happrG(theta[m-1,k],hap[m-1])*mBeta[m-1,k]*alpha[m-1,k]
  *             tScaleTemp+=mBeta[m-1,k]             # <<<<<<<<<<<<<<
  *         # if np.isnan(tScaleTemp):
  *         #     print mBeta[m-1]
  */
       __pyx_t_41 = (__pyx_v_m - 1);
       __pyx_t_42 = __pyx_v_k;
       if (__pyx_t_41 < 0) __pyx_t_41 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
       if (__pyx_t_42 < 0) __pyx_t_42 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       __pyx_v_tScaleTemp = (__pyx_v_tScaleTemp + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_41, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_42, __pyx_pybuffernd_mBeta.diminfo[1].strides)));
     }
 
-    /* "fastphase/fastphase.pyx":1237
+    /* "fastphase/fastphase.pyx":1229
  *         #     print hap[m]
  *         #     print 'BLA'
  *         tScale=int(-log(tScaleTemp)/log(10))             # <<<<<<<<<<<<<<
  *         if tScale<0:
  *             tScale=0
  */
     __pyx_t_43 = (-log(__pyx_v_tScaleTemp));
     __pyx_t_44 = log(10.0);
     if (unlikely(__pyx_t_44 == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-      __PYX_ERR(0, 1237, __pyx_L1_error)
+      __PYX_ERR(0, 1229, __pyx_L1_error)
     }
     __pyx_v_tScale = ((int)(__pyx_t_43 / __pyx_t_44));
 
-    /* "fastphase/fastphase.pyx":1238
+    /* "fastphase/fastphase.pyx":1230
  *         #     print 'BLA'
  *         tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale<0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     __pyx_t_45 = ((__pyx_v_tScale < 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1239
+      /* "fastphase/fastphase.pyx":1231
  *         tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale<0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/fastphase.pyx":1238
+      /* "fastphase/fastphase.pyx":1230
  *         #     print 'BLA'
  *         tScale=int(-log(tScaleTemp)/log(10))
  *         if tScale<0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  */
     }
 
-    /* "fastphase/fastphase.pyx":1240
+    /* "fastphase/fastphase.pyx":1232
  *         if tScale<0:
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale             # <<<<<<<<<<<<<<
  *         if tScale >0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_46 = __pyx_v_m;
     if (__pyx_t_46 < 0) __pyx_t_46 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     __pyx_t_47 = (__pyx_v_m - 1);
     if (__pyx_t_47 < 0) __pyx_t_47 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_47, __pyx_pybuffernd_betaScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_46, __pyx_pybuffernd_betaScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-    /* "fastphase/fastphase.pyx":1241
+    /* "fastphase/fastphase.pyx":1233
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy
  */
     __pyx_t_45 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1242
+      /* "fastphase/fastphase.pyx":1234
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             tSum[m-1]*=dummy
  *             for k in range(nK):
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/fastphase.pyx":1243
+      /* "fastphase/fastphase.pyx":1235
  *         if tScale >0:
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 mBeta[m-1,k]*=dummy
  */
       __pyx_t_48 = (__pyx_v_m - 1);
       if (__pyx_t_48 < 0) __pyx_t_48 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_48, __pyx_pybuffernd_tSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-      /* "fastphase/fastphase.pyx":1244
+      /* "fastphase/fastphase.pyx":1236
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 mBeta[m-1,k]*=dummy
  *     ##
  */
       __pyx_t_10 = __pyx_v_nK;
       __pyx_t_11 = __pyx_t_10;
       for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
         __pyx_v_k = __pyx_t_20;
 
-        /* "fastphase/fastphase.pyx":1245
+        /* "fastphase/fastphase.pyx":1237
  *             tSum[m-1]*=dummy
  *             for k in range(nK):
  *                 mBeta[m-1,k]*=dummy             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute forward probabilities
  */
         __pyx_t_49 = (__pyx_v_m - 1);
         __pyx_t_50 = __pyx_v_k;
         if (__pyx_t_49 < 0) __pyx_t_49 += __pyx_pybuffernd_mBeta.diminfo[0].shape;
         if (__pyx_t_50 < 0) __pyx_t_50 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_49, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_50, __pyx_pybuffernd_mBeta.diminfo[1].strides) *= __pyx_v_dummy;
       }
 
-      /* "fastphase/fastphase.pyx":1241
+      /* "fastphase/fastphase.pyx":1233
  *             tScale=0
  *         betaScale[m-1]=betaScale[m]+tScale
  *         if tScale >0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m-1]*=dummy
  */
     }
   }
 
-  /* "fastphase/fastphase.pyx":1249
+  /* "fastphase/fastphase.pyx":1241
  *     ## compute forward probabilities
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=2] mPhi=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     for k in range(nK):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1249, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1249, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1249, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1241, __pyx_L1_error)
   __pyx_t_51 = ((PyArrayObject *)__pyx_t_5);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_mPhi.rcbuffer->pybuffer, (PyObject*)__pyx_t_51, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_mPhi = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1249, __pyx_L1_error)
+      __PYX_ERR(0, 1241, __pyx_L1_error)
     } else {__pyx_pybuffernd_mPhi.diminfo[0].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_mPhi.diminfo[0].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_mPhi.diminfo[1].strides = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_mPhi.diminfo[1].shape = __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_51 = 0;
   __pyx_v_mPhi = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "fastphase/fastphase.pyx":1250
+  /* "fastphase/fastphase.pyx":1242
  *     ##
  *     cdef np.ndarray[np.float64_t,ndim=2] mPhi=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)             # <<<<<<<<<<<<<<
  *     for k in range(nK):
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1250, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1250, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1250, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1242, __pyx_L1_error)
   __pyx_t_52 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_phiScale.rcbuffer->pybuffer, (PyObject*)__pyx_t_52, &__Pyx_TypeInfo_nn___pyx_t_5numpy_int_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_phiScale = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1250, __pyx_L1_error)
+      __PYX_ERR(0, 1242, __pyx_L1_error)
     } else {__pyx_pybuffernd_phiScale.diminfo[0].strides = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_phiScale.diminfo[0].shape = __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_52 = 0;
   __pyx_v_phiScale = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/fastphase.pyx":1251
+  /* "fastphase/fastphase.pyx":1243
  *     cdef np.ndarray[np.float64_t,ndim=2] mPhi=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])
  *     ## calc the marginal sum at locus 0 (appx A)
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1252
+    /* "fastphase/fastphase.pyx":1244
  *     cdef np.ndarray[np.int_t,ndim=1] phiScale=np.zeros(nLoc,dtype=np.int)
  *     for k in range(nK):
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])             # <<<<<<<<<<<<<<
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tSum[0]=0
  */
     __pyx_t_53 = 0;
@@ -28213,38 +27919,38 @@
     __pyx_t_58 = 0;
     __pyx_t_59 = __pyx_v_k;
     if (__pyx_t_58 < 0) __pyx_t_58 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
     if (__pyx_t_59 < 0) __pyx_t_59 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_58, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_59, __pyx_pybuffernd_mPhi.diminfo[1].strides) = ((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_53, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_54, __pyx_pybuffernd_alpha.diminfo[1].strides)) * __pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_55, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_56, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_57, __pyx_pybuffernd_hap.diminfo[0].strides))));
   }
 
-  /* "fastphase/fastphase.pyx":1254
+  /* "fastphase/fastphase.pyx":1246
  *         mPhi[0,k]=alpha[0,k]*happrG(theta[0,k],hap[0])
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tSum[0]=0             # <<<<<<<<<<<<<<
  *     for k in range(nK):
  *         tSum[0]+=mPhi[0,k]
  */
   __pyx_t_60 = 0;
   if (__pyx_t_60 < 0) __pyx_t_60 += __pyx_pybuffernd_tSum.diminfo[0].shape;
   *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_60, __pyx_pybuffernd_tSum.diminfo[0].strides) = 0.0;
 
-  /* "fastphase/fastphase.pyx":1255
+  /* "fastphase/fastphase.pyx":1247
  *     ## calc the marginal sum at locus 0 (appx A)
  *     tSum[0]=0
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         tSum[0]+=mPhi[0,k]
  *     ## calc Phi
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1256
+    /* "fastphase/fastphase.pyx":1248
  *     tSum[0]=0
  *     for k in range(nK):
  *         tSum[0]+=mPhi[0,k]             # <<<<<<<<<<<<<<
  *     ## calc Phi
  *     for m in range(nLoc-1):
  */
     __pyx_t_61 = 0;
@@ -28252,50 +27958,50 @@
     if (__pyx_t_61 < 0) __pyx_t_61 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
     if (__pyx_t_62 < 0) __pyx_t_62 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
     __pyx_t_63 = 0;
     if (__pyx_t_63 < 0) __pyx_t_63 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_63, __pyx_pybuffernd_tSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_61, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_62, __pyx_pybuffernd_mPhi.diminfo[1].strides));
   }
 
-  /* "fastphase/fastphase.pyx":1258
+  /* "fastphase/fastphase.pyx":1250
  *         tSum[0]+=mPhi[0,k]
  *     ## calc Phi
  *     for m in range(nLoc-1):             # <<<<<<<<<<<<<<
  *         tSum[m+1]=0
  *         ## this loop could be parallelized across clusters #CUDA
  */
   __pyx_t_64 = (__pyx_v_nLoc - 1);
   __pyx_t_65 = __pyx_t_64;
   for (__pyx_t_2 = 0; __pyx_t_2 < __pyx_t_65; __pyx_t_2+=1) {
     __pyx_v_m = __pyx_t_2;
 
-    /* "fastphase/fastphase.pyx":1259
+    /* "fastphase/fastphase.pyx":1251
  *     ## calc Phi
  *     for m in range(nLoc-1):
  *         tSum[m+1]=0             # <<<<<<<<<<<<<<
  *         ## this loop could be parallelized across clusters #CUDA
  *         for k in range(nK):
  */
     __pyx_t_66 = (__pyx_v_m + 1);
     if (__pyx_t_66 < 0) __pyx_t_66 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_66, __pyx_pybuffernd_tSum.diminfo[0].strides) = 0.0;
 
-    /* "fastphase/fastphase.pyx":1261
+    /* "fastphase/fastphase.pyx":1253
  *         tSum[m+1]=0
  *         ## this loop could be parallelized across clusters #CUDA
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  */
     __pyx_t_10 = __pyx_v_nK;
     __pyx_t_11 = __pyx_t_10;
     for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
       __pyx_v_k = __pyx_t_20;
 
-      /* "fastphase/fastphase.pyx":1262
+      /* "fastphase/fastphase.pyx":1254
  *         ## this loop could be parallelized across clusters #CUDA
  *         for k in range(nK):
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]             # <<<<<<<<<<<<<<
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  *             tSum[m+1]+=mPhi[m+1,k]
  */
       __pyx_t_67 = (__pyx_v_m + 1);
@@ -28314,15 +28020,15 @@
       __pyx_t_74 = __pyx_v_k;
       if (__pyx_t_73 < 0) __pyx_t_73 += __pyx_pybuffernd_alpha.diminfo[0].shape;
       if (__pyx_t_74 < 0) __pyx_t_74 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_75 = __pyx_v_m;
       if (__pyx_t_75 < 0) __pyx_t_75 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_v_temp = (((1.0 - (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_67, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_68, __pyx_pybuffernd_rho.diminfo[1].strides))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_69, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_70, __pyx_pybuffernd_mPhi.diminfo[1].strides))) + (((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_71, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_72, __pyx_pybuffernd_rho.diminfo[1].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_73, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_74, __pyx_pybuffernd_alpha.diminfo[1].strides))) * (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_75, __pyx_pybuffernd_tSum.diminfo[0].strides))));
 
-      /* "fastphase/fastphase.pyx":1263
+      /* "fastphase/fastphase.pyx":1255
  *         for k in range(nK):
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])             # <<<<<<<<<<<<<<
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0
  */
       __pyx_t_76 = (__pyx_v_m + 1);
@@ -28333,15 +28039,15 @@
       if (__pyx_t_78 < 0) __pyx_t_78 += __pyx_pybuffernd_hap.diminfo[0].shape;
       __pyx_t_79 = (__pyx_v_m + 1);
       __pyx_t_80 = __pyx_v_k;
       if (__pyx_t_79 < 0) __pyx_t_79 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_80 < 0) __pyx_t_80 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_79, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_80, __pyx_pybuffernd_mPhi.diminfo[1].strides) = (__pyx_v_temp * __pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_76, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_77, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_78, __pyx_pybuffernd_hap.diminfo[0].strides))));
 
-      /* "fastphase/fastphase.pyx":1264
+      /* "fastphase/fastphase.pyx":1256
  *             temp=(1-rho[m+1,0])*mPhi[m,k]+rho[m+1,0]*alpha[m+1,k]*tSum[m]
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  *             tSum[m+1]+=mPhi[m+1,k]             # <<<<<<<<<<<<<<
  *         tScale=0
  *         if tSum[m+1] < 0:
  */
       __pyx_t_81 = (__pyx_v_m + 1);
@@ -28349,516 +28055,516 @@
       if (__pyx_t_81 < 0) __pyx_t_81 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
       if (__pyx_t_82 < 0) __pyx_t_82 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
       __pyx_t_83 = (__pyx_v_m + 1);
       if (__pyx_t_83 < 0) __pyx_t_83 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_83, __pyx_pybuffernd_tSum.diminfo[0].strides) += (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_81, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_82, __pyx_pybuffernd_mPhi.diminfo[1].strides));
     }
 
-    /* "fastphase/fastphase.pyx":1265
+    /* "fastphase/fastphase.pyx":1257
  *             mPhi[m+1,k]=temp*happrG(theta[m+1,k],hap[m+1])
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0             # <<<<<<<<<<<<<<
  *         if tSum[m+1] < 0:
  *             phiScale[m+1]=phiScale[m]
  */
     __pyx_v_tScale = 0;
 
-    /* "fastphase/fastphase.pyx":1266
+    /* "fastphase/fastphase.pyx":1258
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0
  *         if tSum[m+1] < 0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
     __pyx_t_84 = (__pyx_v_m + 1);
     if (__pyx_t_84 < 0) __pyx_t_84 += __pyx_pybuffernd_tSum.diminfo[0].shape;
     __pyx_t_45 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_84, __pyx_pybuffernd_tSum.diminfo[0].strides)) < 0.0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1267
+      /* "fastphase/fastphase.pyx":1259
  *         tScale=0
  *         if tSum[m+1] < 0:
  *             phiScale[m+1]=phiScale[m]             # <<<<<<<<<<<<<<
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))
  */
       __pyx_t_85 = __pyx_v_m;
       if (__pyx_t_85 < 0) __pyx_t_85 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       __pyx_t_86 = (__pyx_v_m + 1);
       if (__pyx_t_86 < 0) __pyx_t_86 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_86, __pyx_pybuffernd_phiScale.diminfo[0].strides) = (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_85, __pyx_pybuffernd_phiScale.diminfo[0].strides));
 
-      /* "fastphase/fastphase.pyx":1266
+      /* "fastphase/fastphase.pyx":1258
  *             tSum[m+1]+=mPhi[m+1,k]
  *         tScale=0
  *         if tSum[m+1] < 0:             # <<<<<<<<<<<<<<
  *             phiScale[m+1]=phiScale[m]
  *         else:
  */
       goto __pyx_L23;
     }
 
-    /* "fastphase/fastphase.pyx":1269
+    /* "fastphase/fastphase.pyx":1261
  *             phiScale[m+1]=phiScale[m]
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))             # <<<<<<<<<<<<<<
  *         if tScale < 0:
  *             tScale=0
  */
     /*else*/ {
       __pyx_t_87 = (__pyx_v_m + 1);
       if (__pyx_t_87 < 0) __pyx_t_87 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_t_44 = (-log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_87, __pyx_pybuffernd_tSum.diminfo[0].strides))));
       __pyx_t_43 = log(10.0);
       if (unlikely(__pyx_t_43 == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-        __PYX_ERR(0, 1269, __pyx_L1_error)
+        __PYX_ERR(0, 1261, __pyx_L1_error)
       }
       __pyx_v_tScale = ((int)(__pyx_t_44 / __pyx_t_43));
     }
     __pyx_L23:;
 
-    /* "fastphase/fastphase.pyx":1270
+    /* "fastphase/fastphase.pyx":1262
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))
  *         if tScale < 0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  */
     __pyx_t_45 = ((__pyx_v_tScale < 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1271
+      /* "fastphase/fastphase.pyx":1263
  *             tScale=int(-log(tSum[m+1])/log(10))
  *         if tScale < 0:
  *             tScale=0             # <<<<<<<<<<<<<<
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:
  */
       __pyx_v_tScale = 0;
 
-      /* "fastphase/fastphase.pyx":1270
+      /* "fastphase/fastphase.pyx":1262
  *         else:
  *             tScale=int(-log(tSum[m+1])/log(10))
  *         if tScale < 0:             # <<<<<<<<<<<<<<
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  */
     }
 
-    /* "fastphase/fastphase.pyx":1272
+    /* "fastphase/fastphase.pyx":1264
  *         if tScale < 0:
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale             # <<<<<<<<<<<<<<
  *         if tScale > 0:
  *             dummy=myPow10(tScale)
  */
     __pyx_t_88 = __pyx_v_m;
     if (__pyx_t_88 < 0) __pyx_t_88 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     __pyx_t_89 = (__pyx_v_m + 1);
     if (__pyx_t_89 < 0) __pyx_t_89 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_89, __pyx_pybuffernd_phiScale.diminfo[0].strides) = ((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_88, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + __pyx_v_tScale);
 
-    /* "fastphase/fastphase.pyx":1273
+    /* "fastphase/fastphase.pyx":1265
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy
  */
     __pyx_t_45 = ((__pyx_v_tScale > 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1274
+      /* "fastphase/fastphase.pyx":1266
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:
  *             dummy=myPow10(tScale)             # <<<<<<<<<<<<<<
  *             tSum[m+1]*=dummy
  *             for k in range(nK):
  */
       __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10(__pyx_v_tScale);
 
-      /* "fastphase/fastphase.pyx":1275
+      /* "fastphase/fastphase.pyx":1267
  *         if tScale > 0:
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 mPhi[m+1,k]*=dummy
  */
       __pyx_t_90 = (__pyx_v_m + 1);
       if (__pyx_t_90 < 0) __pyx_t_90 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       *__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_90, __pyx_pybuffernd_tSum.diminfo[0].strides) *= __pyx_v_dummy;
 
-      /* "fastphase/fastphase.pyx":1276
+      /* "fastphase/fastphase.pyx":1268
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 mPhi[m+1,k]*=dummy
  *     ## end calc Phi
  */
       __pyx_t_10 = __pyx_v_nK;
       __pyx_t_11 = __pyx_t_10;
       for (__pyx_t_20 = 0; __pyx_t_20 < __pyx_t_11; __pyx_t_20+=1) {
         __pyx_v_k = __pyx_t_20;
 
-        /* "fastphase/fastphase.pyx":1277
+        /* "fastphase/fastphase.pyx":1269
  *             tSum[m+1]*=dummy
  *             for k in range(nK):
  *                 mPhi[m+1,k]*=dummy             # <<<<<<<<<<<<<<
  *     ## end calc Phi
  *     logLikelihood=log(tSum[nLoc-1])/log(10)-phiScale[nLoc-1]
  */
         __pyx_t_91 = (__pyx_v_m + 1);
         __pyx_t_92 = __pyx_v_k;
         if (__pyx_t_91 < 0) __pyx_t_91 += __pyx_pybuffernd_mPhi.diminfo[0].shape;
         if (__pyx_t_92 < 0) __pyx_t_92 += __pyx_pybuffernd_mPhi.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mPhi.rcbuffer->pybuffer.buf, __pyx_t_91, __pyx_pybuffernd_mPhi.diminfo[0].strides, __pyx_t_92, __pyx_pybuffernd_mPhi.diminfo[1].strides) *= __pyx_v_dummy;
       }
 
-      /* "fastphase/fastphase.pyx":1273
+      /* "fastphase/fastphase.pyx":1265
  *             tScale=0
  *         phiScale[m+1]=phiScale[m]+tScale
  *         if tScale > 0:             # <<<<<<<<<<<<<<
  *             dummy=myPow10(tScale)
  *             tSum[m+1]*=dummy
  */
     }
   }
 
-  /* "fastphase/fastphase.pyx":1279
+  /* "fastphase/fastphase.pyx":1271
  *                 mPhi[m+1,k]*=dummy
  *     ## end calc Phi
  *     logLikelihood=log(tSum[nLoc-1])/log(10)-phiScale[nLoc-1]             # <<<<<<<<<<<<<<
  *     ##
  *     ## compute individual contributions top,bottom,jmk
  */
   __pyx_t_93 = (__pyx_v_nLoc - 1);
   if (__pyx_t_93 < 0) __pyx_t_93 += __pyx_pybuffernd_tSum.diminfo[0].shape;
   __pyx_t_43 = log((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_93, __pyx_pybuffernd_tSum.diminfo[0].strides)));
   __pyx_t_44 = log(10.0);
   if (unlikely(__pyx_t_44 == 0)) {
     PyErr_SetString(PyExc_ZeroDivisionError, "float division");
-    __PYX_ERR(0, 1279, __pyx_L1_error)
+    __PYX_ERR(0, 1271, __pyx_L1_error)
   }
   __pyx_t_94 = (__pyx_v_nLoc - 1);
   if (__pyx_t_94 < 0) __pyx_t_94 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
   __pyx_v_logLikelihood = ((__pyx_t_43 / __pyx_t_44) - (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_94, __pyx_pybuffernd_phiScale.diminfo[0].strides)));
 
-  /* "fastphase/fastphase.pyx":1284
+  /* "fastphase/fastphase.pyx":1276
  *     ##
  *     # compute probZ see appx A at the end
  *     cdef np.ndarray[np.float64_t,ndim=2] probZ=mPhi*mBeta             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __pyx_t_3 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1284, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(((PyObject *)__pyx_v_mPhi), ((PyObject *)__pyx_v_mBeta)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1284, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1276, __pyx_L1_error)
   __pyx_t_95 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_probZ.rcbuffer->pybuffer, (PyObject*)__pyx_t_95, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_probZ = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1284, __pyx_L1_error)
+      __PYX_ERR(0, 1276, __pyx_L1_error)
     } else {__pyx_pybuffernd_probZ.diminfo[0].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_probZ.diminfo[0].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_probZ.diminfo[1].strides = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_probZ.diminfo[1].shape = __pyx_pybuffernd_probZ.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_95 = 0;
   __pyx_v_probZ = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/fastphase.pyx":1285
+  /* "fastphase/fastphase.pyx":1277
  *     # compute probZ see appx A at the end
  *     cdef np.ndarray[np.float64_t,ndim=2] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1285, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1285, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1285, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1277, __pyx_L1_error)
   __pyx_t_96 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_jmk.rcbuffer->pybuffer, (PyObject*)__pyx_t_96, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_jmk = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1285, __pyx_L1_error)
+      __PYX_ERR(0, 1277, __pyx_L1_error)
     } else {__pyx_pybuffernd_jmk.diminfo[0].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_jmk.diminfo[0].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_jmk.diminfo[1].strides = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_jmk.diminfo[1].shape = __pyx_pybuffernd_jmk.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_96 = 0;
   __pyx_v_jmk = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1286
+  /* "fastphase/fastphase.pyx":1278
  *     cdef np.ndarray[np.float64_t,ndim=2] probZ=mPhi*mBeta
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1286, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1286, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1278, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1286, __pyx_L1_error)
+  if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1278, __pyx_L1_error)
   __pyx_t_97 = ((PyArrayObject *)__pyx_t_3);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_top.rcbuffer->pybuffer, (PyObject*)__pyx_t_97, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_top = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_top.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1286, __pyx_L1_error)
+      __PYX_ERR(0, 1278, __pyx_L1_error)
     } else {__pyx_pybuffernd_top.diminfo[0].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_top.diminfo[0].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_top.diminfo[1].strides = __pyx_pybuffernd_top.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_top.diminfo[1].shape = __pyx_pybuffernd_top.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_97 = 0;
   __pyx_v_top = ((PyArrayObject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "fastphase/fastphase.pyx":1287
+  /* "fastphase/fastphase.pyx":1279
  *     cdef np.ndarray[np.float64_t,ndim=2] jmk=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] top=np.zeros((nLoc,nK),dtype=np.float64)
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)             # <<<<<<<<<<<<<<
  * 
  *     for m in range(nLoc):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nLoc); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nK); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_float64); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1287, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1287, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1279, __pyx_L1_error)
   __pyx_t_98 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_bot.rcbuffer->pybuffer, (PyObject*)__pyx_t_98, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
       __pyx_v_bot = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 1287, __pyx_L1_error)
+      __PYX_ERR(0, 1279, __pyx_L1_error)
     } else {__pyx_pybuffernd_bot.diminfo[0].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_bot.diminfo[0].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_bot.diminfo[1].strides = __pyx_pybuffernd_bot.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_bot.diminfo[1].shape = __pyx_pybuffernd_bot.rcbuffer->pybuffer.shape[1];
     }
   }
   __pyx_t_98 = 0;
   __pyx_v_bot = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "fastphase/fastphase.pyx":1289
+  /* "fastphase/fastphase.pyx":1281
  *     cdef np.ndarray[np.float64_t,ndim=2] bot=np.zeros((nLoc,nK),dtype=np.float64)
  * 
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         normC=0
  *         for k in range(nK):
  */
   __pyx_t_2 = __pyx_v_nLoc;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_m = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1290
+    /* "fastphase/fastphase.pyx":1282
  * 
  *     for m in range(nLoc):
  *         normC=0             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             normC+=probZ[m,k]
  */
     __pyx_v_normC = 0.0;
 
-    /* "fastphase/fastphase.pyx":1291
+    /* "fastphase/fastphase.pyx":1283
  *     for m in range(nLoc):
  *         normC=0
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             normC+=probZ[m,k]
  *         for k in range(nK):
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_99 = __pyx_t_20;
     for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
       __pyx_v_k = __pyx_t_100;
 
-      /* "fastphase/fastphase.pyx":1292
+      /* "fastphase/fastphase.pyx":1284
  *         normC=0
  *         for k in range(nK):
  *             normC+=probZ[m,k]             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             probZ[m,k]/=normC
  */
       __pyx_t_101 = __pyx_v_m;
       __pyx_t_102 = __pyx_v_k;
       if (__pyx_t_101 < 0) __pyx_t_101 += __pyx_pybuffernd_probZ.diminfo[0].shape;
       if (__pyx_t_102 < 0) __pyx_t_102 += __pyx_pybuffernd_probZ.diminfo[1].shape;
       __pyx_v_normC = (__pyx_v_normC + (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_101, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_102, __pyx_pybuffernd_probZ.diminfo[1].strides)));
     }
 
-    /* "fastphase/fastphase.pyx":1293
+    /* "fastphase/fastphase.pyx":1285
  *         for k in range(nK):
  *             normC+=probZ[m,k]
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             probZ[m,k]/=normC
  *     if up2pz:
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_99 = __pyx_t_20;
     for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
       __pyx_v_k = __pyx_t_100;
 
-      /* "fastphase/fastphase.pyx":1294
+      /* "fastphase/fastphase.pyx":1286
  *             normC+=probZ[m,k]
  *         for k in range(nK):
  *             probZ[m,k]/=normC             # <<<<<<<<<<<<<<
  *     if up2pz:
  *         return probZ
  */
       __pyx_t_103 = __pyx_v_m;
       __pyx_t_104 = __pyx_v_k;
       if (__pyx_t_103 < 0) __pyx_t_103 += __pyx_pybuffernd_probZ.diminfo[0].shape;
       if (__pyx_t_104 < 0) __pyx_t_104 += __pyx_pybuffernd_probZ.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_103, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_104, __pyx_pybuffernd_probZ.diminfo[1].strides) /= __pyx_v_normC;
     }
   }
 
-  /* "fastphase/fastphase.pyx":1295
+  /* "fastphase/fastphase.pyx":1287
  *         for k in range(nK):
  *             probZ[m,k]/=normC
  *     if up2pz:             # <<<<<<<<<<<<<<
  *         return probZ
  *     ## compute expected jum prob for each interval (appx C)
  */
   __pyx_t_45 = (__pyx_v_up2pz != 0);
   if (__pyx_t_45) {
 
-    /* "fastphase/fastphase.pyx":1296
+    /* "fastphase/fastphase.pyx":1288
  *             probZ[m,k]/=normC
  *     if up2pz:
  *         return probZ             # <<<<<<<<<<<<<<
  *     ## compute expected jum prob for each interval (appx C)
  *     # locus 0
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_probZ));
     __pyx_r = ((PyObject *)__pyx_v_probZ);
     goto __pyx_L0;
 
-    /* "fastphase/fastphase.pyx":1295
+    /* "fastphase/fastphase.pyx":1287
  *         for k in range(nK):
  *             probZ[m,k]/=normC
  *     if up2pz:             # <<<<<<<<<<<<<<
  *         return probZ
  *     ## compute expected jum prob for each interval (appx C)
  */
   }
 
-  /* "fastphase/fastphase.pyx":1299
+  /* "fastphase/fastphase.pyx":1291
  *     ## compute expected jum prob for each interval (appx C)
  *     # locus 0
  *     for k in range(nK):             # <<<<<<<<<<<<<<
  *         ##jmk[0,k]=alpha[0,k]
  *         jmk[0, k] = probZ[ 0, k]
  */
   __pyx_t_2 = __pyx_v_nK;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_k = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1301
+    /* "fastphase/fastphase.pyx":1293
  *     for k in range(nK):
  *         ##jmk[0,k]=alpha[0,k]
  *         jmk[0, k] = probZ[ 0, k]             # <<<<<<<<<<<<<<
  *     for m in range(1,nLoc):
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  */
     __pyx_t_105 = 0;
@@ -28868,54 +28574,54 @@
     __pyx_t_107 = 0;
     __pyx_t_108 = __pyx_v_k;
     if (__pyx_t_107 < 0) __pyx_t_107 += __pyx_pybuffernd_jmk.diminfo[0].shape;
     if (__pyx_t_108 < 0) __pyx_t_108 += __pyx_pybuffernd_jmk.diminfo[1].shape;
     *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_107, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_108, __pyx_pybuffernd_jmk.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_105, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_106, __pyx_pybuffernd_probZ.diminfo[1].strides));
   }
 
-  /* "fastphase/fastphase.pyx":1302
+  /* "fastphase/fastphase.pyx":1294
  *         ##jmk[0,k]=alpha[0,k]
  *         jmk[0, k] = probZ[ 0, k]
  *     for m in range(1,nLoc):             # <<<<<<<<<<<<<<
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  */
   __pyx_t_2 = __pyx_v_nLoc;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 1; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_m = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1303
+    /* "fastphase/fastphase.pyx":1295
  *         jmk[0, k] = probZ[ 0, k]
  *     for m in range(1,nLoc):
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])             # <<<<<<<<<<<<<<
  *         for k in range(nK):
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  */
     __pyx_t_109 = (__pyx_v_m - 1);
     if (__pyx_t_109 < 0) __pyx_t_109 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     __pyx_t_110 = __pyx_v_m;
     if (__pyx_t_110 < 0) __pyx_t_110 += __pyx_pybuffernd_betaScale.diminfo[0].shape;
     __pyx_t_111 = (__pyx_v_nLoc - 1);
     if (__pyx_t_111 < 0) __pyx_t_111 += __pyx_pybuffernd_phiScale.diminfo[0].shape;
     __pyx_v_dummy = __pyx_f_9fastphase_9fastphase_myPow10((((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_109, __pyx_pybuffernd_phiScale.diminfo[0].strides)) + (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_betaScale.rcbuffer->pybuffer.buf, __pyx_t_110, __pyx_pybuffernd_betaScale.diminfo[0].strides))) - (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_phiScale.rcbuffer->pybuffer.buf, __pyx_t_111, __pyx_pybuffernd_phiScale.diminfo[0].strides))));
 
-    /* "fastphase/fastphase.pyx":1304
+    /* "fastphase/fastphase.pyx":1296
  *     for m in range(1,nLoc):
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):             # <<<<<<<<<<<<<<
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             jmk[m,k] *= alpha[m,k]
  */
     __pyx_t_20 = __pyx_v_nK;
     __pyx_t_99 = __pyx_t_20;
     for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
       __pyx_v_k = __pyx_t_100;
 
-      /* "fastphase/fastphase.pyx":1305
+      /* "fastphase/fastphase.pyx":1297
  *         dummy=myPow10(phiScale[m-1]+betaScale[m]-phiScale[nLoc-1])
  *         for k in range(nK):
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]             # <<<<<<<<<<<<<<
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tSum[nLoc-1]
  */
       __pyx_t_112 = (__pyx_v_m - 1);
@@ -28936,15 +28642,15 @@
       if (__pyx_t_119 < 0) __pyx_t_119 += __pyx_pybuffernd_mBeta.diminfo[1].shape;
       __pyx_t_120 = __pyx_v_m;
       __pyx_t_121 = __pyx_v_k;
       if (__pyx_t_120 < 0) __pyx_t_120 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_121 < 0) __pyx_t_121 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_120, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_121, __pyx_pybuffernd_jmk.diminfo[1].strides) = ((((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_112, __pyx_pybuffernd_tSum.diminfo[0].strides)) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_rho.rcbuffer->pybuffer.buf, __pyx_t_113, __pyx_pybuffernd_rho.diminfo[0].strides, __pyx_t_114, __pyx_pybuffernd_rho.diminfo[1].strides))) * __pyx_f_9fastphase_9fastphase_happrG((*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_theta.rcbuffer->pybuffer.buf, __pyx_t_115, __pyx_pybuffernd_theta.diminfo[0].strides, __pyx_t_116, __pyx_pybuffernd_theta.diminfo[1].strides)), (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_117, __pyx_pybuffernd_hap.diminfo[0].strides)))) * (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_mBeta.rcbuffer->pybuffer.buf, __pyx_t_118, __pyx_pybuffernd_mBeta.diminfo[0].strides, __pyx_t_119, __pyx_pybuffernd_mBeta.diminfo[1].strides)));
 
-      /* "fastphase/fastphase.pyx":1306
+      /* "fastphase/fastphase.pyx":1298
  *         for k in range(nK):
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             jmk[m,k] *= alpha[m,k]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= tSum[nLoc-1]
  *             jmk[m,k] /= dummy
  */
       __pyx_t_122 = __pyx_v_m;
@@ -28953,81 +28659,81 @@
       if (__pyx_t_123 < 0) __pyx_t_123 += __pyx_pybuffernd_alpha.diminfo[1].shape;
       __pyx_t_124 = __pyx_v_m;
       __pyx_t_125 = __pyx_v_k;
       if (__pyx_t_124 < 0) __pyx_t_124 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_125 < 0) __pyx_t_125 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_124, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_125, __pyx_pybuffernd_jmk.diminfo[1].strides) *= (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_alpha.rcbuffer->pybuffer.buf, __pyx_t_122, __pyx_pybuffernd_alpha.diminfo[0].strides, __pyx_t_123, __pyx_pybuffernd_alpha.diminfo[1].strides));
 
-      /* "fastphase/fastphase.pyx":1307
+      /* "fastphase/fastphase.pyx":1299
  *             jmk[m,k]  = tSum[m-1]*rho[m,0]*happrG(theta[m,k],hap[m])*mBeta[m,k]
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tSum[nLoc-1]             # <<<<<<<<<<<<<<
  *             jmk[m,k] /= dummy
  *             # if not np.isfinite(jmk[m,k]):
  */
       __pyx_t_126 = (__pyx_v_nLoc - 1);
       if (__pyx_t_126 < 0) __pyx_t_126 += __pyx_pybuffernd_tSum.diminfo[0].shape;
       __pyx_t_127 = __pyx_v_m;
       __pyx_t_128 = __pyx_v_k;
       if (__pyx_t_127 < 0) __pyx_t_127 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_128 < 0) __pyx_t_128 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_127, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_128, __pyx_pybuffernd_jmk.diminfo[1].strides) /= (*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_tSum.rcbuffer->pybuffer.buf, __pyx_t_126, __pyx_pybuffernd_tSum.diminfo[0].strides));
 
-      /* "fastphase/fastphase.pyx":1308
+      /* "fastphase/fastphase.pyx":1300
  *             jmk[m,k] *= alpha[m,k]
  *             jmk[m,k] /= tSum[nLoc-1]
  *             jmk[m,k] /= dummy             # <<<<<<<<<<<<<<
  *             # if not np.isfinite(jmk[m,k]):
  *             #     print tSum[m-1],rho[m,0],theta[m,k],hap[m],mBeta[m,k]
  */
       __pyx_t_129 = __pyx_v_m;
       __pyx_t_130 = __pyx_v_k;
       if (__pyx_t_129 < 0) __pyx_t_129 += __pyx_pybuffernd_jmk.diminfo[0].shape;
       if (__pyx_t_130 < 0) __pyx_t_130 += __pyx_pybuffernd_jmk.diminfo[1].shape;
       *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_jmk.rcbuffer->pybuffer.buf, __pyx_t_129, __pyx_pybuffernd_jmk.diminfo[0].strides, __pyx_t_130, __pyx_pybuffernd_jmk.diminfo[1].strides) /= __pyx_v_dummy;
     }
   }
 
-  /* "fastphase/fastphase.pyx":1316
+  /* "fastphase/fastphase.pyx":1308
  *             #     raise ValueError
  *     # calc thetablock and its inner product with probZ (appx C.)
  *     for m in range(nLoc):             # <<<<<<<<<<<<<<
  *         if hap[m] == 0:
  *             for k in range(nK):
  */
   __pyx_t_2 = __pyx_v_nLoc;
   __pyx_t_10 = __pyx_t_2;
   for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
     __pyx_v_m = __pyx_t_11;
 
-    /* "fastphase/fastphase.pyx":1317
+    /* "fastphase/fastphase.pyx":1309
  *     # calc thetablock and its inner product with probZ (appx C.)
  *     for m in range(nLoc):
  *         if hap[m] == 0:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  */
     __pyx_t_131 = __pyx_v_m;
     if (__pyx_t_131 < 0) __pyx_t_131 += __pyx_pybuffernd_hap.diminfo[0].shape;
     __pyx_t_45 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_131, __pyx_pybuffernd_hap.diminfo[0].strides)) == 0) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1318
+      /* "fastphase/fastphase.pyx":1310
  *     for m in range(nLoc):
  *         if hap[m] == 0:
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:
  */
       __pyx_t_20 = __pyx_v_nK;
       __pyx_t_99 = __pyx_t_20;
       for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
         __pyx_v_k = __pyx_t_100;
 
-        /* "fastphase/fastphase.pyx":1319
+        /* "fastphase/fastphase.pyx":1311
  *         if hap[m] == 0:
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]             # <<<<<<<<<<<<<<
  *         elif hap[m]==1:
  *             for k in range(nK):
  */
         __pyx_t_132 = __pyx_v_m;
@@ -29037,49 +28743,49 @@
         __pyx_t_134 = __pyx_v_m;
         __pyx_t_135 = __pyx_v_k;
         if (__pyx_t_134 < 0) __pyx_t_134 += __pyx_pybuffernd_bot.diminfo[0].shape;
         if (__pyx_t_135 < 0) __pyx_t_135 += __pyx_pybuffernd_bot.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_134, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_135, __pyx_pybuffernd_bot.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_132, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_133, __pyx_pybuffernd_probZ.diminfo[1].strides));
       }
 
-      /* "fastphase/fastphase.pyx":1317
+      /* "fastphase/fastphase.pyx":1309
  *     # calc thetablock and its inner product with probZ (appx C.)
  *     for m in range(nLoc):
  *         if hap[m] == 0:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  */
       goto __pyx_L43;
     }
 
-    /* "fastphase/fastphase.pyx":1320
+    /* "fastphase/fastphase.pyx":1312
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]
  */
     __pyx_t_136 = __pyx_v_m;
     if (__pyx_t_136 < 0) __pyx_t_136 += __pyx_pybuffernd_hap.diminfo[0].shape;
     __pyx_t_45 = (((*__Pyx_BufPtrStrided1d(__pyx_t_5numpy_int_t *, __pyx_pybuffernd_hap.rcbuffer->pybuffer.buf, __pyx_t_136, __pyx_pybuffernd_hap.diminfo[0].strides)) == 1) != 0);
     if (__pyx_t_45) {
 
-      /* "fastphase/fastphase.pyx":1321
+      /* "fastphase/fastphase.pyx":1313
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:
  *             for k in range(nK):             # <<<<<<<<<<<<<<
  *                 top[m,k]=probZ[m,k]
  *                 bot[m,k]=probZ[m,k]
  */
       __pyx_t_20 = __pyx_v_nK;
       __pyx_t_99 = __pyx_t_20;
       for (__pyx_t_100 = 0; __pyx_t_100 < __pyx_t_99; __pyx_t_100+=1) {
         __pyx_v_k = __pyx_t_100;
 
-        /* "fastphase/fastphase.pyx":1322
+        /* "fastphase/fastphase.pyx":1314
  *         elif hap[m]==1:
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]             # <<<<<<<<<<<<<<
  *                 bot[m,k]=probZ[m,k]
  *     return logLikelihood,top,bot,jmk
  */
         __pyx_t_137 = __pyx_v_m;
@@ -29088,15 +28794,15 @@
         if (__pyx_t_138 < 0) __pyx_t_138 += __pyx_pybuffernd_probZ.diminfo[1].shape;
         __pyx_t_139 = __pyx_v_m;
         __pyx_t_140 = __pyx_v_k;
         if (__pyx_t_139 < 0) __pyx_t_139 += __pyx_pybuffernd_top.diminfo[0].shape;
         if (__pyx_t_140 < 0) __pyx_t_140 += __pyx_pybuffernd_top.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_top.rcbuffer->pybuffer.buf, __pyx_t_139, __pyx_pybuffernd_top.diminfo[0].strides, __pyx_t_140, __pyx_pybuffernd_top.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_137, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_138, __pyx_pybuffernd_probZ.diminfo[1].strides));
 
-        /* "fastphase/fastphase.pyx":1323
+        /* "fastphase/fastphase.pyx":1315
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]
  *                 bot[m,k]=probZ[m,k]             # <<<<<<<<<<<<<<
  *     return logLikelihood,top,bot,jmk
  * 
  */
         __pyx_t_141 = __pyx_v_m;
@@ -29106,36 +28812,36 @@
         __pyx_t_143 = __pyx_v_m;
         __pyx_t_144 = __pyx_v_k;
         if (__pyx_t_143 < 0) __pyx_t_143 += __pyx_pybuffernd_bot.diminfo[0].shape;
         if (__pyx_t_144 < 0) __pyx_t_144 += __pyx_pybuffernd_bot.diminfo[1].shape;
         *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_bot.rcbuffer->pybuffer.buf, __pyx_t_143, __pyx_pybuffernd_bot.diminfo[0].strides, __pyx_t_144, __pyx_pybuffernd_bot.diminfo[1].strides) = (*__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_probZ.rcbuffer->pybuffer.buf, __pyx_t_141, __pyx_pybuffernd_probZ.diminfo[0].strides, __pyx_t_142, __pyx_pybuffernd_probZ.diminfo[1].strides));
       }
 
-      /* "fastphase/fastphase.pyx":1320
+      /* "fastphase/fastphase.pyx":1312
  *             for k in range(nK):
  *                 bot[m,k]=probZ[m,k]
  *         elif hap[m]==1:             # <<<<<<<<<<<<<<
  *             for k in range(nK):
  *                 top[m,k]=probZ[m,k]
  */
     }
     __pyx_L43:;
   }
 
-  /* "fastphase/fastphase.pyx":1324
+  /* "fastphase/fastphase.pyx":1316
  *                 top[m,k]=probZ[m,k]
  *                 bot[m,k]=probZ[m,k]
  *     return logLikelihood,top,bot,jmk             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1324, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_logLikelihood); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1324, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1);
   __Pyx_INCREF(((PyObject *)__pyx_v_top));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_top));
   PyTuple_SET_ITEM(__pyx_t_6, 1, ((PyObject *)__pyx_v_top));
   __Pyx_INCREF(((PyObject *)__pyx_v_bot));
@@ -29145,15 +28851,15 @@
   __Pyx_GIVEREF(((PyObject *)__pyx_v_jmk));
   PyTuple_SET_ITEM(__pyx_t_6, 3, ((PyObject *)__pyx_v_jmk));
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "fastphase/fastphase.pyx":1194
+  /* "fastphase/fastphase.pyx":1186
  *     return soluce
  * 
  * cpdef hapCalc(aa,tt,rr,hh,u2p):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray[np.float64_t, ndim=2] alpha = aa
  *     cdef np.ndarray[np.float64_t,ndim=2] theta = tt
  */
 
@@ -29254,37 +28960,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aa)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tt)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 1); __PYX_ERR(0, 1194, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 1); __PYX_ERR(0, 1186, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_rr)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 2); __PYX_ERR(0, 1194, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 2); __PYX_ERR(0, 1186, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_hh)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 3); __PYX_ERR(0, 1194, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 3); __PYX_ERR(0, 1186, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_u2p)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 4); __PYX_ERR(0, 1194, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, 4); __PYX_ERR(0, 1186, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapCalc") < 0)) __PYX_ERR(0, 1194, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "hapCalc") < 0)) __PYX_ERR(0, 1186, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -29295,15 +29001,15 @@
     __pyx_v_tt = values[1];
     __pyx_v_rr = values[2];
     __pyx_v_hh = values[3];
     __pyx_v_u2p = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1194, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("hapCalc", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1186, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("fastphase.fastphase.hapCalc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9fastphase_9fastphase_24hapCalc(__pyx_self, __pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, __pyx_v_u2p);
 
@@ -29314,15 +29020,15 @@
 
 static PyObject *__pyx_pf_9fastphase_9fastphase_24hapCalc(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_aa, PyObject *__pyx_v_tt, PyObject *__pyx_v_rr, PyObject *__pyx_v_hh, PyObject *__pyx_v_u2p) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("hapCalc", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9fastphase_9fastphase_hapCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1194, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9fastphase_9fastphase_hapCalc(__pyx_v_aa, __pyx_v_tt, __pyx_v_rr, __pyx_v_hh, __pyx_v_u2p, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1186, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -35195,15 +34901,15 @@
  *         return np.array( _tohap(np.array(gen, dtype=int)), dtype=int)
  * 
  */
   __pyx_t_2 = __Pyx_CyFunction_NewEx(&__pyx_mdef_9fastphase_9fastphase_9fastphase_15gen2hap, __Pyx_CYFUNCTION_STATICMETHOD, __pyx_n_s_fastphase_gen2hap, NULL, __pyx_n_s_fastphase_fastphase, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
   /* "fastphase/fastphase.pyx":202
- *         self.genolik[ID] = lik - np.max(lik, axis=1,keepdims=True)
+ *         self.genolik[ID] = np.exp(lik - np.max(lik, axis=1,keepdims=True))
  * 
  *     @staticmethod             # <<<<<<<<<<<<<<
  *     def gen2hap(gen):
  *         return np.array( _tohap(np.array(gen, dtype=int)), dtype=int)
  */
   __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_staticmethod, __pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
```

### Comparing `fastphase-2.0.dev2/fastphase/fastphase.pyx` & `fastphase-2.0.dev3/fastphase/fastphase.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         '''
         try:
             assert lik.shape == (self.nLoci,3)
         except AssertionError:
             print("Wrong Array Size:", lik.shape,"is not",(self.nLoci,3))
             raise
         lik = np.array(lik) 
-        self.genolik[ID] = lik - np.max(lik, axis=1,keepdims=True)
+        self.genolik[ID] = np.exp(lik - np.max(lik, axis=1,keepdims=True))
             
     @staticmethod
     def gen2hap(gen):
         return np.array( _tohap(np.array(gen, dtype=int)), dtype=int)
     
     def fit(self,nClus=20,nstep=20,params=None,verbose=False,rhomin=1e-6, alpha_up = True, theta_up = True, fast=False):
         '''
@@ -904,24 +904,16 @@
             for k in range(nK):
                 top[m,k]=0
                 bot[m,k]=0
     return logLikelihood,top,bot,jmk
 
 
 ########################################### Genotype likelihood Calculations #####################################################
-cdef double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):
-    cdef double rez
-    cdef int i
-    
-    rez = 0.0
-    ## g = 0
-    rez = np.exp(gl[0])*(1-t1)*(1-t2)
-    rez += np.exp(gl[1])*( t1*(1-t2) + (1-t1)*t2)
-    rez += np.exp(gl[2])*t1*t2
-    return rez
+cdef inline double likprG( double t1,double t2, np.ndarray[ np.float64_t, ndim=1] gl):
+    return gl[0]*(1-t1)*(1-t2) + gl[1]*( t1*(1-t2) + (1-t1)*t2) +  gl[2]*t1*t2
 
 cpdef likCalc(aa,tt,rr,ll,u2p):
     cdef np.ndarray[np.float64_t, ndim=2] alpha=aa
     cdef np.ndarray[np.float64_t,ndim=2] theta=tt
     cdef np.ndarray[np.float64_t, ndim=2] rho=rr
     cdef np.ndarray[np.float64_t, ndim=2] lik=ll
     cdef int up2pz=u2p
@@ -1075,34 +1067,34 @@
     ## init at 0
     for k1 in range(nK):
         for k2 in range(k1,nK):
             temp = alpha[0,k1]*alpha[0,k2]*mBeta[0,k1,k2]
             p_g_givX[0,0] += temp*genprG(theta[0,k1],theta[0,k2],0) 
             p_g_givX[0,1] += temp*genprG(theta[0,k1],theta[0,k2],1) 
             p_g_givX[0,2] += temp*genprG(theta[0,k1],theta[0,k2],2)
-    p_g_givX[0,0] *= np.exp(lik[0,0])
-    p_g_givX[0,1] *= np.exp(lik[0,1])
-    p_g_givX[0,2] *= np.exp(lik[0,2])
+    p_g_givX[0,0] *= lik[0,0]
+    p_g_givX[0,1] *= lik[0,1]
+    p_g_givX[0,2] *= lik[0,2]
     normC = p_g_givX[0,0]+p_g_givX[0,1]+p_g_givX[0,2]
     p_g_givX[0]/=normC
             
     for m in range(nLoc-1):
         for k1 in range(nK):
             for k2 in range(k1,nK):
                 temp=alpha[m+1,k1]*tSumk[m,k2]+alpha[m+1,k2]*tSumk[m,k1]
                 temp*=0.5*probJ(m+1,1,rho[m+1,0])
                 temp+=probJ(m+1,0,rho[m+1,0])*mPhi[m,k1,k2]
                 temp+=probJ(m+1,2,rho[m+1,0])*alpha[m+1,k1]*alpha[m+1,k2]*tDoubleSum[m]
                 temp*=mBeta[m+1,k1,k2]
                 p_g_givX[m+1,0] += temp*genprG(theta[m+1,k1],theta[m+1,k2],0)
                 p_g_givX[m+1,1] += temp*genprG(theta[m+1,k1],theta[m+1,k2],1)
                 p_g_givX[m+1,2] += temp*genprG(theta[m+1,k1],theta[m+1,k2],2)
-        p_g_givX[m+1,0] *= np.exp(lik[m+1,0])
-        p_g_givX[m+1,1] *= np.exp(lik[m+1,1])
-        p_g_givX[m+1,2] *= np.exp(lik[m+1,2])
+        p_g_givX[m+1,0] *= lik[m+1,0]
+        p_g_givX[m+1,1] *= lik[m+1,1]
+        p_g_givX[m+1,2] *= lik[m+1,2]
         normC = p_g_givX[m+1,0]+p_g_givX[m+1,1]+p_g_givX[m+1,2]
         p_g_givX[m+1]/=normC
                 
     if up2pz>0:
         return probZ,p_g_givX
     # calc jmk
     for k1 in range(nK):
```

### Comparing `fastphase-2.0.dev2/fastphase/fastphase_ray.py` & `fastphase-2.0.dev3/fastphase/fastphase_ray.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,69 +76,14 @@
         cost_mat[ k1, kp2] -= 0.5
         cost_mat[ k2, kp1] -= 0.5
         cost_mat[ k2, kp2] -= 0.5
     return cost_mat
 
 ### CLASSES
 
-# class modParams():
-#     '''
-#     A class for fastphase model parameters.
-#     Dimensions:
-#     -- number of loci: N
-#     -- number of clusters: K
-#     Parameters:
-#     -- theta (N x K): allele frequencies in clusters at each locus
-#     -- alpha (N x K): cluster weights at each locus
-#     -- rho (N x 1): jump probabilities in each interval
-#     '''
-#     def __init__(self,nLoc,nClus,rhomin=1e-6, alpha_up = True, theta_up = True):
-#         self.nLoc=nLoc
-#         self.nClus=nClus
-#         self.theta=0.98*np.random.random((nLoc,nClus))+0.01 # avoid bounds 0 and 1
-#         self.rho=np.ones((nLoc,1))/1000
-#         self.alpha=1.0/nClus*np.ones((nLoc,nClus))
-#         self.rhomin=rhomin
-#         self.alpha_up = alpha_up
-#         self.theta_up = theta_up
-#         self.loglike = 0
-#     def initUpdate(self):
-#         self.top=np.zeros((self.nLoc,self.nClus))
-#         self.bot=np.zeros((self.nLoc,self.nClus))
-#         self.jmk=np.zeros((self.nLoc,self.nClus))
-#         self.jm=np.zeros((self.nLoc,1))
-#         self.nhap=0.0
-#     def addIndivFit(self,t,b,j,nhap):
-#         self.top += t
-#         self.bot += b
-#         self.jmk += j
-#         self.jm  += np.reshape(np.sum(j,axis=1),(self.nLoc,1))
-#         self.nhap+=nhap
-#     def update(self):
-#         ''' Update parameters using top,bot,jmk jm probabilities'''
-#         ## rho
-#         self.rho=self.jm/self.nhap
-#         self.rho = np.where(self.rho<0, self.rhomin, self.rho)
-#         ## alpha
-#         if self.alpha_up:
-#             self.alpha = self.jmk/self.jm
-#             self.alpha = np.where( self.alpha>0.999,0.999,self.alpha)
-#             self.alpha = np.where( self.alpha<0.001,0.001,self.alpha)
-#             self.alpha /= np.sum(self.alpha, axis=1, keepdims=True)
-#         ## theta
-#         if self.theta_up:
-#             self.theta = self.top/self.bot
-#             self.theta = np.where(self.theta>0.999,0.999,self.theta)
-#             self.theta = np.where(self.theta<0.001,0.001,self.theta)
-#     def write(self,stream=sys.stdout):
-#         print("snp", *["t"+str(i) for i in range(self.nClus)], "rho", *["a"+str(i) for i in range(self.nClus)], file=stream)
-#         for i in range(self.nLoc):
-#             print(i, *[np.round( self.theta[i,k], 3) for k in range(self.nClus)], np.round( self.rho[i,0], 7), *[np.round( self.alpha[i,k], 3) for k in range(self.nClus)], file=stream)
-
-
 class fastphase():
     '''
     A class to manipulate and control a fastphase model (Scheet and Stephens, 2006)
     Initialized with a problem size = number of loci
 
     Usage : 
     with fastphase(nloc, nproc) as fph:
@@ -221,15 +166,15 @@
         '''
         try:
             assert lik.shape == (self.nLoci,3)
         except AssertionError:
             print("Wrong Array Size:", lik.shape,"is not",(self.nLoci,3))
             raise
         ##lik = np.array(lik) 
-        self.genolik[ID] = ray.put(lik - np.max(lik, axis=1,keepdims=True))
+        self.genolik[ID] = ray.put(np.exp(lik - np.max(lik, axis=1,keepdims=True)))
             
     @staticmethod
     def gen2hap(gen):
         return np.array( _tohap(np.array(gen, dtype=int)), dtype=int)
     
     def fit(self,nClus=20,nstep=20,params=None,verbose=False,rhomin=1e-6, alpha_up = True, theta_up = True, fast=False):
         '''
```

### Comparing `fastphase-2.0.dev2/fastphase/fphparams.py` & `fastphase-2.0.dev3/fastphase/fphparams.py`

 * *Files identical despite different names*

### Comparing `fastphase-2.0.dev2/fastphase/params.py` & `fastphase-2.0.dev3/fastphase/params.py`

 * *Files identical despite different names*

### Comparing `fastphase-2.0.dev2/fastphase.egg-info/PKG-INFO` & `fastphase-2.0.dev3/fastphase.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fastphase
-Version: 2.0.dev2
+Version: 2.0.dev3
 Summary: Python implementation of the fastPHASE model
 Home-page: https://forgemia.inra.fr/bertrand.servin/fastphase
 Author: Bertrand Servin
 Author-email: bertrand.servin@inrae.fr
 License: LGPL v3
 Description: # fastphase
```

### Comparing `fastphase-2.0.dev2/setup.py` & `fastphase-2.0.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 if cython:
     from Cython.Build import cythonize
     extensions = cythonize(extensions)
 
 
 setup(
     name = 'fastphase',
-    version = '2.0.dev2',
+    version = '2.0.dev3',
     description = 'Python implementation of the fastPHASE model',
     long_description = read('README.md'),
     license = "LGPL v3",
     author = "Bertrand Servin",
     author_email = "bertrand.servin@inrae.fr",
     url = "https://forgemia.inra.fr/bertrand.servin/fastphase",
     packages = ['fastphase'],
```

