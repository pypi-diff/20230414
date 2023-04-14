# Comparing `tmp/pyclesperanto_prototype-0.9.7.tar.gz` & `tmp/pyclesperanto_prototype-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyclesperanto_prototype-0.9.7.tar", last modified: Thu Jul 15 11:37:20 2021, max compression
+gzip compressed data, was "dist\pyclesperanto_prototype-0.9.9.tar", last modified: Sun Aug  1 09:36:06 2021, max compression
```

## Comparing `pyclesperanto_prototype-0.9.7.tar` & `pyclesperanto_prototype-0.9.9.tar`

### file list

```diff
@@ -1,855 +1,863 @@
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:20.525326 pyclesperanto_prototype-0.9.7/
--rw-rw-rw-   0        0        0     1687 2021-06-16 18:09:27.000000 pyclesperanto_prototype-0.9.7/LICENSE
--rw-rw-rw-   0        0        0       46 2021-06-16 18:09:27.000000 pyclesperanto_prototype-0.9.7/MANIFEST.in
--rw-rw-rw-   0        0        0    16161 2021-07-15 11:37:20.524325 pyclesperanto_prototype-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0    15527 2021-06-16 18:09:27.000000 pyclesperanto_prototype-0.9.7/README.md
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.514789 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/
--rw-rw-rw-   0        0        0      209 2021-07-15 11:36:48.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.536830 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/
--rw-rw-rw-   0        0        0     1368 2021-07-03 15:41:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/__init__.py
--rw-rw-rw-   0        0        0     1108 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_available_device_names.py
--rw-rw-rw-   0        0        0      476 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_categories.py
--rw-rw-rw-   0        0        0     7467 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_cl_image.py
--rw-rw-rw-   0        0        0     1204 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_cl_info.py
--rw-rw-rw-   0        0        0     4598 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_create.py
--rw-rw-rw-   0        0        0    11883 2021-07-03 15:40:12.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_execute.py
--rw-rw-rw-   0        0        0     2175 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_operations.py
--rw-rw-rw-   0        0        0     2805 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_plugin_function.py
--rw-rw-rw-   0        0        0      864 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_pull.py
--rw-rw-rw-   0        0        0     1309 2021-07-03 15:51:05.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_push.py
--rw-rw-rw-   0        0        0    20060 2021-07-10 19:33:27.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_pycl.py
--rw-rw-rw-   0        0        0       62 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_radius_to_kernel_size.py
--rw-rw-rw-   0        0        0      169 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_set_wait_for_kernel_finish.py
--rw-rw-rw-   0        0        0      120 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_sigma_to_kernel_size.py
--rw-rw-rw-   0        0        0      329 2021-07-03 15:51:05.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_types.py
--rw-rw-rw-   0        0        0    27062 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/preamble.cl
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.706868 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/
--rw-rw-rw-   0        0        0     7722 2021-07-10 20:34:01.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/__init__.py
--rw-rw-rw-   0        0        0     1106 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_absolute.py
--rw-rw-rw-   0        0        0     1304 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_add_image_and_scalar.py
--rw-rw-rw-   0        0        0     1729 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_add_images_weighted.py
--rw-rw-rw-   0        0        0     1187 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_average_distance_of_n_far_off_distances.py
--rw-rw-rw-   0        0        0     1190 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_average_distance_of_n_shortest_distances.py
--rw-rw-rw-   0        0        0     1307 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_average_distance_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1520 2021-07-03 17:24:16.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_and.py
--rw-rw-rw-   0        0        0     1320 2021-07-03 13:38:26.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_edge_detection.py
--rw-rw-rw-   0        0        0     1362 2021-07-03 13:38:26.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_not.py
--rw-rw-rw-   0        0        0     1500 2021-07-03 17:24:16.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_or.py
--rw-rw-rw-   0        0        0     1318 2021-07-03 17:24:16.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_subtract.py
--rw-rw-rw-   0        0        0     1579 2021-07-03 17:24:16.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_xor.py
--rw-rw-rw-   0        0        0     1148 2021-07-03 13:38:26.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_convolve.py
--rw-rw-rw-   0        0        0      875 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_copy.py
--rw-rw-rw-   0        0        0     1555 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_copy_slice.py
--rw-rw-rw-   0        0        0     1359 2021-06-26 18:47:43.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_count_touching_neighbors.py
--rw-rw-rw-   0        0        0     1713 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_crop.py
--rw-rw-rw-   0        0        0     1247 2021-07-03 13:38:26.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_detect_label_edges.py
--rw-rw-rw-   0        0        0     1561 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_detect_maxima_box.py
--rw-rw-rw-   0        0        0     1559 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_detect_minima_box.py
--rw-rw-rw-   0        0        0     1472 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_box.py
--rw-rw-rw-   0        0        0     1542 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_box_slice_by_slice.py
--rw-rw-rw-   0        0        0     1285 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_sphere.py
--rw-rw-rw-   0        0        0     1359 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_sphere_slice_by_slice.py
--rw-rw-rw-   0        0        0     1096 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_divide_images.py
--rw-rw-rw-   0        0        0     1918 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_downsample_slice_by_slice_half_median.py
--rw-rw-rw-   0        0        0     1738 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_draw_box.py
--rw-rw-rw-   0        0        0     1993 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_draw_line.py
--rw-rw-rw-   0        0        0     2078 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_draw_sphere.py
--rw-rw-rw-   0        0        0     1353 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_equal.py
--rw-rw-rw-   0        0        0     1422 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_equal_constant.py
--rw-rw-rw-   0        0        0     1465 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_box.py
--rw-rw-rw-   0        0        0     1593 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_box_slice_by_slice.py
--rw-rw-rw-   0        0        0     1279 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_sphere.py
--rw-rw-rw-   0        0        0     1407 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_sphere_slice_by_slice.py
--rw-rw-rw-   0        0        0     2163 2021-07-10 19:33:13.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_execute_separable_kernel.py
--rw-rw-rw-   0        0        0     1034 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_exponential.py
--rw-rw-rw-   0        0        0     1248 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_flip.py
--rw-rw-rw-   0        0        0     1752 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gaussian_blur.py
--rw-rw-rw-   0        0        0     2307 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_angle_matrix.py
--rw-rw-rw-   0        0        0     1535 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_binary_overlap_matrix.py
--rw-rw-rw-   0        0        0     2074 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_distance_matrix.py
--rw-rw-rw-   0        0        0     1565 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_touch_matrix.py
--rw-rw-rw-   0        0        0     1108 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gradient_x.py
--rw-rw-rw-   0        0        0     1106 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gradient_y.py
--rw-rw-rw-   0        0        0     1040 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gradient_z.py
--rw-rw-rw-   0        0        0     1127 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater.py
--rw-rw-rw-   0        0        0     1173 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater_constant.py
--rw-rw-rw-   0        0        0     1179 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater_or_equal.py
--rw-rw-rw-   0        0        0     1228 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater_or_equal_constant.py
--rw-rw-rw-   0        0        0      977 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_laplace_box.py
--rw-rw-rw-   0        0        0      985 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_laplace_diamond.py
--rw-rw-rw-   0        0        0     1026 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_logarithm.py
--rw-rw-rw-   0        0        0     1194 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mask.py
--rw-rw-rw-   0        0        0     1352 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mask_label.py
--rw-rw-rw-   0        0        0     1617 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_box.py
--rw-rw-rw-   0        0        0     1102 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_distance_of_n_shortest_distances.py
--rw-rw-rw-   0        0        0     1219 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_distance_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1168 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_image_and_scalar.py
--rw-rw-rw-   0        0        0     1125 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_images.py
--rw-rw-rw-   0        0        0     1609 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_sphere.py
--rw-rw-rw-   0        0        0     1020 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_x_projection.py
--rw-rw-rw-   0        0        0     1020 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_y_projection.py
--rw-rw-rw-   0        0        0     1036 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_z_projection.py
--rw-rw-rw-   0        0        0     1625 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_box.py
--rw-rw-rw-   0        0        0     1620 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_sphere.py
--rw-rw-rw-   0        0        0      978 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_x_projection.py
--rw-rw-rw-   0        0        0      978 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_y_projection.py
--rw-rw-rw-   0        0        0      994 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_z_projection.py
--rw-rw-rw-   0        0        0     1625 2021-07-10 20:34:01.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_median_box.py
--rw-rw-rw-   0        0        0     1643 2021-07-10 20:34:01.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_median_sphere.py
--rw-rw-rw-   0        0        0     1621 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_box.py
--rw-rw-rw-   0        0        0     1219 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_distance_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1181 2021-07-03 13:38:26.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_image_and_scalar.py
--rw-rw-rw-   0        0        0     1124 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_images.py
--rw-rw-rw-   0        0        0     1621 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_sphere.py
--rw-rw-rw-   0        0        0     1064 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_x_projection.py
--rw-rw-rw-   0        0        0     1064 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_y_projection.py
--rw-rw-rw-   0        0        0     1082 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_z_projection.py
--rw-rw-rw-   0        0        0     1182 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_image_and_coordinate.py
--rw-rw-rw-   0        0        0     1354 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_image_and_scalar.py
--rw-rw-rw-   0        0        0     1264 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_images.py
--rw-rw-rw-   0        0        0     1168 2021-07-15 11:34:49.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_matrix.py
--rw-rw-rw-   0        0        0     2439 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_n_closest_points.py
--rw-rw-rw-   0        0        0     1175 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_maximum_box.py
--rw-rw-rw-   0        0        0     1199 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_maximum_diamond.py
--rw-rw-rw-   0        0        0     1175 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_minimum_box.py
--rw-rw-rw-   0        0        0     1193 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_minimum_diamond.py
--rw-rw-rw-   0        0        0     1369 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_not_equal.py
--rw-rw-rw-   0        0        0     1414 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_not_equal_constant.py
--rw-rw-rw-   0        0        0      991 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_box.py
--rw-rw-rw-   0        0        0     1010 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_diamond.py
--rw-rw-rw-   0        0        0     1332 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_paste.py
--rw-rw-rw-   0        0        0     1123 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_point_index_list_to_mesh.py
--rw-rw-rw-   0        0        0     1145 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_point_index_list_to_touch_matrix.py
--rw-rw-rw-   0        0        0     1079 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_power.py
--rw-rw-rw-   0        0        0     1058 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_power_images.py
--rw-rw-rw-   0        0        0     1206 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_read_intensities_from_map.py
--rw-rw-rw-   0        0        0     1127 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_read_intensities_from_positions.py
--rw-rw-rw-   0        0        0     1414 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_replace_intensities.py
--rw-rw-rw-   0        0        0     1121 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_replace_intensity.py
--rw-rw-rw-   0        0        0     2619 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_resample.py
--rw-rw-rw-   0        0        0      836 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set.py
--rw-rw-rw-   0        0        0      945 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_column.py
--rw-rw-rw-   0        0        0      905 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_image_borders.py
--rw-rw-rw-   0        0        0      542 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_non_zero_pixels_to_pixel_index.py
--rw-rw-rw-   0        0        0      932 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_plane.py
--rw-rw-rw-   0        0        0      737 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_ramp_x.py
--rw-rw-rw-   0        0        0      735 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_ramp_y.py
--rw-rw-rw-   0        0        0      735 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_ramp_z.py
--rw-rw-rw-   0        0        0      910 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_row.py
--rw-rw-rw-   0        0        0      937 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_where_x_equals_y.py
--rw-rw-rw-   0        0        0      960 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_where_x_greater_than_y.py
--rw-rw-rw-   0        0        0      958 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_where_x_smaller_than_y.py
--rw-rw-rw-   0        0        0     1125 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller.py
--rw-rw-rw-   0        0        0     1172 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller_constant.py
--rw-rw-rw-   0        0        0     1178 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller_or_equal.py
--rw-rw-rw-   0        0        0     1227 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller_or_equal_constant.py
--rw-rw-rw-   0        0        0      983 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sobel.py
--rw-rw-rw-   0        0        0     1081 2021-07-10 19:31:23.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_standard_deviation_z_projection.py
--rw-rw-rw-   0        0        0     1137 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_subtract_image_from_scalar.py
--rw-rw-rw-   0        0        0     1008 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sum_x_projection.py
--rw-rw-rw-   0        0        0      964 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sum_y_projection.py
--rw-rw-rw-   0        0        0      992 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sum_z_projection.py
--rw-rw-rw-   0        0        0     1616 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_touch_matrix_to_mesh.py
--rw-rw-rw-   0        0        0     1409 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_transpose_xy.py
--rw-rw-rw-   0        0        0     1386 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_transpose_xz.py
--rw-rw-rw-   0        0        0     1419 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_transpose_yz.py
--rw-rw-rw-   0        0        0      927 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_undefined_to_zero.py
--rw-rw-rw-   0        0        0     1556 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_variance_box.py
--rw-rw-rw-   0        0        0     1571 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_variance_sphere.py
--rw-rw-rw-   0        0        0     1682 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_write_values_to_positions.py
--rw-rw-rw-   0        0        0     1889 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/maximum_distance_of_n_shortest_distances_x.cl
--rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/maximum_distance_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/minimum_distance_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0     1183 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/point_index_list_to_touch_matrix_x.cl
--rw-rw-rw-   0        0        0      730 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/read_intensities_from_map_x.cl
--rw-rw-rw-   0        0        0      929 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/read_intensities_from_positions_x.cl
--rw-rw-rw-   0        0        0     1043 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_box_2d_x.cl
--rw-rw-rw-   0        0        0     1527 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_box_3d_x.cl
--rw-rw-rw-   0        0        0     1496 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     2195 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_sphere_3d_x.cl
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.749953 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/
--rw-rw-rw-   0        0        0     2388 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/__init__.py
--rw-rw-rw-   0        0        0      862 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_add_images.py
--rw-rw-rw-   0        0        0     1476 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_block_enumerate.py
--rw-rw-rw-   0        0        0     1568 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_bottom_hat_box.py
--rw-rw-rw-   0        0        0     1591 2021-07-03 17:26:12.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_bottom_hat_sphere.py
--rw-rw-rw-   0        0        0     1091 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_combine_horizontally.py
--rw-rw-rw-   0        0        0     1087 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_combine_vertically.py
--rw-rw-rw-   0        0        0      964 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_concatenate_stacks.py
--rw-rw-rw-   0        0        0      346 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_degrees_to_radians.py
--rw-rw-rw-   0        0        0     1413 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_distance_matrix_to_mesh.py
--rw-rw-rw-   0        0        0     1204 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_flag_existing_labels.py
--rw-rw-rw-   0        0        0     1207 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_gamma_correction.py
--rw-rw-rw-   0        0        0      976 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_invert.py
--rw-rw-rw-   0        0        0     1826 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_label_spots.py
--rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_maximum_of_all_pixels.py
--rw-rw-rw-   0        0        0     1728 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_maximum_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1705 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_mean_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1438 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_median_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1433 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_minimum_of_all_pixels.py
--rw-rw-rw-   0        0        0     2928 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_minimum_of_masked_pixels.py
--rw-rw-rw-   0        0        0     1728 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_minimum_of_touching_neighbors.py
--rw-rw-rw-   0        0        0      978 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_mode_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1079 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_neighbors_of_neighbors.py
--rw-rw-rw-   0        0        0     1285 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_pointlist_to_labelled_spots.py
--rw-rw-rw-   0        0        0      346 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_radians_to_degrees.py
--rw-rw-rw-   0        0        0     1452 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_reduce_stack.py
--rw-rw-rw-   0        0        0     1569 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_standard_deviation_of_touching_neighbors.py
--rw-rw-rw-   0        0        0     1388 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_sub_stack.py
--rw-rw-rw-   0        0        0      862 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_subtract_images.py
--rw-rw-rw-   0        0        0     1374 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_sum_of_all_pixels.py
--rw-rw-rw-   0        0        0     1150 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_sum_reduction_x.py
--rw-rw-rw-   0        0        0     1557 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_top_hat_box.py
--rw-rw-rw-   0        0        0     1566 2021-07-03 17:26:12.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_top_hat_sphere.py
--rw-rw-rw-   0        0        0     1375 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_touch_matrix_to_adjacency_matrix.py
--rw-rw-rw-   0        0        0     1000 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_z_position_of_maximum_z_projection.py
--rw-rw-rw-   0        0        0     1013 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_z_position_of_minimum_z_projection.py
--rw-rw-rw-   0        0        0     1029 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_z_position_projection.py
--rw-rw-rw-   0        0        0      652 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/z_position_of_maximum_z_projection_x.cl
--rw-rw-rw-   0        0        0      652 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/z_position_of_minimum_z_projection_x.cl
--rw-rw-rw-   0        0        0      558 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/z_position_projection_x.cl
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.795964 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/
--rw-rw-rw-   0        0        0     3434 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/__init__.py
--rw-rw-rw-   0        0        0     1253 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_absolute_difference.py
--rw-rw-rw-   0        0        0     1628 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_bounding_box.py
--rw-rw-rw-   0        0        0     1107 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_center_of_mass.py
--rw-rw-rw-   0        0        0     1932 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_close_index_gaps_in_label_map.py
--rw-rw-rw-   0        0        0     2072 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_difference_of_gaussian.py
--rw-rw-rw-   0        0        0     1082 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_divide_by_gaussian_background.py
--rw-rw-rw-   0        0        0     1806 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels.py
--rw-rw-rw-   0        0        0     2841 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_on_edges.py
--rw-rw-rw-   0        0        0     1621 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_outside_size_range.py
--rw-rw-rw-   0        0        0     1599 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_out_of_range.py
--rw-rw-rw-   0        0        0     1672 2021-06-26 14:06:03.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_within_range.py
--rw-rw-rw-   0        0        0     2115 2021-06-26 18:47:43.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_generate_n_nearest_neighbors_matrix.py
--rw-rw-rw-   0        0        0     1875 2021-06-26 18:47:43.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_generate_proximal_neighbors_matrix.py
--rw-rw-rw-   0        0        0     5290 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_histogram.py
--rw-rw-rw-   0        0        0     1297 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_jaccard_index.py
--rw-rw-rw-   0        0        0     1390 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_labelled_spots_to_pointlist.py
--rw-rw-rw-   0        0        0     2026 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_maximum_of_n_nearest_neighbors_map.py
--rw-rw-rw-   0        0        0     2230 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_maximum_of_proximal_neighbors_map.py
--rw-rw-rw-   0        0        0     2275 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_maximum_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0      895 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_all_pixels.py
--rw-rw-rw-   0        0        0     2011 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_n_nearest_neighbors_map.py
--rw-rw-rw-   0        0        0     2215 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_proximal_neighbors_map.py
--rw-rw-rw-   0        0        0     2240 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0     1898 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_minimum_of_n_nearest_neighbors_map.py
--rw-rw-rw-   0        0        0     2102 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_minimum_of_proximal_neighbors_map.py
--rw-rw-rw-   0        0        0     2275 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_minimum_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0     1805 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mode_of_n_nearest_neighbors_map.py
--rw-rw-rw-   0        0        0     2009 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mode_of_proximal_neighbors_map.py
--rw-rw-rw-   0        0        0     2225 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mode_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0     1046 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_squared_difference.py
--rw-rw-rw-   0        0        0     1874 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_standard_deviation_of_n_nearest_neighbors_map.py
--rw-rw-rw-   0        0        0     2078 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_standard_deviation_of_proximal_neighbors_map.py
--rw-rw-rw-   0        0        0     2288 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_standard_deviation_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0     1081 2021-07-10 20:32:04.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_subtract_gaussian_background.py
--rw-rw-rw-   0        0        0     1596 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_z_position_range_projection.py
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.822101 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/
--rw-rw-rw-   0        0        0     1323 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/__init__.py
--rw-rw-rw-   0        0        0     2087 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_connected_components_labeling_box.py
--rw-rw-rw-   0        0        0     1813 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_extend_labeling_via_voronoi.py
--rw-rw-rw-   0        0        0     1297 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_extend_labels_with_maximum_radius.py
--rw-rw-rw-   0        0        0     1312 2021-07-10 19:34:56.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_extended_depth_of_focus_variance_projection.py
--rw-rw-rw-   0        0        0     1283 2021-07-10 20:56:46.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_maximum_touching_neighbor_count_map.py
--rw-rw-rw-   0        0        0     1268 2021-07-10 20:56:46.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_mean_touching_neighbor_count_map.py
--rw-rw-rw-   0        0        0     1278 2021-07-10 20:56:46.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_median_touching_neighbor_count_map.py
--rw-rw-rw-   0        0        0     1283 2021-07-10 20:56:46.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_minimum_touching_neighbor_count_map.py
--rw-rw-rw-   0        0        0     1314 2021-07-10 20:56:46.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_standard_deviation_touching_neighbor_count_map.py
--rw-rw-rw-   0        0        0      880 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_mean_squared_error.py
--rw-rw-rw-   0        0        0     2950 2021-07-03 13:40:04.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_merge_touching_labels.py
--rw-rw-rw-   0        0        0     1737 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_proximal_neighbor_count_map.py
--rw-rw-rw-   0        0        0     1015 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_sorensen_dice_coefficient.py
--rw-rw-rw-   0        0        0     1080 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_spots_to_pointlist.py
--rw-rw-rw-   0        0        0     1141 2021-06-26 18:47:43.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_touching_neighbor_count_map.py
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.825970 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/
--rw-rw-rw-   0        0        0      205 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/__init__.py
--rw-rw-rw-   0        0        0     1158 2021-07-03 13:27:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/_connected_components_labeling_diamond.py
--rw-rw-rw-   0        0        0     2359 2021-07-03 13:53:23.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/_masked_voronoi_labeling.py
--rw-rw-rw-   0        0        0     1182 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/_voronoi_labeling.py
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.838973 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/
--rw-rw-rw-   0        0        0     6024 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_AffineTransform3D.py
--rw-rw-rw-   0        0        0      295 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/__init__.py
--rw-rw-rw-   0        0        0     3278 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_affine_transform.py
--rw-rw-rw-   0        0        0     2148 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_apply_vector_field.py
--rw-rw-rw-   0        0        0     2335 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_rigid_transform.py
--rw-rw-rw-   0        0        0     1974 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_rotate.py
--rw-rw-rw-   0        0        0     1451 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_scale.py
--rw-rw-rw-   0        0        0     1212 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_translate.py
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.885984 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/
--rw-rw-rw-   0        0        0     2960 2021-06-26 20:45:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/__init__.py
--rw-rw-rw-   0        0        0     1790 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_artificial_tissue_2d.py
--rw-rw-rw-   0        0        0     1220 2021-07-03 13:34:22.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_average_distance_of_n_closest_neighbors_map.py
--rw-rw-rw-   0        0        0     1337 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_average_neighbor_distance_map.py
--rw-rw-rw-   0        0        0      396 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_centroids_of_background_and_labels.py
--rw-rw-rw-   0        0        0     3675 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_centroids_of_labels.py
--rw-rw-rw-   0        0        0     1558 2021-07-03 18:34:21.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_angle_mesh_between_touching_labels.py
--rw-rw-rw-   0        0        0     1564 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_distance_mesh_between_touching_labels.py
--rw-rw-rw-   0        0        0     1556 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_mesh_between_n_closest_labels.py
--rw-rw-rw-   0        0        0     1421 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_mesh_between_proximal_labels.py
--rw-rw-rw-   0        0        0     1180 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_mesh_between_touching_labels.py
--rw-rw-rw-   0        0        0     1292 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_euclidean_distance_from_label_centroid_map.py
--rw-rw-rw-   0        0        0      206 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_imread.py
--rw-rw-rw-   0        0        0      951 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_imshow.py
--rw-rw-rw-   0        0        0     1163 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_maximum_extension_map.py
--rw-rw-rw-   0        0        0     1333 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_maximum_extension_ratio_map.py
--rw-rw-rw-   0        0        0     1312 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_maximum_intensity_map.py
--rw-rw-rw-   0        0        0     1160 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_mean_extension_map.py
--rw-rw-rw-   0        0        0     1290 2021-07-10 20:59:45.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_mean_intensity_map.py
--rw-rw-rw-   0        0        0     1317 2021-07-10 21:04:08.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_minimum_intensity_map.py
--rw-rw-rw-   0        0        0     1167 2021-07-10 21:00:27.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_pixel_count_map.py
--rw-rw-rw-   0        0        0     1443 2021-07-10 21:01:20.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_standard_deviation_intensity_map.py
--rw-rw-rw-   0        0        0     9912 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_push_regionprops.py
--rw-rw-rw-   0        0        0      790 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_push_regionprops_column.py
--rw-rw-rw-   0        0        0     1965 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_regionprops.py
--rw-rw-rw-   0        0        0     1435 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_entry.py
--rw-rw-rw-   0        0        0     1522 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_of_background_and_labelled_pixels.py
--rw-rw-rw-   0        0        0     1139 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_of_image.py
--rw-rw-rw-   0        0        0    11805 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_of_labelled_pixels.py
--rw-rw-rw-   0        0        0     3548 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_threshold_otsu.py
--rw-rw-rw-   0        0        0     2465 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_voronoi_otsu_labeling.py
--rw-rw-rw-   0        0        0     4429 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/standard_deviation_per_label_x.cl
--rw-rw-rw-   0        0        0     5287 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/statistics_per_label_x.cl
--rw-rw-rw-   0        0        0     1689 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/sum_per_label_x.cl
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.509789 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:20.259239 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/
--rw-rw-rw-   0        0        0      512 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_2d_x.cl
--rw-rw-rw-   0        0        0      551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_3d_x.cl
--rw-rw-rw-   0        0        0      486 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_image_and_scalar_2d_x.cl
--rw-rw-rw-   0        0        0      524 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_image_and_scalar_3d_x.cl
--rw-rw-rw-   0        0        0      564 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_2d_x.cl
--rw-rw-rw-   0        0        0      656 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_3d_x.cl
--rw-rw-rw-   0        0        0     2691 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_interpolate_x.cl
--rw-rw-rw-   0        0        0     2847 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_x.cl
--rw-rw-rw-   0        0        0     3265 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_interpolate_x.cl
--rw-rw-rw-   0        0        0     3427 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_x.cl
--rw-rw-rw-   0        0        0     1256 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_interpolate_x.cl
--rw-rw-rw-   0        0        0     1226 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_x.cl
--rw-rw-rw-   0        0        0     1541 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_interpolate_x.cl
--rw-rw-rw-   0        0        0     1506 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_x.cl
--rw-rw-rw-   0        0        0      771 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/arg_maximum_z_projection_x.cl
--rw-rw-rw-   0        0        0     1865 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_far_off_distances_x.cl
--rw-rw-rw-   0        0        0     1863 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_shortest_distances_x.cl
--rw-rw-rw-   0        0        0     1483 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      660 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_2d_x.cl
--rw-rw-rw-   0        0        0      699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_3d_x.cl
--rw-rw-rw-   0        0        0     1143 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_2d_x.cl
--rw-rw-rw-   0        0        0     1597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_3d_x.cl
--rw-rw-rw-   0        0        0      522 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_2d_x.cl
--rw-rw-rw-   0        0        0      561 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_3d_x.cl
--rw-rw-rw-   0        0        0      661 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_2d_x.cl
--rw-rw-rw-   0        0        0      700 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_3d_x.cl
--rw-rw-rw-   0        0        0      589 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_2d_x.cl
--rw-rw-rw-   0        0        0      628 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_3d_x.cl
--rw-rw-rw-   0        0        0      695 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_2d_x.cl
--rw-rw-rw-   0        0        0      732 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_3d_x.cl
--rw-rw-rw-   0        0        0      903 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/block_enumerate_x.cl
--rw-rw-rw-   0        0        0      921 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_2d_x.cl
--rw-rw-rw-   0        0        0     1096 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_3d_x.cl
--rw-rw-rw-   0        0        0      418 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_2d_x.cl
--rw-rw-rw-   0        0        0      459 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_3d_x.cl
--rw-rw-rw-   0        0        0      493 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_slice_from_3d_x.cl
--rw-rw-rw-   0        0        0      492 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_slice_to_3d_x.cl
--rw-rw-rw-   0        0        0      689 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_non_zero_projection_3d_2d_x.cl
--rw-rw-rw-   0        0        0     1271 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_slice_by_slice_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1193 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     1677 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_voxels_sphere_3d_x.cl
--rw-rw-rw-   0        0        0      982 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      613 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_2d_x.cl
--rw-rw-rw-   0        0        0      702 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_3d_x.cl
--rw-rw-rw-   0        0        0     1842 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_interpolation_x.cl
--rw-rw-rw-   0        0        0     1764 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_x.cl
--rw-rw-rw-   0        0        0     1229 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_2d_x.cl
--rw-rw-rw-   0        0        0     1697 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_3d_x.cl
--rw-rw-rw-   0        0        0      936 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_2d_x.cl
--rw-rw-rw-   0        0        0     1002 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_slice_by_slice_x.cl
--rw-rw-rw-   0        0        0     1417 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_x.cl
--rw-rw-rw-   0        0        0      936 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_2d_x.cl
--rw-rw-rw-   0        0        0     1008 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_slice_by_slice_x.cl
--rw-rw-rw-   0        0        0     1100 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_x.cl
--rw-rw-rw-   0        0        0      772 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_2d_x.cl
--rw-rw-rw-   0        0        0      936 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_3d_x.cl
--rw-rw-rw-   0        0        0      832 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_slice_by_slice_3d_x.cl
--rw-rw-rw-   0        0        0      882 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     1200 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_3d_x.cl
--rw-rw-rw-   0        0        0      962 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_slice_by_slice_3d_x.cl
--rw-rw-rw-   0        0        0     2441 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distance_matrix_to_mesh_x.cl
--rw-rw-rw-   0        0        0      894 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_2d_x.cl
--rw-rw-rw-   0        0        0     1001 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_3d_x.cl
--rw-rw-rw-   0        0        0     1051 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1323 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      511 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/divide_images_2d_x.cl
--rw-rw-rw-   0        0        0      551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/divide_images_3d_x.cl
--rw-rw-rw-   0        0        0      518 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_2d_x.cl
--rw-rw-rw-   0        0        0      616 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_3d_x.cl
--rw-rw-rw-   0        0        0     2147 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_xy_by_half_median_3d_x.cl
--rw-rw-rw-   0        0        0      459 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_box_2d_x.cl
--rw-rw-rw-   0        0        0      604 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_box_3d_x.cl
--rw-rw-rw-   0        0        0      606 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_2d_x.cl
--rw-rw-rw-   0        0        0      807 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1000 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_2d_x.cl
--rw-rw-rw-   0        0        0     1277 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_3d_x.cl
--rw-rw-rw-   0        0        0     1414 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_2d_x.cl
--rw-rw-rw-   0        0        0     1567 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_3d_x.cl
--rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_2d_x.cl
--rw-rw-rw-   0        0        0      633 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_3d_x.cl
--rw-rw-rw-   0        0        0      524 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_2d_x.cl
--rw-rw-rw-   0        0        0      564 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_3d_x.cl
--rw-rw-rw-   0        0        0      774 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_2d_x.cl
--rw-rw-rw-   0        0        0      937 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_3d_x.cl
--rw-rw-rw-   0        0        0      832 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_slice_by_slice_3d_x.cl
--rw-rw-rw-   0        0        0      882 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     1198 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_3d_x.cl
--rw-rw-rw-   0        0        0      960 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_slice_by_slice_3d_x.cl
--rw-rw-rw-   0        0        0     1247 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/euclidean_distance_from_label_centroid_map_x.cl
--rw-rw-rw-   0        0        0     2537 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/excludeLabelsOnEdges_3d_x.cl
--rw-rw-rw-   0        0        0     2537 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_edges_3d_x.cl
--rw-rw-rw-   0        0        0     2485 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_2d_x.cl
--rw-rw-rw-   0        0        0     2335 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_3d_x.cl
--rw-rw-rw-   0        0        0     2485 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_2d_x.cl
--rw-rw-rw-   0        0        0     2335 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_3d_x.cl
--rw-rw-rw-   0        0        0      491 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exponential_2d_x.cl
--rw-rw-rw-   0        0        0      530 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exponential_3d_x.cl
--rw-rw-rw-   0        0        0      441 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flag_existing_labels_x.cl
--rw-rw-rw-   0        0        0      747 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_2d_x.cl
--rw-rw-rw-   0        0        0      935 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_3d_x.cl
--rw-rw-rw-   0        0        0     1887 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flood_fill_diamond_x.cl
--rw-rw-rw-   0        0        0      906 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_2d_x.cl
--rw-rw-rw-   0        0        0      949 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_3d_x.cl
--rw-rw-rw-   0        0        0     1285 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_angle_matrix_2d_x.cl
--rw-rw-rw-   0        0        0      693 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_2d_x.cl
--rw-rw-rw-   0        0        0      728 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_3d_x.cl
--rw-rw-rw-   0        0        0     1113 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_distance_matrix_x.cl
--rw-rw-rw-   0        0        0     1403 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_2d_x.cl
--rw-rw-rw-   0        0        0     1931 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_3d_x.cl
--rw-rw-rw-   0        0        0      597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_2d_x.cl
--rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_3d_x.cl
--rw-rw-rw-   0        0        0      591 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_2d_x.cl
--rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_3d_x.cl
--rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_z_3d_x.cl
--rw-rw-rw-   0        0        0      594 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_2d_x.cl
--rw-rw-rw-   0        0        0      634 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_3d_x.cl
--rw-rw-rw-   0        0        0      525 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_2d_x.cl
--rw-rw-rw-   0        0        0      565 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_3d_x.cl
--rw-rw-rw-   0        0        0      604 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_2d_x.cl
--rw-rw-rw-   0        0        0      644 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_3d_x.cl
--rw-rw-rw-   0        0        0      535 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_2d_x.cl
--rw-rw-rw-   0        0        0      575 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_3d_x.cl
--rw-rw-rw-   0        0        0     1847 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_2d_x.cl
--rw-rw-rw-   0        0        0     1999 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_3d_x.cl
--rw-rw-rw-   0        0        0      987 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/label_spots_in_x.cl
--rw-rw-rw-   0        0        0     1024 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/labelled_spots_to_point_list_x.cl
--rw-rw-rw-   0        0        0     1348 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_2d_x.cl
--rw-rw-rw-   0        0        0      810 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_3d_x.cl
--rw-rw-rw-   0        0        0      926 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1225 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      489 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/logarithm_2d_x.cl
--rw-rw-rw-   0        0        0      528 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/logarithm_3d_x.cl
--rw-rw-rw-   0        0        0      537 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_2d_x.cl
--rw-rw-rw-   0        0        0      576 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_3d_x.cl
--rw-rw-rw-   0        0        0      619 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_2d_x.cl
--rw-rw-rw-   0        0        0      658 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_3d_x.cl
--rw-rw-rw-   0        0        0      636 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_stack_with_plane_3d_x.cl
--rw-rw-rw-   0        0        0     8736 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/matrix_multiply_float_buffer.cl
--rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_distance_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      557 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_2d_x.cl
--rw-rw-rw-   0        0        0      596 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_3d_x.cl
--rw-rw-rw-   0        0        0      618 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_2d_x.cl
--rw-rw-rw-   0        0        0      626 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_3d_x.cl
--rw-rw-rw-   0        0        0     1391 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_2d_x.cl
--rw-rw-rw-   0        0        0      770 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_3d_x.cl
--rw-rw-rw-   0        0        0      919 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1231 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      950 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_masked_pixels_3d_2d_x.cl
--rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      549 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_projection_3d_2d_x.cl
--rw-rw-rw-   0        0        0      699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_2d_x.cl
--rw-rw-rw-   0        0        0      699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_3d_x.cl
--rw-rw-rw-   0        0        0     1297 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_slice_by_slice_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1277 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     1695 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_3d_x.cl
--rw-rw-rw-   0        0        0      592 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_x_projection_x.cl
--rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_y_projection_x.cl
--rw-rw-rw-   0        0        0      740 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_bounded_3d_2d_x.cl
--rw-rw-rw-   0        0        0      652 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_x.cl
--rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      683 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_2d_x.cl
--rw-rw-rw-   0        0        0      752 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_3d_x.cl
--rw-rw-rw-   0        0        0     1103 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_slice_by_slice_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1043 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     1496 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_3d_x.cl
--rw-rw-rw-   0        0        0      542 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_x_projection_x.cl
--rw-rw-rw-   0        0        0      543 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_y_projection_x.cl
--rw-rw-rw-   0        0        0      759 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_bounded_3d_2d_x.cl
--rw-rw-rw-   0        0        0      545 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_x.cl
--rw-rw-rw-   0        0        0     1418 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_2d_x.cl
--rw-rw-rw-   0        0        0     1732 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_3d_x.cl
--rw-rw-rw-   0        0        0     1907 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0     1511 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_box_3d_x.cl
--rw-rw-rw-   0        0        0     1616 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1619 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     2120 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1125 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_z_projection_x.cl
--rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_distance_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      564 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_2d_x.cl
--rw-rw-rw-   0        0        0      596 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_3d_x.cl
--rw-rw-rw-   0        0        0      587 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_2d_x.cl
--rw-rw-rw-   0        0        0      626 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_3d_x.cl
--rw-rw-rw-   0        0        0     1391 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_2d_x.cl
--rw-rw-rw-   0        0        0      770 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_3d_x.cl
--rw-rw-rw-   0        0        0      919 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1231 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      950 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_masked_pixels_3d_2d_x.cl
--rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      549 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_projection_3d_2d_x.cl
--rw-rw-rw-   0        0        0      701 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_2d_x.cl
--rw-rw-rw-   0        0        0      697 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_3d_x.cl
--rw-rw-rw-   0        0        0     1299 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_slice_by_slice_sphere_3d_x.cl
--rw-rw-rw-   0        0        0     1399 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_2d_x.cl
--rw-rw-rw-   0        0        0     1695 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_3d_x.cl
--rw-rw-rw-   0        0        0      592 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_x_projection_x.cl
--rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_y_projection_x.cl
--rw-rw-rw-   0        0        0      757 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_bounded_3d_2d_x.cl
--rw-rw-rw-   0        0        0      892 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_thresholded_bounded_3d_2d_x.cl
--rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_x.cl
--rw-rw-rw-   0        0        0     1643 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mode_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      516 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_2d_x.cl
--rw-rw-rw-   0        0        0      552 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_3d_x.cl
--rw-rw-rw-   0        0        0      491 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_scalar_2d_x.cl
--rw-rw-rw-   0        0        0      529 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_scalar_3d_x.cl
--rw-rw-rw-   0        0        0      514 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_2d_x.cl
--rw-rw-rw-   0        0        0      551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_3d_x.cl
--rw-rw-rw-   0        0        0      696 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_matrix_x.cl
--rw-rw-rw-   0        0        0      617 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_plane_3d_x.cl
--rw-rw-rw-   0        0        0      739 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_scalars_x.cl
--rw-rw-rw-   0        0        0     1851 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_distances_x.cl
--rw-rw-rw-   0        0        0     1644 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_points_x.cl
--rw-rw-rw-   0        0        0      955 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_2d_x.cl
--rw-rw-rw-   0        0        0     1699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_3d_x.cl
--rw-rw-rw-   0        0        0     1309 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1701 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      953 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_2d_x.cl
--rw-rw-rw-   0        0        0     1066 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_3d_x.cl
--rw-rw-rw-   0        0        0     1309 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1701 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_2d_x.cl
--rw-rw-rw-   0        0        0      637 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_3d_x.cl
--rw-rw-rw-   0        0        0      528 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_2d_x.cl
--rw-rw-rw-   0        0        0      568 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_3d_x.cl
--rw-rw-rw-   0        0        0     1985 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_2d_x.cl
--rw-rw-rw-   0        0        0     1015 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_3d_x.cl
--rw-rw-rw-   0        0        0     1320 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_2d_x.cl
--rw-rw-rw-   0        0        0     1712 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_3d_x.cl
--rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_2d_x.cl
--rw-rw-rw-   0        0        0      782 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_3d_x.cl
--rw-rw-rw-   0        0        0     3756 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/piv.cl
--rw-rw-rw-   0        0        0     2160 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/pointindexlist_to_mesh_3d_x.cl
--rw-rw-rw-   0        0        0      526 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_2d_x.cl
--rw-rw-rw-   0        0        0      565 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_3d_x.cl
--rw-rw-rw-   0        0        0      540 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_2d_x.cl
--rw-rw-rw-   0        0        0      579 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_3d_x.cl
--rw-rw-rw-   0        0        0      666 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensities_x.cl
--rw-rw-rw-   0        0        0      806 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensity_x.cl
--rw-rw-rw-   0        0        0      710 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_pixels_if_zero_x.cl
--rw-rw-rw-   0        0        0      717 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_bottom_3d_x.cl
--rw-rw-rw-   0        0        0      691 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_left_3d_x.cl
--rw-rw-rw-   0        0        0     1341 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_2d_x.cl
--rw-rw-rw-   0        0        0     1353 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_3d_x.cl
--rw-rw-rw-   0        0        0      718 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_right_3d_x.cl
--rw-rw-rw-   0        0        0      689 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_top_3d_x.cl
--rw-rw-rw-   0        0        0      634 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_2d_x.cl
--rw-rw-rw-   0        0        0      714 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_3d_x.cl
--rw-rw-rw-   0        0        0      637 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_2d_x.cl
--rw-rw-rw-   0        0        0      720 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_3d_x.cl
--rw-rw-rw-   0        0        0      218 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_2d_x.cl
--rw-rw-rw-   0        0        0      260 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_3d_x.cl
--rw-rw-rw-   0        0        0      232 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_column_2d_x.cl
--rw-rw-rw-   0        0        0      274 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_column_3d_x.cl
--rw-rw-rw-   0        0        0      347 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_image_borders_2d_x.cl
--rw-rw-rw-   0        0        0      425 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_image_borders_3d_x.cl
--rw-rw-rw-   0        0        0      756 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_nonzero_pixels_to_pixelindex_x.cl
--rw-rw-rw-   0        0        0      275 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_plane_2d_x.cl
--rw-rw-rw-   0        0        0      271 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_plane_3d_x.cl
--rw-rw-rw-   0        0        0      206 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_x_2d_x.cl
--rw-rw-rw-   0        0        0      245 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_x_3d_x.cl
--rw-rw-rw-   0        0        0      206 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_y_2d_x.cl
--rw-rw-rw-   0        0        0      245 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_y_3d_x.cl
--rw-rw-rw-   0        0        0      182 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_z_2d_x.cl
--rw-rw-rw-   0        0        0      245 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_z_3d_x.cl
--rw-rw-rw-   0        0        0      223 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_row_2d_x.cl
--rw-rw-rw-   0        0        0      265 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_row_3d_x.cl
--rw-rw-rw-   0        0        0      254 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_equals_y_2d_x.cl
--rw-rw-rw-   0        0        0      290 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_equals_y_3d_x.cl
--rw-rw-rw-   0        0        0      259 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_greater_than_y_2d_x.cl
--rw-rw-rw-   0        0        0      299 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_greater_than_y_3d_x.cl
--rw-rw-rw-   0        0        0      259 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_smaller_than_y_2d_x.cl
--rw-rw-rw-   0        0        0      300 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_smaller_than_y_3d_x.cl
--rw-rw-rw-   0        0        0      594 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_2d_x.cl
--rw-rw-rw-   0        0        0      634 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_3d_x.cl
--rw-rw-rw-   0        0        0      525 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_2d_x.cl
--rw-rw-rw-   0        0        0      565 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_3d_x.cl
--rw-rw-rw-   0        0        0      604 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_2d_x.cl
--rw-rw-rw-   0        0        0      644 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_3d_x.cl
--rw-rw-rw-   0        0        0      535 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_2d_x.cl
--rw-rw-rw-   0        0        0      575 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_3d_x.cl
--rw-rw-rw-   0        0        0     1612 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_2d_x.cl
--rw-rw-rw-   0        0        0     1550 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_3d_x.cl
--rw-rw-rw-   0        0        0     2597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_of_touching_neighbors_x.cl
--rw-rw-rw-   0        0        0      847 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_z_projection_x.cl
--rw-rw-rw-   0        0        0      492 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/subtract_image_from_scalar_2d_x.cl
--rw-rw-rw-   0        0        0      531 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/subtract_image_from_scalar_3d_x.cl
--rw-rw-rw-   0        0        0      567 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_reduction_x_x.cl
--rw-rw-rw-   0        0        0      504 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_x_projection_x.cl
--rw-rw-rw-   0        0        0      505 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_y_projection_x.cl
--rw-rw-rw-   0        0        0      504 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_z_projection_x.cl
--rw-rw-rw-   0        0        0     2224 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/touch_matrix_to_mesh_3d_x.cl
--rw-rw-rw-   0        0        0      553 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xy_3d_x.cl
--rw-rw-rw-   0        0        0      547 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xz_3d_x.cl
--rw-rw-rw-   0        0        0      545 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_yz_3d_x.cl
--rw-rw-rw-   0        0        0      531 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/undefined_to_zero_x.cl
--rw-rw-rw-   0        0        0      599 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_2d_x.cl
--rw-rw-rw-   0        0        0      725 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_masked_projection_x.cl
--rw-rw-rw-   0        0        0      581 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_projection_x.cl
--rw-rw-rw-   0        0        0     1051 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_2d_x.cl
--rw-rw-rw-   0        0        0     1186 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_3d_x.cl
--rw-rw-rw-   0        0        0     1091 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_2d.cl
--rw-rw-rw-   0        0        0     1215 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_3d.cl
--rw-rw-rw-   0        0        0     1421 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_2d_x.cl
--rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_3d_x.cl
--rw-rw-rw-   0        0        0     1594 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_2d_x.cl
--rw-rw-rw-   0        0        0     1704 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_3d_x.cl
--rw-rw-rw-   0        0        0      712 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_2d_x.cl
--rw-rw-rw-   0        0        0      804 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_3d_x.cl
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:19.520826 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/
--rw-rw-rw-   0        0        0    16161 2021-07-15 11:37:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    48913 2021-07-15 11:37:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-15 11:37:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2021-07-15 11:37:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2021-07-15 11:37:19.000000 pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-07-15 11:37:20.525326 pyclesperanto_prototype-0.9.7/setup.cfg
--rw-rw-rw-   0        0        0      963 2021-07-15 11:36:48.000000 pyclesperanto_prototype-0.9.7/setup.py
-drwxrwxrwx   0        0        0        0 2021-07-15 11:37:20.523326 pyclesperanto_prototype-0.9.7/tests/
--rw-rw-rw-   0        0        0      187 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/__init__.py
--rw-rw-rw-   0        0        0      544 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_absolute.py
--rw-rw-rw-   0        0        0      346 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_absolute_difference.py
--rw-rw-rw-   0        0        0      624 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_add_image_and_scalar.py
--rw-rw-rw-   0        0        0     1279 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_add_images.py
--rw-rw-rw-   0        0        0     1915 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_add_images_weighted.py
--rw-rw-rw-   0        0        0     3596 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_affine_transform.py
--rw-rw-rw-   0        0        0     4708 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_apply_vector_field.py
--rw-rw-rw-   0        0        0      902 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_average_distance_of_n_far_off_distances.py
--rw-rw-rw-   0        0        0      894 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_average_distance_of_n_shortest_distances.py
--rw-rw-rw-   0        0        0      951 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_average_distance_of_touching_neighbors.py
--rw-rw-rw-   0        0        0      749 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_binary_and.py
--rw-rw-rw-   0        0        0      541 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_binary_edge_detection.py
--rw-rw-rw-   0        0        0      367 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_binary_not.py
--rw-rw-rw-   0        0        0      448 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_binary_or.py
--rw-rw-rw-   0        0        0      460 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_binary_subtract.py
--rw-rw-rw-   0        0        0      449 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_binary_xor.py
--rw-rw-rw-   0        0        0      926 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_block_enumerate.py
--rw-rw-rw-   0        0        0      466 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_bottom_hat_box.py
--rw-rw-rw-   0        0        0      469 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_bottom_hat_sphere.py
--rw-rw-rw-   0        0        0      947 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_bounding_box.py
--rw-rw-rw-   0        0        0      310 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_center_of_mass.py
--rw-rw-rw-   0        0        0     1233 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_centroids_of_labels.py
--rw-rw-rw-   0        0        0      638 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_close_index_gaps_in_label_maps.py
--rw-rw-rw-   0        0        0      542 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_combine_horizontally.py
--rw-rw-rw-   0        0        0      548 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_combine_vertically.py
--rw-rw-rw-   0        0        0      783 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_concatenate_stacks.py
--rw-rw-rw-   0        0        0     1633 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_connected_components_labeling_box.py
--rw-rw-rw-   0        0        0      631 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_connected_components_labeling_diamond.py
--rw-rw-rw-   0        0        0      547 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_convolve.py
--rw-rw-rw-   0        0        0      357 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_copy.py
--rw-rw-rw-   0        0        0     2464 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_copy_slice.py
--rw-rw-rw-   0        0        0      696 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_count_touching_neighbors.py
--rw-rw-rw-   0        0        0     3313 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_create.py
--rw-rw-rw-   0        0        0     1194 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_crop.py
--rw-rw-rw-   0        0        0      383 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_degrees_to_radians.py
--rw-rw-rw-   0        0        0      654 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_detect_label_edges.py
--rw-rw-rw-   0        0        0      733 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_detect_maxima_box.py
--rw-rw-rw-   0        0        0      733 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_detect_minima_box.py
--rw-rw-rw-   0        0        0      545 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_difference_of_gaussian.py
--rw-rw-rw-   0        0        0      618 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_dilate_box.py
--rw-rw-rw-   0        0        0     1379 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_dilate_box_slice_by_slice.py
--rw-rw-rw-   0        0        0      628 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_dilate_sphere.py
--rw-rw-rw-   0        0        0     1385 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_dilate_sphere_slice_by_slice.py
--rw-rw-rw-   0        0        0      814 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_divide_images.py
--rw-rw-rw-   0        0        0     1519 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_downsample_xy_half_median.py
--rw-rw-rw-   0        0        0      483 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_draw_box.py
--rw-rw-rw-   0        0        0      488 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_draw_line.py
--rw-rw-rw-   0        0        0      489 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_draw_sphere.py
--rw-rw-rw-   0        0        0      791 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_equal.py
--rw-rw-rw-   0        0        0      632 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_equal_constant.py
--rw-rw-rw-   0        0        0      616 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_erode_box.py
--rw-rw-rw-   0        0        0     1379 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_erode_box_slice_by_slice.py
--rw-rw-rw-   0        0        0      622 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_erode_sphere.py
--rw-rw-rw-   0        0        0     1385 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_erode_sphere_slice_by_slice.py
--rw-rw-rw-   0        0        0      750 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_euclidean_distance_from_label_centroid_map.py
--rw-rw-rw-   0        0        0     1805 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_exclude_labels.py
--rw-rw-rw-   0        0        0     3646 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_on_edges.py
--rw-rw-rw-   0        0        0      792 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_out_of_size_range.py
--rw-rw-rw-   0        0        0      569 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_with_values_out_of_range.py
--rw-rw-rw-   0        0        0      569 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_with_values_within_range.py
--rw-rw-rw-   0        0        0      353 2021-07-03 15:17:03.000000 pyclesperanto_prototype-0.9.7/tests/test_execute.py
--rw-rw-rw-   0        0        0      701 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_exponential.py
--rw-rw-rw-   0        0        0      843 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_extend_labeling_via_voronoi.py
--rw-rw-rw-   0        0        0     2060 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_extend_labels_with_maximum_radius.py
--rw-rw-rw-   0        0        0     1881 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_extended_depth_of_focus_variance_projection.py
--rw-rw-rw-   0        0        0      518 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_flag_existing_labels.py
--rw-rw-rw-   0        0        0      626 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_flip.py
--rw-rw-rw-   0        0        0      556 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_gamma_correction.py
--rw-rw-rw-   0        0        0      482 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_gaussian_blur.py
--rw-rw-rw-   0        0        0      828 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_generate_angle_matrix.py
--rw-rw-rw-   0        0        0     1825 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_generate_binary_overlap_matrix.py
--rw-rw-rw-   0        0        0     1016 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_generate_distance_matrix.py
--rw-rw-rw-   0        0        0      855 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_generate_n_nearest_neighbor_matrix.py
--rw-rw-rw-   0        0        0     1644 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_generate_proximal_neighbor_matrix.py
--rw-rw-rw-   0        0        0      743 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_generate_touch_matrix.py
--rw-rw-rw-   0        0        0      617 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_gradient_x.py
--rw-rw-rw-   0        0        0      619 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_gradient_y.py
--rw-rw-rw-   0        0        0     1357 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_gradient_z.py
--rw-rw-rw-   0        0        0     1670 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_greater.py
--rw-rw-rw-   0        0        0      638 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_greater_constant.py
--rw-rw-rw-   0        0        0     1637 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_greater_or_equal.py
--rw-rw-rw-   0        0        0      656 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_greater_or_equal_constant.py
--rw-rw-rw-   0        0        0     1590 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_histogram.py
--rw-rw-rw-   0        0        0      890 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_image.py
--rw-rw-rw-   0        0        0      469 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_invert.py
--rw-rw-rw-   0        0        0      668 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_jaccard_index.py
--rw-rw-rw-   0        0        0     1169 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_maximum_extension_map.py
--rw-rw-rw-   0        0        0     1179 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_maximum_extension_ratio_map.py
--rw-rw-rw-   0        0        0     1390 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_maximum_intensity_map.py
--rw-rw-rw-   0        0        0     1157 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_mean_extension_map.py
--rw-rw-rw-   0        0        0     1378 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_mean_intensity_map.py
--rw-rw-rw-   0        0        0     1390 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_minimum_intensity_map.py
--rw-rw-rw-   0        0        0     1060 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_pixelcount_map.py
--rw-rw-rw-   0        0        0     1541 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_spots.py
--rw-rw-rw-   0        0        0     1472 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_label_standard_deviation_intensity_map.py
--rw-rw-rw-   0        0        0      649 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_labelled_spots_to_pointlist.py
--rw-rw-rw-   0        0        0      630 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_laplace_box.py
--rw-rw-rw-   0        0        0      632 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_laplace_diamond.py
--rw-rw-rw-   0        0        0      464 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_logarithm.py
--rw-rw-rw-   0        0        0      784 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mask.py
--rw-rw-rw-   0        0        0      799 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mask_label.py
--rw-rw-rw-   0        0        0     1114 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_masked_voronoi_labeling.py
--rw-rw-rw-   0        0        0      627 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_box.py
--rw-rw-rw-   0        0        0      894 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_distance_of_n_shortest_distances.py
--rw-rw-rw-   0        0        0      975 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_distance_of_touching_neighbors.py
--rw-rw-rw-   0        0        0      545 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_image_and_scalar.py
--rw-rw-rw-   0        0        0      804 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_images.py
--rw-rw-rw-   0        0        0      614 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_of_all_pixels.py
--rw-rw-rw-   0        0        0      740 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0      868 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_sphere.py
--rw-rw-rw-   0        0        0     1797 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_x_projection.py
--rw-rw-rw-   0        0        0     1355 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_y_projection.py
--rw-rw-rw-   0        0        0     1625 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_maximum_z_projection.py
--rw-rw-rw-   0        0        0      622 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_box.py
--rw-rw-rw-   0        0        0     1213 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_of_all_pixels.py
--rw-rw-rw-   0        0        0      758 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0      658 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_sphere.py
--rw-rw-rw-   0        0        0      269 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_squared_error.py
--rw-rw-rw-   0        0        0     1408 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_x_projection.py
--rw-rw-rw-   0        0        0     1403 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_y_projection.py
--rw-rw-rw-   0        0        0     1384 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mean_z_projection.py
--rw-rw-rw-   0        0        0      646 2021-07-10 20:34:01.000000 pyclesperanto_prototype-0.9.7/tests/test_median_box.py
--rw-rw-rw-   0        0        0      652 2021-07-10 20:34:01.000000 pyclesperanto_prototype-0.9.7/tests/test_median_sphere.py
--rw-rw-rw-   0        0        0     1374 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_merge_touching_labels.py
--rw-rw-rw-   0        0        0      627 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_box.py
--rw-rw-rw-   0        0        0      974 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_distance_of_touching_neighbors.py
--rw-rw-rw-   0        0        0      549 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_image_and_scalar.py
--rw-rw-rw-   0        0        0      804 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_images.py
--rw-rw-rw-   0        0        0      612 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_of_all_pixels.py
--rw-rw-rw-   0        0        0     1690 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_of_masked_pixels.py
--rw-rw-rw-   0        0        0      740 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0     1429 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_x_projection.py
--rw-rw-rw-   0        0        0     1342 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_y_projection.py
--rw-rw-rw-   0        0        0     1342 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_minimum_z_projection.py
--rw-rw-rw-   0        0        0      818 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_mode_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0      553 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_multiply_image_and_coordinate.py
--rw-rw-rw-   0        0        0      547 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_multiply_image_and_scalar.py
--rw-rw-rw-   0        0        0      809 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_multiply_images.py
--rw-rw-rw-   0        0        0      911 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_multiply_matrix.py
--rw-rw-rw-   0        0        0     2054 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_n_closest_points.py
--rw-rw-rw-   0        0        0      809 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_nonzero_maximum_box.py
--rw-rw-rw-   0        0        0      816 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_nonzero_maximum_diamond.py
--rw-rw-rw-   0        0        0      808 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_nonzero_minimum_box.py
--rw-rw-rw-   0        0        0      818 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_nonzero_minimum_diamond.py
--rw-rw-rw-   0        0        0      794 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_not_equal.py
--rw-rw-rw-   0        0        0      640 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_not_equal_constant.py
--rw-rw-rw-   0        0        0      699 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_onlyzero_overwrite_maximum_box.py
--rw-rw-rw-   0        0        0      704 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_onlyzero_overwrite_maximum_diamond.py
--rw-rw-rw-   0        0        0    18430 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_operators.py
--rw-rw-rw-   0        0        0      627 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_paste.py
--rw-rw-rw-   0        0        0      756 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_point_index_list_to_mesh.py
--rw-rw-rw-   0        0        0      858 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_point_index_list_to_touch_matrix.py
--rw-rw-rw-   0        0        0     1588 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_pointlist_to_labelled_spots.py
--rw-rw-rw-   0        0        0      622 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_power.py
--rw-rw-rw-   0        0        0      812 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_power_images.py
--rw-rw-rw-   0        0        0      775 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_proximal_neighbor_count_map.py
--rw-rw-rw-   0        0        0      663 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_push.py
--rw-rw-rw-   0        0        0     1024 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_push_regionprops_column.py
--rw-rw-rw-   0        0        0      383 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_radians_to_degrees.py
--rw-rw-rw-   0        0        0      601 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_read_intensities_from_map.py
--rw-rw-rw-   0        0        0      587 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_read_intensities_from_positions.py
--rw-rw-rw-   0        0        0     1365 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_reduce_stack.py
--rw-rw-rw-   0        0        0     3707 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_reduction.py
--rw-rw-rw-   0        0        0     7790 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_regionprops.py
--rw-rw-rw-   0        0        0      724 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_replace_intensities.py
--rw-rw-rw-   0        0        0      645 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_replace_intensity.py
--rw-rw-rw-   0        0        0     5116 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_resample.py
--rw-rw-rw-   0        0        0      675 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_rigid_transform.py
--rw-rw-rw-   0        0        0     1328 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_rotate.py
--rw-rw-rw-   0        0        0     1223 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_scale.py
--rw-rw-rw-   0        0        0      435 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set.py
--rw-rw-rw-   0        0        0      593 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_column.py
--rw-rw-rw-   0        0        0      604 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_image_borders.py
--rw-rw-rw-   0        0        0      591 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_nonzero_pixels_to_pixelindex.py
--rw-rw-rw-   0        0        0     1010 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_plane.py
--rw-rw-rw-   0        0        0      694 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_ramp_x.py
--rw-rw-rw-   0        0        0      694 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_ramp_y.py
--rw-rw-rw-   0        0        0      680 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_ramp_z.py
--rw-rw-rw-   0        0        0      587 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_row.py
--rw-rw-rw-   0        0        0      525 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_where_x_equals_y.py
--rw-rw-rw-   0        0        0      541 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_where_x_greater_than_y.py
--rw-rw-rw-   0        0        0      541 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_set_where_x_smaller_than_y.py
--rw-rw-rw-   0        0        0      170 2021-07-10 06:16:46.000000 pyclesperanto_prototype-0.9.7/tests/test_skimage_imsave.py
--rw-rw-rw-   0        0        0     1624 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_smaller.py
--rw-rw-rw-   0        0        0      636 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_smaller_constant.py
--rw-rw-rw-   0        0        0     1633 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_smaller_or_equal.py
--rw-rw-rw-   0        0        0      645 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_smaller_or_equal_constant.py
--rw-rw-rw-   0        0        0      631 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sobel.py
--rw-rw-rw-   0        0        0      745 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sorenson_dice_coefficient.py
--rw-rw-rw-   0        0        0      606 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_spots_to_pointlist.py
--rw-rw-rw-   0        0        0      345 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_squared_difference.py
--rw-rw-rw-   0        0        0      849 2021-06-26 18:47:43.000000 pyclesperanto_prototype-0.9.7/tests/test_standard_deviation_of_touching_neighbors_map.py
--rw-rw-rw-   0        0        0     1448 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_standard_deviation_z_projection.py
--rw-rw-rw-   0        0        0     9731 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_statistics_of_background_and_labelled_pixels.py
--rw-rw-rw-   0        0        0      482 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_statistics_of_image.py
--rw-rw-rw-   0        0        0     7337 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_statistics_of_labelled_pixels.py
--rw-rw-rw-   0        0        0      495 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_subtract_image_from_scalar.py
--rw-rw-rw-   0        0        0      338 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_subtract_images.py
--rw-rw-rw-   0        0        0     1205 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sum_of_all_pixels.py
--rw-rw-rw-   0        0        0      694 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sum_reduction.py
--rw-rw-rw-   0        0        0     1355 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sum_x_projection.py
--rw-rw-rw-   0        0        0     1353 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sum_y_projection.py
--rw-rw-rw-   0        0        0     1368 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_sum_z_projection.py
--rw-rw-rw-   0        0        0      780 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_threshold_otsu.py
--rw-rw-rw-   0        0        0      460 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_top_hat_box.py
--rw-rw-rw-   0        0        0      463 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_top_hat_sphere.py
--rw-rw-rw-   0        0        0      743 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_touch_matrix_to_adjacency_matrix.py
--rw-rw-rw-   0        0        0      887 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_touch_matrix_to_mesh.py
--rw-rw-rw-   0        0        0      743 2021-06-26 18:47:43.000000 pyclesperanto_prototype-0.9.7/tests/test_touching_neighbor_count_map.py
--rw-rw-rw-   0        0        0      649 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_translate.py
--rw-rw-rw-   0        0        0     1543 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_transpose_xy.py
--rw-rw-rw-   0        0        0     1529 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_transpose_xz.py
--rw-rw-rw-   0        0        0     1545 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_transpose_yz.py
--rw-rw-rw-   0        0        0      896 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_undefined_to_zero.py
--rw-rw-rw-   0        0        0      677 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_variance_box.py
--rw-rw-rw-   0        0        0      653 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_variance_sphere.py
--rw-rw-rw-   0        0        0      821 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_voronoi_labeling.py
--rw-rw-rw-   0        0        0      896 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_voronoi_otsu_labeling.py
--rw-rw-rw-   0        0        0     1778 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.7/tests/test_write_values_to_positions.py
--rw-rw-rw-   0        0        0     1697 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_z_position_of_maximum_z_projection.py
--rw-rw-rw-   0        0        0     1697 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_z_position_of_minimum_z_projection.py
--rw-rw-rw-   0        0        0     1858 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_z_position_projection.py
--rw-rw-rw-   0        0        0     2284 2021-07-10 18:34:38.000000 pyclesperanto_prototype-0.9.7/tests/test_z_position_range_projection.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:06.739340 pyclesperanto_prototype-0.9.9/
+-rw-rw-rw-   0        0        0     1687 2021-06-16 18:09:27.000000 pyclesperanto_prototype-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0       46 2021-06-16 18:09:27.000000 pyclesperanto_prototype-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    18603 2021-08-01 09:36:06.739340 pyclesperanto_prototype-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0    17959 2021-08-01 08:45:55.000000 pyclesperanto_prototype-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.396037 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/
+-rw-rw-rw-   0        0        0      209 2021-08-01 09:34:37.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/__init__.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.431043 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/
+-rw-rw-rw-   0        0        0     1419 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/__init__.py
+-rw-rw-rw-   0        0        0     1110 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_available_device_names.py
+-rw-rw-rw-   0        0        0      476 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_categories.py
+-rw-rw-rw-   0        0        0     7467 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_cl_image.py
+-rw-rw-rw-   0        0        0     1204 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_cl_info.py
+-rw-rw-rw-   0        0        0     4598 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_create.py
+-rw-rw-rw-   0        0        0     4277 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_device.py
+-rw-rw-rw-   0        0        0    12121 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_execute.py
+-rw-rw-rw-   0        0        0     2272 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_operations.py
+-rw-rw-rw-   0        0        0     2805 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_plugin_function.py
+-rw-rw-rw-   0        0        0     1439 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_program.py
+-rw-rw-rw-   0        0        0      864 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_pull.py
+-rw-rw-rw-   0        0        0     1309 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_push.py
+-rw-rw-rw-   0        0        0    15064 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_pycl.py
+-rw-rw-rw-   0        0        0       62 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_radius_to_kernel_size.py
+-rw-rw-rw-   0        0        0      172 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_set_wait_for_kernel_finish.py
+-rw-rw-rw-   0        0        0      120 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_sigma_to_kernel_size.py
+-rw-rw-rw-   0        0        0      329 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_types.py
+-rw-rw-rw-   0        0        0    27062 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/preamble.cl
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.622086 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/
+-rw-rw-rw-   0        0        0     7722 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/__init__.py
+-rw-rw-rw-   0        0        0     1106 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_absolute.py
+-rw-rw-rw-   0        0        0     1304 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_add_image_and_scalar.py
+-rw-rw-rw-   0        0        0     1729 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_add_images_weighted.py
+-rw-rw-rw-   0        0        0     1187 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_average_distance_of_n_far_off_distances.py
+-rw-rw-rw-   0        0        0     1190 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_average_distance_of_n_shortest_distances.py
+-rw-rw-rw-   0        0        0     1307 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_average_distance_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1520 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_and.py
+-rw-rw-rw-   0        0        0     1320 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_edge_detection.py
+-rw-rw-rw-   0        0        0     1362 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_not.py
+-rw-rw-rw-   0        0        0     1500 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_or.py
+-rw-rw-rw-   0        0        0     1318 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_subtract.py
+-rw-rw-rw-   0        0        0     1579 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_xor.py
+-rw-rw-rw-   0        0        0     1148 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_convolve.py
+-rw-rw-rw-   0        0        0      875 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_copy.py
+-rw-rw-rw-   0        0        0     1555 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_copy_slice.py
+-rw-rw-rw-   0        0        0     1359 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_count_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1713 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_crop.py
+-rw-rw-rw-   0        0        0     1247 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_detect_label_edges.py
+-rw-rw-rw-   0        0        0     1561 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_detect_maxima_box.py
+-rw-rw-rw-   0        0        0     1559 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_detect_minima_box.py
+-rw-rw-rw-   0        0        0     1472 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_box.py
+-rw-rw-rw-   0        0        0     1542 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_box_slice_by_slice.py
+-rw-rw-rw-   0        0        0     1285 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_sphere.py
+-rw-rw-rw-   0        0        0     1359 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_sphere_slice_by_slice.py
+-rw-rw-rw-   0        0        0     1096 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_divide_images.py
+-rw-rw-rw-   0        0        0     1918 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_downsample_slice_by_slice_half_median.py
+-rw-rw-rw-   0        0        0     1738 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_draw_box.py
+-rw-rw-rw-   0        0        0     1993 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_draw_line.py
+-rw-rw-rw-   0        0        0     2078 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_draw_sphere.py
+-rw-rw-rw-   0        0        0     1353 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_equal.py
+-rw-rw-rw-   0        0        0     1422 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_equal_constant.py
+-rw-rw-rw-   0        0        0     1465 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_box.py
+-rw-rw-rw-   0        0        0     1593 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_box_slice_by_slice.py
+-rw-rw-rw-   0        0        0     1279 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_sphere.py
+-rw-rw-rw-   0        0        0     1407 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_sphere_slice_by_slice.py
+-rw-rw-rw-   0        0        0     2163 2021-07-31 16:58:35.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_execute_separable_kernel.py
+-rw-rw-rw-   0        0        0     1034 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_exponential.py
+-rw-rw-rw-   0        0        0     1248 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_flip.py
+-rw-rw-rw-   0        0        0     1752 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gaussian_blur.py
+-rw-rw-rw-   0        0        0     2307 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_angle_matrix.py
+-rw-rw-rw-   0        0        0     1535 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_binary_overlap_matrix.py
+-rw-rw-rw-   0        0        0     2074 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_distance_matrix.py
+-rw-rw-rw-   0        0        0     1565 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_touch_matrix.py
+-rw-rw-rw-   0        0        0     1108 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gradient_x.py
+-rw-rw-rw-   0        0        0     1106 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gradient_y.py
+-rw-rw-rw-   0        0        0     1040 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gradient_z.py
+-rw-rw-rw-   0        0        0     1127 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater.py
+-rw-rw-rw-   0        0        0     1173 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater_constant.py
+-rw-rw-rw-   0        0        0     1179 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater_or_equal.py
+-rw-rw-rw-   0        0        0     1228 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater_or_equal_constant.py
+-rw-rw-rw-   0        0        0      977 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_laplace_box.py
+-rw-rw-rw-   0        0        0      985 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_laplace_diamond.py
+-rw-rw-rw-   0        0        0     1026 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_logarithm.py
+-rw-rw-rw-   0        0        0     1194 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mask.py
+-rw-rw-rw-   0        0        0     1352 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mask_label.py
+-rw-rw-rw-   0        0        0     1617 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_box.py
+-rw-rw-rw-   0        0        0     1102 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_distance_of_n_shortest_distances.py
+-rw-rw-rw-   0        0        0     1219 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_distance_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1184 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_image_and_scalar.py
+-rw-rw-rw-   0        0        0     1125 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_images.py
+-rw-rw-rw-   0        0        0     1609 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_sphere.py
+-rw-rw-rw-   0        0        0     1020 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_x_projection.py
+-rw-rw-rw-   0        0        0     1020 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_y_projection.py
+-rw-rw-rw-   0        0        0     1036 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_z_projection.py
+-rw-rw-rw-   0        0        0     1625 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_box.py
+-rw-rw-rw-   0        0        0     1620 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_sphere.py
+-rw-rw-rw-   0        0        0      978 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_x_projection.py
+-rw-rw-rw-   0        0        0      978 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_y_projection.py
+-rw-rw-rw-   0        0        0      994 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_z_projection.py
+-rw-rw-rw-   0        0        0     1625 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_median_box.py
+-rw-rw-rw-   0        0        0     1643 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_median_sphere.py
+-rw-rw-rw-   0        0        0     1621 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_box.py
+-rw-rw-rw-   0        0        0     1219 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_distance_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1181 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_image_and_scalar.py
+-rw-rw-rw-   0        0        0     1124 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_images.py
+-rw-rw-rw-   0        0        0     1621 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_sphere.py
+-rw-rw-rw-   0        0        0     1064 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_x_projection.py
+-rw-rw-rw-   0        0        0     1064 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_y_projection.py
+-rw-rw-rw-   0        0        0     1082 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_z_projection.py
+-rw-rw-rw-   0        0        0     1182 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_image_and_coordinate.py
+-rw-rw-rw-   0        0        0     1354 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_image_and_scalar.py
+-rw-rw-rw-   0        0        0     1264 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_images.py
+-rw-rw-rw-   0        0        0     1168 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_matrix.py
+-rw-rw-rw-   0        0        0     2439 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_n_closest_points.py
+-rw-rw-rw-   0        0        0     1175 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_maximum_box.py
+-rw-rw-rw-   0        0        0     1199 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_maximum_diamond.py
+-rw-rw-rw-   0        0        0     1175 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_minimum_box.py
+-rw-rw-rw-   0        0        0     1193 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_minimum_diamond.py
+-rw-rw-rw-   0        0        0     1369 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_not_equal.py
+-rw-rw-rw-   0        0        0     1414 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_not_equal_constant.py
+-rw-rw-rw-   0        0        0      991 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_box.py
+-rw-rw-rw-   0        0        0     1010 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_diamond.py
+-rw-rw-rw-   0        0        0     1332 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_paste.py
+-rw-rw-rw-   0        0        0     1123 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_point_index_list_to_mesh.py
+-rw-rw-rw-   0        0        0     1145 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_point_index_list_to_touch_matrix.py
+-rw-rw-rw-   0        0        0     1079 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_power.py
+-rw-rw-rw-   0        0        0     1058 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_power_images.py
+-rw-rw-rw-   0        0        0     1206 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_read_intensities_from_map.py
+-rw-rw-rw-   0        0        0     1127 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_read_intensities_from_positions.py
+-rw-rw-rw-   0        0        0     1414 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_replace_intensities.py
+-rw-rw-rw-   0        0        0     1121 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_replace_intensity.py
+-rw-rw-rw-   0        0        0     2619 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_resample.py
+-rw-rw-rw-   0        0        0      836 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set.py
+-rw-rw-rw-   0        0        0      945 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_column.py
+-rw-rw-rw-   0        0        0      905 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_image_borders.py
+-rw-rw-rw-   0        0        0      542 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_non_zero_pixels_to_pixel_index.py
+-rw-rw-rw-   0        0        0      932 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_plane.py
+-rw-rw-rw-   0        0        0      737 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_ramp_x.py
+-rw-rw-rw-   0        0        0      735 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_ramp_y.py
+-rw-rw-rw-   0        0        0      735 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_ramp_z.py
+-rw-rw-rw-   0        0        0      910 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_row.py
+-rw-rw-rw-   0        0        0      937 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_where_x_equals_y.py
+-rw-rw-rw-   0        0        0      960 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_where_x_greater_than_y.py
+-rw-rw-rw-   0        0        0      958 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_where_x_smaller_than_y.py
+-rw-rw-rw-   0        0        0     1125 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller.py
+-rw-rw-rw-   0        0        0     1172 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller_constant.py
+-rw-rw-rw-   0        0        0     1178 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller_or_equal.py
+-rw-rw-rw-   0        0        0     1227 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller_or_equal_constant.py
+-rw-rw-rw-   0        0        0      983 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sobel.py
+-rw-rw-rw-   0        0        0     1081 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_standard_deviation_z_projection.py
+-rw-rw-rw-   0        0        0     1137 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_subtract_image_from_scalar.py
+-rw-rw-rw-   0        0        0     1008 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sum_x_projection.py
+-rw-rw-rw-   0        0        0      964 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sum_y_projection.py
+-rw-rw-rw-   0        0        0      992 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sum_z_projection.py
+-rw-rw-rw-   0        0        0     1616 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_touch_matrix_to_mesh.py
+-rw-rw-rw-   0        0        0     1409 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_transpose_xy.py
+-rw-rw-rw-   0        0        0     1386 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_transpose_xz.py
+-rw-rw-rw-   0        0        0     1419 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_transpose_yz.py
+-rw-rw-rw-   0        0        0      927 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_undefined_to_zero.py
+-rw-rw-rw-   0        0        0     1556 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_variance_box.py
+-rw-rw-rw-   0        0        0     1571 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_variance_sphere.py
+-rw-rw-rw-   0        0        0     1682 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_write_values_to_positions.py
+-rw-rw-rw-   0        0        0     1889 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/maximum_distance_of_n_shortest_distances_x.cl
+-rw-rw-rw-   0        0        0     1551 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/maximum_distance_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0     1551 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/minimum_distance_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0     1183 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/point_index_list_to_touch_matrix_x.cl
+-rw-rw-rw-   0        0        0      730 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/read_intensities_from_map_x.cl
+-rw-rw-rw-   0        0        0      929 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/read_intensities_from_positions_x.cl
+-rw-rw-rw-   0        0        0     1043 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_box_2d_x.cl
+-rw-rw-rw-   0        0        0     1527 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1496 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     2195 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_sphere_3d_x.cl
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.682100 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/
+-rw-rw-rw-   0        0        0     2388 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/__init__.py
+-rw-rw-rw-   0        0        0      862 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_add_images.py
+-rw-rw-rw-   0        0        0     1476 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_block_enumerate.py
+-rw-rw-rw-   0        0        0     1568 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_bottom_hat_box.py
+-rw-rw-rw-   0        0        0     1591 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_bottom_hat_sphere.py
+-rw-rw-rw-   0        0        0     1091 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_combine_horizontally.py
+-rw-rw-rw-   0        0        0     1087 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_combine_vertically.py
+-rw-rw-rw-   0        0        0      964 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_concatenate_stacks.py
+-rw-rw-rw-   0        0        0      346 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_degrees_to_radians.py
+-rw-rw-rw-   0        0        0     1413 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_distance_matrix_to_mesh.py
+-rw-rw-rw-   0        0        0     1204 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_flag_existing_labels.py
+-rw-rw-rw-   0        0        0     1207 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_gamma_correction.py
+-rw-rw-rw-   0        0        0      976 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_invert.py
+-rw-rw-rw-   0        0        0     1826 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_label_spots.py
+-rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_maximum_of_all_pixels.py
+-rw-rw-rw-   0        0        0     1728 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_maximum_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1705 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_mean_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1438 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_median_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1433 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_minimum_of_all_pixels.py
+-rw-rw-rw-   0        0        0     2928 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_minimum_of_masked_pixels.py
+-rw-rw-rw-   0        0        0     1728 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_minimum_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0      978 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_mode_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1079 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_neighbors_of_neighbors.py
+-rw-rw-rw-   0        0        0     1285 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_pointlist_to_labelled_spots.py
+-rw-rw-rw-   0        0        0      346 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_radians_to_degrees.py
+-rw-rw-rw-   0        0        0     1452 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_reduce_stack.py
+-rw-rw-rw-   0        0        0     1569 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_standard_deviation_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0     1388 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_sub_stack.py
+-rw-rw-rw-   0        0        0      862 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_subtract_images.py
+-rw-rw-rw-   0        0        0     1374 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_sum_of_all_pixels.py
+-rw-rw-rw-   0        0        0     1150 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_sum_reduction_x.py
+-rw-rw-rw-   0        0        0     1557 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_top_hat_box.py
+-rw-rw-rw-   0        0        0     1566 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_top_hat_sphere.py
+-rw-rw-rw-   0        0        0     1375 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_touch_matrix_to_adjacency_matrix.py
+-rw-rw-rw-   0        0        0     1016 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_z_position_of_maximum_z_projection.py
+-rw-rw-rw-   0        0        0     1029 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_z_position_of_minimum_z_projection.py
+-rw-rw-rw-   0        0        0     1029 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_z_position_projection.py
+-rw-rw-rw-   0        0        0      652 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/z_position_of_maximum_z_projection_x.cl
+-rw-rw-rw-   0        0        0      652 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/z_position_of_minimum_z_projection_x.cl
+-rw-rw-rw-   0        0        0      558 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/z_position_projection_x.cl
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.733112 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/
+-rw-rw-rw-   0        0        0     3498 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/__init__.py
+-rw-rw-rw-   0        0        0     1253 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_absolute_difference.py
+-rw-rw-rw-   0        0        0     1628 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_bounding_box.py
+-rw-rw-rw-   0        0        0     1107 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_center_of_mass.py
+-rw-rw-rw-   0        0        0     2072 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_difference_of_gaussian.py
+-rw-rw-rw-   0        0        0     1082 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_divide_by_gaussian_background.py
+-rw-rw-rw-   0        0        0     1806 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels.py
+-rw-rw-rw-   0        0        0     2841 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_on_edges.py
+-rw-rw-rw-   0        0        0     1621 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_outside_size_range.py
+-rw-rw-rw-   0        0        0     1599 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_out_of_range.py
+-rw-rw-rw-   0        0        0     1672 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_within_range.py
+-rw-rw-rw-   0        0        0     2115 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_generate_n_nearest_neighbors_matrix.py
+-rw-rw-rw-   0        0        0     1875 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_generate_proximal_neighbors_matrix.py
+-rw-rw-rw-   0        0        0     5290 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_histogram.py
+-rw-rw-rw-   0        0        0     1297 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_jaccard_index.py
+-rw-rw-rw-   0        0        0     1390 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_labelled_spots_to_pointlist.py
+-rw-rw-rw-   0        0        0     2026 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_maximum_of_n_nearest_neighbors_map.py
+-rw-rw-rw-   0        0        0     2230 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_maximum_of_proximal_neighbors_map.py
+-rw-rw-rw-   0        0        0     2275 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_maximum_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0      895 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_all_pixels.py
+-rw-rw-rw-   0        0        0     2011 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_n_nearest_neighbors_map.py
+-rw-rw-rw-   0        0        0     2215 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_proximal_neighbors_map.py
+-rw-rw-rw-   0        0        0     2240 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0     1898 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_minimum_of_n_nearest_neighbors_map.py
+-rw-rw-rw-   0        0        0     2102 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_minimum_of_proximal_neighbors_map.py
+-rw-rw-rw-   0        0        0     2275 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_minimum_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0     1805 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mode_of_n_nearest_neighbors_map.py
+-rw-rw-rw-   0        0        0     2009 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mode_of_proximal_neighbors_map.py
+-rw-rw-rw-   0        0        0     2225 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mode_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0     2076 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_relabel_sequential.py
+-rw-rw-rw-   0        0        0     1046 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_squared_difference.py
+-rw-rw-rw-   0        0        0     1874 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_standard_deviation_of_n_nearest_neighbors_map.py
+-rw-rw-rw-   0        0        0     2078 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_standard_deviation_of_proximal_neighbors_map.py
+-rw-rw-rw-   0        0        0     2288 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_standard_deviation_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0     1081 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_subtract_gaussian_background.py
+-rw-rw-rw-   0        0        0     1596 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_z_position_range_projection.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.760118 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/
+-rw-rw-rw-   0        0        0     1418 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/__init__.py
+-rw-rw-rw-   0        0        0     2054 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_connected_components_labeling_box.py
+-rw-rw-rw-   0        0        0     1929 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_dilate_labels.py
+-rw-rw-rw-   0        0        0     2374 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_erode_labels.py
+-rw-rw-rw-   0        0        0      985 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_exclude_large_labels.py
+-rw-rw-rw-   0        0        0     1032 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_exclude_small_labels.py
+-rw-rw-rw-   0        0        0     1813 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_extend_labeling_via_voronoi.py
+-rw-rw-rw-   0        0        0     1312 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_extended_depth_of_focus_variance_projection.py
+-rw-rw-rw-   0        0        0     1283 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_maximum_touching_neighbor_count_map.py
+-rw-rw-rw-   0        0        0     1268 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_mean_touching_neighbor_count_map.py
+-rw-rw-rw-   0        0        0     1278 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_median_touching_neighbor_count_map.py
+-rw-rw-rw-   0        0        0     1283 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_minimum_touching_neighbor_count_map.py
+-rw-rw-rw-   0        0        0     1314 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_standard_deviation_touching_neighbor_count_map.py
+-rw-rw-rw-   0        0        0      880 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_mean_squared_error.py
+-rw-rw-rw-   0        0        0     3031 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_merge_touching_labels.py
+-rw-rw-rw-   0        0        0     1712 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_proximal_neighbor_count_map.py
+-rw-rw-rw-   0        0        0     1015 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_sorensen_dice_coefficient.py
+-rw-rw-rw-   0        0        0     1080 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_spots_to_pointlist.py
+-rw-rw-rw-   0        0        0     1141 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_touching_neighbor_count_map.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.765119 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/
+-rw-rw-rw-   0        0        0      205 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/__init__.py
+-rw-rw-rw-   0        0        0     1158 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/_connected_components_labeling_diamond.py
+-rw-rw-rw-   0        0        0     2359 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/_masked_voronoi_labeling.py
+-rw-rw-rw-   0        0        0     1182 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/_voronoi_labeling.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.777121 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/
+-rw-rw-rw-   0        0        0     6024 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_AffineTransform3D.py
+-rw-rw-rw-   0        0        0      295 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/__init__.py
+-rw-rw-rw-   0        0        0     3278 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_affine_transform.py
+-rw-rw-rw-   0        0        0     2148 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_apply_vector_field.py
+-rw-rw-rw-   0        0        0     2335 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_rigid_transform.py
+-rw-rw-rw-   0        0        0     1974 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_rotate.py
+-rw-rw-rw-   0        0        0     1451 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_scale.py
+-rw-rw-rw-   0        0        0     1212 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_translate.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.831139 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/
+-rw-rw-rw-   0        0        0     2960 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/__init__.py
+-rw-rw-rw-   0        0        0     1790 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_artificial_tissue_2d.py
+-rw-rw-rw-   0        0        0     1220 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_average_distance_of_n_closest_neighbors_map.py
+-rw-rw-rw-   0        0        0     1337 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_average_neighbor_distance_map.py
+-rw-rw-rw-   0        0        0      396 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_centroids_of_background_and_labels.py
+-rw-rw-rw-   0        0        0     3675 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_centroids_of_labels.py
+-rw-rw-rw-   0        0        0     1558 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_angle_mesh_between_touching_labels.py
+-rw-rw-rw-   0        0        0     1564 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_distance_mesh_between_touching_labels.py
+-rw-rw-rw-   0        0        0     1556 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_mesh_between_n_closest_labels.py
+-rw-rw-rw-   0        0        0     1421 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_mesh_between_proximal_labels.py
+-rw-rw-rw-   0        0        0     1180 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_mesh_between_touching_labels.py
+-rw-rw-rw-   0        0        0     1292 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_euclidean_distance_from_label_centroid_map.py
+-rw-rw-rw-   0        0        0      206 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_imread.py
+-rw-rw-rw-   0        0        0      951 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_imshow.py
+-rw-rw-rw-   0        0        0     1163 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_maximum_extension_map.py
+-rw-rw-rw-   0        0        0     1333 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_maximum_extension_ratio_map.py
+-rw-rw-rw-   0        0        0     1312 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_maximum_intensity_map.py
+-rw-rw-rw-   0        0        0     1160 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_mean_extension_map.py
+-rw-rw-rw-   0        0        0     1290 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_mean_intensity_map.py
+-rw-rw-rw-   0        0        0     1317 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_minimum_intensity_map.py
+-rw-rw-rw-   0        0        0     1167 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_pixel_count_map.py
+-rw-rw-rw-   0        0        0     1443 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_standard_deviation_intensity_map.py
+-rw-rw-rw-   0        0        0     9912 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_push_regionprops.py
+-rw-rw-rw-   0        0        0      790 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_push_regionprops_column.py
+-rw-rw-rw-   0        0        0     1965 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_regionprops.py
+-rw-rw-rw-   0        0        0     1435 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_entry.py
+-rw-rw-rw-   0        0        0     1522 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_of_background_and_labelled_pixels.py
+-rw-rw-rw-   0        0        0     1139 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_of_image.py
+-rw-rw-rw-   0        0        0    11805 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_of_labelled_pixels.py
+-rw-rw-rw-   0        0        0     3548 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_threshold_otsu.py
+-rw-rw-rw-   0        0        0     2465 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_voronoi_otsu_labeling.py
+-rw-rw-rw-   0        0        0     4429 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/standard_deviation_per_label_x.cl
+-rw-rw-rw-   0        0        0     5287 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/statistics_per_label_x.cl
+-rw-rw-rw-   0        0        0     1689 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/sum_per_label_x.cl
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.389035 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:06.420266 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/
+-rw-rw-rw-   0        0        0      512 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_2d_x.cl
+-rw-rw-rw-   0        0        0      551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_3d_x.cl
+-rw-rw-rw-   0        0        0      486 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_image_and_scalar_2d_x.cl
+-rw-rw-rw-   0        0        0      524 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_image_and_scalar_3d_x.cl
+-rw-rw-rw-   0        0        0      564 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_2d_x.cl
+-rw-rw-rw-   0        0        0      656 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_3d_x.cl
+-rw-rw-rw-   0        0        0     2691 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_interpolate_x.cl
+-rw-rw-rw-   0        0        0     2847 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_x.cl
+-rw-rw-rw-   0        0        0     3265 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_interpolate_x.cl
+-rw-rw-rw-   0        0        0     3427 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_x.cl
+-rw-rw-rw-   0        0        0     1256 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_interpolate_x.cl
+-rw-rw-rw-   0        0        0     1226 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_x.cl
+-rw-rw-rw-   0        0        0     1541 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_interpolate_x.cl
+-rw-rw-rw-   0        0        0     1506 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_x.cl
+-rw-rw-rw-   0        0        0      771 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/arg_maximum_z_projection_x.cl
+-rw-rw-rw-   0        0        0     1865 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_far_off_distances_x.cl
+-rw-rw-rw-   0        0        0     1863 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_shortest_distances_x.cl
+-rw-rw-rw-   0        0        0     1483 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      660 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_2d_x.cl
+-rw-rw-rw-   0        0        0      699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_3d_x.cl
+-rw-rw-rw-   0        0        0     1143 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_2d_x.cl
+-rw-rw-rw-   0        0        0     1597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_3d_x.cl
+-rw-rw-rw-   0        0        0      522 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_2d_x.cl
+-rw-rw-rw-   0        0        0      561 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_3d_x.cl
+-rw-rw-rw-   0        0        0      661 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_2d_x.cl
+-rw-rw-rw-   0        0        0      700 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_3d_x.cl
+-rw-rw-rw-   0        0        0      589 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_2d_x.cl
+-rw-rw-rw-   0        0        0      628 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_3d_x.cl
+-rw-rw-rw-   0        0        0      695 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_2d_x.cl
+-rw-rw-rw-   0        0        0      732 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_3d_x.cl
+-rw-rw-rw-   0        0        0      903 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/block_enumerate_x.cl
+-rw-rw-rw-   0        0        0      921 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_2d_x.cl
+-rw-rw-rw-   0        0        0     1096 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_3d_x.cl
+-rw-rw-rw-   0        0        0      418 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_2d_x.cl
+-rw-rw-rw-   0        0        0      459 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_3d_x.cl
+-rw-rw-rw-   0        0        0      493 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_slice_from_3d_x.cl
+-rw-rw-rw-   0        0        0      492 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/copy_slice_to_3d_x.cl
+-rw-rw-rw-   0        0        0      689 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_non_zero_projection_3d_2d_x.cl
+-rw-rw-rw-   0        0        0     1271 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_slice_by_slice_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1193 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     1677 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_voxels_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0      982 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      613 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_2d_x.cl
+-rw-rw-rw-   0        0        0      702 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_3d_x.cl
+-rw-rw-rw-   0        0        0     1842 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_interpolation_x.cl
+-rw-rw-rw-   0        0        0     1764 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_x.cl
+-rw-rw-rw-   0        0        0     1229 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_2d_x.cl
+-rw-rw-rw-   0        0        0     1697 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_3d_x.cl
+-rw-rw-rw-   0        0        0      936 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_2d_x.cl
+-rw-rw-rw-   0        0        0     1002 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_slice_by_slice_x.cl
+-rw-rw-rw-   0        0        0     1417 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_x.cl
+-rw-rw-rw-   0        0        0      936 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_2d_x.cl
+-rw-rw-rw-   0        0        0     1008 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_slice_by_slice_x.cl
+-rw-rw-rw-   0        0        0     1100 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_x.cl
+-rw-rw-rw-   0        0        0      772 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_2d_x.cl
+-rw-rw-rw-   0        0        0      936 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_3d_x.cl
+-rw-rw-rw-   0        0        0      832 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_slice_by_slice_3d_x.cl
+-rw-rw-rw-   0        0        0      882 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     1200 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0      962 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_slice_by_slice_3d_x.cl
+-rw-rw-rw-   0        0        0     2441 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distance_matrix_to_mesh_x.cl
+-rw-rw-rw-   0        0        0      894 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_2d_x.cl
+-rw-rw-rw-   0        0        0     1001 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1051 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1323 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      511 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/divide_images_2d_x.cl
+-rw-rw-rw-   0        0        0      551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/divide_images_3d_x.cl
+-rw-rw-rw-   0        0        0      518 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_2d_x.cl
+-rw-rw-rw-   0        0        0      616 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_3d_x.cl
+-rw-rw-rw-   0        0        0     2147 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_xy_by_half_median_3d_x.cl
+-rw-rw-rw-   0        0        0      459 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_box_2d_x.cl
+-rw-rw-rw-   0        0        0      604 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_box_3d_x.cl
+-rw-rw-rw-   0        0        0      606 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0      807 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1000 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_2d_x.cl
+-rw-rw-rw-   0        0        0     1277 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_3d_x.cl
+-rw-rw-rw-   0        0        0     1414 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_2d_x.cl
+-rw-rw-rw-   0        0        0     1567 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_3d_x.cl
+-rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_2d_x.cl
+-rw-rw-rw-   0        0        0      633 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_3d_x.cl
+-rw-rw-rw-   0        0        0      524 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_2d_x.cl
+-rw-rw-rw-   0        0        0      564 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_3d_x.cl
+-rw-rw-rw-   0        0        0      774 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_2d_x.cl
+-rw-rw-rw-   0        0        0      937 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_3d_x.cl
+-rw-rw-rw-   0        0        0      832 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_slice_by_slice_3d_x.cl
+-rw-rw-rw-   0        0        0      882 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     1198 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0      960 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_slice_by_slice_3d_x.cl
+-rw-rw-rw-   0        0        0     1247 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/euclidean_distance_from_label_centroid_map_x.cl
+-rw-rw-rw-   0        0        0     2537 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/excludeLabelsOnEdges_3d_x.cl
+-rw-rw-rw-   0        0        0     2537 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_edges_3d_x.cl
+-rw-rw-rw-   0        0        0     2485 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_2d_x.cl
+-rw-rw-rw-   0        0        0     2335 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_3d_x.cl
+-rw-rw-rw-   0        0        0     2485 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_2d_x.cl
+-rw-rw-rw-   0        0        0     2335 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_3d_x.cl
+-rw-rw-rw-   0        0        0      491 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exponential_2d_x.cl
+-rw-rw-rw-   0        0        0      530 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exponential_3d_x.cl
+-rw-rw-rw-   0        0        0      441 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flag_existing_labels_x.cl
+-rw-rw-rw-   0        0        0      747 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_2d_x.cl
+-rw-rw-rw-   0        0        0      935 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_3d_x.cl
+-rw-rw-rw-   0        0        0     1887 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flood_fill_diamond_x.cl
+-rw-rw-rw-   0        0        0      906 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_2d_x.cl
+-rw-rw-rw-   0        0        0      949 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_3d_x.cl
+-rw-rw-rw-   0        0        0     1285 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_angle_matrix_2d_x.cl
+-rw-rw-rw-   0        0        0      693 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_2d_x.cl
+-rw-rw-rw-   0        0        0      728 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_3d_x.cl
+-rw-rw-rw-   0        0        0     1113 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_distance_matrix_x.cl
+-rw-rw-rw-   0        0        0     1403 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_2d_x.cl
+-rw-rw-rw-   0        0        0     1931 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_3d_x.cl
+-rw-rw-rw-   0        0        0      597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_2d_x.cl
+-rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_3d_x.cl
+-rw-rw-rw-   0        0        0      591 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_2d_x.cl
+-rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_3d_x.cl
+-rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_z_3d_x.cl
+-rw-rw-rw-   0        0        0      594 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_2d_x.cl
+-rw-rw-rw-   0        0        0      634 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_3d_x.cl
+-rw-rw-rw-   0        0        0      525 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_2d_x.cl
+-rw-rw-rw-   0        0        0      565 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_3d_x.cl
+-rw-rw-rw-   0        0        0      604 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_2d_x.cl
+-rw-rw-rw-   0        0        0      644 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_3d_x.cl
+-rw-rw-rw-   0        0        0      535 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_2d_x.cl
+-rw-rw-rw-   0        0        0      575 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_3d_x.cl
+-rw-rw-rw-   0        0        0     1847 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_2d_x.cl
+-rw-rw-rw-   0        0        0     1999 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_3d_x.cl
+-rw-rw-rw-   0        0        0      987 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/label_spots_in_x.cl
+-rw-rw-rw-   0        0        0     1024 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/labelled_spots_to_point_list_x.cl
+-rw-rw-rw-   0        0        0     1348 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_2d_x.cl
+-rw-rw-rw-   0        0        0      810 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_3d_x.cl
+-rw-rw-rw-   0        0        0      926 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1225 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      489 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/logarithm_2d_x.cl
+-rw-rw-rw-   0        0        0      528 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/logarithm_3d_x.cl
+-rw-rw-rw-   0        0        0      537 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_2d_x.cl
+-rw-rw-rw-   0        0        0      576 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_3d_x.cl
+-rw-rw-rw-   0        0        0      619 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_2d_x.cl
+-rw-rw-rw-   0        0        0      658 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_3d_x.cl
+-rw-rw-rw-   0        0        0      636 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_stack_with_plane_3d_x.cl
+-rw-rw-rw-   0        0        0     8736 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/matrix_multiply_float_buffer.cl
+-rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_distance_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      557 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_2d_x.cl
+-rw-rw-rw-   0        0        0      596 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_3d_x.cl
+-rw-rw-rw-   0        0        0      618 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_2d_x.cl
+-rw-rw-rw-   0        0        0      626 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_3d_x.cl
+-rw-rw-rw-   0        0        0     1391 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_2d_x.cl
+-rw-rw-rw-   0        0        0      770 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_3d_x.cl
+-rw-rw-rw-   0        0        0      919 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1231 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      950 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_masked_pixels_3d_2d_x.cl
+-rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      549 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_projection_3d_2d_x.cl
+-rw-rw-rw-   0        0        0      699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_2d_x.cl
+-rw-rw-rw-   0        0        0      699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_3d_x.cl
+-rw-rw-rw-   0        0        0     1297 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_slice_by_slice_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1277 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     1695 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0      592 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_x_projection_x.cl
+-rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_y_projection_x.cl
+-rw-rw-rw-   0        0        0      740 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_bounded_3d_2d_x.cl
+-rw-rw-rw-   0        0        0      652 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_x.cl
+-rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      683 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_2d_x.cl
+-rw-rw-rw-   0        0        0      752 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_3d_x.cl
+-rw-rw-rw-   0        0        0     1103 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_slice_by_slice_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1043 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     1496 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0      542 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_x_projection_x.cl
+-rw-rw-rw-   0        0        0      543 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_y_projection_x.cl
+-rw-rw-rw-   0        0        0      759 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_bounded_3d_2d_x.cl
+-rw-rw-rw-   0        0        0      545 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_x.cl
+-rw-rw-rw-   0        0        0     1418 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_2d_x.cl
+-rw-rw-rw-   0        0        0     1732 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1907 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0     1511 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1616 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1619 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     2120 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1125 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_z_projection_x.cl
+-rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_distance_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      564 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_2d_x.cl
+-rw-rw-rw-   0        0        0      596 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_3d_x.cl
+-rw-rw-rw-   0        0        0      587 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_2d_x.cl
+-rw-rw-rw-   0        0        0      626 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_3d_x.cl
+-rw-rw-rw-   0        0        0     1391 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_2d_x.cl
+-rw-rw-rw-   0        0        0      770 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_3d_x.cl
+-rw-rw-rw-   0        0        0      919 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1231 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      950 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_masked_pixels_3d_2d_x.cl
+-rw-rw-rw-   0        0        0     1434 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      549 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_projection_3d_2d_x.cl
+-rw-rw-rw-   0        0        0      701 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_2d_x.cl
+-rw-rw-rw-   0        0        0      697 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_3d_x.cl
+-rw-rw-rw-   0        0        0     1299 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_slice_by_slice_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0     1399 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_2d_x.cl
+-rw-rw-rw-   0        0        0     1695 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_3d_x.cl
+-rw-rw-rw-   0        0        0      592 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_x_projection_x.cl
+-rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_y_projection_x.cl
+-rw-rw-rw-   0        0        0      757 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_bounded_3d_2d_x.cl
+-rw-rw-rw-   0        0        0      892 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_thresholded_bounded_3d_2d_x.cl
+-rw-rw-rw-   0        0        0      593 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_x.cl
+-rw-rw-rw-   0        0        0     1643 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mode_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      516 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_2d_x.cl
+-rw-rw-rw-   0        0        0      552 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_3d_x.cl
+-rw-rw-rw-   0        0        0      491 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_scalar_2d_x.cl
+-rw-rw-rw-   0        0        0      529 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_scalar_3d_x.cl
+-rw-rw-rw-   0        0        0      514 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_2d_x.cl
+-rw-rw-rw-   0        0        0      551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_3d_x.cl
+-rw-rw-rw-   0        0        0      696 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_matrix_x.cl
+-rw-rw-rw-   0        0        0      617 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_plane_3d_x.cl
+-rw-rw-rw-   0        0        0      739 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_scalars_x.cl
+-rw-rw-rw-   0        0        0     1851 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_distances_x.cl
+-rw-rw-rw-   0        0        0     1644 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_points_x.cl
+-rw-rw-rw-   0        0        0      955 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_2d_x.cl
+-rw-rw-rw-   0        0        0     1699 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1309 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1701 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      953 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_2d_x.cl
+-rw-rw-rw-   0        0        0     1066 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1309 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1701 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_2d_x.cl
+-rw-rw-rw-   0        0        0      637 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_3d_x.cl
+-rw-rw-rw-   0        0        0      528 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_2d_x.cl
+-rw-rw-rw-   0        0        0      568 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_3d_x.cl
+-rw-rw-rw-   0        0        0     1985 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_2d_x.cl
+-rw-rw-rw-   0        0        0     1015 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_3d_x.cl
+-rw-rw-rw-   0        0        0     1320 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_2d_x.cl
+-rw-rw-rw-   0        0        0     1712 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_3d_x.cl
+-rw-rw-rw-   0        0        0      663 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_2d_x.cl
+-rw-rw-rw-   0        0        0      782 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_3d_x.cl
+-rw-rw-rw-   0        0        0     3756 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/piv.cl
+-rw-rw-rw-   0        0        0     2160 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/pointindexlist_to_mesh_3d_x.cl
+-rw-rw-rw-   0        0        0      526 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_2d_x.cl
+-rw-rw-rw-   0        0        0      565 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_3d_x.cl
+-rw-rw-rw-   0        0        0      540 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_2d_x.cl
+-rw-rw-rw-   0        0        0      579 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_3d_x.cl
+-rw-rw-rw-   0        0        0      666 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensities_x.cl
+-rw-rw-rw-   0        0        0      806 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensity_x.cl
+-rw-rw-rw-   0        0        0      710 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_pixels_if_zero_x.cl
+-rw-rw-rw-   0        0        0      717 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_bottom_3d_x.cl
+-rw-rw-rw-   0        0        0      691 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_left_3d_x.cl
+-rw-rw-rw-   0        0        0     1341 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_2d_x.cl
+-rw-rw-rw-   0        0        0     1353 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_3d_x.cl
+-rw-rw-rw-   0        0        0      718 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_right_3d_x.cl
+-rw-rw-rw-   0        0        0      689 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_top_3d_x.cl
+-rw-rw-rw-   0        0        0      634 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_2d_x.cl
+-rw-rw-rw-   0        0        0      714 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_3d_x.cl
+-rw-rw-rw-   0        0        0      637 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_2d_x.cl
+-rw-rw-rw-   0        0        0      720 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_3d_x.cl
+-rw-rw-rw-   0        0        0      218 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_2d_x.cl
+-rw-rw-rw-   0        0        0      260 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_3d_x.cl
+-rw-rw-rw-   0        0        0      232 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_column_2d_x.cl
+-rw-rw-rw-   0        0        0      274 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_column_3d_x.cl
+-rw-rw-rw-   0        0        0      347 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_image_borders_2d_x.cl
+-rw-rw-rw-   0        0        0      425 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_image_borders_3d_x.cl
+-rw-rw-rw-   0        0        0      756 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_nonzero_pixels_to_pixelindex_x.cl
+-rw-rw-rw-   0        0        0      275 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_plane_2d_x.cl
+-rw-rw-rw-   0        0        0      271 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_plane_3d_x.cl
+-rw-rw-rw-   0        0        0      206 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_x_2d_x.cl
+-rw-rw-rw-   0        0        0      245 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_x_3d_x.cl
+-rw-rw-rw-   0        0        0      206 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_y_2d_x.cl
+-rw-rw-rw-   0        0        0      245 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_y_3d_x.cl
+-rw-rw-rw-   0        0        0      182 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_z_2d_x.cl
+-rw-rw-rw-   0        0        0      245 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_ramp_z_3d_x.cl
+-rw-rw-rw-   0        0        0      223 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_row_2d_x.cl
+-rw-rw-rw-   0        0        0      265 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_row_3d_x.cl
+-rw-rw-rw-   0        0        0      254 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_equals_y_2d_x.cl
+-rw-rw-rw-   0        0        0      290 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_equals_y_3d_x.cl
+-rw-rw-rw-   0        0        0      259 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_greater_than_y_2d_x.cl
+-rw-rw-rw-   0        0        0      299 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_greater_than_y_3d_x.cl
+-rw-rw-rw-   0        0        0      259 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_smaller_than_y_2d_x.cl
+-rw-rw-rw-   0        0        0      300 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_where_x_smaller_than_y_3d_x.cl
+-rw-rw-rw-   0        0        0      594 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_2d_x.cl
+-rw-rw-rw-   0        0        0      634 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_3d_x.cl
+-rw-rw-rw-   0        0        0      525 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_2d_x.cl
+-rw-rw-rw-   0        0        0      565 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_3d_x.cl
+-rw-rw-rw-   0        0        0      604 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_2d_x.cl
+-rw-rw-rw-   0        0        0      644 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_3d_x.cl
+-rw-rw-rw-   0        0        0      535 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_2d_x.cl
+-rw-rw-rw-   0        0        0      575 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_3d_x.cl
+-rw-rw-rw-   0        0        0     1612 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_2d_x.cl
+-rw-rw-rw-   0        0        0     1550 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_3d_x.cl
+-rw-rw-rw-   0        0        0     2597 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_of_touching_neighbors_x.cl
+-rw-rw-rw-   0        0        0      847 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_z_projection_x.cl
+-rw-rw-rw-   0        0        0      492 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/subtract_image_from_scalar_2d_x.cl
+-rw-rw-rw-   0        0        0      531 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/subtract_image_from_scalar_3d_x.cl
+-rw-rw-rw-   0        0        0      567 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_reduction_x_x.cl
+-rw-rw-rw-   0        0        0      504 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_x_projection_x.cl
+-rw-rw-rw-   0        0        0      505 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_y_projection_x.cl
+-rw-rw-rw-   0        0        0      504 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_z_projection_x.cl
+-rw-rw-rw-   0        0        0     2224 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/touch_matrix_to_mesh_3d_x.cl
+-rw-rw-rw-   0        0        0      553 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xy_3d_x.cl
+-rw-rw-rw-   0        0        0      547 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xz_3d_x.cl
+-rw-rw-rw-   0        0        0      545 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_yz_3d_x.cl
+-rw-rw-rw-   0        0        0      531 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/undefined_to_zero_x.cl
+-rw-rw-rw-   0        0        0      599 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_2d_x.cl
+-rw-rw-rw-   0        0        0      725 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_masked_projection_x.cl
+-rw-rw-rw-   0        0        0      581 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_projection_x.cl
+-rw-rw-rw-   0        0        0     1051 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_2d_x.cl
+-rw-rw-rw-   0        0        0     1186 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_3d_x.cl
+-rw-rw-rw-   0        0        0     1091 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_2d.cl
+-rw-rw-rw-   0        0        0     1215 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_3d.cl
+-rw-rw-rw-   0        0        0     1421 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_2d_x.cl
+-rw-rw-rw-   0        0        0     1551 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_3d_x.cl
+-rw-rw-rw-   0        0        0     1594 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_2d_x.cl
+-rw-rw-rw-   0        0        0     1704 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_3d_x.cl
+-rw-rw-rw-   0        0        0      712 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_2d_x.cl
+-rw-rw-rw-   0        0        0      804 2021-06-16 18:09:30.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_3d_x.cl
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:05.403037 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/
+-rw-rw-rw-   0        0        0    18603 2021-08-01 09:36:04.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    49188 2021-08-01 09:36:05.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-01 09:36:04.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2021-08-01 09:36:04.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2021-08-01 09:36:04.000000 pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-08-01 09:36:06.739340 pyclesperanto_prototype-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      973 2021-08-01 09:34:37.000000 pyclesperanto_prototype-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-08-01 09:36:06.737339 pyclesperanto_prototype-0.9.9/tests/
+-rw-rw-rw-   0        0        0      187 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/__init__.py
+-rw-rw-rw-   0        0        0      544 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_absolute.py
+-rw-rw-rw-   0        0        0      346 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_absolute_difference.py
+-rw-rw-rw-   0        0        0      624 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_add_image_and_scalar.py
+-rw-rw-rw-   0        0        0     1279 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_add_images.py
+-rw-rw-rw-   0        0        0     1915 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_add_images_weighted.py
+-rw-rw-rw-   0        0        0     3596 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_affine_transform.py
+-rw-rw-rw-   0        0        0     4708 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_apply_vector_field.py
+-rw-rw-rw-   0        0        0      902 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_average_distance_of_n_far_off_distances.py
+-rw-rw-rw-   0        0        0      894 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_average_distance_of_n_shortest_distances.py
+-rw-rw-rw-   0        0        0      951 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_average_distance_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0      749 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_binary_and.py
+-rw-rw-rw-   0        0        0      541 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_binary_edge_detection.py
+-rw-rw-rw-   0        0        0      367 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_binary_not.py
+-rw-rw-rw-   0        0        0      448 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_binary_or.py
+-rw-rw-rw-   0        0        0      460 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_binary_subtract.py
+-rw-rw-rw-   0        0        0      449 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_binary_xor.py
+-rw-rw-rw-   0        0        0      926 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_block_enumerate.py
+-rw-rw-rw-   0        0        0      466 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_bottom_hat_box.py
+-rw-rw-rw-   0        0        0      469 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_bottom_hat_sphere.py
+-rw-rw-rw-   0        0        0      947 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_bounding_box.py
+-rw-rw-rw-   0        0        0      310 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_center_of_mass.py
+-rw-rw-rw-   0        0        0     1233 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_centroids_of_labels.py
+-rw-rw-rw-   0        0        0      542 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_combine_horizontally.py
+-rw-rw-rw-   0        0        0      548 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_combine_vertically.py
+-rw-rw-rw-   0        0        0      783 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_concatenate_stacks.py
+-rw-rw-rw-   0        0        0     1633 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_connected_components_labeling_box.py
+-rw-rw-rw-   0        0        0      631 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_connected_components_labeling_diamond.py
+-rw-rw-rw-   0        0        0      547 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_convolve.py
+-rw-rw-rw-   0        0        0      357 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_copy.py
+-rw-rw-rw-   0        0        0     2464 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_copy_slice.py
+-rw-rw-rw-   0        0        0      696 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_count_touching_neighbors.py
+-rw-rw-rw-   0        0        0     3313 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_create.py
+-rw-rw-rw-   0        0        0     1194 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_crop.py
+-rw-rw-rw-   0        0        0      383 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_degrees_to_radians.py
+-rw-rw-rw-   0        0        0      654 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_detect_label_edges.py
+-rw-rw-rw-   0        0        0      733 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_detect_maxima_box.py
+-rw-rw-rw-   0        0        0      733 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_detect_minima_box.py
+-rw-rw-rw-   0        0        0      545 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_difference_of_gaussian.py
+-rw-rw-rw-   0        0        0      618 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_dilate_box.py
+-rw-rw-rw-   0        0        0     1379 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_dilate_box_slice_by_slice.py
+-rw-rw-rw-   0        0        0     2020 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_dilate_labels.py
+-rw-rw-rw-   0        0        0      628 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_dilate_sphere.py
+-rw-rw-rw-   0        0        0     1385 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_dilate_sphere_slice_by_slice.py
+-rw-rw-rw-   0        0        0      814 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_divide_images.py
+-rw-rw-rw-   0        0        0     1519 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_downsample_xy_half_median.py
+-rw-rw-rw-   0        0        0      483 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_draw_box.py
+-rw-rw-rw-   0        0        0      488 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_draw_line.py
+-rw-rw-rw-   0        0        0      489 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_draw_sphere.py
+-rw-rw-rw-   0        0        0      791 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_equal.py
+-rw-rw-rw-   0        0        0      632 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_equal_constant.py
+-rw-rw-rw-   0        0        0      616 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_erode_box.py
+-rw-rw-rw-   0        0        0     1379 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_erode_box_slice_by_slice.py
+-rw-rw-rw-   0        0        0     3313 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_erode_labels.py
+-rw-rw-rw-   0        0        0      622 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_erode_sphere.py
+-rw-rw-rw-   0        0        0     1385 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_erode_sphere_slice_by_slice.py
+-rw-rw-rw-   0        0        0      750 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_euclidean_distance_from_label_centroid_map.py
+-rw-rw-rw-   0        0        0     1805 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_exclude_labels.py
+-rw-rw-rw-   0        0        0     3646 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_on_edges.py
+-rw-rw-rw-   0        0        0     2084 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_out_of_size_range.py
+-rw-rw-rw-   0        0        0      569 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_with_values_out_of_range.py
+-rw-rw-rw-   0        0        0      569 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_with_values_within_range.py
+-rw-rw-rw-   0        0        0      353 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_execute.py
+-rw-rw-rw-   0        0        0      701 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_exponential.py
+-rw-rw-rw-   0        0        0      843 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_extend_labeling_via_voronoi.py
+-rw-rw-rw-   0        0        0     1881 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_extended_depth_of_focus_variance_projection.py
+-rw-rw-rw-   0        0        0      518 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_flag_existing_labels.py
+-rw-rw-rw-   0        0        0      626 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_flip.py
+-rw-rw-rw-   0        0        0      556 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_gamma_correction.py
+-rw-rw-rw-   0        0        0      482 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_gaussian_blur.py
+-rw-rw-rw-   0        0        0      828 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_generate_angle_matrix.py
+-rw-rw-rw-   0        0        0     1825 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_generate_binary_overlap_matrix.py
+-rw-rw-rw-   0        0        0     1016 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_generate_distance_matrix.py
+-rw-rw-rw-   0        0        0      855 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_generate_n_nearest_neighbor_matrix.py
+-rw-rw-rw-   0        0        0     1644 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_generate_proximal_neighbor_matrix.py
+-rw-rw-rw-   0        0        0      743 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_generate_touch_matrix.py
+-rw-rw-rw-   0        0        0      521 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_gpu_switch.py
+-rw-rw-rw-   0        0        0      617 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_gradient_x.py
+-rw-rw-rw-   0        0        0      619 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_gradient_y.py
+-rw-rw-rw-   0        0        0     1357 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_gradient_z.py
+-rw-rw-rw-   0        0        0     1670 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_greater.py
+-rw-rw-rw-   0        0        0      638 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_greater_constant.py
+-rw-rw-rw-   0        0        0     1637 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_greater_or_equal.py
+-rw-rw-rw-   0        0        0      656 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_greater_or_equal_constant.py
+-rw-rw-rw-   0        0        0     1590 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_histogram.py
+-rw-rw-rw-   0        0        0      890 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_image.py
+-rw-rw-rw-   0        0        0      469 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_invert.py
+-rw-rw-rw-   0        0        0      668 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_jaccard_index.py
+-rw-rw-rw-   0        0        0     1169 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_maximum_extension_map.py
+-rw-rw-rw-   0        0        0     1179 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_maximum_extension_ratio_map.py
+-rw-rw-rw-   0        0        0     1390 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_maximum_intensity_map.py
+-rw-rw-rw-   0        0        0     1157 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_mean_extension_map.py
+-rw-rw-rw-   0        0        0     1378 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_mean_intensity_map.py
+-rw-rw-rw-   0        0        0     1390 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_minimum_intensity_map.py
+-rw-rw-rw-   0        0        0     1060 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_pixelcount_map.py
+-rw-rw-rw-   0        0        0     1541 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_spots.py
+-rw-rw-rw-   0        0        0     1472 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_label_standard_deviation_intensity_map.py
+-rw-rw-rw-   0        0        0      649 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_labelled_spots_to_pointlist.py
+-rw-rw-rw-   0        0        0      630 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_laplace_box.py
+-rw-rw-rw-   0        0        0      632 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_laplace_diamond.py
+-rw-rw-rw-   0        0        0      464 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_logarithm.py
+-rw-rw-rw-   0        0        0      784 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_mask.py
+-rw-rw-rw-   0        0        0      799 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_mask_label.py
+-rw-rw-rw-   0        0        0     1114 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_masked_voronoi_labeling.py
+-rw-rw-rw-   0        0        0      627 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_box.py
+-rw-rw-rw-   0        0        0      894 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_distance_of_n_shortest_distances.py
+-rw-rw-rw-   0        0        0      975 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_distance_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0      545 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_image_and_scalar.py
+-rw-rw-rw-   0        0        0      804 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_images.py
+-rw-rw-rw-   0        0        0      614 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_of_all_pixels.py
+-rw-rw-rw-   0        0        0      740 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0      868 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_sphere.py
+-rw-rw-rw-   0        0        0     1797 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_x_projection.py
+-rw-rw-rw-   0        0        0     1355 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_y_projection.py
+-rw-rw-rw-   0        0        0     1625 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_maximum_z_projection.py
+-rw-rw-rw-   0        0        0      622 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_box.py
+-rw-rw-rw-   0        0        0     1213 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_of_all_pixels.py
+-rw-rw-rw-   0        0        0      758 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0      658 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_sphere.py
+-rw-rw-rw-   0        0        0      269 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_squared_error.py
+-rw-rw-rw-   0        0        0     1408 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_x_projection.py
+-rw-rw-rw-   0        0        0     1403 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_y_projection.py
+-rw-rw-rw-   0        0        0     1384 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_mean_z_projection.py
+-rw-rw-rw-   0        0        0      646 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_median_box.py
+-rw-rw-rw-   0        0        0      652 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_median_sphere.py
+-rw-rw-rw-   0        0        0     1374 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_merge_touching_labels.py
+-rw-rw-rw-   0        0        0      627 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_box.py
+-rw-rw-rw-   0        0        0      974 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_distance_of_touching_neighbors.py
+-rw-rw-rw-   0        0        0      549 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_image_and_scalar.py
+-rw-rw-rw-   0        0        0      804 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_images.py
+-rw-rw-rw-   0        0        0      612 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_of_all_pixels.py
+-rw-rw-rw-   0        0        0     1690 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_of_masked_pixels.py
+-rw-rw-rw-   0        0        0      740 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0     1429 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_x_projection.py
+-rw-rw-rw-   0        0        0     1342 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_y_projection.py
+-rw-rw-rw-   0        0        0     1342 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_minimum_z_projection.py
+-rw-rw-rw-   0        0        0      818 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_mode_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0      553 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_multiply_image_and_coordinate.py
+-rw-rw-rw-   0        0        0      547 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_multiply_image_and_scalar.py
+-rw-rw-rw-   0        0        0      809 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_multiply_images.py
+-rw-rw-rw-   0        0        0      911 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_multiply_matrix.py
+-rw-rw-rw-   0        0        0     2054 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_n_closest_points.py
+-rw-rw-rw-   0        0        0      809 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_nonzero_maximum_box.py
+-rw-rw-rw-   0        0        0      816 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_nonzero_maximum_diamond.py
+-rw-rw-rw-   0        0        0      808 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_nonzero_minimum_box.py
+-rw-rw-rw-   0        0        0      818 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_nonzero_minimum_diamond.py
+-rw-rw-rw-   0        0        0      794 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_not_equal.py
+-rw-rw-rw-   0        0        0      640 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_not_equal_constant.py
+-rw-rw-rw-   0        0        0      699 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_onlyzero_overwrite_maximum_box.py
+-rw-rw-rw-   0        0        0      704 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_onlyzero_overwrite_maximum_diamond.py
+-rw-rw-rw-   0        0        0    18430 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_operators.py
+-rw-rw-rw-   0        0        0      627 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_paste.py
+-rw-rw-rw-   0        0        0      756 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_point_index_list_to_mesh.py
+-rw-rw-rw-   0        0        0      858 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_point_index_list_to_touch_matrix.py
+-rw-rw-rw-   0        0        0     1588 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_pointlist_to_labelled_spots.py
+-rw-rw-rw-   0        0        0      622 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_power.py
+-rw-rw-rw-   0        0        0      812 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_power_images.py
+-rw-rw-rw-   0        0        0      775 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_proximal_neighbor_count_map.py
+-rw-rw-rw-   0        0        0      663 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_push.py
+-rw-rw-rw-   0        0        0     1024 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_push_regionprops_column.py
+-rw-rw-rw-   0        0        0      383 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_radians_to_degrees.py
+-rw-rw-rw-   0        0        0      601 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_read_intensities_from_map.py
+-rw-rw-rw-   0        0        0      587 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_read_intensities_from_positions.py
+-rw-rw-rw-   0        0        0     1365 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_reduce_stack.py
+-rw-rw-rw-   0        0        0     3707 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_reduction.py
+-rw-rw-rw-   0        0        0     7790 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_regionprops.py
+-rw-rw-rw-   0        0        0      615 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_relabel_sequential.py
+-rw-rw-rw-   0        0        0      724 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_replace_intensities.py
+-rw-rw-rw-   0        0        0      645 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_replace_intensity.py
+-rw-rw-rw-   0        0        0     5116 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_resample.py
+-rw-rw-rw-   0        0        0      675 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_rigid_transform.py
+-rw-rw-rw-   0        0        0     1328 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_rotate.py
+-rw-rw-rw-   0        0        0     1223 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_scale.py
+-rw-rw-rw-   0        0        0      435 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_set.py
+-rw-rw-rw-   0        0        0      593 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_column.py
+-rw-rw-rw-   0        0        0      604 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_set_image_borders.py
+-rw-rw-rw-   0        0        0      591 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_nonzero_pixels_to_pixelindex.py
+-rw-rw-rw-   0        0        0     1010 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_plane.py
+-rw-rw-rw-   0        0        0      694 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_ramp_x.py
+-rw-rw-rw-   0        0        0      694 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_ramp_y.py
+-rw-rw-rw-   0        0        0      680 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_ramp_z.py
+-rw-rw-rw-   0        0        0      587 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_row.py
+-rw-rw-rw-   0        0        0      121 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_wait_for_kernel_finish.py
+-rw-rw-rw-   0        0        0      525 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_set_where_x_equals_y.py
+-rw-rw-rw-   0        0        0      541 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_where_x_greater_than_y.py
+-rw-rw-rw-   0        0        0      541 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_set_where_x_smaller_than_y.py
+-rw-rw-rw-   0        0        0      170 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_skimage_imsave.py
+-rw-rw-rw-   0        0        0     1624 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_smaller.py
+-rw-rw-rw-   0        0        0      636 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_smaller_constant.py
+-rw-rw-rw-   0        0        0     1633 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_smaller_or_equal.py
+-rw-rw-rw-   0        0        0      645 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_smaller_or_equal_constant.py
+-rw-rw-rw-   0        0        0      631 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_sobel.py
+-rw-rw-rw-   0        0        0      745 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_sorenson_dice_coefficient.py
+-rw-rw-rw-   0        0        0      606 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_spots_to_pointlist.py
+-rw-rw-rw-   0        0        0      345 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_squared_difference.py
+-rw-rw-rw-   0        0        0      849 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_standard_deviation_of_touching_neighbors_map.py
+-rw-rw-rw-   0        0        0     1448 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_standard_deviation_z_projection.py
+-rw-rw-rw-   0        0        0     9731 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_statistics_of_background_and_labelled_pixels.py
+-rw-rw-rw-   0        0        0      482 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_statistics_of_image.py
+-rw-rw-rw-   0        0        0     7337 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_statistics_of_labelled_pixels.py
+-rw-rw-rw-   0        0        0      495 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_subtract_image_from_scalar.py
+-rw-rw-rw-   0        0        0      338 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_subtract_images.py
+-rw-rw-rw-   0        0        0     1205 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_sum_of_all_pixels.py
+-rw-rw-rw-   0        0        0      694 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_sum_reduction.py
+-rw-rw-rw-   0        0        0     1355 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_sum_x_projection.py
+-rw-rw-rw-   0        0        0     1353 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_sum_y_projection.py
+-rw-rw-rw-   0        0        0     1368 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_sum_z_projection.py
+-rw-rw-rw-   0        0        0      780 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_threshold_otsu.py
+-rw-rw-rw-   0        0        0      460 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_top_hat_box.py
+-rw-rw-rw-   0        0        0      463 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_top_hat_sphere.py
+-rw-rw-rw-   0        0        0      743 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_touch_matrix_to_adjacency_matrix.py
+-rw-rw-rw-   0        0        0      887 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_touch_matrix_to_mesh.py
+-rw-rw-rw-   0        0        0      743 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_touching_neighbor_count_map.py
+-rw-rw-rw-   0        0        0      649 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_translate.py
+-rw-rw-rw-   0        0        0     1543 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_transpose_xy.py
+-rw-rw-rw-   0        0        0     1529 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_transpose_xz.py
+-rw-rw-rw-   0        0        0     1545 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_transpose_yz.py
+-rw-rw-rw-   0        0        0      896 2021-06-16 18:09:28.000000 pyclesperanto_prototype-0.9.9/tests/test_undefined_to_zero.py
+-rw-rw-rw-   0        0        0      677 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_variance_box.py
+-rw-rw-rw-   0        0        0      653 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_variance_sphere.py
+-rw-rw-rw-   0        0        0      821 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_voronoi_labeling.py
+-rw-rw-rw-   0        0        0      896 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_voronoi_otsu_labeling.py
+-rw-rw-rw-   0        0        0     1778 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_write_values_to_positions.py
+-rw-rw-rw-   0        0        0     1697 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_z_position_of_maximum_z_projection.py
+-rw-rw-rw-   0        0        0     1697 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_z_position_of_minimum_z_projection.py
+-rw-rw-rw-   0        0        0     1858 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_z_position_projection.py
+-rw-rw-rw-   0        0        0     2284 2021-08-01 08:45:56.000000 pyclesperanto_prototype-0.9.9/tests/test_z_position_range_projection.py
```

### Comparing `pyclesperanto_prototype-0.9.7/LICENSE` & `pyclesperanto_prototype-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/PKG-INFO` & `pyclesperanto_prototype-0.9.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pyclesperanto_prototype
-Version: 0.9.7
-Summary: OpenCL-based GPU-accelerated image processing
-Home-page: https://github.com/clEsperanto/pyclesperanto_prototype
-Author: haesleinhuepf
-Author-email: robert.haase@tu-dresden.de
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # py-clEsperanto
 [![Image.sc forum](https://img.shields.io/badge/dynamic/json.svg?label=forum&url=https%3A%2F%2Fforum.image.sc%2Ftag%2Fclesperanto.json&query=%24.topic_list.tags.0.topic_count&colorB=brightgreen&suffix=%20topics&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAYAAAAfSC3RAAABPklEQVR42m3SyyqFURTA8Y2BER0TDyExZ+aSPIKUlPIITFzKeQWXwhBlQrmFgUzMMFLKZeguBu5y+//17dP3nc5vuPdee6299gohUYYaDGOyyACq4JmQVoFujOMR77hNfOAGM+hBOQqB9TjHD36xhAa04RCuuXeKOvwHVWIKL9jCK2bRiV284QgL8MwEjAneeo9VNOEaBhzALGtoRy02cIcWhE34jj5YxgW+E5Z4iTPkMYpPLCNY3hdOYEfNbKYdmNngZ1jyEzw7h7AIb3fRTQ95OAZ6yQpGYHMMtOTgouktYwxuXsHgWLLl+4x++Kx1FJrjLTagA77bTPvYgw1rRqY56e+w7GNYsqX6JfPwi7aR+Y5SA+BXtKIRfkfJAYgj14tpOF6+I46c4/cAM3UhM3JxyKsxiOIhH0IO6SH/A1Kb1WBeUjbkAAAAAElFTkSuQmCC)](https://forum.image.sc/tag/clesperanto)
 [![website](https://img.shields.io/website?url=http%3A%2F%2Fclesperanto.net)](http://clesperanto.net)
 [![PyPI](https://img.shields.io/pypi/v/pyclesperanto-prototype.svg?color=green)](https://pypi.org/project/pyclesperanto-prototype)
 [![Contributors](https://img.shields.io/github/contributors-anon/clEsperanto/pyclesperanto_prototype)](https://github.com/clEsperanto/pyclesperanto_prototype/graphs/contributors)
 [![GitHub stars](https://img.shields.io/github/stars/clEsperanto/pyclesperanto_prototype?style=social)](https://github.com/clEsperanto/pyclesperanto_prototype/)
 [![GitHub forks](https://img.shields.io/github/forks/clEsperanto/pyclesperanto_prototype?style=social)](https://github.com/clEsperanto/pyclesperanto_prototype/)
@@ -118,159 +100,182 @@
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_count_blobs.png" width="300"/>
 
 </td><td>
 
-[Counting blobs](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/count_blobs.ipynb)
+[Counting blobs](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/count_blobs.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/voronoi_otsu_labeling.png" width="300"/>
 
 </td><td>
 
-[Voronoi-Otsu labeling](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/voronoi_otsu_labeling.ipynb)
+[Voronoi-Otsu labeling](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/voronoi_otsu_labeling.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/segmentation_3d.png" width="300"/>
 
 </td><td>
 
-[3D Image segmentation ](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/Segmentation_3D.ipynb)
+[3D Image segmentation ](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/Segmentation_3D.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/segmentation_2d_membranes.png" width="300"/>
 
 </td><td>
 
-[Cell segmentation based on membranes](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/segmentation_2d_membranes.ipynb)
+[Cell segmentation based on membranes](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/segmentation_2d_membranes.ipynb)
 
-</td></tr><tr><td>
+</td></tr>
+
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/bead_segmentation.png" width="300"/>
+
+</td><td>
+
+[Detecting beads and measuring their size](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/bead_segmentation.ipynb)
+
+</td></tr>
+
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/parametric_maps.png" width="300"/>
+
+</td><td>
+
+[Parametric maps](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/tissues/parametric_maps.ipynb)
+
+</td></tr>
+
+
+<tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_crop_and_paste_images.png" width="300"/>
 
 </td><td>
 
-[Crop and paste images](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/crop_and_paste_images.ipynb)
+[Crop and paste images](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/crop_and_paste_images.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_inspecting_3d_images.png" width="300"/>
 
 </td><td>
 
-[Inspecting 3D image data](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/inspecting_3d_images.ipynb)
+[Inspecting 3D image data](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/inspecting_3d_images.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_affine_transforms.png" width="300"/>
 
 </td><td>
 
-[Rotation, scaling, translation, affine transforms](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/transforms/affine_transforms.ipynb)
+[Rotation, scaling, translation, affine transforms](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/transforms/affine_transforms.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_multiply_vectors_and_matrices.png" width="300"/>
 
 </td><td>
 
-[Multiply vectors and matrices](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_vectors_and_matrices.ipynb)
+[Multiply vectors and matrices](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_vectors_and_matrices.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_multiply_matrices.png" width="300"/>
 
 </td><td>
 
-[Matrix multiplication](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_matrices.ipynb)
+[Matrix multiplication](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_matrices.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_spots_pointlists_matrices_tables.png" width="300"/>
 
 </td><td>
 
-[Working with spots, pointlist and matrices](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/spots_pointlists_matrices_tables.ipynb)
+[Working with spots, pointlist and matrices](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/spots_pointlists_matrices_tables.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_between_centroids.png" width="300"/>
 
 </td><td>
 
-[Mesh between centroids](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_centroids.ipynb)
+[Mesh between centroids](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_centroids.ipynb)
 
 </td></tr><tr><td>
 
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_between_touching_neighbors.png" width="300"/>
 
 </td><td>
 
-[Mesh between touching neighbors](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_touching_neighbors.ipynb)
+[Mesh between touching neighbors](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_touching_neighbors.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_with_distances.png" width="300"/>
 
 </td><td>
 
-[Mesh with distances](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_with_distances.ipynb)
+[Mesh with distances](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_with_distances.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_nearest_neighbors.png" width="300"/>
 
 </td><td>
 
-[Mesh nearest_neighbors](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_nearest_neighbors.ipynb)
+[Mesh nearest_neighbors](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_nearest_neighbors.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/neighborhood_definitions.png" width="300"/>
 
 </td><td>
 
-[Neighborhood definitions](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighborhood_definitions.ipynb)
+[Neighborhood definitions](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighborhood_definitions.ipynb)
 
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/tissue_neighborhood_quantification.png" width="300"/>
 
 </td><td>
 
-[Tissue neighborhood quantification](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/tissues/tissue_neighborhood_quantification.ipynb)
+[Tissue neighborhood quantification](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/tissues/tissue_neighborhood_quantification.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/neighbors_of_neighbors.png" width="300"/>
 
 </td><td>
 
-[Neighbors of neighbors](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighbors_of_neighbors.ipynb)
+[Neighbors of neighbors](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighbors_of_neighbors.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_voronoi_diagrams.png" width="300"/>
 
 </td><td>
 
-[Voronoi diagrams](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/voronoi_diagrams.ipynb)
+[Voronoi diagrams](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/voronoi_diagrams.ipynb)
 
 </td></tr><tr><td>
 
 </td><td>
 
-[Shape descriptors based on neighborhood graphs](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/shape_descriptors_based_on_neighborhood_graphs.ipynb)
+[Shape descriptors based on neighborhood graphs](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/shape_descriptors_based_on_neighborhood_graphs.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_tribolium_napari.png" width="300"/>
 
 </td><td>
 
@@ -278,50 +283,121 @@
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_tribolium_morphometry.png" width="300"/>
 
 </td><td>
 
-[Tribolium morphometry](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/tribolium_morphometry/tribolium_morphometry.ipynb)
+[Tribolium morphometry](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/tribolium_morphometry/tribolium_morphometry.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_napari_dask.png" width="300"/>
 
 </td><td>
 
-[napari+dask timelapse processing](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/napari_gui/napari_dask.ipynb)
+[napari+dask timelapse processing](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/napari_gui/napari_dask.ipynb)
 
-</td></tr><tr><td>
+</td></tr>
+</table>
+
+## Technical insights
+
+<table border="0"><tr><td>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/browse_operations.png" width="300"/>
+
+</td><td>
+
+[Browsing operations](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/browse_operations.ipynb)
+
+</td></tr>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/interactive_widgets.gif" width="300"/>
+
+</td><td>
+
+[Interactive widgets](https://colab.research.google.com/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/browse_operations.ipynb)
+
+</td></tr>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/optimize_blobs_segmentation.png" width="300"/>
+
+</td><td>
+
+[Automatic workflow optimization](https://colab.research.google.com/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/optimization/optimize_blobs_segmentation.ipynb)
+
+</td></tr>
+
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/switching_gpus.png" width="300"/>
+
+</td><td>
+
+[Exploring and switching between GPUs](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/switching_gpus.ipynb)
+
+</td></tr>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/cupy_compatibility.png" width="300"/>
+
+</td><td>
+
+[Interoperability with cupy](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/interoperability_cupy.ipynb)
+
+</td></tr>
+</table>
+
+## Related projects
+
+<table border="0"><tr><td>
 
 <img src="https://github.com/clesperanto/napari_pyclesperanto_assistant/raw/master/docs/images/screenshot.png" width="300"/>
 
 </td><td>
 
-[pyclesperanto assistant](https://github.com/clesperanto/napari_pyclesperanto_assistant)
+[napari-pyclesperanto-assistant](https://github.com/clesperanto/napari_pyclesperanto_assistant):
+A graphical user interface for general purpose GPU-accelerated image processing and analysis in napari.
+
+</td></tr><tr><td>
+
+<img src="https://github.com/haesleinhuepf/napari-oclrfc/raw/master/images/screenshot.png" width="300"/>
+
+</td><td>
+
+[napari-oclrfc](https://github.com/haesleinhuepf/napari-oclrfc):
+GPU-accelerated Random Forest Classifiers for pixel and labeled object classification
 
 </td></tr></table>
 
 ## Benchmarking
 We implemented some basic benchmarking notebooks allowing to see performance differences between pyclesperanto and 
 some other image processing libraries, typically using the CPU. Such benchmarking results vary heavily depending on 
 image size, kernel size, used operations, parameters and used hardware. Feel free to use those notebooks, adapt them to 
 your use-case scenario and benchmark on your target hardware. If you have different scenarios or use-cases, you are very 
 welcome to submit your notebook as pull-request!
 
-* [Affine transforms](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/affine_transforms.ipynb)
-* [Gaussian blur](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/gaussian_blur.ipynb)
-* [Convolution](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/convolution.ipynb)
-* [Otsu's thresholding](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/threshold_otsu.ipynb)
-* [Connected component labeling](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/connected_component_labeling.ipynb)  
-* [Extend labels](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/extend_labels.ipynb)
-* [Statistics of labeled pixels / regionprops](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/statistics_of_labeled_pixels.ipynb)
-* [Matrix multiplication](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/matrix_multiplication.ipynb)
-* [Pixel-wise comparison](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/pixelwise_comparison.ipynb)
-* [Intensity projections](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/intensity_projections.ipynb)
-* [Axis transposition](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/transpose.ipynb)
+* [Affine transforms](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/affine_transforms.ipynb)
+* [Gaussian blur](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/gaussian_blur.ipynb)
+* [Convolution](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/convolution.ipynb)
+* [Otsu's thresholding](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/threshold_otsu.ipynb)
+* [Connected component labeling](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/connected_component_labeling.ipynb)  
+* [Extend labels](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/extend_labels.ipynb)
+* [Statistics of labeled pixels / regionprops](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/statistics_of_labeled_pixels.ipynb)
+* [Matrix multiplication](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/matrix_multiplication.ipynb)
+* [Pixel-wise comparison](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/pixelwise_comparison.ipynb)
+* [Intensity projections](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/intensity_projections.ipynb)
+* [Axis transposition](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/transpose.ipynb)
+
+## See also
+There are other libraries for code acceleration and GPU-acceleration for image processing.
+* [numba](https://numba.pydata.org/)
+* [cupy](https://cupy.dev)
+* [cucim](https://github.com/rapidsai/cucim)
+* [clij](https://clij.github.io)
 
 ## Feedback welcome!
 clEsperanto is developed in the open because we believe in the open source community. See our [community guidelines](https://clij.github.io/clij2-docs/community_guidelines). Feel free to drop feedback as [github issue](https://github.com/clEsperanto/pyclesperanto_prototype/issues) or via [image.sc](https://image.sc)
-
-
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/__init__.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,20 +22,21 @@
     create_2d_zy,
     create_2d_yz,
     create_none,
 )
 from ._execute import execute
 from ._operations import operation
 from ._operations import operations
+from ._operations import search_operation_names
 from ._pull import pull_zyx
 from ._pull import pull
 from ._pull import pull as nparray
 from ._push import push_zyx
 from ._push import push
 from ._push import push as asarray
 from ._plugin_function import plugin_function
 from ._types import Image
 from ._cl_info import cl_info
-from ._pycl import get_device, select_device, set_device_scoring_key
+from ._device import get_device, select_device, set_device_scoring_key
 from ._cl_image import create_image, empty_image_like, empty_image
 from ._available_device_names import available_device_names
 from ._set_wait_for_kernel_finish import set_wait_for_kernel_finish
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_available_device_names.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_available_device_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .._tier0._pycl import filter_devices
+from .._tier0._device import filter_devices
 from typing import List
 
 def available_device_names(dev_type: str = None, score_key = None) -> List[str]:
     """Retrieve a list of names of available OpenCL-devices
 
     Parameters
     ----------
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_cl_image.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_cl_image.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_cl_info.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_cl_info.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_create.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_create.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_execute.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 from functools import lru_cache
 from pathlib import Path
 
 import numpy as np
 
 import pyopencl as cl
-from ._pycl import OCLProgram, _OCLImage
+from ._pycl import _OCLImage
+from ._device import Device
+from ._program import OCLProgram
 
 if not os.getenv("PYOPENCL_COMPILER_OUTPUT"):
     import warnings
     warnings.filterwarnings('ignore', 'Non-empty compiler output', module='pyopencl')
 
 
 # should write a test to make sure kernels and filenames always match
@@ -64,15 +66,15 @@
 
 IMAGE_HEADER = COMMON_HEADER + """
 #define IMAGE_{key}_TYPE {size_parameters} {type_name} 
 #define READ_{key}_IMAGE(a,b,c) read_image{typeId}(a,b,c)
 #define WRITE_{key}_IMAGE(a,b,c) write_image{typeId}(a,b,c)
 """
 
-def execute(anchor, opencl_kernel_filename, kernel_name, global_size, parameters, prog : OCLProgram = None, constants = None, image_size_independent_kernel_compilation : bool = True):
+def execute(anchor, opencl_kernel_filename, kernel_name, global_size, parameters, prog : OCLProgram = None, constants = None, image_size_independent_kernel_compilation : bool = True, device: Device = None):
     """
     Convenience method for calling opencl kernel files
 
     This method basically does the same as the CLKernelExecutor in CLIJ:
     https://github.com/clij/clij-clearcl/blob/master/src/main/java/net/haesleinhuepf/clij/clearcl/util/CLKernelExecutor.java
 
     :param anchor: Enter __file__ when calling this method and the corresponding open.cl
@@ -270,16 +272,20 @@
             )
 
     # print("Assembling " + opencl_kernel_filename + " took " + str((time.time() - time_stamp) * 1000) + " ms")
     if prog is None:
         # time_stamp = time.time()
 
         defines.append(get_ocl_source(anchor, opencl_kernel_filename))
-        
-        prog = OCLProgram.from_source("\n".join(defines))
+
+        if device is None:
+            from ._device import get_device
+            device = get_device()
+        prog = device.program_from_source("\n".join(defines))
+        #prog = OCLProgram.from_source("\n".join(defines))
 
         # Todo: the order of the arguments matters; fix that
         # print("Compilation " + opencl_kernel_filename + " took " + str((time.time() - time_stamp) * 1000) + " ms")
 
     prog.run_kernel(kernel_name, tuple(global_size[::-1]), None, *arguments)
 
     return prog
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_operations.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,8 +56,9 @@
     Returns
     -------
         function
     """
     dict = operations()
     return dict[name]
 
-
+def search_operation_names(name):
+    return [a for a in list(operations().keys()) if name in a]
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_plugin_function.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_plugin_function.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_pull.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_pull.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_push.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_push.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/_pycl.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/_pycl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,116 +1,15 @@
 import os
 import sys
+
 import numpy as np
 import pyopencl as cl
 from pyopencl import characterize
 from pyopencl import array
-from typing import Callable, List, Optional
-from functools import lru_cache
-
-
-# TODO: we should discuss whether this collection is actually the best thing to pass
-# around. might be better to work lower level with contexts...
-class Device:
-    """Just a container for a device, context and queue."""
-
-    def __init__(self, device: cl.Device, context: cl.Context, queue: cl.CommandQueue):
-        self.device = device
-        self.context = context
-        self.queue = queue
-
-    def __repr__(self) -> str:
-        refs = self.context.reference_count
-        return f"<{self.name} on Platform: {self.device.platform.name} ({refs} refs)>"
-
-    @property
-    def name(self) -> str:
-        return self.device.name
-
-
-def score_device(dev: cl.Device) -> float:
-    score = 4e12 if dev.type == cl.device_type.GPU else 2e12
-    score += dev.get_info(cl.device_info.GLOBAL_MEM_SIZE)
-    return score
-
-
-# container for singleton device
-class _current_device:
-    _instance: Optional[Device] = None
-    score_key: Callable[[cl.Device], float] = score_device
-
-
-def get_device() -> Device:
-    """Get the current device GPU class."""
-    return _current_device._instance or select_device()
-
-
-def select_device(name: str = None, dev_type: str = None, score_key=None) -> Device:
-    """Set current GPU device based on optional parameters.
-
-    :param name: First device that contains ``name`` will be returned, defaults to None
-    :type name: str, optional
-    :param dev_type: {'cpu', 'gpu', or None}, defaults to None
-    :type dev_type: str, optional
-    :param score_key: scoring function, accepts device and returns int, defaults to None
-    :type score_key: callable, optional
-    :return: The current GPU instance.
-    :rtype: GPU
-    """
-    device = filter_devices(name, dev_type, score_key)[-1]
-    if _current_device._instance and device == _current_device._instance.device:
-        return _current_device._instance
-    context = cl.Context(devices=[device])
-    queue = cl.CommandQueue(context)
-    _current_device._instance = Device(device, context, queue)
-    return _current_device._instance
-
-
-def filter_devices(
-    name: str = None, dev_type: str = None, score_key=None
-) -> List[cl.Device]:
-    """Filter devices based on various options
-
-    :param name: First device that contains ``name`` will be returned, defaults to None
-    :type name: str, optional
-    :param dev_type: {'cpu', 'gpu', or None}, defaults to None
-    :type dev_type: str, optional
-    :param score_key: scoring function, accepts device and returns int, defaults to None
-    :type score_key: callable, optional
-    :return: list of devices
-    :rtype: List[cl.Device]
-    """
-    devices = []
-    for platform in cl.get_platforms():
-        for device in platform.get_devices():
-            if name and name.lower() in device.name.lower():
-                return [device]
-            if dev_type is not None:
-                if isinstance(dev_type, str):
-                    if dev_type.lower() == "cpu":
-                        dev_type = cl.device_type.CPU
-                    elif dev_type.lower() == "gpu":
-                        dev_type = cl.device_type.GPU
-                if device.type != dev_type:
-                    continue
-            devices.append(device)
-    return sorted(devices, key=score_key or _current_device.score_key)
-
-
-def set_device_scoring_key(func: Callable[[cl.Device], int]) -> None:
-    if not callable(func):
-        raise TypeError(
-            "Scoring key must be a callable that takes a device and returns an int"
-        )
-    try:
-        filter_devices(score_key=func)
-    except Exception as e:
-        raise ValueError(f"Scoring algorithm invalid: {e}")
-    _current_device.score_key = func
-
+from ._device import get_device
 
 """ Below here, vendored from GPUtools
 Copyright (c) 2016, Martin Weigert
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
@@ -135,51 +34,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
 
-class OCLProgram(cl.Program):
-    """ a wrapper class representing a CPU/GPU Program
-    example:
-         prog = OCLProgram("mykernels.cl",build_options=["-D FLAG"])
-    """
-    _wait_for_kernel_finish = None
-
-    def __init__(self, file_name=None, src_str=None, build_options=[], dev=None):
-        if file_name is not None:
-            with open(file_name, "r") as f:
-                src_str = f.read()
-
-        if src_str is None:
-            raise ValueError("empty src_str! ")
-
-        if dev is None:
-            dev = get_device()
-
-        self._dev = dev
-        self._kernel_dict = {}
-        super().__init__(self._dev.context, src_str)
-        self.build(options=build_options)
-
-    def run_kernel(self, name, global_size, local_size, *args, **kwargs):
-        if name not in self._kernel_dict:
-            self._kernel_dict[name] = getattr(self, name)
-
-        self._kernel_dict[name](
-            self._dev.queue, global_size, local_size, *args, **kwargs
-        )
-        if OCLProgram._wait_for_kernel_finish:
-            self._dev.queue.finish()
-
-    @classmethod
-    @lru_cache(maxsize=128)
-    def from_source(cls, source):
-        return cls(src_str=source)
+
 
 
 cl_image_datatype_dict = {
     cl.channel_type.FLOAT: np.float32,
     cl.channel_type.UNSIGNED_INT8: np.uint8,
     cl.channel_type.UNSIGNED_INT16: np.uint16,
     cl.channel_type.SIGNED_INT8: np.int8,
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier0/preamble.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier0/preamble.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/__init__.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_absolute.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_absolute.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_add_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_add_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_add_images_weighted.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_add_images_weighted.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_average_distance_of_n_far_off_distances.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_average_distance_of_n_far_off_distances.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_average_distance_of_n_shortest_distances.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_average_distance_of_n_shortest_distances.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_average_distance_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_average_distance_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_and.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_and.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_edge_detection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_edge_detection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_not.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_not.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_or.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_or.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_subtract.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_subtract.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_binary_xor.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_binary_xor.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_convolve.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_convolve.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_copy.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_copy.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_copy_slice.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_copy_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_count_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_count_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_crop.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_crop.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_detect_label_edges.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_detect_label_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_detect_maxima_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_detect_maxima_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_detect_minima_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_detect_minima_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_box_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_box_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_dilate_sphere_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_dilate_sphere_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_divide_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_divide_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_downsample_slice_by_slice_half_median.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_downsample_slice_by_slice_half_median.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_draw_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_draw_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_draw_line.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_draw_line.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_draw_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_draw_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_equal.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_equal_constant.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_box_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_box_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_erode_sphere_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_erode_sphere_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_execute_separable_kernel.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_execute_separable_kernel.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_exponential.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_exponential.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_flip.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_flip.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gaussian_blur.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_angle_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_angle_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_binary_overlap_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_binary_overlap_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_distance_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_distance_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_generate_touch_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_generate_touch_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gradient_x.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gradient_x.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gradient_y.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gradient_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_gradient_z.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_gradient_z.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater_constant.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater_or_equal.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_greater_or_equal_constant.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_greater_or_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_laplace_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_laplace_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_laplace_diamond.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_laplace_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_logarithm.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_logarithm.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mask.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mask.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mask_label.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mask_label.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_distance_of_n_shortest_distances.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_distance_of_n_shortest_distances.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_distance_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_distance_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_image_and_scalar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .._tier0 import execute
 
 from .._tier0 import plugin_function
 from .._tier0 import Image
 
-@plugin_function(categories=['filter'])
+@plugin_function(categories=['filter', 'in assistant'])
 def maximum_image_and_scalar(source : Image, destination : Image = None, scalar : float = 0):
     """Computes the maximum of a constant scalar s and each pixel value x in a 
     given image X. 
     
     <pre>f(x, s) = max(x, s)</pre> 
     
     Parameters
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_x_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_y_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_maximum_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_maximum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_x_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_y_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_mean_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_mean_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_median_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_median_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_median_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_median_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_distance_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_distance_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_x_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_y_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_minimum_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_minimum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_image_and_coordinate.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_image_and_coordinate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_multiply_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_multiply_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_n_closest_points.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_n_closest_points.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_maximum_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_maximum_diamond.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_maximum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_minimum_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_minimum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_nonzero_minimum_diamond.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_nonzero_minimum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_not_equal.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_not_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_not_equal_constant.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_not_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_diamond.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_onlyzero_overwrite_maximum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_paste.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_paste.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_point_index_list_to_mesh.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_point_index_list_to_mesh.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_point_index_list_to_touch_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_point_index_list_to_touch_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_power.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_power.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_power_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_power_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_read_intensities_from_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_read_intensities_from_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_read_intensities_from_positions.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_read_intensities_from_positions.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_replace_intensities.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_replace_intensities.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_replace_intensity.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_replace_intensity.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_resample.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_resample.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_column.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_column.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_image_borders.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_image_borders.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_non_zero_pixels_to_pixel_index.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_non_zero_pixels_to_pixel_index.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_plane.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_plane.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_ramp_x.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_ramp_x.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_ramp_y.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_ramp_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_ramp_z.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_ramp_z.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_row.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_row.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_where_x_equals_y.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_where_x_equals_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_where_x_greater_than_y.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_where_x_greater_than_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_set_where_x_smaller_than_y.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_set_where_x_smaller_than_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller_constant.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller_or_equal.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller_or_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_smaller_or_equal_constant.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_smaller_or_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sobel.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sobel.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_standard_deviation_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_standard_deviation_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_subtract_image_from_scalar.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_subtract_image_from_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sum_x_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sum_y_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_sum_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_sum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_touch_matrix_to_mesh.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_touch_matrix_to_mesh.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_transpose_xy.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_transpose_xy.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_transpose_xz.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_transpose_xz.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_transpose_yz.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_transpose_yz.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_undefined_to_zero.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_undefined_to_zero.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_variance_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_variance_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_variance_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_variance_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/_write_values_to_positions.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/_write_values_to_positions.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/maximum_distance_of_n_shortest_distances_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/maximum_distance_of_n_shortest_distances_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/maximum_distance_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/maximum_distance_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/minimum_distance_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/minimum_distance_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/point_index_list_to_touch_matrix_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/point_index_list_to_touch_matrix_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/read_intensities_from_map_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/read_intensities_from_map_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/read_intensities_from_positions_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/read_intensities_from_positions_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier1/variance_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier1/variance_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/__init__.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_add_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_add_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_block_enumerate.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_block_enumerate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_bottom_hat_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_bottom_hat_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_bottom_hat_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_bottom_hat_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_combine_horizontally.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_combine_horizontally.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_combine_vertically.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_combine_vertically.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_concatenate_stacks.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_concatenate_stacks.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_distance_matrix_to_mesh.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_distance_matrix_to_mesh.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_flag_existing_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_flag_existing_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_gamma_correction.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_gamma_correction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_invert.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_invert.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_label_spots.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_label_spots.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_maximum_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_maximum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_maximum_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_maximum_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_mean_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_mean_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_median_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_median_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_minimum_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_minimum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_minimum_of_masked_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_minimum_of_masked_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_minimum_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_minimum_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_mode_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_mode_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_neighbors_of_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_neighbors_of_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_pointlist_to_labelled_spots.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_pointlist_to_labelled_spots.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_reduce_stack.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_reduce_stack.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_standard_deviation_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_standard_deviation_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_sub_stack.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_sub_stack.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_subtract_images.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_subtract_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_sum_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_sum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_sum_reduction_x.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_sum_reduction_x.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_top_hat_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_top_hat_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_top_hat_sphere.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_top_hat_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_touch_matrix_to_adjacency_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_touch_matrix_to_adjacency_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_z_position_of_maximum_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_z_position_of_maximum_z_projection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pyclesperanto_prototype._tier0 import plugin_function, Image, create_2d_xy, execute
 
-@plugin_function(output_creator = create_2d_xy, categories=['projection'])
+@plugin_function(output_creator = create_2d_xy, categories=['projection', 'in assistant'])
 def z_position_of_maximum_z_projection(source : Image, destination : Image = None):
     """Determines a Z-position of the maximum intensity along Z and writes it into the resulting image.
 
     If there are multiple z-slices with the same value, the smallest Z will be chosen.
 
     Parameters
     ----------
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_z_position_of_minimum_z_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_z_position_of_minimum_z_projection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pyclesperanto_prototype._tier0 import plugin_function, Image, create_2d_xy, execute
 
 
-@plugin_function(output_creator=create_2d_xy, categories=['projection'])
+@plugin_function(output_creator=create_2d_xy, categories=['projection', 'in assistant'])
 def z_position_of_minimum_z_projection(source: Image, destination: Image = None):
     """Determines a Z-position of the minimum intensity along Z and writes it into the resulting image.
 
     If there are multiple z-slices with the same value, the smallest Z will be chosen.
 
     Parameters
     ----------
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/_z_position_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/_z_position_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/z_position_of_maximum_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/z_position_of_maximum_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/z_position_of_minimum_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/z_position_of_minimum_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier2/z_position_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier2/z_position_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/__init__.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ._absolute_difference import absolute_difference
 from ._bounding_box import bounding_box
 from ._center_of_mass import center_of_mass
-from ._close_index_gaps_in_label_map import close_index_gaps_in_label_map
+from ._relabel_sequential import relabel_sequential
+from ._relabel_sequential import relabel_sequential as close_index_gaps_in_label_map
 from ._difference_of_gaussian import difference_of_gaussian
 from ._divide_by_gaussian_background import divide_by_gaussian_background
 from ._exclude_labels import exclude_labels
 from ._exclude_labels_on_edges import exclude_labels_on_edges
 from ._exclude_labels_outside_size_range import exclude_labels_outside_size_range
 from ._exclude_labels_outside_size_range import exclude_labels_outside_size_range as exclude_labels_out_of_size_range
 from ._exclude_labels_with_values_out_of_range import exclude_labels_with_values_out_of_range
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_absolute_difference.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_absolute_difference.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_bounding_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_center_of_mass.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_close_index_gaps_in_label_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_relabel_sequential.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,35 +6,38 @@
 from .._tier1 import set_column
 from .._tier2 import flag_existing_intensities
 from .._tier2 import maximum_of_all_pixels
 from .._tier2 import sum_reduction_x
 from .._tier2 import block_enumerate
 
 @plugin_function(output_creator=create_labels_like)
-def close_index_gaps_in_label_map(input : Image, output : Image = None, blocksize = 4096):
+def relabel_sequential(input : Image, output : Image = None, blocksize : int = 4096):
     """Analyses a label map and if there are gaps in the indexing (e.g. label 
     5 is not present) all 
     subsequent labels will be relabelled. 
     
     Thus, afterwards number of labels and maximum label index are equal.
     This operation is mostly performed on the CPU. 
     
     Parameters
     ----------
     labeling_input : Image
     labeling_destination : Image
+    blocksize : int, optional
+        Renumbering is done in blocks for performance reasons.
+        Change the blocksize to adapt to your data and hardware
     
     Returns
     -------
     labeling_destination
     
     Examples
     --------
     >>> import pyclesperanto_prototype as cle
-    >>> cle.close_index_gaps_in_label_map(labeling_input, labeling_destination)
+    >>> cle.relabel_sequential(labeling_input, labeling_destination)
     
     References
     ----------
     .. [1] https://clij.github.io/clij2-docs/reference_closeIndexGapsInLabelMap
     """
     max_label = maximum_of_all_pixels(input)
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_difference_of_gaussian.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_difference_of_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_divide_by_gaussian_background.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_divide_by_gaussian_background.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_on_edges.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_on_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_outside_size_range.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_outside_size_range.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_out_of_range.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_out_of_range.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_within_range.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_exclude_labels_with_values_within_range.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_generate_n_nearest_neighbors_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_generate_n_nearest_neighbors_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_generate_proximal_neighbors_matrix.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_generate_proximal_neighbors_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_histogram.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_histogram.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_jaccard_index.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_jaccard_index.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_labelled_spots_to_pointlist.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_labelled_spots_to_pointlist.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_maximum_of_n_nearest_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_maximum_of_n_nearest_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_maximum_of_proximal_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_maximum_of_proximal_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_maximum_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_maximum_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_n_nearest_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_n_nearest_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_proximal_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_proximal_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mean_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mean_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_minimum_of_n_nearest_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_minimum_of_n_nearest_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_minimum_of_proximal_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_minimum_of_proximal_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_minimum_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_minimum_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mode_of_n_nearest_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mode_of_n_nearest_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mode_of_proximal_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mode_of_proximal_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_mode_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_mode_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_squared_difference.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_squared_difference.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_standard_deviation_of_n_nearest_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_standard_deviation_of_n_nearest_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_standard_deviation_of_proximal_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_standard_deviation_of_proximal_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_standard_deviation_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_standard_deviation_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_subtract_gaussian_background.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_subtract_gaussian_background.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier3/_z_position_range_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier3/_z_position_range_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/__init__.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from ._connected_components_labeling_box import connected_components_labeling_box
+from ._erode_labels import erode_labels
+from ._exclude_large_labels import exclude_large_labels
+from ._exclude_small_labels import exclude_small_labels
 from ._extend_labeling_via_voronoi import extend_labeling_via_voronoi
-from ._extend_labels_with_maximum_radius import extend_labels_with_maximum_radius
-from ._extend_labels_with_maximum_radius import extend_labels_with_maximum_radius as dilate_labels
+from ._dilate_labels import dilate_labels
+from ._dilate_labels import dilate_labels as extend_labels_with_maximum_radius
 from ._extended_depth_of_focus_variance_projection import extended_depth_of_focus_variance_projection
 from ._mean_squared_error import mean_squared_error
 from ._local_maximum_touching_neighbor_count_map import local_maximum_touching_neighbor_count_map
 from ._local_mean_touching_neighbor_count_map import local_mean_touching_neighbor_count_map
 from ._local_median_touching_neighbor_count_map import local_median_touching_neighbor_count_map
 from ._local_minimum_touching_neighbor_count_map import local_minimum_touching_neighbor_count_map
 from ._local_standard_deviation_touching_neighbor_count_map import local_standard_deviation_touching_neighbor_count_map
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_connected_components_labeling_box.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_connected_components_labeling_box.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .._tier0 import pull
 from .._tier0 import push
 from .._tier0 import create_like, create_labels_like
 from .._tier1 import set
 from .._tier1 import set_non_zero_pixels_to_pixel_index
 from .._tier1 import nonzero_minimum_box
 from .._tier1 import nonzero_minimum_diamond
-from .._tier3 import close_index_gaps_in_label_map
+from .._tier3 import relabel_sequential
 
 import numpy as np
 
 from .._tier0 import plugin_function
 from .._tier0 import Image
 
 @plugin_function(categories=['label', 'in assistant'], priority=1, output_creator=create_labels_like)
@@ -55,12 +55,12 @@
         else:
             flagged_nonzero_minimum_filter(temp2, flag, temp1)
         flag_value = pull(flag)[0][0][0]
         set(flag, 0)
         iteration_count += 1
 
     if (iteration_count % 2 == 0):
-        close_index_gaps_in_label_map(temp1, labeling_destination)
+        relabel_sequential(temp1, labeling_destination)
     else:
-        close_index_gaps_in_label_map(temp2, labeling_destination)
+        relabel_sequential(temp2, labeling_destination)
 
     return labeling_destination
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_extend_labeling_via_voronoi.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_extend_labeling_via_voronoi.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_extended_depth_of_focus_variance_projection.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_extended_depth_of_focus_variance_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_maximum_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_maximum_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_mean_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_mean_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_median_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_median_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_minimum_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_minimum_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_local_standard_deviation_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_local_standard_deviation_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_mean_squared_error.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_merge_touching_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_merge_touching_labels.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,26 +11,29 @@
     labels_input : Image
     labels_destination : Image
 
     Returns
     -------
     labels_destination : Image
 
+    See Also
+    --------
+    ..[1] https://clij.github.io/clij2-docs/reference_mergeTouchingLabels
     """
     from .._tier1 import generate_touch_matrix
     from .._tier1 import set_ramp_y
     from .._tier1 import transpose_xy
     from .._tier0 import create
     from .._tier1 import binary_or
     from .._tier1 import set_where_x_equals_y
     from .._tier1 import set_column
     from .._tier1 import set_row
     from .._tier1 import multiply_images
     from .._tier1 import maximum_y_projection
-    from .._tier3 import close_index_gaps_in_label_map
+    from .._tier3 import relabel_sequential
     from .._tier1 import replace_intensities
 
     # touch matrices are half-filled. The upper right corner is empth
     touch_matrix = generate_touch_matrix(labels_input)
 
     # make a full matrix (in CLIJ2 we call them adjacency matrix
     touch_matrix_t = transpose_xy(touch_matrix)
@@ -48,15 +51,15 @@
 
     # the new list of label-IDs for each label is the maximum-y-projection of the matrix
     # if labels 2 and 3 should be merged, both have then label-ID 3
     label_id_vector = create([1, touch_matrix.shape[0]])
     maximum_y_projection(touch_matrix, label_id_vector)
 
     # renumber the labels
-    new_labels = close_index_gaps_in_label_map(label_id_vector)
+    new_labels = relabel_sequential(label_id_vector)
 
     # write the new labels into the label image
     labels_destination = replace_intensities(labels_input, new_labels, labels_destination)
 
     # todo: the following might be suboptimal with regard to performance.
     #       Check if there is a faster way of doing this, e.g. in the lines above.
     # check if labels are still touching
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_proximal_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_proximal_neighbor_count_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,13 @@
     from .._tier9 import centroids_of_labels
     from .._tier1 import generate_distance_matrix
 
     pointlist = centroids_of_labels(source)
     distance_matrix = generate_distance_matrix(pointlist, pointlist)
 
     touch_matrix = generate_proximal_neighbors_matrix(distance_matrix, min_distance=min_distance, max_distance=max_distance)
-    print(touch_matrix)
     number_of_touching_neighbors_vector = count_touching_neighbors(touch_matrix)
 
     # ignore how many objects touch the background
     set_column(number_of_touching_neighbors_vector, 0, 0)
     replace_intensities(source, number_of_touching_neighbors_vector, destination)
     return destination
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_sorensen_dice_coefficient.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_spots_to_pointlist.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_spots_to_pointlist.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier4/_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier4/_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/_connected_components_labeling_diamond.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/_connected_components_labeling_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/_masked_voronoi_labeling.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/_masked_voronoi_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier5/_voronoi_labeling.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier5/_voronoi_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_AffineTransform3D.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_AffineTransform3D.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_affine_transform.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_affine_transform.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_apply_vector_field.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_apply_vector_field.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_rigid_transform.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_rigid_transform.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_rotate.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_rotate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_scale.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_scale.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier8/_translate.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier8/_translate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/__init__.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_artificial_tissue_2d.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_artificial_tissue_2d.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_average_distance_of_n_closest_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_average_distance_of_n_closest_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_average_neighbor_distance_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_average_neighbor_distance_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_centroids_of_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_centroids_of_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_angle_mesh_between_touching_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_angle_mesh_between_touching_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_distance_mesh_between_touching_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_distance_mesh_between_touching_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_mesh_between_n_closest_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_mesh_between_n_closest_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_mesh_between_proximal_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_mesh_between_proximal_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_draw_mesh_between_touching_labels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_draw_mesh_between_touching_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_euclidean_distance_from_label_centroid_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_euclidean_distance_from_label_centroid_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_imshow.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_imshow.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_maximum_extension_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_maximum_extension_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_maximum_extension_ratio_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_maximum_extension_ratio_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_maximum_intensity_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_maximum_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_mean_extension_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_mean_extension_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_mean_intensity_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_mean_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_minimum_intensity_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_minimum_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_pixel_count_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_pixel_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_label_standard_deviation_intensity_map.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_label_standard_deviation_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_push_regionprops.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_push_regionprops.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_push_regionprops_column.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_push_regionprops_column.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_regionprops.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_regionprops.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_entry.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_entry.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_of_background_and_labelled_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_of_background_and_labelled_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_of_image.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_of_image.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_statistics_of_labelled_pixels.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_statistics_of_labelled_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_threshold_otsu.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_threshold_otsu.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/_voronoi_otsu_labeling.py` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/_voronoi_otsu_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/standard_deviation_per_label_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/standard_deviation_per_label_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/statistics_per_label_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/statistics_per_label_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/_tier9/sum_per_label_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/_tier9/sum_per_label_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/absolute_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_image_and_scalar_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_image_and_scalar_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/add_images_weighted_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_interpolate_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_interpolate_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_interpolate_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_interpolate_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/affine_transform_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_interpolate_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_interpolate_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_interpolate_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_interpolate_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/apply_vectorfield_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/arg_maximum_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/arg_maximum_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_far_off_distances_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_far_off_distances_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_shortest_distances_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_n_shortest_distances_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/average_distance_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_and_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_edge_detection_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_not_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_or_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_subtract_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/binary_xor_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/block_enumerate_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/block_enumerate_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/convolve_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_non_zero_projection_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_non_zero_projection_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_slice_by_slice_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_slice_by_slice_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_pixels_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_voxels_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_nonzero_voxels_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/count_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/crop_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_interpolation_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_interpolation_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/depth_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_label_edges_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_slice_by_slice_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_slice_by_slice_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_maxima_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_slice_by_slice_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_slice_by_slice_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/detect_minima_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_slice_by_slice_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_box_slice_by_slice_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_slice_by_slice_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/dilate_sphere_slice_by_slice_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distance_matrix_to_mesh_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distance_matrix_to_mesh_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/distancemap_localPositiveMinimum_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/divide_images_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/divide_images_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_xy_by_half_median_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/downsample_xy_by_half_median_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/draw_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/drawline_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/entropy_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/equal_constant_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_slice_by_slice_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_box_slice_by_slice_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_slice_by_slice_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/erode_sphere_slice_by_slice_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/euclidean_distance_from_label_centroid_map_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/euclidean_distance_from_label_centroid_map_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/excludeLabelsOnEdges_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/excludeLabelsOnEdges_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_edges_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_edges_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_on_surface_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exclude_labels_sub_surface_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/exponential_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/exponential_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flip_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/flood_fill_diamond_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/flood_fill_diamond_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gaussian_blur_separable_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_angle_matrix_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_angle_matrix_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_binary_overlap_matrix_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_distance_matrix_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_distance_matrix_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/generate_touch_matrix_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_x_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_y_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_z_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/gradient_z_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_constant_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/greater_or_equal_constant_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/histogram_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/label_spots_in_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/label_spots_in_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/labelled_spots_to_point_list_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/labelled_spots_to_point_list_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/laplace_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/logarithm_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/logarithm_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_label_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_stack_with_plane_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mask_stack_with_plane_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/matrix_multiply_float_buffer.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/matrix_multiply_float_buffer.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_distance_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_distance_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_image_and_scalar_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_images_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_octagon_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_masked_pixels_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_masked_pixels_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_projection_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_projection_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_separable_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_slice_by_slice_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_slice_by_slice_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_x_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_x_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_y_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_y_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_bounded_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_bounded_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/maximum_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_separable_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_slice_by_slice_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_slice_by_slice_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_x_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_x_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_y_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_y_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_bounded_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_bounded_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mean_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_slice_by_slice_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/median_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_distance_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_distance_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_image_and_scalar_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_images_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_octagon_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_masked_pixels_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_masked_pixels_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_projection_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_projection_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_separable_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_slice_by_slice_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_slice_by_slice_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_sphere_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_x_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_x_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_y_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_y_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_bounded_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_bounded_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_thresholded_bounded_3d_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_thresholded_bounded_3d_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/minimum_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/mode_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/mode_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_coordinate_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_scalar_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_image_and_scalar_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_images_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_matrix_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_matrix_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_plane_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_plane_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_scalars_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/multiply_stack_with_scalars_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_distances_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_distances_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_points_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/n_shortest_points_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_maximum_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/nonzero_minimum_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/not_equal_constant_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_box_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/onlyzero_overwrite_maximum_diamond_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/paste_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/piv.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/piv.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/pointindexlist_to_mesh_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/pointindexlist_to_mesh_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/power_images_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensities_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensities_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensity_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_intensity_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_pixels_if_zero_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/replace_pixels_if_zero_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_bottom_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_bottom_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_left_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_left_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_radial_interpolate_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_right_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_right_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_top_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/reslice_top_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_clockwise_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/rotate_counter_clockwise_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_nonzero_pixels_to_pixelindex_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/set_nonzero_pixels_to_pixelindex_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_constant_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/smaller_or_equal_constant_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sobel_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_of_touching_neighbors_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_of_touching_neighbors_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_z_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/standard_deviation_z_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/subtract_image_from_scalar_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/subtract_image_from_scalar_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_reduction_x_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/sum_reduction_x_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/touch_matrix_to_mesh_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/touch_matrix_to_mesh_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xy_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xy_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xz_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_xz_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_yz_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/transpose_yz_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/undefined_to_zero_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/undefined_to_zero_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_masked_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_masked_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_projection_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/variance_projection_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_binarize_labelmap_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_2d.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_2d.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_3d.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_detect_maxima_region_box_3d.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_eliminate_wrong_maxima_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/watershed_local_maximum_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_2d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_2d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_3d_x.cl` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype/clij-opencl-kernels/kernels/write_values_to_positions_3d_x.cl`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/PKG-INFO` & `pyclesperanto_prototype-0.9.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: pyclesperanto-prototype
-Version: 0.9.7
-Summary: OpenCL-based GPU-accelerated image processing
+Name: pyclesperanto_prototype
+Version: 0.9.9
+Summary: GPU-accelerated image processing in python using OpenCL
 Home-page: https://github.com/clEsperanto/pyclesperanto_prototype
 Author: haesleinhuepf
 Author-email: robert.haase@tu-dresden.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -118,159 +118,182 @@
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_count_blobs.png" width="300"/>
 
 </td><td>
 
-[Counting blobs](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/count_blobs.ipynb)
+[Counting blobs](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/count_blobs.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/voronoi_otsu_labeling.png" width="300"/>
 
 </td><td>
 
-[Voronoi-Otsu labeling](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/voronoi_otsu_labeling.ipynb)
+[Voronoi-Otsu labeling](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/voronoi_otsu_labeling.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/segmentation_3d.png" width="300"/>
 
 </td><td>
 
-[3D Image segmentation ](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/Segmentation_3D.ipynb)
+[3D Image segmentation ](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/Segmentation_3D.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/segmentation_2d_membranes.png" width="300"/>
 
 </td><td>
 
-[Cell segmentation based on membranes](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/segmentation_2d_membranes.ipynb)
+[Cell segmentation based on membranes](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/segmentation_2d_membranes.ipynb)
 
-</td></tr><tr><td>
+</td></tr>
+
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/bead_segmentation.png" width="300"/>
+
+</td><td>
+
+[Detecting beads and measuring their size](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/segmentation/bead_segmentation.ipynb)
+
+</td></tr>
+
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/parametric_maps.png" width="300"/>
+
+</td><td>
+
+[Parametric maps](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/tissues/parametric_maps.ipynb)
+
+</td></tr>
+
+
+<tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_crop_and_paste_images.png" width="300"/>
 
 </td><td>
 
-[Crop and paste images](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/crop_and_paste_images.ipynb)
+[Crop and paste images](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/crop_and_paste_images.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_inspecting_3d_images.png" width="300"/>
 
 </td><td>
 
-[Inspecting 3D image data](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/inspecting_3d_images.ipynb)
+[Inspecting 3D image data](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/inspecting_3d_images.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_affine_transforms.png" width="300"/>
 
 </td><td>
 
-[Rotation, scaling, translation, affine transforms](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/transforms/affine_transforms.ipynb)
+[Rotation, scaling, translation, affine transforms](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/transforms/affine_transforms.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_multiply_vectors_and_matrices.png" width="300"/>
 
 </td><td>
 
-[Multiply vectors and matrices](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_vectors_and_matrices.ipynb)
+[Multiply vectors and matrices](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_vectors_and_matrices.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_multiply_matrices.png" width="300"/>
 
 </td><td>
 
-[Matrix multiplication](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_matrices.ipynb)
+[Matrix multiplication](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/multiply_matrices.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_spots_pointlists_matrices_tables.png" width="300"/>
 
 </td><td>
 
-[Working with spots, pointlist and matrices](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/spots_pointlists_matrices_tables.ipynb)
+[Working with spots, pointlist and matrices](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/spots_pointlists_matrices_tables.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_between_centroids.png" width="300"/>
 
 </td><td>
 
-[Mesh between centroids](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_centroids.ipynb)
+[Mesh between centroids](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_centroids.ipynb)
 
 </td></tr><tr><td>
 
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_between_touching_neighbors.png" width="300"/>
 
 </td><td>
 
-[Mesh between touching neighbors](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_touching_neighbors.ipynb)
+[Mesh between touching neighbors](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_between_touching_neighbors.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_with_distances.png" width="300"/>
 
 </td><td>
 
-[Mesh with distances](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_with_distances.ipynb)
+[Mesh with distances](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_with_distances.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/mesh_nearest_neighbors.png" width="300"/>
 
 </td><td>
 
-[Mesh nearest_neighbors](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_nearest_neighbors.ipynb)
+[Mesh nearest_neighbors](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/mesh_nearest_neighbors.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/neighborhood_definitions.png" width="300"/>
 
 </td><td>
 
-[Neighborhood definitions](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighborhood_definitions.ipynb)
+[Neighborhood definitions](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighborhood_definitions.ipynb)
 
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/tissue_neighborhood_quantification.png" width="300"/>
 
 </td><td>
 
-[Tissue neighborhood quantification](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/tissues/tissue_neighborhood_quantification.ipynb)
+[Tissue neighborhood quantification](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/tissues/tissue_neighborhood_quantification.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/neighbors_of_neighbors.png" width="300"/>
 
 </td><td>
 
-[Neighbors of neighbors](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighbors_of_neighbors.ipynb)
+[Neighbors of neighbors](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/neighbors_of_neighbors.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_voronoi_diagrams.png" width="300"/>
 
 </td><td>
 
-[Voronoi diagrams](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/voronoi_diagrams.ipynb)
+[Voronoi diagrams](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/voronoi_diagrams.ipynb)
 
 </td></tr><tr><td>
 
 </td><td>
 
-[Shape descriptors based on neighborhood graphs](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/shape_descriptors_based_on_neighborhood_graphs.ipynb)
+[Shape descriptors based on neighborhood graphs](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/neighbors/shape_descriptors_based_on_neighborhood_graphs.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_tribolium_napari.png" width="300"/>
 
 </td><td>
 
@@ -278,50 +301,123 @@
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_tribolium_morphometry.png" width="300"/>
 
 </td><td>
 
-[Tribolium morphometry](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/tribolium_morphometry/tribolium_morphometry.ipynb)
+[Tribolium morphometry](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/tribolium_morphometry/tribolium_morphometry.ipynb)
 
 </td></tr><tr><td>
 
 <img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/screenshot_napari_dask.png" width="300"/>
 
 </td><td>
 
-[napari+dask timelapse processing](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/napari_gui/napari_dask.ipynb)
+[napari+dask timelapse processing](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/napari_gui/napari_dask.ipynb)
 
-</td></tr><tr><td>
+</td></tr>
+</table>
+
+## Technical insights
+
+<table border="0"><tr><td>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/browse_operations.png" width="300"/>
+
+</td><td>
+
+[Browsing operations](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/browse_operations.ipynb)
+
+</td></tr>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/interactive_widgets.gif" width="300"/>
+
+</td><td>
+
+[Interactive widgets](https://colab.research.google.com/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/browse_operations.ipynb)
+
+</td></tr>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/optimize_blobs_segmentation.png" width="300"/>
+
+</td><td>
+
+[Automatic workflow optimization](https://colab.research.google.com/github/clEsperanto/pyclesperanto_prototype/tree/master/demo/optimization/optimize_blobs_segmentation.ipynb)
+
+</td></tr>
+
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/switching_gpus.png" width="300"/>
+
+</td><td>
+
+[Exploring and switching between GPUs](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/switching_gpus.ipynb)
+
+</td></tr>
+<tr><td>
+
+<img src="https://github.com/clEsperanto/pyclesperanto_prototype/raw/master/docs/images/cupy_compatibility.png" width="300"/>
+
+</td><td>
+
+[Interoperability with cupy](http://github.com/clEsperanto/pyclesperanto_prototype/tree/master/demo/basics/interoperability_cupy.ipynb)
+
+</td></tr>
+</table>
+
+## Related projects
+
+<table border="0"><tr><td>
 
 <img src="https://github.com/clesperanto/napari_pyclesperanto_assistant/raw/master/docs/images/screenshot.png" width="300"/>
 
 </td><td>
 
-[pyclesperanto assistant](https://github.com/clesperanto/napari_pyclesperanto_assistant)
+[napari-pyclesperanto-assistant](https://github.com/clesperanto/napari_pyclesperanto_assistant):
+A graphical user interface for general purpose GPU-accelerated image processing and analysis in napari.
+
+</td></tr><tr><td>
+
+<img src="https://github.com/haesleinhuepf/napari-oclrfc/raw/master/images/screenshot.png" width="300"/>
+
+</td><td>
+
+[napari-oclrfc](https://github.com/haesleinhuepf/napari-oclrfc):
+GPU-accelerated Random Forest Classifiers for pixel and labeled object classification
 
 </td></tr></table>
 
 ## Benchmarking
 We implemented some basic benchmarking notebooks allowing to see performance differences between pyclesperanto and 
 some other image processing libraries, typically using the CPU. Such benchmarking results vary heavily depending on 
 image size, kernel size, used operations, parameters and used hardware. Feel free to use those notebooks, adapt them to 
 your use-case scenario and benchmark on your target hardware. If you have different scenarios or use-cases, you are very 
 welcome to submit your notebook as pull-request!
 
-* [Affine transforms](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/affine_transforms.ipynb)
-* [Gaussian blur](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/gaussian_blur.ipynb)
-* [Convolution](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/convolution.ipynb)
-* [Otsu's thresholding](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/threshold_otsu.ipynb)
-* [Connected component labeling](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/connected_component_labeling.ipynb)  
-* [Extend labels](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/extend_labels.ipynb)
-* [Statistics of labeled pixels / regionprops](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/statistics_of_labeled_pixels.ipynb)
-* [Matrix multiplication](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/matrix_multiplication.ipynb)
-* [Pixel-wise comparison](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/pixelwise_comparison.ipynb)
-* [Intensity projections](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/intensity_projections.ipynb)
-* [Axis transposition](http://nbviewer.jupyter.org/github/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/transpose.ipynb)
+* [Affine transforms](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/affine_transforms.ipynb)
+* [Gaussian blur](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/gaussian_blur.ipynb)
+* [Convolution](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/convolution.ipynb)
+* [Otsu's thresholding](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/threshold_otsu.ipynb)
+* [Connected component labeling](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/connected_component_labeling.ipynb)  
+* [Extend labels](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/extend_labels.ipynb)
+* [Statistics of labeled pixels / regionprops](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/statistics_of_labeled_pixels.ipynb)
+* [Matrix multiplication](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/matrix_multiplication.ipynb)
+* [Pixel-wise comparison](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/pixelwise_comparison.ipynb)
+* [Intensity projections](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/intensity_projections.ipynb)
+* [Axis transposition](http://github.com/clEsperanto/pyclesperanto_prototype/blob/master/benchmarks/transpose.ipynb)
+
+## See also
+There are other libraries for code acceleration and GPU-acceleration for image processing.
+* [numba](https://numba.pydata.org/)
+* [cupy](https://cupy.dev)
+* [cucim](https://github.com/rapidsai/cucim)
+* [clij](https://clij.github.io)
 
 ## Feedback welcome!
 clEsperanto is developed in the open because we believe in the open source community. See our [community guidelines](https://clij.github.io/clij2-docs/community_guidelines). Feel free to drop feedback as [github issue](https://github.com/clEsperanto/pyclesperanto_prototype/issues) or via [image.sc](https://image.sc)
```

### Comparing `pyclesperanto_prototype-0.9.7/pyclesperanto_prototype.egg-info/SOURCES.txt` & `pyclesperanto_prototype-0.9.9/pyclesperanto_prototype.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 pyclesperanto_prototype.egg-info/top_level.txt
 pyclesperanto_prototype/_tier0/__init__.py
 pyclesperanto_prototype/_tier0/_available_device_names.py
 pyclesperanto_prototype/_tier0/_categories.py
 pyclesperanto_prototype/_tier0/_cl_image.py
 pyclesperanto_prototype/_tier0/_cl_info.py
 pyclesperanto_prototype/_tier0/_create.py
+pyclesperanto_prototype/_tier0/_device.py
 pyclesperanto_prototype/_tier0/_execute.py
 pyclesperanto_prototype/_tier0/_operations.py
 pyclesperanto_prototype/_tier0/_plugin_function.py
+pyclesperanto_prototype/_tier0/_program.py
 pyclesperanto_prototype/_tier0/_pull.py
 pyclesperanto_prototype/_tier0/_push.py
 pyclesperanto_prototype/_tier0/_pycl.py
 pyclesperanto_prototype/_tier0/_radius_to_kernel_size.py
 pyclesperanto_prototype/_tier0/_set_wait_for_kernel_finish.py
 pyclesperanto_prototype/_tier0/_sigma_to_kernel_size.py
 pyclesperanto_prototype/_tier0/_types.py
@@ -208,15 +210,14 @@
 pyclesperanto_prototype/_tier2/z_position_of_maximum_z_projection_x.cl
 pyclesperanto_prototype/_tier2/z_position_of_minimum_z_projection_x.cl
 pyclesperanto_prototype/_tier2/z_position_projection_x.cl
 pyclesperanto_prototype/_tier3/__init__.py
 pyclesperanto_prototype/_tier3/_absolute_difference.py
 pyclesperanto_prototype/_tier3/_bounding_box.py
 pyclesperanto_prototype/_tier3/_center_of_mass.py
-pyclesperanto_prototype/_tier3/_close_index_gaps_in_label_map.py
 pyclesperanto_prototype/_tier3/_difference_of_gaussian.py
 pyclesperanto_prototype/_tier3/_divide_by_gaussian_background.py
 pyclesperanto_prototype/_tier3/_exclude_labels.py
 pyclesperanto_prototype/_tier3/_exclude_labels_on_edges.py
 pyclesperanto_prototype/_tier3/_exclude_labels_outside_size_range.py
 pyclesperanto_prototype/_tier3/_exclude_labels_with_values_out_of_range.py
 pyclesperanto_prototype/_tier3/_exclude_labels_with_values_within_range.py
@@ -234,24 +235,28 @@
 pyclesperanto_prototype/_tier3/_mean_of_touching_neighbors_map.py
 pyclesperanto_prototype/_tier3/_minimum_of_n_nearest_neighbors_map.py
 pyclesperanto_prototype/_tier3/_minimum_of_proximal_neighbors_map.py
 pyclesperanto_prototype/_tier3/_minimum_of_touching_neighbors_map.py
 pyclesperanto_prototype/_tier3/_mode_of_n_nearest_neighbors_map.py
 pyclesperanto_prototype/_tier3/_mode_of_proximal_neighbors_map.py
 pyclesperanto_prototype/_tier3/_mode_of_touching_neighbors_map.py
+pyclesperanto_prototype/_tier3/_relabel_sequential.py
 pyclesperanto_prototype/_tier3/_squared_difference.py
 pyclesperanto_prototype/_tier3/_standard_deviation_of_n_nearest_neighbors_map.py
 pyclesperanto_prototype/_tier3/_standard_deviation_of_proximal_neighbors_map.py
 pyclesperanto_prototype/_tier3/_standard_deviation_of_touching_neighbors_map.py
 pyclesperanto_prototype/_tier3/_subtract_gaussian_background.py
 pyclesperanto_prototype/_tier3/_z_position_range_projection.py
 pyclesperanto_prototype/_tier4/__init__.py
 pyclesperanto_prototype/_tier4/_connected_components_labeling_box.py
+pyclesperanto_prototype/_tier4/_dilate_labels.py
+pyclesperanto_prototype/_tier4/_erode_labels.py
+pyclesperanto_prototype/_tier4/_exclude_large_labels.py
+pyclesperanto_prototype/_tier4/_exclude_small_labels.py
 pyclesperanto_prototype/_tier4/_extend_labeling_via_voronoi.py
-pyclesperanto_prototype/_tier4/_extend_labels_with_maximum_radius.py
 pyclesperanto_prototype/_tier4/_extended_depth_of_focus_variance_projection.py
 pyclesperanto_prototype/_tier4/_local_maximum_touching_neighbor_count_map.py
 pyclesperanto_prototype/_tier4/_local_mean_touching_neighbor_count_map.py
 pyclesperanto_prototype/_tier4/_local_median_touching_neighbor_count_map.py
 pyclesperanto_prototype/_tier4/_local_minimum_touching_neighbor_count_map.py
 pyclesperanto_prototype/_tier4/_local_standard_deviation_touching_neighbor_count_map.py
 pyclesperanto_prototype/_tier4/_mean_squared_error.py
@@ -632,15 +637,14 @@
 tests/test_binary_xor.py
 tests/test_block_enumerate.py
 tests/test_bottom_hat_box.py
 tests/test_bottom_hat_sphere.py
 tests/test_bounding_box.py
 tests/test_center_of_mass.py
 tests/test_centroids_of_labels.py
-tests/test_close_index_gaps_in_label_maps.py
 tests/test_combine_horizontally.py
 tests/test_combine_vertically.py
 tests/test_concatenate_stacks.py
 tests/test_connected_components_labeling_box.py
 tests/test_connected_components_labeling_diamond.py
 tests/test_convolve.py
 tests/test_copy.py
@@ -651,48 +655,50 @@
 tests/test_degrees_to_radians.py
 tests/test_detect_label_edges.py
 tests/test_detect_maxima_box.py
 tests/test_detect_minima_box.py
 tests/test_difference_of_gaussian.py
 tests/test_dilate_box.py
 tests/test_dilate_box_slice_by_slice.py
+tests/test_dilate_labels.py
 tests/test_dilate_sphere.py
 tests/test_dilate_sphere_slice_by_slice.py
 tests/test_divide_images.py
 tests/test_downsample_xy_half_median.py
 tests/test_draw_box.py
 tests/test_draw_line.py
 tests/test_draw_sphere.py
 tests/test_equal.py
 tests/test_equal_constant.py
 tests/test_erode_box.py
 tests/test_erode_box_slice_by_slice.py
+tests/test_erode_labels.py
 tests/test_erode_sphere.py
 tests/test_erode_sphere_slice_by_slice.py
 tests/test_euclidean_distance_from_label_centroid_map.py
 tests/test_exclude_labels.py
 tests/test_exclude_labels_on_edges.py
 tests/test_exclude_labels_out_of_size_range.py
 tests/test_exclude_labels_with_values_out_of_range.py
 tests/test_exclude_labels_with_values_within_range.py
 tests/test_execute.py
 tests/test_exponential.py
 tests/test_extend_labeling_via_voronoi.py
-tests/test_extend_labels_with_maximum_radius.py
 tests/test_extended_depth_of_focus_variance_projection.py
 tests/test_flag_existing_labels.py
 tests/test_flip.py
 tests/test_gamma_correction.py
 tests/test_gaussian_blur.py
 tests/test_generate_angle_matrix.py
 tests/test_generate_binary_overlap_matrix.py
 tests/test_generate_distance_matrix.py
 tests/test_generate_n_nearest_neighbor_matrix.py
 tests/test_generate_proximal_neighbor_matrix.py
 tests/test_generate_touch_matrix.py
+tests/test_gpu_switch.py
 tests/test_gradient_x.py
 tests/test_gradient_y.py
 tests/test_gradient_z.py
 tests/test_greater.py
 tests/test_greater_constant.py
 tests/test_greater_or_equal.py
 tests/test_greater_or_equal_constant.py
@@ -774,14 +780,15 @@
 tests/test_push_regionprops_column.py
 tests/test_radians_to_degrees.py
 tests/test_read_intensities_from_map.py
 tests/test_read_intensities_from_positions.py
 tests/test_reduce_stack.py
 tests/test_reduction.py
 tests/test_regionprops.py
+tests/test_relabel_sequential.py
 tests/test_replace_intensities.py
 tests/test_replace_intensity.py
 tests/test_resample.py
 tests/test_rigid_transform.py
 tests/test_rotate.py
 tests/test_scale.py
 tests/test_set.py
@@ -789,14 +796,15 @@
 tests/test_set_image_borders.py
 tests/test_set_nonzero_pixels_to_pixelindex.py
 tests/test_set_plane.py
 tests/test_set_ramp_x.py
 tests/test_set_ramp_y.py
 tests/test_set_ramp_z.py
 tests/test_set_row.py
+tests/test_set_wait_for_kernel_finish.py
 tests/test_set_where_x_equals_y.py
 tests/test_set_where_x_greater_than_y.py
 tests/test_set_where_x_smaller_than_y.py
 tests/test_skimage_imsave.py
 tests/test_smaller.py
 tests/test_smaller_constant.py
 tests/test_smaller_or_equal.py
```

### Comparing `pyclesperanto_prototype-0.9.7/setup.py` & `pyclesperanto_prototype-0.9.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyclesperanto_prototype",
-    version="0.9.7",
+    version="0.9.9",
     author="haesleinhuepf",
     author_email="robert.haase@tu-dresden.de",
-    description="OpenCL-based GPU-accelerated image processing",
+    description="GPU-accelerated image processing in python using OpenCL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/clEsperanto/pyclesperanto_prototype",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=["numpy!=1.19.4", "pyopencl", "toolz", "scikit-image>=0.18.0", "matplotlib", "transforms3d"],
     python_requires='>=3.6',
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_absolute.py` & `pyclesperanto_prototype-0.9.9/tests/test_absolute.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_add_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/tests/test_add_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_add_images.py` & `pyclesperanto_prototype-0.9.9/tests/test_add_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_add_images_weighted.py` & `pyclesperanto_prototype-0.9.9/tests/test_add_images_weighted.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_affine_transform.py` & `pyclesperanto_prototype-0.9.9/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_apply_vector_field.py` & `pyclesperanto_prototype-0.9.9/tests/test_apply_vector_field.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_average_distance_of_n_far_off_distances.py` & `pyclesperanto_prototype-0.9.9/tests/test_average_distance_of_n_far_off_distances.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_average_distance_of_n_shortest_distances.py` & `pyclesperanto_prototype-0.9.9/tests/test_average_distance_of_n_shortest_distances.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_average_distance_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/tests/test_average_distance_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_binary_and.py` & `pyclesperanto_prototype-0.9.9/tests/test_binary_and.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_binary_edge_detection.py` & `pyclesperanto_prototype-0.9.9/tests/test_binary_edge_detection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_block_enumerate.py` & `pyclesperanto_prototype-0.9.9/tests/test_block_enumerate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_bounding_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_centroids_of_labels.py` & `pyclesperanto_prototype-0.9.9/tests/test_centroids_of_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_close_index_gaps_in_label_maps.py` & `pyclesperanto_prototype-0.9.9/tests/test_flag_existing_labels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_close_index_gaps_in_label_maps():
+def test_flag_existing_labels():
 
     gpu_input = cle.push(np.asarray([
         [
             [1, 2, 3],
             [1, 6, 6],
             [7, 8, 9]
         ]
     ]))
-    gpu_output = cle.create_like(gpu_input)
 
     gpu_reference = cle.push(np.asarray([
-        [
-            [1, 2, 3],
-            [1, 4, 4],
-            [5, 6, 7]
-        ]
+        [0, 1, 1, 1, 0, 0, 1, 1, 1, 1]
     ]))
 
-
-
-    cle.close_index_gaps_in_label_map(gpu_input, gpu_output)
+    gpu_output = cle.flag_existing_labels(gpu_input)
 
     a = cle.pull(gpu_output)
     b = cle.pull(gpu_reference)
 
     print(a)
     print(b)
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_combine_horizontally.py` & `pyclesperanto_prototype-0.9.9/tests/test_combine_horizontally.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_combine_vertically.py` & `pyclesperanto_prototype-0.9.9/tests/test_combine_vertically.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_concatenate_stacks.py` & `pyclesperanto_prototype-0.9.9/tests/test_concatenate_stacks.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_connected_components_labeling_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_connected_components_labeling_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_connected_components_labeling_diamond.py` & `pyclesperanto_prototype-0.9.9/tests/test_connected_components_labeling_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_convolve.py` & `pyclesperanto_prototype-0.9.9/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_copy_slice.py` & `pyclesperanto_prototype-0.9.9/tests/test_copy_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_count_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/tests/test_count_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_create.py` & `pyclesperanto_prototype-0.9.9/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_crop.py` & `pyclesperanto_prototype-0.9.9/tests/test_crop.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_detect_label_edges.py` & `pyclesperanto_prototype-0.9.9/tests/test_detect_label_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_detect_maxima_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_detect_maxima_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_detect_minima_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_detect_minima_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_difference_of_gaussian.py` & `pyclesperanto_prototype-0.9.9/tests/test_difference_of_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_dilate_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_dilate_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_dilate_box_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/tests/test_dilate_box_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_dilate_sphere.py` & `pyclesperanto_prototype-0.9.9/tests/test_dilate_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_dilate_sphere_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/tests/test_dilate_sphere_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_divide_images.py` & `pyclesperanto_prototype-0.9.9/tests/test_divide_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_downsample_xy_half_median.py` & `pyclesperanto_prototype-0.9.9/tests/test_downsample_xy_half_median.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_equal.py` & `pyclesperanto_prototype-0.9.9/tests/test_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_equal_constant.py` & `pyclesperanto_prototype-0.9.9/tests/test_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_erode_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_erode_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_erode_box_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/tests/test_erode_box_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_erode_sphere.py` & `pyclesperanto_prototype-0.9.9/tests/test_erode_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_erode_sphere_slice_by_slice.py` & `pyclesperanto_prototype-0.9.9/tests/test_erode_sphere_slice_by_slice.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_euclidean_distance_from_label_centroid_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_euclidean_distance_from_label_centroid_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_exclude_labels.py` & `pyclesperanto_prototype-0.9.9/tests/test_exclude_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_on_edges.py` & `pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_on_edges.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_out_of_size_range.py` & `pyclesperanto_prototype-0.9.9/tests/test_nonzero_minimum_diamond.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_exclude_labels_out_of_size_range_2d():
-    
-    gpu_input = cle.push(np.asarray([
-            [1, 1, 2, 0, 3, 3],
-            [1, 1, 2, 0, 3, 3],
-            [0, 0, 0, 0, 0, 0],
-            [4, 4, 5, 6, 6, 6],
-            [4, 4, 5, 6, 6, 6]
+def test_nonzero_minimum_diamond():
+    test = cle.push(np.asarray([
+        [0, 0, 0, 0, 0],
+        [0, 1, 1, 2, 0],
+        [0, 2, 2, 3, 0],
+        [0, 3, 3, 4, 0],
+        [0, 0, 0, 0, 0]
     ]))
 
-    gpu_reference = cle.push(np.asarray([
-            [1, 1, 0, 0, 2, 2],
-            [1, 1, 0, 0, 2, 2],
-            [0, 0, 0, 0, 0, 0],
-            [3, 3, 0, 0, 0, 0],
-            [3, 3, 0, 0, 0, 0]
+    reference = cle.push(np.asarray([
+        [0, 0, 0, 0, 0],
+        [0, 1, 1, 1, 0],
+        [0, 1, 1, 2, 0],
+        [0, 2, 2, 3, 0],
+        [0, 0, 0, 0, 0]
     ]))
 
-    gpu_output = cle.exclude_labels_outside_size_range(gpu_input, gpu_input, minimum_size=4, maximum_size=5)
+    result = cle.create(test)
+    flag = cle.create((1, 1, 1))
 
-    a = cle.pull(gpu_output)
-    b = cle.pull(gpu_reference)
+    # as nonzero filters don't touch zero values, we need to initialize the result in advance
+    cle.set(result, 0)
 
-    print(a)
-    print(b)
+    cle.nonzero_minimum_diamond(test, flag, result)
 
-    assert (np.array_equal(a, b))
+    print(result)
+
+    a = cle.pull(result)
+    b = cle.pull(reference)
+    assert (np.allclose(a, b, atol=0.00001))
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_with_values_out_of_range.py` & `pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_with_values_out_of_range.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_exclude_labels_with_values_within_range.py` & `pyclesperanto_prototype-0.9.9/tests/test_exclude_labels_with_values_within_range.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_exponential.py` & `pyclesperanto_prototype-0.9.9/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_extend_labeling_via_voronoi.py` & `pyclesperanto_prototype-0.9.9/tests/test_extend_labeling_via_voronoi.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_extend_labels_with_maximum_radius.py` & `pyclesperanto_prototype-0.9.9/tests/test_dilate_labels.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_extend_labels_with_maximum_radius_2d():
+def test_dilate_labels_2d():
     
     gpu_input = cle.push(np.asarray([
 
             [1, 0, 0, 0, 0, 2],
             [0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0],
             [0, 0, 0, 4, 0, 0],
@@ -31,15 +31,15 @@
     b = cle.pull(gpu_reference)
 
     print(a)
     print(b)
 
     assert (np.array_equal(a, b))
 
-def test_extend_labels_with_maximum_radius_3d():
+def test_dilate_labels_3d():
     gpu_input = cle.push(np.asarray([
         [
             [0, 0, 0, 0, 0, 2],
             [0, 0, 0, 0, 0, 0],
             [0, 0, 0, 0, 0, 0],
             [0, 0, 0, 4, 0, 0],
             [0, 0, 0, 0, 0, 0],
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_extended_depth_of_focus_variance_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_extended_depth_of_focus_variance_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_flag_existing_labels.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_ramp_x.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_flag_existing_labels():
-
-    gpu_input = cle.push(np.asarray([
+def test_set_ramp_x():
+    result = cle.push(np.asarray([
         [
-            [1, 2, 3],
-            [1, 6, 6],
-            [7, 8, 9]
+            [0, 0, 0],
+            [3, 4, 3],
+            [3, 4, 3]
+        ], [
+            [3, 4, 3],
+            [3, 4, 3],
+            [3, 4, 3]
         ]
     ]))
 
-    gpu_reference = cle.push(np.asarray([
-        [0, 1, 1, 1, 0, 0, 1, 1, 1, 1]
+    reference = cle.push(np.asarray([
+        [
+            [0, 1, 2],
+            [0, 1, 2],
+            [0, 1, 2]
+        ], [
+            [0, 1, 2],
+            [0, 1, 2],
+            [0, 1, 2]
+        ]
     ]))
 
-    gpu_output = cle.flag_existing_labels(gpu_input)
+    cle.set_ramp_x(result)
 
-    a = cle.pull(gpu_output)
-    b = cle.pull(gpu_reference)
+    a = cle.pull(result)
+    b = cle.pull(reference)
 
     print(a)
     print(b)
 
-    assert (np.array_equal(a, b))
+    assert (np.allclose(a, b, 0.001))
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_flip.py` & `pyclesperanto_prototype-0.9.9/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_gamma_correction.py` & `pyclesperanto_prototype-0.9.9/tests/test_gamma_correction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_generate_angle_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_generate_angle_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_generate_binary_overlap_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_generate_binary_overlap_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_generate_distance_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_generate_distance_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_generate_n_nearest_neighbor_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_generate_n_nearest_neighbor_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_generate_proximal_neighbor_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_generate_proximal_neighbor_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_generate_touch_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_generate_touch_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_gradient_x.py` & `pyclesperanto_prototype-0.9.9/tests/test_gradient_x.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_gradient_y.py` & `pyclesperanto_prototype-0.9.9/tests/test_gradient_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_gradient_z.py` & `pyclesperanto_prototype-0.9.9/tests/test_gradient_z.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_greater.py` & `pyclesperanto_prototype-0.9.9/tests/test_greater.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_greater_constant.py` & `pyclesperanto_prototype-0.9.9/tests/test_greater_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_greater_or_equal.py` & `pyclesperanto_prototype-0.9.9/tests/test_greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_greater_or_equal_constant.py` & `pyclesperanto_prototype-0.9.9/tests/test_greater_or_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_histogram.py` & `pyclesperanto_prototype-0.9.9/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_image.py` & `pyclesperanto_prototype-0.9.9/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_jaccard_index.py` & `pyclesperanto_prototype-0.9.9/tests/test_jaccard_index.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_maximum_extension_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_maximum_extension_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_maximum_extension_ratio_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_maximum_extension_ratio_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_maximum_intensity_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_maximum_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_mean_extension_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_mean_extension_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_mean_intensity_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_mean_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_minimum_intensity_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_minimum_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_pixelcount_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_pixelcount_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_spots.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_spots.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_label_standard_deviation_intensity_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_label_standard_deviation_intensity_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_labelled_spots_to_pointlist.py` & `pyclesperanto_prototype-0.9.9/tests/test_labelled_spots_to_pointlist.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_laplace_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_laplace_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_laplace_diamond.py` & `pyclesperanto_prototype-0.9.9/tests/test_laplace_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mask.py` & `pyclesperanto_prototype-0.9.9/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mask_label.py` & `pyclesperanto_prototype-0.9.9/tests/test_mask_label.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_masked_voronoi_labeling.py` & `pyclesperanto_prototype-0.9.9/tests/test_masked_voronoi_labeling.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_distance_of_n_shortest_distances.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_distance_of_n_shortest_distances.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_distance_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_distance_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_images.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_sphere.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_x_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_y_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_maximum_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_maximum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_sphere.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_x_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_y_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mean_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_mean_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_median_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_median_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_median_sphere.py` & `pyclesperanto_prototype-0.9.9/tests/test_median_sphere.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_merge_touching_labels.py` & `pyclesperanto_prototype-0.9.9/tests/test_merge_touching_labels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_distance_of_touching_neighbors.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_distance_of_touching_neighbors.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_images.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_of_masked_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_of_masked_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_x_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_y_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_minimum_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_minimum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_mode_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_mode_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_multiply_image_and_coordinate.py` & `pyclesperanto_prototype-0.9.9/tests/test_multiply_image_and_coordinate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_multiply_image_and_scalar.py` & `pyclesperanto_prototype-0.9.9/tests/test_multiply_image_and_scalar.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_multiply_images.py` & `pyclesperanto_prototype-0.9.9/tests/test_multiply_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_multiply_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_multiply_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_n_closest_points.py` & `pyclesperanto_prototype-0.9.9/tests/test_n_closest_points.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_nonzero_maximum_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_nonzero_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_nonzero_maximum_diamond.py` & `pyclesperanto_prototype-0.9.9/tests/test_nonzero_maximum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_nonzero_minimum_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_nonzero_minimum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_nonzero_minimum_diamond.py` & `pyclesperanto_prototype-0.9.9/tests/test_replace_intensities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_nonzero_minimum_diamond():
-    test = cle.push(np.asarray([
+
+def test_replace_intensities():
+    test1 = cle.push(np.asarray([
         [0, 0, 0, 0, 0],
-        [0, 1, 1, 2, 0],
-        [0, 2, 2, 3, 0],
-        [0, 3, 3, 4, 0],
+        [0, 1, 2, 3, 0],
+        [0, 2, 3, 4, 0],
+        [0, 4, 4, 5, 0],
         [0, 0, 0, 0, 0]
     ]))
 
+    test2 = cle.push(np.asarray([
+        [0, 9, 8, 7, 6, 5]
+    ]))
+
     reference = cle.push(np.asarray([
         [0, 0, 0, 0, 0],
-        [0, 1, 1, 1, 0],
-        [0, 1, 1, 2, 0],
-        [0, 2, 2, 3, 0],
+        [0, 9, 8, 7, 0],
+        [0, 8, 7, 6, 0],
+        [0, 6, 6, 5, 0],
         [0, 0, 0, 0, 0]
     ]))
 
-    result = cle.create(test)
-    flag = cle.create((1, 1, 1))
-
-    # as nonzero filters don't touch zero values, we need to initialize the result in advance
-    cle.set(result, 0)
-
-    cle.nonzero_minimum_diamond(test, flag, result)
+    result = cle.create(test1)
+    cle.replace_intensities(test1, test2, result)
 
     print(result)
 
     a = cle.pull(result)
     b = cle.pull(reference)
-    assert (np.allclose(a, b, atol=0.00001))
-
+    assert (np.allclose(a, b, 0.001))
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_not_equal.py` & `pyclesperanto_prototype-0.9.9/tests/test_not_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_not_equal_constant.py` & `pyclesperanto_prototype-0.9.9/tests/test_not_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_onlyzero_overwrite_maximum_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_onlyzero_overwrite_maximum_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_onlyzero_overwrite_maximum_diamond.py` & `pyclesperanto_prototype-0.9.9/tests/test_onlyzero_overwrite_maximum_diamond.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_operators.py` & `pyclesperanto_prototype-0.9.9/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_paste.py` & `pyclesperanto_prototype-0.9.9/tests/test_paste.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_point_index_list_to_mesh.py` & `pyclesperanto_prototype-0.9.9/tests/test_point_index_list_to_mesh.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_point_index_list_to_touch_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_point_index_list_to_touch_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_pointlist_to_labelled_spots.py` & `pyclesperanto_prototype-0.9.9/tests/test_pointlist_to_labelled_spots.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_power.py` & `pyclesperanto_prototype-0.9.9/tests/test_power.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_power_images.py` & `pyclesperanto_prototype-0.9.9/tests/test_power_images.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_proximal_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_proximal_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_push.py` & `pyclesperanto_prototype-0.9.9/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_push_regionprops_column.py` & `pyclesperanto_prototype-0.9.9/tests/test_push_regionprops_column.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_read_intensities_from_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_read_intensities_from_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_read_intensities_from_positions.py` & `pyclesperanto_prototype-0.9.9/tests/test_read_intensities_from_positions.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_reduce_stack.py` & `pyclesperanto_prototype-0.9.9/tests/test_reduce_stack.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_reduction.py` & `pyclesperanto_prototype-0.9.9/tests/test_reduction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_regionprops.py` & `pyclesperanto_prototype-0.9.9/tests/test_regionprops.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_replace_intensities.py` & `pyclesperanto_prototype-0.9.9/tests/test_voronoi_labeling.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-
-def test_replace_intensities():
-    test1 = cle.push(np.asarray([
-        [0, 0, 0, 0, 0],
-        [0, 1, 2, 3, 0],
-        [0, 2, 3, 4, 0],
-        [0, 4, 4, 5, 0],
-        [0, 0, 0, 0, 0]
+def test_voronoi_labeling():
+    
+    gpu_input = cle.push(np.asarray([
+        [
+            [0, 0, 0, 0, 0, 0],
+            [0, 1, 0, 0, 1, 0],
+            [0, 0, 0, 0, 0, 0],
+            [0, 0, 0, 0, 0, 0],
+            [0, 1, 0, 0, 1, 0],
+            [0, 0, 0, 0, 0, 0],
+        ]
     ]))
 
-    test2 = cle.push(np.asarray([
-        [0, 9, 8, 7, 6, 5]
+    gpu_reference = cle.push(np.asarray([
+        [
+            [1, 1, 1, 3, 3, 3],
+            [1, 1, 1, 3, 3, 3],
+            [1, 1, 1, 3, 3, 3],
+            [2, 2, 2, 4, 4, 4],
+            [2, 2, 2, 4, 4, 4],
+            [2, 2, 2, 4, 4, 4],
+        ]
     ]))
 
-    reference = cle.push(np.asarray([
-        [0, 0, 0, 0, 0],
-        [0, 9, 8, 7, 0],
-        [0, 8, 7, 6, 0],
-        [0, 6, 6, 5, 0],
-        [0, 0, 0, 0, 0]
-    ]))
+    gpu_output = cle.voronoi_labeling(gpu_input)
 
-    result = cle.create(test1)
-    cle.replace_intensities(test1, test2, result)
+    a = cle.pull(gpu_output)
+    b = cle.pull(gpu_reference)
 
-    print(result)
+    print(a)
+    print(b)
 
-    a = cle.pull(result)
-    b = cle.pull(reference)
-    assert (np.allclose(a, b, 0.001))
+    assert (np.array_equal(a, b))
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_replace_intensity.py` & `pyclesperanto_prototype-0.9.9/tests/test_replace_intensity.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_resample.py` & `pyclesperanto_prototype-0.9.9/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_rigid_transform.py` & `pyclesperanto_prototype-0.9.9/tests/test_rigid_transform.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_rotate.py` & `pyclesperanto_prototype-0.9.9/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_scale.py` & `pyclesperanto_prototype-0.9.9/tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_column.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_column.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_image_borders.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_image_borders.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_nonzero_pixels_to_pixelindex.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_nonzero_pixels_to_pixelindex.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_plane.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_plane.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_ramp_x.py` & `pyclesperanto_prototype-0.9.9/tests/test_translate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_set_ramp_x():
-    result = cle.push(np.asarray([
-        [
-            [0, 0, 0],
-            [3, 4, 3],
-            [3, 4, 3]
-        ], [
-            [3, 4, 3],
-            [3, 4, 3],
-            [3, 4, 3]
-        ]
-    ]))
-
-    reference = cle.push(np.asarray([
-        [
-            [0, 1, 2],
-            [0, 1, 2],
-            [0, 1, 2]
-        ], [
-            [0, 1, 2],
-            [0, 1, 2],
-            [0, 1, 2]
-        ]
-    ]))
+def test_translate():
+    source = cle.push(np.asarray([[
+          [0, 0, 0, 0, 0],
+          [0, 0, 0, 0, 0],
+          [0, 0, 1, 1, 0],
+          [0, 0, 0, 0, 0],
+          [0, 0, 0, 0, 0],
+    ]]))
+
+    reference = cle.push(np.asarray([[
+        [0, 0, 0, 0, 0],
+        [0, 1, 1, 0, 0],
+        [0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0],
+    ]]))
 
-    cle.set_ramp_x(result)
+    result = cle.translate(source, translate_x=-1, translate_y=-1)
 
     a = cle.pull(result)
     b = cle.pull(reference)
 
     print(a)
     print(b)
 
-    assert (np.allclose(a, b, 0.001))
+    assert (np.array_equal(a, b))
+
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_ramp_y.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_ramp_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_ramp_z.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_ramp_z.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_row.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_row.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_where_x_equals_y.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_where_x_equals_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_where_x_greater_than_y.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_where_x_greater_than_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_set_where_x_smaller_than_y.py` & `pyclesperanto_prototype-0.9.9/tests/test_set_where_x_smaller_than_y.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_smaller.py` & `pyclesperanto_prototype-0.9.9/tests/test_smaller.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_smaller_constant.py` & `pyclesperanto_prototype-0.9.9/tests/test_smaller_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_smaller_or_equal.py` & `pyclesperanto_prototype-0.9.9/tests/test_smaller_or_equal.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_smaller_or_equal_constant.py` & `pyclesperanto_prototype-0.9.9/tests/test_smaller_or_equal_constant.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sobel.py` & `pyclesperanto_prototype-0.9.9/tests/test_sobel.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sorenson_dice_coefficient.py` & `pyclesperanto_prototype-0.9.9/tests/test_sorenson_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_spots_to_pointlist.py` & `pyclesperanto_prototype-0.9.9/tests/test_spots_to_pointlist.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_standard_deviation_of_touching_neighbors_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_standard_deviation_of_touching_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_standard_deviation_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_standard_deviation_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_statistics_of_background_and_labelled_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_statistics_of_background_and_labelled_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_statistics_of_labelled_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_statistics_of_labelled_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sum_of_all_pixels.py` & `pyclesperanto_prototype-0.9.9/tests/test_sum_of_all_pixels.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sum_reduction.py` & `pyclesperanto_prototype-0.9.9/tests/test_sum_reduction.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sum_x_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_sum_x_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sum_y_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_sum_y_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_sum_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_sum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_threshold_otsu.py` & `pyclesperanto_prototype-0.9.9/tests/test_threshold_otsu.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_touch_matrix_to_adjacency_matrix.py` & `pyclesperanto_prototype-0.9.9/tests/test_touch_matrix_to_adjacency_matrix.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_touch_matrix_to_mesh.py` & `pyclesperanto_prototype-0.9.9/tests/test_touch_matrix_to_mesh.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_touching_neighbor_count_map.py` & `pyclesperanto_prototype-0.9.9/tests/test_touching_neighbor_count_map.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_translate.py` & `pyclesperanto_prototype-0.9.9/tests/test_variance_sphere.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_translate():
-    source = cle.push(np.asarray([[
-          [0, 0, 0, 0, 0],
-          [0, 0, 0, 0, 0],
-          [0, 0, 1, 1, 0],
-          [0, 0, 0, 0, 0],
-          [0, 0, 0, 0, 0],
-    ]]))
-
-    reference = cle.push(np.asarray([[
+def test_variance_sphere():
+    test1 = cle.push(np.asarray([
         [0, 0, 0, 0, 0],
-        [0, 1, 1, 0, 0],
         [0, 0, 0, 0, 0],
+        [0, 0, 1, 0, 0],
         [0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0]
+    ]))
+
+    reference = cle.push(np.asarray([
         [0, 0, 0, 0, 0],
-    ]]))
+        [0, 0, 0.16, 0, 0],
+        [0, 0.16, 0.16, 0.16, 0],
+        [0, 0, 0.16, 0, 0],
+        [0, 0, 0, 0, 0]
+    ]))
 
-    result = cle.translate(source, translate_x=-1, translate_y=-1)
+    result = cle.create(test1)
+    cle.variance_sphere(test1, result, 1, 1, 0)
 
     a = cle.pull(result)
     b = cle.pull(reference)
 
     print(a)
-    print(b)
-
-    assert (np.array_equal(a, b))
 
+    assert (np.allclose(a, b, 0.01))
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_transpose_xy.py` & `pyclesperanto_prototype-0.9.9/tests/test_transpose_xy.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_transpose_xz.py` & `pyclesperanto_prototype-0.9.9/tests/test_transpose_xz.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_transpose_yz.py` & `pyclesperanto_prototype-0.9.9/tests/test_transpose_yz.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_undefined_to_zero.py` & `pyclesperanto_prototype-0.9.9/tests/test_undefined_to_zero.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_variance_box.py` & `pyclesperanto_prototype-0.9.9/tests/test_variance_box.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_voronoi_labeling.py` & `pyclesperanto_prototype-0.9.9/tests/test_voronoi_otsu_labeling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import pyclesperanto_prototype as cle
 import numpy as np
 
-def test_voronoi_labeling():
+def test_masked_voronoi_labeling():
     
     gpu_input = cle.push(np.asarray([
-        [
-            [0, 0, 0, 0, 0, 0],
-            [0, 1, 0, 0, 1, 0],
-            [0, 0, 0, 0, 0, 0],
-            [0, 0, 0, 0, 0, 0],
-            [0, 1, 0, 0, 1, 0],
-            [0, 0, 0, 0, 0, 0],
-        ]
+
+            [0, 0, 1, 1, 0, 0],
+            [0, 1, 8, 9, 1, 0],
+            [0, 1, 7, 6, 1, 0],
+            [0, 0, 1, 1, 1, 0],
+            [0, 0, 1, 1, 1, 0],
+            [0, 0, 1, 8, 7, 1],
+            [0, 0, 1, 1, 1, 0],
+
     ]))
 
+
     gpu_reference = cle.push(np.asarray([
-        [
-            [1, 1, 1, 3, 3, 3],
-            [1, 1, 1, 3, 3, 3],
-            [1, 1, 1, 3, 3, 3],
-            [2, 2, 2, 4, 4, 4],
-            [2, 2, 2, 4, 4, 4],
-            [2, 2, 2, 4, 4, 4],
-        ]
+
+            [0, 0, 1, 1, 0, 0],
+            [0, 1, 1, 1, 1, 0],
+            [0, 1, 1, 1, 1, 0],
+            [0, 0, 2, 2, 2, 0],
+            [0, 0, 2, 2, 2, 0],
+            [0, 0, 2, 2, 2, 0],
+            [0, 0, 0, 2, 2, 0],
+
     ]))
 
-    gpu_output = cle.voronoi_labeling(gpu_input)
+    gpu_output = cle.voronoi_otsu_labeling(gpu_input, spot_sigma=1, outline_sigma=1)
 
     a = cle.pull(gpu_output)
     b = cle.pull(gpu_reference)
 
     print(a)
     print(b)
```

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_write_values_to_positions.py` & `pyclesperanto_prototype-0.9.9/tests/test_write_values_to_positions.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_z_position_of_maximum_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_z_position_of_maximum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_z_position_of_minimum_z_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_z_position_of_minimum_z_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_z_position_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_z_position_projection.py`

 * *Files identical despite different names*

### Comparing `pyclesperanto_prototype-0.9.7/tests/test_z_position_range_projection.py` & `pyclesperanto_prototype-0.9.9/tests/test_z_position_range_projection.py`

 * *Files identical despite different names*

