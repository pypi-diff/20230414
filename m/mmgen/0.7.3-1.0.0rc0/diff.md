# Comparing `tmp/mmgen-0.7.3.tar.gz` & `tmp/mmgen-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmgen-0.7.3.tar", last modified: Fri Apr 14 12:07:38 2023, max compression
+gzip compressed data, was "dist/mmgen-1.0.0rc0.tar", last modified: Thu Sep  1 03:09:44 2022, max compression
```

## Comparing `mmgen-0.7.3.tar` & `mmgen-1.0.0rc0.tar`

### file list

```diff
@@ -1,418 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-14 12:07:06.000000 mmgen-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-04-14 12:07:38.000000 mmgen-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 12:07:06.000000 mmgen-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/Inception_Score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/cifar10_inception_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/cifar10_noaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/cifar10_nopad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/cifar10_random_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/cifar10_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/ffhq_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/grow_scale_imgs_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/grow_scale_imgs_celeba-hq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/grow_scale_imgs_ffhq_styleganv1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_128x128_inception_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_64x64_inception_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_noaug_128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_noaug_256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_noaug_64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/imagenet_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/lsun-car_pad_512.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/lsun_stylegan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/paired_imgs_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/paired_imgs_256x256_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/singan.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/unconditional_imgs_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/unconditional_imgs_64x64.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/unconditional_imgs_flip_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/unconditional_imgs_flip_512x512.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/unconditional_imgs_flip_lanczos_resize_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/datasets/unpaired_imgs_256x256.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/default_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/biggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/biggan/biggan_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/biggan/biggan_32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/cyclegan/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/cyclegan/cyclegan_lsgan_resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/dcgan/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/dcgan/dcgan_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/dcgan/dcgan_64x64.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/improved_ddpm/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/improved_ddpm/ddpm_32x32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/improved_ddpm/ddpm_64x64.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/lsgan/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/lsgan/lsgan_128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/pggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/pggan/pggan_1024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/pggan/pggan_128x128.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/pix2pix/pix2pix_vanilla_unet_bn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/sagan/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/sagan/sagan_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/sagan/sagan_32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/singan/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/singan/singan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/sngan_proj/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/sngan_proj/sngan_proj_128x128.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/sngan_proj/sngan_proj_32x32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/stylegan/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/stylegan/stylegan2_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/stylegan/stylegan3_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/stylegan/styleganv1_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/wgangp/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/_base_/models/wgangp/wgangp_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/ada/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ada/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ada/stylegan3_r_ada_fp16_gamma3.3_metfaces_1024_b4x8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ada/stylegan3_t_ada_fp16_gamma6.6_metfaces_1024_b4x8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan-deep_128x128_cvt_hugging-face_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan-deep_256x256_cvt_hugging-face_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan-deep_512x512_cvt_hugging-face_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan_128x128_cvt_BigGAN-PyTorch_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan_ajbrock-sn_imagenet1k_128x128_b32x8_1500k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan_cifar10_32x32_b25x2_500k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/biggan_torch-sn_imagenet1k_128x128_b32x8_1500k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/biggan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/cyclegan_lsgan_id0_resnet_in_facades_b1x1_80k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/cyclegan_lsgan_id0_resnet_in_horse2zebra_b1x1_270k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/cyclegan_lsgan_id0_resnet_in_summer2winter_b1x1_250k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/cyclegan_lsgan_resnet_in_facades_b1x1_80k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/cyclegan_lsgan_resnet_in_horse2zebra_b1x1_270k.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/cyclegan_lsgan_resnet_in_summer2winter_b1x1_250k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/cyclegan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/dcgan/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/dcgan/dcgan_celeba-cropped_64_b128x1_300k.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/dcgan/dcgan_lsun-bedroom_64x64_b128x1_5e.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/dcgan/dcgan_mnist-64_b128x1_Glr4e-4_Dlr1e-4_5k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/dcgan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/ggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ggan/ggan_celeba-cropped_dcgan-archi_lr-1e-3_64_b128x1_12m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ggan/ggan_celeba-cropped_dcgan-archi_lr-1e-4_128_b64x1_10m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ggan/ggan_lsun-bedroom_lsgan_archi_lr-1e-4_64_b128x1_20m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/ggan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/improved_ddpm/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/improved_ddpm/ddpm_cosine_hybird_timestep-4k_drop0.3_cifar10_32x32_b8x16_500k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/improved_ddpm/ddpm_cosine_hybird_timestep-4k_drop0.3_imagenet1k_64x64_b8x16_1500k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/improved_ddpm/ddpm_cosine_hybird_timestep-4k_imagenet1k_64x64_b8x16_1500k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/improved_ddpm/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/lsgan/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/lsgan/lsgan_dcgan-archi_lr-1e-3_celeba-cropped_64_b128x1_12m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/lsgan/lsgan_dcgan-archi_lr-1e-4_celeba-cropped_128_b64x1_10m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/lsgan/lsgan_dcgan-archi_lr-1e-4_lsun-bedroom_64_b128x1_12m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/lsgan/lsgan_lsgan-archi_lr-1e-4_lsun-bedroom_128_b64x1_10m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/lsgan/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/pggan/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pggan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pggan/pggan_celeba-cropped_128_g8_12Mimgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pggan/pggan_celeba-hq_1024_g8_12Mimg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pggan/pggan_lsun-bedroom_128_g8_12Mimgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pix2pix/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pix2pix/pix2pix_vanilla_unet_bn_aerial2maps_b1x1_220k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pix2pix/pix2pix_vanilla_unet_bn_facades_b1x1_80k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pix2pix/pix2pix_vanilla_unet_bn_maps2aerial_b1x1_220k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/pix2pix/pix2pix_vanilla_unet_bn_wo_jitter_flip_edges2shoes_b1x4_190k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c1_config-f_ffhq_256-1024_b2x8_1600k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c1_config-g_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-c_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-d_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-e_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-f_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-f_ffhq_256-896_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-h_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-i_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-j_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/mspie-stylegan2_c2_config-k_ffhq_256-512_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_csg_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_csg_fish.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_interp-pad_balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_interp-pad_disc-nobn_balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_interp-pad_disc-nobn_fish.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_spe-dim4_fish.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/singan_spe-dim8_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/stylegan2_c2_ffhq_256_b3x8_1100k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/positional_encoding_in_gans/stylegan2_c2_ffhq_512_b3x8_1100k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/sagan_128_cvt_studioGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/sagan_128_woReLUinplace_Glr-1e-4_Dlr-4e-4_ndisc1_imagenet1k_b64x4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/sagan_128_woReLUinplace_noaug_bigGAN_Glr-1e-4_Dlr-4e-4_ndisc1_imagenet1k_b32x8.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/sagan_32_cvt_studioGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/sagan_32_wReLUinplace_lr-2e-4_ndisc5_cifar10_b64x1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sagan/sagan_32_woReLUinplace_lr-2e-4_ndisc5_cifar10_b64x1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/singan/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/singan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/singan/singan_balloons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/singan/singan_bohemian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/singan/singan_fish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/sngan_proj_128_cvt_studioGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/sngan_proj_128_wReLUinplace_Glr-2e-4_Dlr-5e-5_ndisc5_imagenet1k_b128x2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/sngan_proj_128_woReLUinplace_Glr-2e-4_Dlr-5e-5_ndisc5_imagenet1k_b128x2.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/sngan_proj_32_cvt_studioGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/sngan_proj_32_wReLUinplace_lr-2e-4_ndisc5_cifar10_b64x1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/sngan_proj/sngan_proj_32_woReLUinplace_lr-2e-4_ndisc5_cifar10_b64x1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv1/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv1/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv1/styleganv1_ffhq_1024_g8_25Mimg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv1/styleganv1_ffhq_256_g8_25Mimg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_apex_fp16_PL-R1-no-scaler_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_apex_fp16_quicktest_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_ffhq_1024_b4x8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_fp16-globalG-partialD_PL-R1-no-scaler_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_fp16-global_quicktest_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_fp16_partial-GD_PL-no-scaler_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_fp16_quicktest_ffhq_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_lsun-car_384x512_b4x8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_lsun-cat_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_lsun-church_256_b4x8_800k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv2/stylegan2_c2_lsun-horse_256_b4x8_800k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5133 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_r_ada_fp16_gamma3.3_metfaces_1024_b4x8.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_r_afhqv2_512_b4x8_cvt_official_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_r_ffhq_1024_b4x8_cvt_official_rgb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      458 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_r_ffhqu_256_b4x8_cvt_official_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_t_ada_fp16_gamma6.6_metfaces_1024_b4x8.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_t_afhqv2_512_b4x8_cvt_official_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_t_ffhq_1024_b4x8_cvt_official_rgb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      403 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_t_ffhqu_256_b4x8_cvt_official_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_t_noaug_fp16_gamma2.0_ffhq_256_b4x8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/styleganv3/stylegan3_t_noaug_fp16_gamma32.8_ffhq_1024_b4x8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/configs/wgan-gp/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/wgan-gp/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/wgan-gp/wgangp_GN_GP-50_lsun-bedroom_128_b64x1_160kiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/configs/wgan-gp/wgangp_GN_celeba-cropped_128_b64x1_160kiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/tools/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/deployment/mmgen2torchserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/deployment/mmgen_unconditional_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/deployment/test_torchserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/dist_eval.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      457 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/dist_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/eval.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/misc/print_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/publish_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/slurm_eval.sh
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/slurm_eval_multi_gpu.sh
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/.mim/tools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/utils/inception_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/utils/singan_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/.mim/tools/utils/translation_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/core/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/ddp_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19612 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/evaluation/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    58410 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/core/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/ceph_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/pggan_fetch_data_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/pickle_data_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/hooks/visualize_training_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/core/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/core/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/runners/apex_amp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/runners/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16136 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/runners/dynamic_iterbased_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/runners/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/core/scheduler/lr_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/grow_scale_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/paired_image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/pipelines/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/quick_test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/datasets/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/samplers/distributed_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/singan_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/unconditional_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/datasets/unpaired_image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/arcface/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/arcface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/arcface/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/arcface/id_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/arcface/model_irse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/biggan/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/biggan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/biggan/biggan_snmodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    31575 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/biggan/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33172 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/biggan/generator_discriminator_deep.py
--rw-r--r--   0 runner    (1001) docker     (123)    30150 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/biggan/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/cyclegan/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/cyclegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/cyclegan/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/cyclegan/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/dcgan/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/dcgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/dcgan/generator_discriminator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/ddpm/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/ddpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/ddpm/denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/ddpm/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/fid_inception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/lpips/
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/lpips/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6689 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/lpips/networks_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/lpips/perceptual_loss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1901 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/lpips/pretrained_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/lsgan/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/lsgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/lsgan/generator_discriminator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/pggan/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/pggan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/pggan/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/pggan/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/pix2pix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/pix2pix/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/pix2pix/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/positional_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/singan/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/singan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/singan/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/singan/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/singan/positional_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/sngan_proj/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/sngan_proj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37312 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/sngan_proj/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25257 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/sngan_proj/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19244 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/generator_discriminator_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    28667 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/generator_discriminator_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/generator_discriminator_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/styleganv1_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    41674 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/styleganv2_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    26930 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/styleganv3_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    21182 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/mspie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/stylegan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/architectures/wgan_gp/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/wgan_gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/wgan_gp/generator_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/architectures/wgan_gp/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/common/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/common/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/diffusions/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/diffusions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43348 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/diffusions/base_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/diffusions/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/diffusions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/gans/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/base_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/basic_conditional_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/mspie_stylegan2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/progressive_growing_unconditional_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/singan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/gans/static_unconditional_gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/ddpm_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/disc_auxiliary_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/gan_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    34737 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/gen_auxiliary_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    27866 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/pixelwise_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/losses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/models/translation_models/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/translation_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/translation_models/base_translation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/translation_models/cyclegan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/translation_models/pix2pix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/models/translation_models/static_translation_gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/conv2d_gradfix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/ops/stylegan3/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/stylegan3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/stylegan3/custom_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/ops/stylegan3/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/stylegan3/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/stylegan3/ops/bias_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/stylegan3/ops/filtered_lrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16682 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/ops/stylegan3/ops/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/utils/dist_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-14 12:07:06.000000 mmgen-0.7.3/mmgen/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14091 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 12:07:38.000000 mmgen-0.7.3/mmgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:07:38.000000 mmgen-0.7.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 12:07:06.000000 mmgen-0.7.3/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 12:07:06.000000 mmgen-0.7.3/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 12:07:06.000000 mmgen-0.7.3/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 12:07:06.000000 mmgen-0.7.3/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 12:07:06.000000 mmgen-0.7.3/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 12:07:38.000000 mmgen-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-14 12:07:06.000000 mmgen-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14201 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11545 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10421 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/apis/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/datasets/
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/grow_scale_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/paired_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/quick_test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/datasets/samplers/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3892 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4735 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/singan_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6949 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/transforms/loading.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12540 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/transforms/processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/unconditional_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5250 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/unpaired_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/engine/
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3356 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/hooks/iter_time_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/hooks/pggan_fetch_data_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/hooks/pickle_data_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17089 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/hooks/visualization_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/engine/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)      122 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7093 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/logging/log_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/engine/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11306 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/optimizers/optimizer_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/engine/runners/
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7460 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/runners/fp16_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6583 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/runners/loops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/engine/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/engine/schedulers/lr_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6945 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22972 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/evaluation/inception_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17845 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/evaluation/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    78586 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/arcface/
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/arcface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6054 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/arcface/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/arcface/id_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3867 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/arcface/model_irse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/biggan/
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/biggan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9438 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/biggan/biggan_snmodule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31556 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/biggan/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33153 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/biggan/generator_discriminator_deep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30023 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/biggan/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/common.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/cyclegan/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/cyclegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5651 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/cyclegan/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/cyclegan/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/dcgan/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/dcgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12299 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/dcgan/generator_discriminator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/ddpm/
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/ddpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19580 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/ddpm/denoising.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14946 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/ddpm/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12348 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/fid_inception.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lpips/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      370 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lpips/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6689 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lpips/networks_basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lpips/perceptual_loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1901 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lpips/pretrained_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lsgan/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lsgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11619 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/lsgan/generator_discriminator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pggan/
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pggan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17674 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pggan/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19780 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pggan/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pix2pix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9329 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pix2pix/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6151 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/pix2pix/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7895 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/positional_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/singan/
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/singan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10352 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/singan/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/singan/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/singan/positional_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/sngan_proj/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/sngan_proj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37760 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/sngan_proj/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25177 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/sngan_proj/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19196 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/generator_discriminator_v1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29195 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/generator_discriminator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8150 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/generator_discriminator_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6245 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/styleganv1_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42543 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/styleganv2_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27200 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/styleganv3_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21166 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/mspie.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8360 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/architectures/wgan_gp/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/wgan_gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9339 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/wgan_gp/generator_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6774 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/architectures/wgan_gp/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14820 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/averaged_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/common/
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/common/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/common/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6137 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/common/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3728 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/common/sampling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/diffusions/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/diffusions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36748 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/diffusions/base_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/diffusions/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/diffusions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26508 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/base_gan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6593 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/biggan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/dcgan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11049 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/gan_data_processer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/ggan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/lsgan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8986 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/mspie_stylegan2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18839 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/progressive_growing_unconditional_gan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7022 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/sagan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26765 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/singan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6530 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/stylegan1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14355 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/stylegan2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/stylegan3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/gans/wgan_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22613 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/ddpm_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21277 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/disc_auxiliary_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/gan_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21849 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/gen_auxiliary_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27860 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/pixelwise_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/losses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/models/translation_models/
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/translation_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/translation_models/base_translation_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11012 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/translation_models/cyclegan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8884 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/translation_models/pix2pix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/models/translation_models/static_translation_gan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/ops/
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10449 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/conv2d_gradfix.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6725 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/custom_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10305 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/bias_act.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14178 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/filtered_lrelu.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16682 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4670 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/structures/
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6684 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/structures/gen_data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/utils/dist_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen/visualization/
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12164 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/visualization/gen_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/visualization/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16683 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/mmgen/visualization/vis_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14201 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6373 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/mmgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-01 03:09:44.000000 mmgen-1.0.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7324 2022-09-01 03:09:07.000000 mmgen-1.0.0rc0/setup.py
```

### Comparing `mmgen-0.7.3/PKG-INFO` & `mmgen-1.0.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmgen
-Version: 0.7.3
+Version: 1.0.0rc0
 Summary: MMGeneration
 Home-page: https://github.com/open-mmlab/mmgen
 Author: MMGeneration Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
             <img src="https://user-images.githubusercontent.com/12726765/114528756-de55af80-9c7b-11eb-94d7-d3224ada1585.png" width="400"/>
@@ -24,58 +24,44 @@
                </a>
              </sup>
            </div>
            <div>&nbsp;</div>
         </div>
         
         [![PyPI](https://img.shields.io/pypi/v/mmgen)](https://pypi.org/project/mmgen)
-        [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmgeneration.readthedocs.io/en/latest/)
+        [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmgeneration.readthedocs.io/en/1.x/)
         [![badge](https://github.com/open-mmlab/mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/mmgeneration/actions)
-        [![codecov](https://codecov.io/gh/open-mmlab/mmgeneration/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmgeneration)
-        [![license](https://img.shields.io/github/license/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/master/LICENSE)
+        [![codecov](https://codecov.io/gh/open-mmlab/mmgeneration/branch/1.x/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmgeneration)
+        [![license](https://img.shields.io/github/license/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/1.x/LICENSE)
         [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
         [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
         
-        [📘Documentation](https://mmgeneration.readthedocs.io/en/latest/) |
-        [🛠️Installation](https://mmgeneration.readthedocs.io/en/latest/get_started.html#installation) |
-        [👀Model Zoo](https://mmgeneration.readthedocs.io/en/latest/modelzoo_statistics.html) |
-        [🆕Update News](https://github.com/open-mmlab/mmgeneration/blob/master/docs/en/changelog.md) |
+        [📘Documentation](https://mmgeneration.readthedocs.io/en/1.x/) |
+        [🛠️Installation](https://mmgeneration.readthedocs.io/en/1.x/get_started.html#installation) |
+        [👀Model Zoo](https://mmgeneration.readthedocs.io/en/1.x/modelzoo_statistics.html) |
+        [🆕Update News](https://github.com/open-mmlab/mmgeneration/blob/1.x/docs/en/notes/changelog.md) |
         [🚀Ongoing Projects](https://github.com/open-mmlab/mmgeneration/projects) |
         [🤔Reporting Issues](https://github.com/open-mmlab/mmgeneration/issues)
         
         English | [简体中文](README_zh-CN.md)
         
-        ## What's New
-        
-        MMGeneration has been merged in [MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x). And we have supported new generation tasks and models. We highlight the following new features:
-        
-        - 🌟 Text2Image
-        
-          - ✅ [GLIDE](https://github.com/open-mmlab/mmediting/tree/1.x/projects/glide/configs/README.md)
-          - ✅ [Disco-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/disco_diffusion/README.md)
-          - ✅ [Stable-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/stable_diffusion/README.md)
-        
-        - 🌟 3D-aware Generation
-        
-          - ✅ [EG3D](https://github.com/open-mmlab/mmediting/tree/1.x/configs/eg3d/README.md)
-        
         ## Introduction
         
-        MMGeneration is a powerful toolkit for generative models, especially for GANs now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv). The master branch works with **PyTorch 1.5+**.
+        MMGeneration is a powerful toolkit for generative models, especially for GANs now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x). The master branch works with **PyTorch 1.5+**.
         
         <div align="center">
             <img src="https://user-images.githubusercontent.com/12726765/114534478-9a65a900-9c81-11eb-8087-de8b6816eed8.png" width="800"/>
         </div>
         
         ## Major Features
         
-        - **High-quality Training Performance:** We currently support training on Unconditional GANs, Internal GANs, and Image Translation Models. Support for conditional models will come soon.
-        - **Powerful Application Toolkit:** A plentiful toolkit containing multiple applications in GANs is provided to users. GAN interpolation, GAN projection, and GAN manipulations are integrated into our framework. It's time to play with your GANs! ([Tutorial for applications](docs/en/tutorials/applications.md))
-        - **Efficient Distributed Training for Generative Models:** For the highly dynamic training in generative models, we adopt a new way to train dynamic models with `MMDDP`. ([Tutorial for DDP](docs/en/tutorials/ddp_train_gans.md))
-        - **New Modular Design for Flexible Combination:** A new design for complex loss modules is proposed for customizing the links between modules, which can achieve flexible combination among different modules. ([Tutorial for new modular design](docs/en/tutorials/customize_losses.md))
+        - **High-quality Training Performance:** MMGeneration currently support training on Unconditional GANs, Conditional GANs, Internal GANs, Image Translation Models, and Diffusion Models.
+        - **Powerful Application Toolkit:** A toolkit that provides plentiful applications to users. MMGeneration supports GAN interpolation, GAN projection, GAN manipulations and many other popular GAN's applications. It's time to play with your GANs! ([Tutorial for applications](docs/en/advanced_guides/applications.md))
+        - **Efficient Distributed Training for Generative Models:** With support of [MMSeparateDistributedDataParallel](https://github.com/open-mmlab/mmengine/blob/main/mmengine/model/wrappers/seperate_distributed.py), distributed training for dynamic architectures can be easily implemented.
+        - **New Modular Design for Flexible Combination:** A new design for complex loss modules is proposed for customizing the links between modules, which can achieve flexible combination among different modules.(Tutorial for [losses](docs/en/advanced_guides/losses.md))
         
         <table>
         <thead>
           <tr>
             <td>
         <div align="center">
           <b> Training Visualization</b>
@@ -106,53 +92,63 @@
         
         ## Highlight
         
         - **Positional Encoding as Spatial Inductive Bias in GANs (CVPR2021)** has been released in `MMGeneration`.  [\[Config\]](configs/positional_encoding_in_gans/README.md), [\[Project Page\]](https://nbei.github.io/gan-pos-encoding.html)
         - Conditional GANs have been supported in our toolkit. More methods and pre-trained weights will come soon.
         - Mixed-precision training (FP16) for StyleGAN2 has been supported. Please check [the comparison](configs/styleganv2/README.md) between different implementations.
         
-        ## Changelog
+        ## What's new
+        
+        v1.0.0rc0 was released in 31/8/2022.
+        
+        This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
+        to try according to [the documentation](https://mmgeneration.readthedocs.io/en/1.x/).
         
-        v0.7.3 was released on 14/04/2023. Please refer to [changelog.md](docs/en/changelog.md) for details and release history.
+        And there are some BC-breaking changes. Please check [the migration tutorial](https://mmgeneration.readthedocs.io/en/1.x/migration.html).
+        
+        The release candidate will last until the end of 2022, and during the release candidate, we will develop on the `1.x` branch. And we will still maintain 0.x version still at least the end of 2023.
+        
+        Please refer to [changelog.md](https://mmgeneration.readthedocs.io/en/1.x/notes/changelog.html) for more details and other release history.
         
         ## Installation
         
-        MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv).
+        MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x).
         Below are quick steps for installation.
         
         **Step 1.**
         Install PyTorch following [official instructions](https://pytorch.org/get-started/locally/), e.g.
         
         ```python
         pip3 install torch torchvision
         
         ```
         
         **Step 2.**
         Install MMCV with [MIM](https://github.com/open-mmlab/mim).
         
         ```
-        pip3 install openmim
-        mim install mmcv-full
+        pip install -U openmim
+        # wait for more pre-compiled pkgs to release
+        mim install 'mmcv>=2.0.0rc1'
         ```
         
         **Step 3.**
         Install MMGeneration from source.
         
         ```
-        git clone https://github.com/open-mmlab/mmgeneration.git
+        git clone -b 1.x https://github.com/open-mmlab/mmgeneration.git
         cd mmgeneration
-        pip3 install -e .
+        pip3 install -e .[all]
         ```
         
         Please refer to [get_started.md](docs/en/get_started.md) for more detailed instruction.
         
         ## Getting Started
         
-        Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration. [docs/en/quick_run.md](docs/en/quick_run.md) can offer full guidance for quick run. For other details and tutorials, please go to our [documentation](https://mmgeneration.readthedocs.io/).
+        Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration. For other details and tutorials, please go to our [documentation](https://mmgeneration.readthedocs.io/en/1.x/).
         
         ## ModelZoo
         
         These methods have been carefully studied and supported in our frameworks:
         
         <details open>
         <summary>Unconditional GANs (click to collapse)</summary>
@@ -176,21 +172,14 @@
         - ✅ [Projection GAN](configs/sngan_proj/README.md) (ICLR'2018)
         - ✅ [SAGAN](configs/sagan/README.md) (ICML'2019)
         - ✅ [BIGGAN/BIGGAN-DEEP](configs/biggan/README.md) (ICLR'2019)
         
         </details>
         
         <details open>
-        <summary>Tricks for GANs (click to collapse)</summary>
-        
-        - ✅ [ADA](configs/ada/README.md) (NeurIPS'2020)
-        
-        </details>
-        
-        <details open>
         <summary>Image2Image Translation (click to collapse)</summary>
         
         - ✅ [Pix2Pix](configs/pix2pix/README.md) (CVPR'2017)
         - ✅ [CycleGAN](configs/cyclegan/README.md) (ICCV'2017)
         
         </details>
         
@@ -210,15 +199,15 @@
         
         ## Related-Applications
         
         - ✅ [MMGEN-FaceStylor](https://github.com/open-mmlab/MMGEN-FaceStylor)
         
         ## Contributing
         
-        We appreciate all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/blob/master/CONTRIBUTING.md) in MMCV for more details about the contributing guideline.
+        We appreciate all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/tree/2.x/CONTRIBUTING.md) in MMCV and \[https://github.com/open-mmlab/mmengine/blob/main/CONTRIBUTING.md\] in MMEngine for more details about the contributing guideline.
         
         ## Citation
         
         If you find this project useful in your research, please consider cite:
         
         ```BibTeX
         @misc{2021mmgeneration,
@@ -229,34 +218,35 @@
         }
         ```
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE). Some operations in `MMGeneration` are with other licenses instead of Apache2.0. Please refer to [LICENSES.md](LICENSES.md) for the careful check, if you are using our code for commercial matters.
         
-        ## Projects in OpenMMLab
+        ## Projects in OpenMMLab 2.0
         
-        - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+        - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+        - [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x): OpenMMLab foundational library for computer vision.
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-        - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
-        - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-        - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-        - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-        - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-        - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-        - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+        - [MMClassification](https://github.com/open-mmlab/mmclassification/tree/1.x): OpenMMLab image classification toolbox and benchmark.
+        - [MMDetection](https://github.com/open-mmlab/mmdetection/tree/3.x): OpenMMLab detection toolbox and benchmark.
+        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d/tree/1.x): OpenMMLab's next-generation platform for general 3D object detection.
+        - [MMRotate](https://github.com/open-mmlab/mmrotate/tree/1.x): OpenMMLab rotated object detection toolbox and benchmark.
+        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation/tree/1.x): OpenMMLab semantic segmentation toolbox and benchmark.
+        - [MMOCR](https://github.com/open-mmlab/mmocr/tree/1.x): OpenMMLab text detection, recognition, and understanding toolbox.
+        - [MMPose](https://github.com/open-mmlab/mmpose/tree/1.x): OpenMMLab pose estimation toolbox and benchmark.
+        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d/tree/1.x): OpenMMLab 3D human parametric model toolbox and benchmark.
+        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup/tree/1.x): OpenMMLab self-supervised learning toolbox and benchmark.
+        - [MMRazor](https://github.com/open-mmlab/mmrazor/tree/1.x): OpenMMLab model compression toolbox and benchmark.
+        - [MMFewShot](https://github.com/open-mmlab/mmfewshot/tree/1.x): OpenMMLab fewshot learning toolbox and benchmark.
+        - [MMAction2](https://github.com/open-mmlab/mmaction2/tree/1.x): OpenMMLab's next-generation action understanding toolbox and benchmark.
+        - [MMTracking](https://github.com/open-mmlab/mmtracking/tree/1.x): OpenMMLab video perception toolbox and benchmark.
+        - [MMFlow](https://github.com/open-mmlab/mmflow/tree/1.x): OpenMMLab optical flow toolbox and benchmark.
+        - [MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x): OpenMMLab image and video editing toolbox.
+        - [MMGeneration](https://github.com/open-mmlab/mmgeneration/tree/1.x): OpenMMLab image and video generative models toolbox.
         - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,149 +1,152 @@
-Metadata-Version: 2.1 Name: mmgen Version: 0.7.3 Summary: MMGeneration Home-
+Metadata-Version: 2.1 Name: mmgen Version: 1.0.0rc0 Summary: MMGeneration Home-
 page: https://github.com/open-mmlab/mmgen Author: MMGeneration Contributors
 Author-email: openmmlab@gmail.com License: Apache License 2.0 Description:
  [https://user-images.githubusercontent.com/12726765/114528756-de55af80-9c7b-
                           11eb-94d7-d3224ada1585.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
 [![PyPI](https://img.shields.io/pypi/v/mmgen)](https://pypi.org/project/mmgen)
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
-mmgeneration.readthedocs.io/en/latest/) [![badge](https://github.com/open-
-mmlab/mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/
+mmgeneration.readthedocs.io/en/1.x/) [![badge](https://github.com/open-mmlab/
+mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/
 mmgeneration/actions) [![codecov](https://codecov.io/gh/open-mmlab/
-mmgeneration/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
+mmgeneration/branch/1.x/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
 mmgeneration) [![license](https://img.shields.io/github/license/open-mmlab/
-mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/master/
-LICENSE) [![open issues](https://isitmaintained.com/badge/open/open-mmlab/
+mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/1.x/LICENSE)
+[![open issues](https://isitmaintained.com/badge/open/open-mmlab/
 mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues) [![issue
 resolution](https://isitmaintained.com/badge/resolution/open-mmlab/
 mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
-[ðDocumentation](https://mmgeneration.readthedocs.io/en/latest/) |
-[ð ï¸Installation](https://mmgeneration.readthedocs.io/en/latest/
+[ðDocumentation](https://mmgeneration.readthedocs.io/en/1.x/) |
+[ð ï¸Installation](https://mmgeneration.readthedocs.io/en/1.x/
 get_started.html#installation) | [ðModel Zoo](https://
-mmgeneration.readthedocs.io/en/latest/modelzoo_statistics.html) | [ðUpdate
-News](https://github.com/open-mmlab/mmgeneration/blob/master/docs/en/
+mmgeneration.readthedocs.io/en/1.x/modelzoo_statistics.html) | [ðUpdate
+News](https://github.com/open-mmlab/mmgeneration/blob/1.x/docs/en/notes/
 changelog.md) | [ðOngoing Projects](https://github.com/open-mmlab/
 mmgeneration/projects) | [ð¤Reporting Issues](https://github.com/open-mmlab/
-mmgeneration/issues) English | [ç®ä½ä¸­æ](README_zh-CN.md) ## What's New
-MMGeneration has been merged in [MMEditing](https://github.com/open-mmlab/
-mmediting/tree/1.x). And we have supported new generation tasks and models. We
-highlight the following new features: - ð Text2Image - â [GLIDE](https://
-github.com/open-mmlab/mmediting/tree/1.x/projects/glide/configs/README.md) -
-â [Disco-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/
-disco_diffusion/README.md) - â [Stable-Diffusion](https://github.com/open-
-mmlab/mmediting/tree/1.x/configs/stable_diffusion/README.md) - ð 3D-aware
-Generation - â [EG3D](https://github.com/open-mmlab/mmediting/tree/1.x/
-configs/eg3d/README.md) ## Introduction MMGeneration is a powerful toolkit for
-generative models, especially for GANs now. It is based on PyTorch and [MMCV]
-(https://github.com/open-mmlab/mmcv). The master branch works with **PyTorch
-1.5+**.
+mmgeneration/issues) English | [ç®ä½ä¸­æ](README_zh-CN.md) ## Introduction
+MMGeneration is a powerful toolkit for generative models, especially for GANs
+now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv/tree/
+2.x). The master branch works with **PyTorch 1.5+**.
  [https://user-images.githubusercontent.com/12726765/114534478-9a65a900-9c81-
                           11eb-8087-de8b6816eed8.png]
-## Major Features - **High-quality Training Performance:** We currently support
-training on Unconditional GANs, Internal GANs, and Image Translation Models.
-Support for conditional models will come soon. - **Powerful Application
-Toolkit:** A plentiful toolkit containing multiple applications in GANs is
-provided to users. GAN interpolation, GAN projection, and GAN manipulations are
-integrated into our framework. It's time to play with your GANs! ([Tutorial for
-applications](docs/en/tutorials/applications.md)) - **Efficient Distributed
-Training for Generative Models:** For the highly dynamic training in generative
-models, we adopt a new way to train dynamic models with `MMDDP`. ([Tutorial for
-DDP](docs/en/tutorials/ddp_train_gans.md)) - **New Modular Design for Flexible
-Combination:** A new design for complex loss modules is proposed for
-customizing the links between modules, which can achieve flexible combination
-among different modules. ([Tutorial for new modular design](docs/en/tutorials/
-customize_losses.md))
+## Major Features - **High-quality Training Performance:** MMGeneration
+currently support training on Unconditional GANs, Conditional GANs, Internal
+GANs, Image Translation Models, and Diffusion Models. - **Powerful Application
+Toolkit:** A toolkit that provides plentiful applications to users.
+MMGeneration supports GAN interpolation, GAN projection, GAN manipulations and
+many other popular GAN's applications. It's time to play with your GANs! (
+[Tutorial for applications](docs/en/advanced_guides/applications.md)) -
+**Efficient Distributed Training for Generative Models:** With support of
+[MMSeparateDistributedDataParallel](https://github.com/open-mmlab/mmengine/
+blob/main/mmengine/model/wrappers/seperate_distributed.py), distributed
+training for dynamic architectures can be easily implemented. - **New Modular
+Design for Flexible Combination:** A new design for complex loss modules is
+proposed for customizing the links between modules, which can achieve flexible
+combination among different modules.(Tutorial for [losses](docs/en/
+advanced_guides/losses.md))
    Training Visualization          GAN Interpolation               GAN Projector                GAN Manipulation
        [https://user-                [https://user-                [https://user-                [https://user-
 images.githubusercontent.com/ images.githubusercontent.com/ images.githubusercontent.com/ images.githubusercontent.com/
 12726765/114509105-b6f4e780-  12726765/114679300-9fd4f900-  12726765/114524392-c11ee200-  12726765/114523716-20302700-
        9c67-11eb-8644-               9d3e-11eb-8f37-               9c77-11eb-8b6d-               9c77-11eb-804e-
       110b3cb01314.gif]             c36a018c02f7.gif]             37bc637f5626.gif]             327ae1ca0c5b.gif]
 ## Highlight - **Positional Encoding as Spatial Inductive Bias in GANs
 (CVPR2021)** has been released in `MMGeneration`. [\[Config\]](configs/
 positional_encoding_in_gans/README.md), [\[Project Page\]](https://
 nbei.github.io/gan-pos-encoding.html) - Conditional GANs have been supported in
 our toolkit. More methods and pre-trained weights will come soon. - Mixed-
 precision training (FP16) for StyleGAN2 has been supported. Please check [the
 comparison](configs/styleganv2/README.md) between different implementations. ##
-Changelog v0.7.3 was released on 14/04/2023. Please refer to [changelog.md]
-(docs/en/changelog.md) for details and release history. ## Installation
-MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://
-github.com/open-mmlab/mmcv). Below are quick steps for installation. **Step
-1.** Install PyTorch following [official instructions](https://pytorch.org/get-
-started/locally/), e.g. ```python pip3 install torch torchvision ``` **Step
-2.** Install MMCV with [MIM](https://github.com/open-mmlab/mim). ``` pip3
-install openmim mim install mmcv-full ``` **Step 3.** Install MMGeneration from
-source. ``` git clone https://github.com/open-mmlab/mmgeneration.git cd
-mmgeneration pip3 install -e . ``` Please refer to [get_started.md](docs/en/
-get_started.md) for more detailed instruction. ## Getting Started Please see
-[get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration.
-[docs/en/quick_run.md](docs/en/quick_run.md) can offer full guidance for quick
-run. For other details and tutorials, please go to our [documentation](https://
-mmgeneration.readthedocs.io/). ## ModelZoo These methods have been carefully
-studied and supported in our frameworks:  Unconditional GANs (click to
-collapse) - â [DCGAN](configs/dcgan/README.md) (ICLR'2016) - â [WGAN-GP]
-(configs/wgan-gp/README.md) (NIPS'2017) - â [LSGAN](configs/lsgan/README.md)
-(ICCV'2017) - â [GGAN](configs/ggan/README.md) (arXiv'2017) - â [PGGAN]
-(configs/pggan/README.md) (ICLR'2018) - â [StyleGANV1](configs/styleganv1/
-README.md) (CVPR'2019) - â [StyleGANV2](configs/styleganv2/README.md)
-(CVPR'2020) - â [StyleGANV3](configs/styleganv3/README.md) (NeurIPS'2021) -
-â [Positional Encoding in GANs](configs/positional_encoding_in_gans/
-README.md) (CVPR'2021)   Conditional GANs (click to collapse) - â [SNGAN]
-(configs/sngan_proj/README.md) (ICLR'2018) - â [Projection GAN](configs/
-sngan_proj/README.md) (ICLR'2018) - â [SAGAN](configs/sagan/README.md)
-(ICML'2019) - â [BIGGAN/BIGGAN-DEEP](configs/biggan/README.md) (ICLR'2019)
-Tricks for GANs (click to collapse) - â [ADA](configs/ada/README.md)
-(NeurIPS'2020)   Image2Image Translation (click to collapse) - â [Pix2Pix]
-(configs/pix2pix/README.md) (CVPR'2017) - â [CycleGAN](configs/cyclegan/
-README.md) (ICCV'2017)   Internal Learning (click to collapse) - â [SinGAN]
-(configs/singan/README.md) (ICCV'2019)   Denoising Diffusion Probabilistic
-Models (click to collapse) - â [Improved DDPM](configs/improved_ddpm/
-README.md) (arXiv'2021)  ## Related-Applications - â [MMGEN-FaceStylor]
-(https://github.com/open-mmlab/MMGEN-FaceStylor) ## Contributing We appreciate
-all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md]
-(https://github.com/open-mmlab/mmcv/blob/master/CONTRIBUTING.md) in MMCV for
-more details about the contributing guideline. ## Citation If you find this
-project useful in your research, please consider cite: ```BibTeX @misc
-{2021mmgeneration, title={{MMGeneration}: OpenMMLab Generative Model Toolbox
-and Benchmark}, author={MMGeneration Contributors}, howpublished = {\url{https:
-//github.com/open-mmlab/mmgeneration}}, year={2021} } ``` ## License This
-project is released under the [Apache 2.0 license](LICENSE). Some operations in
-`MMGeneration` are with other licenses instead of Apache2.0. Please refer to
-[LICENSES.md](LICENSES.md) for the careful check, if you are using our code for
-commercial matters. ## Projects in OpenMMLab - [MMCV](https://github.com/open-
-mmlab/mmcv): OpenMMLab foundational library for computer vision. - [MIM](https:
-//github.com/open-mmlab/mim): MIM installs OpenMMLab packages. -
-[MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab
-image classification toolbox and benchmark. - [MMDetection](https://github.com/
-open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark. -
-[MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-
-generation platform for general 3D object detection. - [MMRotate](https://
-github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and
-benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
-OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR](https://
-github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and
-understanding toolbox. - [MMPose](https://github.com/open-mmlab/mmpose):
-OpenMMLab pose estimation toolbox and benchmark. - [MMHuman3D](https://
-github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox
-and benchmark. - [MMSelfSup](https://github.com/open-mmlab/mmselfsup):
-OpenMMLab self-supervised learning toolbox and benchmark. - [MMRazor](https://
-github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and
-benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab
-fewshot learning toolbox and benchmark. - [MMAction2](https://github.com/open-
-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and
-benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
+What's new v1.0.0rc0 was released in 31/8/2022. This release introduced a brand
+new and flexible training & test engine, but it's still in progress. Welcome to
+try according to [the documentation](https://mmgeneration.readthedocs.io/en/
+1.x/). And there are some BC-breaking changes. Please check [the migration
+tutorial](https://mmgeneration.readthedocs.io/en/1.x/migration.html). The
+release candidate will last until the end of 2022, and during the release
+candidate, we will develop on the `1.x` branch. And we will still maintain 0.x
+version still at least the end of 2023. Please refer to [changelog.md](https://
+mmgeneration.readthedocs.io/en/1.x/notes/changelog.html) for more details and
+other release history. ## Installation MMGeneration depends on [PyTorch](https:
+//pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x). Below
+are quick steps for installation. **Step 1.** Install PyTorch following
+[official instructions](https://pytorch.org/get-started/locally/), e.g.
+```python pip3 install torch torchvision ``` **Step 2.** Install MMCV with
+[MIM](https://github.com/open-mmlab/mim). ``` pip install -U openmim # wait for
+more pre-compiled pkgs to release mim install 'mmcv>=2.0.0rc1' ``` **Step 3.**
+Install MMGeneration from source. ``` git clone -b 1.x https://github.com/open-
+mmlab/mmgeneration.git cd mmgeneration pip3 install -e .[all] ``` Please refer
+to [get_started.md](docs/en/get_started.md) for more detailed instruction. ##
+Getting Started Please see [get_started.md](docs/en/get_started.md) for the
+basic usage of MMGeneration. For other details and tutorials, please go to our
+[documentation](https://mmgeneration.readthedocs.io/en/1.x/). ## ModelZoo These
+methods have been carefully studied and supported in our frameworks:
+Unconditional GANs (click to collapse) - â [DCGAN](configs/dcgan/README.md)
+(ICLR'2016) - â [WGAN-GP](configs/wgan-gp/README.md) (NIPS'2017) - â
+[LSGAN](configs/lsgan/README.md) (ICCV'2017) - â [GGAN](configs/ggan/
+README.md) (arXiv'2017) - â [PGGAN](configs/pggan/README.md) (ICLR'2018) -
+â [StyleGANV1](configs/styleganv1/README.md) (CVPR'2019) - â [StyleGANV2]
+(configs/styleganv2/README.md) (CVPR'2020) - â [StyleGANV3](configs/
+styleganv3/README.md) (NeurIPS'2021) - â [Positional Encoding in GANs]
+(configs/positional_encoding_in_gans/README.md) (CVPR'2021)   Conditional GANs
+(click to collapse) - â [SNGAN](configs/sngan_proj/README.md) (ICLR'2018) -
+â [Projection GAN](configs/sngan_proj/README.md) (ICLR'2018) - â [SAGAN]
+(configs/sagan/README.md) (ICML'2019) - â [BIGGAN/BIGGAN-DEEP](configs/
+biggan/README.md) (ICLR'2019)   Image2Image Translation (click to collapse) -
+â [Pix2Pix](configs/pix2pix/README.md) (CVPR'2017) - â [CycleGAN](configs/
+cyclegan/README.md) (ICCV'2017)   Internal Learning (click to collapse) - â
+[SinGAN](configs/singan/README.md) (ICCV'2019)   Denoising Diffusion
+Probabilistic Models (click to collapse) - â [Improved DDPM](configs/
+improved_ddpm/README.md) (arXiv'2021)  ## Related-Applications - â [MMGEN-
+FaceStylor](https://github.com/open-mmlab/MMGEN-FaceStylor) ## Contributing We
+appreciate all contributions to improve MMGeneration. Please refer to
+[CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/tree/2.x/CONTRIBUTING.md)
+in MMCV and \[https://github.com/open-mmlab/mmengine/blob/main/
+CONTRIBUTING.md\] in MMEngine for more details about the contributing
+guideline. ## Citation If you find this project useful in your research, please
+consider cite: ```BibTeX @misc{2021mmgeneration, title={{MMGeneration}:
+OpenMMLab Generative Model Toolbox and Benchmark}, author={MMGeneration
+Contributors}, howpublished = {\url{https://github.com/open-mmlab/
+mmgeneration}}, year={2021} } ``` ## License This project is released under the
+[Apache 2.0 license](LICENSE). Some operations in `MMGeneration` are with other
+licenses instead of Apache2.0. Please refer to [LICENSES.md](LICENSES.md) for
+the careful check, if you are using our code for commercial matters. ##
+Projects in OpenMMLab 2.0 - [MMEngine](https://github.com/open-mmlab/mmengine):
+OpenMMLab foundational library for training deep learning models. - [MMCV]
+(https://github.com/open-mmlab/mmcv/tree/2.x): OpenMMLab foundational library
+for computer vision. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [MMClassification](https://github.com/open-mmlab/
+mmclassification/tree/1.x): OpenMMLab image classification toolbox and
+benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection/tree/3.x):
+OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d/tree/1.x): OpenMMLab's next-generation
+platform for general 3D object detection. - [MMRotate](https://github.com/open-
+mmlab/mmrotate/tree/1.x): OpenMMLab rotated object detection toolbox and
+benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation/
+tree/1.x): OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR]
+(https://github.com/open-mmlab/mmocr/tree/1.x): OpenMMLab text detection,
+recognition, and understanding toolbox. - [MMPose](https://github.com/open-
+mmlab/mmpose/tree/1.x): OpenMMLab pose estimation toolbox and benchmark. -
+[MMHuman3D](https://github.com/open-mmlab/mmhuman3d/tree/1.x): OpenMMLab 3D
+human parametric model toolbox and benchmark. - [MMSelfSup](https://github.com/
+open-mmlab/mmselfsup/tree/1.x): OpenMMLab self-supervised learning toolbox and
+benchmark. - [MMRazor](https://github.com/open-mmlab/mmrazor/tree/1.x):
+OpenMMLab model compression toolbox and benchmark. - [MMFewShot](https://
+github.com/open-mmlab/mmfewshot/tree/1.x): OpenMMLab fewshot learning toolbox
+and benchmark. - [MMAction2](https://github.com/open-mmlab/mmaction2/tree/1.x):
+OpenMMLab's next-generation action understanding toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking/tree/1.x): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMEditing]
-(https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing
-toolbox. - [MMGeneration](https://github.com/open-mmlab/mmgeneration):
-OpenMMLab image and video generative models toolbox. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
-Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: tests Provides-Extra: mim
+mmlab/mmflow/tree/1.x): OpenMMLab optical flow toolbox and benchmark. -
+[MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x): OpenMMLab image
+and video editing toolbox. - [MMGeneration](https://github.com/open-mmlab/
+mmgeneration/tree/1.x): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown Provides-Extra: all Provides-Extra: tests Provides-Extra: mim
```

### Comparing `mmgen-0.7.3/README.md` & `mmgen-1.0.0rc0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,58 +16,44 @@
        </a>
      </sup>
    </div>
    <div>&nbsp;</div>
 </div>
 
 [![PyPI](https://img.shields.io/pypi/v/mmgen)](https://pypi.org/project/mmgen)
-[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmgeneration.readthedocs.io/en/latest/)
+[![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmgeneration.readthedocs.io/en/1.x/)
 [![badge](https://github.com/open-mmlab/mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/mmgeneration/actions)
-[![codecov](https://codecov.io/gh/open-mmlab/mmgeneration/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmgeneration)
-[![license](https://img.shields.io/github/license/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/master/LICENSE)
+[![codecov](https://codecov.io/gh/open-mmlab/mmgeneration/branch/1.x/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmgeneration)
+[![license](https://img.shields.io/github/license/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/1.x/LICENSE)
 [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
 [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
 
-[📘Documentation](https://mmgeneration.readthedocs.io/en/latest/) |
-[🛠️Installation](https://mmgeneration.readthedocs.io/en/latest/get_started.html#installation) |
-[👀Model Zoo](https://mmgeneration.readthedocs.io/en/latest/modelzoo_statistics.html) |
-[🆕Update News](https://github.com/open-mmlab/mmgeneration/blob/master/docs/en/changelog.md) |
+[📘Documentation](https://mmgeneration.readthedocs.io/en/1.x/) |
+[🛠️Installation](https://mmgeneration.readthedocs.io/en/1.x/get_started.html#installation) |
+[👀Model Zoo](https://mmgeneration.readthedocs.io/en/1.x/modelzoo_statistics.html) |
+[🆕Update News](https://github.com/open-mmlab/mmgeneration/blob/1.x/docs/en/notes/changelog.md) |
 [🚀Ongoing Projects](https://github.com/open-mmlab/mmgeneration/projects) |
 [🤔Reporting Issues](https://github.com/open-mmlab/mmgeneration/issues)
 
 English | [简体中文](README_zh-CN.md)
 
-## What's New
-
-MMGeneration has been merged in [MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x). And we have supported new generation tasks and models. We highlight the following new features:
-
-- 🌟 Text2Image
-
-  - ✅ [GLIDE](https://github.com/open-mmlab/mmediting/tree/1.x/projects/glide/configs/README.md)
-  - ✅ [Disco-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/disco_diffusion/README.md)
-  - ✅ [Stable-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/stable_diffusion/README.md)
-
-- 🌟 3D-aware Generation
-
-  - ✅ [EG3D](https://github.com/open-mmlab/mmediting/tree/1.x/configs/eg3d/README.md)
-
 ## Introduction
 
-MMGeneration is a powerful toolkit for generative models, especially for GANs now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv). The master branch works with **PyTorch 1.5+**.
+MMGeneration is a powerful toolkit for generative models, especially for GANs now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x). The master branch works with **PyTorch 1.5+**.
 
 <div align="center">
     <img src="https://user-images.githubusercontent.com/12726765/114534478-9a65a900-9c81-11eb-8087-de8b6816eed8.png" width="800"/>
 </div>
 
 ## Major Features
 
-- **High-quality Training Performance:** We currently support training on Unconditional GANs, Internal GANs, and Image Translation Models. Support for conditional models will come soon.
-- **Powerful Application Toolkit:** A plentiful toolkit containing multiple applications in GANs is provided to users. GAN interpolation, GAN projection, and GAN manipulations are integrated into our framework. It's time to play with your GANs! ([Tutorial for applications](docs/en/tutorials/applications.md))
-- **Efficient Distributed Training for Generative Models:** For the highly dynamic training in generative models, we adopt a new way to train dynamic models with `MMDDP`. ([Tutorial for DDP](docs/en/tutorials/ddp_train_gans.md))
-- **New Modular Design for Flexible Combination:** A new design for complex loss modules is proposed for customizing the links between modules, which can achieve flexible combination among different modules. ([Tutorial for new modular design](docs/en/tutorials/customize_losses.md))
+- **High-quality Training Performance:** MMGeneration currently support training on Unconditional GANs, Conditional GANs, Internal GANs, Image Translation Models, and Diffusion Models.
+- **Powerful Application Toolkit:** A toolkit that provides plentiful applications to users. MMGeneration supports GAN interpolation, GAN projection, GAN manipulations and many other popular GAN's applications. It's time to play with your GANs! ([Tutorial for applications](docs/en/advanced_guides/applications.md))
+- **Efficient Distributed Training for Generative Models:** With support of [MMSeparateDistributedDataParallel](https://github.com/open-mmlab/mmengine/blob/main/mmengine/model/wrappers/seperate_distributed.py), distributed training for dynamic architectures can be easily implemented.
+- **New Modular Design for Flexible Combination:** A new design for complex loss modules is proposed for customizing the links between modules, which can achieve flexible combination among different modules.(Tutorial for [losses](docs/en/advanced_guides/losses.md))
 
 <table>
 <thead>
   <tr>
     <td>
 <div align="center">
   <b> Training Visualization</b>
@@ -98,53 +84,63 @@
 
 ## Highlight
 
 - **Positional Encoding as Spatial Inductive Bias in GANs (CVPR2021)** has been released in `MMGeneration`.  [\[Config\]](configs/positional_encoding_in_gans/README.md), [\[Project Page\]](https://nbei.github.io/gan-pos-encoding.html)
 - Conditional GANs have been supported in our toolkit. More methods and pre-trained weights will come soon.
 - Mixed-precision training (FP16) for StyleGAN2 has been supported. Please check [the comparison](configs/styleganv2/README.md) between different implementations.
 
-## Changelog
+## What's new
+
+v1.0.0rc0 was released in 31/8/2022.
+
+This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
+to try according to [the documentation](https://mmgeneration.readthedocs.io/en/1.x/).
 
-v0.7.3 was released on 14/04/2023. Please refer to [changelog.md](docs/en/changelog.md) for details and release history.
+And there are some BC-breaking changes. Please check [the migration tutorial](https://mmgeneration.readthedocs.io/en/1.x/migration.html).
+
+The release candidate will last until the end of 2022, and during the release candidate, we will develop on the `1.x` branch. And we will still maintain 0.x version still at least the end of 2023.
+
+Please refer to [changelog.md](https://mmgeneration.readthedocs.io/en/1.x/notes/changelog.html) for more details and other release history.
 
 ## Installation
 
-MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv).
+MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x).
 Below are quick steps for installation.
 
 **Step 1.**
 Install PyTorch following [official instructions](https://pytorch.org/get-started/locally/), e.g.
 
 ```python
 pip3 install torch torchvision
 
 ```
 
 **Step 2.**
 Install MMCV with [MIM](https://github.com/open-mmlab/mim).
 
 ```
-pip3 install openmim
-mim install mmcv-full
+pip install -U openmim
+# wait for more pre-compiled pkgs to release
+mim install 'mmcv>=2.0.0rc1'
 ```
 
 **Step 3.**
 Install MMGeneration from source.
 
 ```
-git clone https://github.com/open-mmlab/mmgeneration.git
+git clone -b 1.x https://github.com/open-mmlab/mmgeneration.git
 cd mmgeneration
-pip3 install -e .
+pip3 install -e .[all]
 ```
 
 Please refer to [get_started.md](docs/en/get_started.md) for more detailed instruction.
 
 ## Getting Started
 
-Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration. [docs/en/quick_run.md](docs/en/quick_run.md) can offer full guidance for quick run. For other details and tutorials, please go to our [documentation](https://mmgeneration.readthedocs.io/).
+Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration. For other details and tutorials, please go to our [documentation](https://mmgeneration.readthedocs.io/en/1.x/).
 
 ## ModelZoo
 
 These methods have been carefully studied and supported in our frameworks:
 
 <details open>
 <summary>Unconditional GANs (click to collapse)</summary>
@@ -168,21 +164,14 @@
 - ✅ [Projection GAN](configs/sngan_proj/README.md) (ICLR'2018)
 - ✅ [SAGAN](configs/sagan/README.md) (ICML'2019)
 - ✅ [BIGGAN/BIGGAN-DEEP](configs/biggan/README.md) (ICLR'2019)
 
 </details>
 
 <details open>
-<summary>Tricks for GANs (click to collapse)</summary>
-
-- ✅ [ADA](configs/ada/README.md) (NeurIPS'2020)
-
-</details>
-
-<details open>
 <summary>Image2Image Translation (click to collapse)</summary>
 
 - ✅ [Pix2Pix](configs/pix2pix/README.md) (CVPR'2017)
 - ✅ [CycleGAN](configs/cyclegan/README.md) (ICCV'2017)
 
 </details>
 
@@ -202,15 +191,15 @@
 
 ## Related-Applications
 
 - ✅ [MMGEN-FaceStylor](https://github.com/open-mmlab/MMGEN-FaceStylor)
 
 ## Contributing
 
-We appreciate all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/blob/master/CONTRIBUTING.md) in MMCV for more details about the contributing guideline.
+We appreciate all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/tree/2.x/CONTRIBUTING.md) in MMCV and \[https://github.com/open-mmlab/mmengine/blob/main/CONTRIBUTING.md\] in MMEngine for more details about the contributing guideline.
 
 ## Citation
 
 If you find this project useful in your research, please consider cite:
 
 ```BibTeX
 @misc{2021mmgeneration,
@@ -221,28 +210,29 @@
 }
 ```
 
 ## License
 
 This project is released under the [Apache 2.0 license](LICENSE). Some operations in `MMGeneration` are with other licenses instead of Apache2.0. Please refer to [LICENSES.md](LICENSES.md) for the careful check, if you are using our code for commercial matters.
 
-## Projects in OpenMMLab
+## Projects in OpenMMLab 2.0
 
-- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+- [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+- [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x): OpenMMLab foundational library for computer vision.
 - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-- [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
-- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-- [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+- [MMClassification](https://github.com/open-mmlab/mmclassification/tree/1.x): OpenMMLab image classification toolbox and benchmark.
+- [MMDetection](https://github.com/open-mmlab/mmdetection/tree/3.x): OpenMMLab detection toolbox and benchmark.
+- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d/tree/1.x): OpenMMLab's next-generation platform for general 3D object detection.
+- [MMRotate](https://github.com/open-mmlab/mmrotate/tree/1.x): OpenMMLab rotated object detection toolbox and benchmark.
+- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation/tree/1.x): OpenMMLab semantic segmentation toolbox and benchmark.
+- [MMOCR](https://github.com/open-mmlab/mmocr/tree/1.x): OpenMMLab text detection, recognition, and understanding toolbox.
+- [MMPose](https://github.com/open-mmlab/mmpose/tree/1.x): OpenMMLab pose estimation toolbox and benchmark.
+- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d/tree/1.x): OpenMMLab 3D human parametric model toolbox and benchmark.
+- [MMSelfSup](https://github.com/open-mmlab/mmselfsup/tree/1.x): OpenMMLab self-supervised learning toolbox and benchmark.
+- [MMRazor](https://github.com/open-mmlab/mmrazor/tree/1.x): OpenMMLab model compression toolbox and benchmark.
+- [MMFewShot](https://github.com/open-mmlab/mmfewshot/tree/1.x): OpenMMLab fewshot learning toolbox and benchmark.
+- [MMAction2](https://github.com/open-mmlab/mmaction2/tree/1.x): OpenMMLab's next-generation action understanding toolbox and benchmark.
+- [MMTracking](https://github.com/open-mmlab/mmtracking/tree/1.x): OpenMMLab video perception toolbox and benchmark.
+- [MMFlow](https://github.com/open-mmlab/mmflow/tree/1.x): OpenMMLab optical flow toolbox and benchmark.
+- [MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x): OpenMMLab image and video editing toolbox.
+- [MMGeneration](https://github.com/open-mmlab/mmgeneration/tree/1.x): OpenMMLab image and video generative models toolbox.
 - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
```

#### html2text {}

```diff
@@ -1,139 +1,143 @@
  [https://user-images.githubusercontent.com/12726765/114528756-de55af80-9c7b-
                           11eb-94d7-d3224ada1585.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
 [![PyPI](https://img.shields.io/pypi/v/mmgen)](https://pypi.org/project/mmgen)
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
-mmgeneration.readthedocs.io/en/latest/) [![badge](https://github.com/open-
-mmlab/mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/
+mmgeneration.readthedocs.io/en/1.x/) [![badge](https://github.com/open-mmlab/
+mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/
 mmgeneration/actions) [![codecov](https://codecov.io/gh/open-mmlab/
-mmgeneration/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
+mmgeneration/branch/1.x/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
 mmgeneration) [![license](https://img.shields.io/github/license/open-mmlab/
-mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/master/
-LICENSE) [![open issues](https://isitmaintained.com/badge/open/open-mmlab/
+mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/1.x/LICENSE)
+[![open issues](https://isitmaintained.com/badge/open/open-mmlab/
 mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues) [![issue
 resolution](https://isitmaintained.com/badge/resolution/open-mmlab/
 mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
-[ðDocumentation](https://mmgeneration.readthedocs.io/en/latest/) |
-[ð ï¸Installation](https://mmgeneration.readthedocs.io/en/latest/
+[ðDocumentation](https://mmgeneration.readthedocs.io/en/1.x/) |
+[ð ï¸Installation](https://mmgeneration.readthedocs.io/en/1.x/
 get_started.html#installation) | [ðModel Zoo](https://
-mmgeneration.readthedocs.io/en/latest/modelzoo_statistics.html) | [ðUpdate
-News](https://github.com/open-mmlab/mmgeneration/blob/master/docs/en/
+mmgeneration.readthedocs.io/en/1.x/modelzoo_statistics.html) | [ðUpdate
+News](https://github.com/open-mmlab/mmgeneration/blob/1.x/docs/en/notes/
 changelog.md) | [ðOngoing Projects](https://github.com/open-mmlab/
 mmgeneration/projects) | [ð¤Reporting Issues](https://github.com/open-mmlab/
-mmgeneration/issues) English | [ç®ä½ä¸­æ](README_zh-CN.md) ## What's New
-MMGeneration has been merged in [MMEditing](https://github.com/open-mmlab/
-mmediting/tree/1.x). And we have supported new generation tasks and models. We
-highlight the following new features: - ð Text2Image - â [GLIDE](https://
-github.com/open-mmlab/mmediting/tree/1.x/projects/glide/configs/README.md) -
-â [Disco-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/
-disco_diffusion/README.md) - â [Stable-Diffusion](https://github.com/open-
-mmlab/mmediting/tree/1.x/configs/stable_diffusion/README.md) - ð 3D-aware
-Generation - â [EG3D](https://github.com/open-mmlab/mmediting/tree/1.x/
-configs/eg3d/README.md) ## Introduction MMGeneration is a powerful toolkit for
-generative models, especially for GANs now. It is based on PyTorch and [MMCV]
-(https://github.com/open-mmlab/mmcv). The master branch works with **PyTorch
-1.5+**.
+mmgeneration/issues) English | [ç®ä½ä¸­æ](README_zh-CN.md) ## Introduction
+MMGeneration is a powerful toolkit for generative models, especially for GANs
+now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv/tree/
+2.x). The master branch works with **PyTorch 1.5+**.
  [https://user-images.githubusercontent.com/12726765/114534478-9a65a900-9c81-
                           11eb-8087-de8b6816eed8.png]
-## Major Features - **High-quality Training Performance:** We currently support
-training on Unconditional GANs, Internal GANs, and Image Translation Models.
-Support for conditional models will come soon. - **Powerful Application
-Toolkit:** A plentiful toolkit containing multiple applications in GANs is
-provided to users. GAN interpolation, GAN projection, and GAN manipulations are
-integrated into our framework. It's time to play with your GANs! ([Tutorial for
-applications](docs/en/tutorials/applications.md)) - **Efficient Distributed
-Training for Generative Models:** For the highly dynamic training in generative
-models, we adopt a new way to train dynamic models with `MMDDP`. ([Tutorial for
-DDP](docs/en/tutorials/ddp_train_gans.md)) - **New Modular Design for Flexible
-Combination:** A new design for complex loss modules is proposed for
-customizing the links between modules, which can achieve flexible combination
-among different modules. ([Tutorial for new modular design](docs/en/tutorials/
-customize_losses.md))
+## Major Features - **High-quality Training Performance:** MMGeneration
+currently support training on Unconditional GANs, Conditional GANs, Internal
+GANs, Image Translation Models, and Diffusion Models. - **Powerful Application
+Toolkit:** A toolkit that provides plentiful applications to users.
+MMGeneration supports GAN interpolation, GAN projection, GAN manipulations and
+many other popular GAN's applications. It's time to play with your GANs! (
+[Tutorial for applications](docs/en/advanced_guides/applications.md)) -
+**Efficient Distributed Training for Generative Models:** With support of
+[MMSeparateDistributedDataParallel](https://github.com/open-mmlab/mmengine/
+blob/main/mmengine/model/wrappers/seperate_distributed.py), distributed
+training for dynamic architectures can be easily implemented. - **New Modular
+Design for Flexible Combination:** A new design for complex loss modules is
+proposed for customizing the links between modules, which can achieve flexible
+combination among different modules.(Tutorial for [losses](docs/en/
+advanced_guides/losses.md))
    Training Visualization          GAN Interpolation               GAN Projector                GAN Manipulation
        [https://user-                [https://user-                [https://user-                [https://user-
 images.githubusercontent.com/ images.githubusercontent.com/ images.githubusercontent.com/ images.githubusercontent.com/
 12726765/114509105-b6f4e780-  12726765/114679300-9fd4f900-  12726765/114524392-c11ee200-  12726765/114523716-20302700-
        9c67-11eb-8644-               9d3e-11eb-8f37-               9c77-11eb-8b6d-               9c77-11eb-804e-
       110b3cb01314.gif]             c36a018c02f7.gif]             37bc637f5626.gif]             327ae1ca0c5b.gif]
 ## Highlight - **Positional Encoding as Spatial Inductive Bias in GANs
 (CVPR2021)** has been released in `MMGeneration`. [\[Config\]](configs/
 positional_encoding_in_gans/README.md), [\[Project Page\]](https://
 nbei.github.io/gan-pos-encoding.html) - Conditional GANs have been supported in
 our toolkit. More methods and pre-trained weights will come soon. - Mixed-
 precision training (FP16) for StyleGAN2 has been supported. Please check [the
 comparison](configs/styleganv2/README.md) between different implementations. ##
-Changelog v0.7.3 was released on 14/04/2023. Please refer to [changelog.md]
-(docs/en/changelog.md) for details and release history. ## Installation
-MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://
-github.com/open-mmlab/mmcv). Below are quick steps for installation. **Step
-1.** Install PyTorch following [official instructions](https://pytorch.org/get-
-started/locally/), e.g. ```python pip3 install torch torchvision ``` **Step
-2.** Install MMCV with [MIM](https://github.com/open-mmlab/mim). ``` pip3
-install openmim mim install mmcv-full ``` **Step 3.** Install MMGeneration from
-source. ``` git clone https://github.com/open-mmlab/mmgeneration.git cd
-mmgeneration pip3 install -e . ``` Please refer to [get_started.md](docs/en/
-get_started.md) for more detailed instruction. ## Getting Started Please see
-[get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration.
-[docs/en/quick_run.md](docs/en/quick_run.md) can offer full guidance for quick
-run. For other details and tutorials, please go to our [documentation](https://
-mmgeneration.readthedocs.io/). ## ModelZoo These methods have been carefully
-studied and supported in our frameworks:  Unconditional GANs (click to
-collapse) - â [DCGAN](configs/dcgan/README.md) (ICLR'2016) - â [WGAN-GP]
-(configs/wgan-gp/README.md) (NIPS'2017) - â [LSGAN](configs/lsgan/README.md)
-(ICCV'2017) - â [GGAN](configs/ggan/README.md) (arXiv'2017) - â [PGGAN]
-(configs/pggan/README.md) (ICLR'2018) - â [StyleGANV1](configs/styleganv1/
-README.md) (CVPR'2019) - â [StyleGANV2](configs/styleganv2/README.md)
-(CVPR'2020) - â [StyleGANV3](configs/styleganv3/README.md) (NeurIPS'2021) -
-â [Positional Encoding in GANs](configs/positional_encoding_in_gans/
-README.md) (CVPR'2021)   Conditional GANs (click to collapse) - â [SNGAN]
-(configs/sngan_proj/README.md) (ICLR'2018) - â [Projection GAN](configs/
-sngan_proj/README.md) (ICLR'2018) - â [SAGAN](configs/sagan/README.md)
-(ICML'2019) - â [BIGGAN/BIGGAN-DEEP](configs/biggan/README.md) (ICLR'2019)
-Tricks for GANs (click to collapse) - â [ADA](configs/ada/README.md)
-(NeurIPS'2020)   Image2Image Translation (click to collapse) - â [Pix2Pix]
-(configs/pix2pix/README.md) (CVPR'2017) - â [CycleGAN](configs/cyclegan/
-README.md) (ICCV'2017)   Internal Learning (click to collapse) - â [SinGAN]
-(configs/singan/README.md) (ICCV'2019)   Denoising Diffusion Probabilistic
-Models (click to collapse) - â [Improved DDPM](configs/improved_ddpm/
-README.md) (arXiv'2021)  ## Related-Applications - â [MMGEN-FaceStylor]
-(https://github.com/open-mmlab/MMGEN-FaceStylor) ## Contributing We appreciate
-all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md]
-(https://github.com/open-mmlab/mmcv/blob/master/CONTRIBUTING.md) in MMCV for
-more details about the contributing guideline. ## Citation If you find this
-project useful in your research, please consider cite: ```BibTeX @misc
-{2021mmgeneration, title={{MMGeneration}: OpenMMLab Generative Model Toolbox
-and Benchmark}, author={MMGeneration Contributors}, howpublished = {\url{https:
-//github.com/open-mmlab/mmgeneration}}, year={2021} } ``` ## License This
-project is released under the [Apache 2.0 license](LICENSE). Some operations in
-`MMGeneration` are with other licenses instead of Apache2.0. Please refer to
-[LICENSES.md](LICENSES.md) for the careful check, if you are using our code for
-commercial matters. ## Projects in OpenMMLab - [MMCV](https://github.com/open-
-mmlab/mmcv): OpenMMLab foundational library for computer vision. - [MIM](https:
-//github.com/open-mmlab/mim): MIM installs OpenMMLab packages. -
-[MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab
-image classification toolbox and benchmark. - [MMDetection](https://github.com/
-open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark. -
-[MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-
-generation platform for general 3D object detection. - [MMRotate](https://
-github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and
-benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
-OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR](https://
-github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and
-understanding toolbox. - [MMPose](https://github.com/open-mmlab/mmpose):
-OpenMMLab pose estimation toolbox and benchmark. - [MMHuman3D](https://
-github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox
-and benchmark. - [MMSelfSup](https://github.com/open-mmlab/mmselfsup):
-OpenMMLab self-supervised learning toolbox and benchmark. - [MMRazor](https://
-github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and
-benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab
-fewshot learning toolbox and benchmark. - [MMAction2](https://github.com/open-
-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and
-benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
+What's new v1.0.0rc0 was released in 31/8/2022. This release introduced a brand
+new and flexible training & test engine, but it's still in progress. Welcome to
+try according to [the documentation](https://mmgeneration.readthedocs.io/en/
+1.x/). And there are some BC-breaking changes. Please check [the migration
+tutorial](https://mmgeneration.readthedocs.io/en/1.x/migration.html). The
+release candidate will last until the end of 2022, and during the release
+candidate, we will develop on the `1.x` branch. And we will still maintain 0.x
+version still at least the end of 2023. Please refer to [changelog.md](https://
+mmgeneration.readthedocs.io/en/1.x/notes/changelog.html) for more details and
+other release history. ## Installation MMGeneration depends on [PyTorch](https:
+//pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x). Below
+are quick steps for installation. **Step 1.** Install PyTorch following
+[official instructions](https://pytorch.org/get-started/locally/), e.g.
+```python pip3 install torch torchvision ``` **Step 2.** Install MMCV with
+[MIM](https://github.com/open-mmlab/mim). ``` pip install -U openmim # wait for
+more pre-compiled pkgs to release mim install 'mmcv>=2.0.0rc1' ``` **Step 3.**
+Install MMGeneration from source. ``` git clone -b 1.x https://github.com/open-
+mmlab/mmgeneration.git cd mmgeneration pip3 install -e .[all] ``` Please refer
+to [get_started.md](docs/en/get_started.md) for more detailed instruction. ##
+Getting Started Please see [get_started.md](docs/en/get_started.md) for the
+basic usage of MMGeneration. For other details and tutorials, please go to our
+[documentation](https://mmgeneration.readthedocs.io/en/1.x/). ## ModelZoo These
+methods have been carefully studied and supported in our frameworks:
+Unconditional GANs (click to collapse) - â [DCGAN](configs/dcgan/README.md)
+(ICLR'2016) - â [WGAN-GP](configs/wgan-gp/README.md) (NIPS'2017) - â
+[LSGAN](configs/lsgan/README.md) (ICCV'2017) - â [GGAN](configs/ggan/
+README.md) (arXiv'2017) - â [PGGAN](configs/pggan/README.md) (ICLR'2018) -
+â [StyleGANV1](configs/styleganv1/README.md) (CVPR'2019) - â [StyleGANV2]
+(configs/styleganv2/README.md) (CVPR'2020) - â [StyleGANV3](configs/
+styleganv3/README.md) (NeurIPS'2021) - â [Positional Encoding in GANs]
+(configs/positional_encoding_in_gans/README.md) (CVPR'2021)   Conditional GANs
+(click to collapse) - â [SNGAN](configs/sngan_proj/README.md) (ICLR'2018) -
+â [Projection GAN](configs/sngan_proj/README.md) (ICLR'2018) - â [SAGAN]
+(configs/sagan/README.md) (ICML'2019) - â [BIGGAN/BIGGAN-DEEP](configs/
+biggan/README.md) (ICLR'2019)   Image2Image Translation (click to collapse) -
+â [Pix2Pix](configs/pix2pix/README.md) (CVPR'2017) - â [CycleGAN](configs/
+cyclegan/README.md) (ICCV'2017)   Internal Learning (click to collapse) - â
+[SinGAN](configs/singan/README.md) (ICCV'2019)   Denoising Diffusion
+Probabilistic Models (click to collapse) - â [Improved DDPM](configs/
+improved_ddpm/README.md) (arXiv'2021)  ## Related-Applications - â [MMGEN-
+FaceStylor](https://github.com/open-mmlab/MMGEN-FaceStylor) ## Contributing We
+appreciate all contributions to improve MMGeneration. Please refer to
+[CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/tree/2.x/CONTRIBUTING.md)
+in MMCV and \[https://github.com/open-mmlab/mmengine/blob/main/
+CONTRIBUTING.md\] in MMEngine for more details about the contributing
+guideline. ## Citation If you find this project useful in your research, please
+consider cite: ```BibTeX @misc{2021mmgeneration, title={{MMGeneration}:
+OpenMMLab Generative Model Toolbox and Benchmark}, author={MMGeneration
+Contributors}, howpublished = {\url{https://github.com/open-mmlab/
+mmgeneration}}, year={2021} } ``` ## License This project is released under the
+[Apache 2.0 license](LICENSE). Some operations in `MMGeneration` are with other
+licenses instead of Apache2.0. Please refer to [LICENSES.md](LICENSES.md) for
+the careful check, if you are using our code for commercial matters. ##
+Projects in OpenMMLab 2.0 - [MMEngine](https://github.com/open-mmlab/mmengine):
+OpenMMLab foundational library for training deep learning models. - [MMCV]
+(https://github.com/open-mmlab/mmcv/tree/2.x): OpenMMLab foundational library
+for computer vision. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [MMClassification](https://github.com/open-mmlab/
+mmclassification/tree/1.x): OpenMMLab image classification toolbox and
+benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection/tree/3.x):
+OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d/tree/1.x): OpenMMLab's next-generation
+platform for general 3D object detection. - [MMRotate](https://github.com/open-
+mmlab/mmrotate/tree/1.x): OpenMMLab rotated object detection toolbox and
+benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation/
+tree/1.x): OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR]
+(https://github.com/open-mmlab/mmocr/tree/1.x): OpenMMLab text detection,
+recognition, and understanding toolbox. - [MMPose](https://github.com/open-
+mmlab/mmpose/tree/1.x): OpenMMLab pose estimation toolbox and benchmark. -
+[MMHuman3D](https://github.com/open-mmlab/mmhuman3d/tree/1.x): OpenMMLab 3D
+human parametric model toolbox and benchmark. - [MMSelfSup](https://github.com/
+open-mmlab/mmselfsup/tree/1.x): OpenMMLab self-supervised learning toolbox and
+benchmark. - [MMRazor](https://github.com/open-mmlab/mmrazor/tree/1.x):
+OpenMMLab model compression toolbox and benchmark. - [MMFewShot](https://
+github.com/open-mmlab/mmfewshot/tree/1.x): OpenMMLab fewshot learning toolbox
+and benchmark. - [MMAction2](https://github.com/open-mmlab/mmaction2/tree/1.x):
+OpenMMLab's next-generation action understanding toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking/tree/1.x): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMEditing]
-(https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing
-toolbox. - [MMGeneration](https://github.com/open-mmlab/mmgeneration):
-OpenMMLab image and video generative models toolbox. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+mmlab/mmflow/tree/1.x): OpenMMLab optical flow toolbox and benchmark. -
+[MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x): OpenMMLab image
+and video editing toolbox. - [MMGeneration](https://github.com/open-mmlab/
+mmgeneration/tree/1.x): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework.
```

### Comparing `mmgen-0.7.3/mmgen/.mim/tools/utils/translation_eval.py` & `mmgen-1.0.0rc0/mmgen/models/translation_models/cyclegan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,329 +1,282 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import argparse
-import os
-import shutil
-import sys
-
-import mmcv
 import torch
-from mmcv import Config
-from mmcv.parallel import MMDataParallel
-from mmcv.runner import load_checkpoint
-from torchvision.utils import save_image
-
-from mmgen.apis import set_random_seed
-from mmgen.core import build_metric
-from mmgen.core.evaluation import make_metrics_table, make_vanilla_dataloader
-from mmgen.datasets import build_dataloader, build_dataset
-from mmgen.models import build_model
-from mmgen.models.translation_models import BaseTranslationModel
-from mmgen.utils import get_root_logger
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(description='Evaluate a GAN model')
-    parser.add_argument('config', help='evaluation config file path')
-    parser.add_argument('checkpoint', help='checkpoint file')
-    parser.add_argument(
-        '--target-domain', type=str, default=None, help='Desired image domain')
-    parser.add_argument('--seed', type=int, default=2021, help='random seed')
-    parser.add_argument(
-        '--deterministic',
-        action='store_true',
-        help='whether to set deterministic options for CUDNN backend.')
-    parser.add_argument(
-        '--batch-size', type=int, default=1, help='batch size of dataloader')
-    parser.add_argument(
-        '--samples-path',
-        type=str,
-        default=None,
-        help='path to store images. If not given, remove it after evaluation\
-             finished')
-    parser.add_argument(
-        '--sample-model',
-        type=str,
-        default='ema',
-        help='use which mode (ema/orig) in sampling')
-    parser.add_argument(
-        '--eval',
-        nargs='*',
-        type=str,
-        default=None,
-        help='select the metrics you want to access')
-    parser.add_argument(
-        '--online',
-        action='store_true',
-        help='whether to use online mode for evaluation')
-    args = parser.parse_args()
-    return args
-
-
-@torch.no_grad()
-def single_gpu_evaluation(model,
-                          data_loader,
-                          metrics,
-                          logger,
-                          basic_table_info,
-                          batch_size,
-                          samples_path=None,
-                          **kwargs):
-    """Evaluate model with a single gpu.
-
-    This method evaluate model with a single gpu and displays eval progress
-        bar.
-
-    Args:
-        model (nn.Module): Model to be tested.
-        data_loader (nn.Dataloader): PyTorch data loader.
-        metrics (list): List of metric objects.
-        logger (Logger): logger used to record results of evaluation.
-        basic_table_info (dict): Dictionary containing the basic information \
-            of the metric table include training configuration and ckpt.
-        batch_size (int): Batch size of images fed into metrics.
-        samples_path (str): Used to save generated images. If it's none, we'll
-            give it a default directory and delete it after finishing the
-            evaluation. Default to None.
-        kwargs (dict): Other arguments.
-    """
-    # decide samples path
-    delete_samples_path = False
-    if samples_path:
-        mmcv.mkdir_or_exist(samples_path)
-    else:
-        temp_path = './work_dirs/temp_samples'
-        # if temp_path exists, add suffix
-        suffix = 1
-        samples_path = temp_path
-        while os.path.exists(samples_path):
-            samples_path = temp_path + '_' + str(suffix)
-            suffix += 1
-        os.makedirs(samples_path)
-        delete_samples_path = True
-
-    # sample images
-    num_exist = len(
-        list(
-            mmcv.scandir(
-                samples_path, suffix=('.jpg', '.png', '.jpeg', '.JPEG'))))
-    if basic_table_info['num_samples'] > 0:
-        max_num_images = basic_table_info['num_samples']
-    else:
-        max_num_images = max(metric.num_images for metric in metrics)
-    num_needed = max(max_num_images - num_exist, 0)
-
-    if num_needed > 0:
-        mmcv.print_log(f'Sample {num_needed} fake images for evaluation',
-                       'mmgen')
-        # define mmcv progress bar
-        pbar = mmcv.ProgressBar(num_needed)
-    # select key to fetch fake images
-    target_domain = basic_table_info['target_domain']
-    source_domain = basic_table_info['source_domain']
-    # if no images, `num_needed` should be zero
-    data_loader_iter = iter(data_loader)
-    for begin in range(0, num_needed, batch_size):
-        end = min(begin + batch_size, max_num_images)
-        # for translation model, we feed them images from dataloader
-        data_batch = next(data_loader_iter)
-        output_dict = model(
-            data_batch[f'img_{source_domain}'],
-            test_mode=True,
-            target_domain=target_domain)
-        fakes = output_dict['target']
-        pbar.update(end - begin)
-        for i in range(end - begin):
-            images = fakes[i:i + 1]
-            images = ((images + 1) / 2)
-            images = images[:, [2, 1, 0], ...]
-            images = images.clamp_(0, 1)
-            image_name = str(begin + i) + '.png'
-            save_image(images, os.path.join(samples_path, image_name))
-
-    if num_needed > 0:
-        sys.stdout.write('\n')
-
-    # return if only save sampled images
-    if len(metrics) == 0:
-        return
-
-    # empty cache to release GPU memory
-    torch.cuda.empty_cache()
-    fake_dataloader = make_vanilla_dataloader(samples_path, batch_size)
-
-    for metric in metrics:
-        mmcv.print_log(f'Evaluate with {metric.name} metric.', 'mmgen')
-        metric.prepare()
-        # feed in real images
-        for data in data_loader:
-            reals = data[f'img_{target_domain}']
-            num_left = metric.feed(reals, 'reals')
-            if num_left <= 0:
-                break
-        # feed in fake images
-        for data in fake_dataloader:
-            fakes = data['real_img']
-            num_left = metric.feed(fakes, 'fakes')
-            if num_left <= 0:
-                break
-        metric.summary()
-    table_str = make_metrics_table(basic_table_info['train_cfg'],
-                                   basic_table_info['ckpt'],
-                                   basic_table_info['sample_model'], metrics)
-    logger.info('\n' + table_str)
-    if delete_samples_path:
-        shutil.rmtree(samples_path)
-
-
-@torch.no_grad()
-def single_gpu_online_evaluation(model, data_loader, metrics, logger,
-                                 basic_table_info, batch_size, **kwargs):
-    """Evaluate model with a single gpu in online mode.
-
-    This method evaluate model with a single gpu and displays eval progress
-    bar. Different form `single_gpu_evaluation`, this function will not save
-    the images or read images from disks. Namely, there do not exist any IO
-    operations in this function. Thus, in general, `online` mode will achieve a
-    faster evaluation. However, this mode will take much more memory cost.
-    Therefore this evaluation function is recommended to evaluate your model
-    with a single metric.
-
-    Args:
-        model (nn.Module): Model to be tested.
-        data_loader (nn.Dataloader): PyTorch data loader.
-        metrics (list): List of metric objects.
-        logger (Logger): logger used to record results of evaluation.
-        basic_table_info (dict): Dictionary containing the basic information \
-            of the metric table include training configuration and ckpt.
-        batch_size (int): Batch size of images fed into metrics.
-        kwargs (dict): Other arguments.
+import torch.nn.functional as F
+from mmengine import MessageHub
+from mmengine.optim import OptimWrapperDict
+
+from mmgen.registry import MODELS
+from mmgen.structures import GenDataSample, PixelData
+from mmgen.utils.typing import ForwardOutputs
+from ..common import GANImageBuffer, set_requires_grad
+from .static_translation_gan import StaticTranslationGAN
+
+
+@MODELS.register_module()
+class CycleGAN(StaticTranslationGAN):
+    """CycleGAN model for unpaired image-to-image translation.
+
+    Ref:
+    Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial
+    Networks
     """
-    # sample images
-    max_num_images = 0 if len(metrics) == 0 else max(metric.num_fake_need
-                                                     for metric in metrics)
-    pbar = mmcv.ProgressBar(max_num_images)
-
-    # select key to fetch images
-    target_domain = basic_table_info['target_domain']
-    source_domain = basic_table_info['source_domain']
-
-    for metric in metrics:
-        mmcv.print_log(f'Evaluate with {metric.name} metric.', 'mmgen')
-        metric.prepare()
-
-    # feed reals and fakes
-    data_loader_iter = iter(data_loader)
-    for begin in range(0, max_num_images, batch_size):
-        end = min(begin + batch_size, max_num_images)
-        # for translation model, we feed them images from dataloader
-        data_batch = next(data_loader_iter)
-        output_dict = model(
-            data_batch[f'img_{source_domain}'],
-            test_mode=True,
-            target_domain=target_domain)
-        fakes = output_dict['target']
-        reals = data_batch[f'img_{target_domain}']
-        pbar.update(end - begin)
-        for metric in metrics:
-            metric.feed(reals, 'reals')
-            metric.feed(fakes, 'fakes')
-
-    for metric in metrics:
-        metric.summary()
-
-    table_str = make_metrics_table(basic_table_info['train_cfg'],
-                                   basic_table_info['ckpt'],
-                                   basic_table_info['sample_model'], metrics)
-    logger.info('\n' + table_str)
-
-
-def main():
-    args = parse_args()
-    cfg = Config.fromfile(args.config)
-
-    dirname = os.path.dirname(args.checkpoint)
-    ckpt = os.path.basename(args.checkpoint)
-
-    if 'http' in args.checkpoint:
-        log_path = None
-    else:
-        log_name = ckpt.split('.')[0] + '_eval_log' + '.txt'
-        log_path = os.path.join(dirname, log_name)
-
-    logger = get_root_logger(
-        log_file=log_path, log_level=cfg.log_level, file_mode='a')
-    logger.info('evaluation')
-
-    # set random seeds
-    if args.seed is not None:
-        set_random_seed(args.seed, deterministic=args.deterministic)
-
-    # build the model and load checkpoint
-    model = build_model(
-        cfg.model, train_cfg=cfg.train_cfg, test_cfg=cfg.test_cfg)
-    assert isinstance(model, BaseTranslationModel)
-    # sanity check for models without ema
-    if not model.use_ema:
-        args.sample_model = 'orig'
-
-    mmcv.print_log(f'Sampling model: {args.sample_model}', 'mmgen')
-
-    model.eval()
-
-    _ = load_checkpoint(model, args.checkpoint, map_location='cpu')
-    model = MMDataParallel(model, device_ids=[0])
-
-    # build metrics
-    if args.eval:
-        if args.eval[0] == 'none':
-            # only sample images
-            metrics = []
-            assert args.num_samples is not None and args.num_samples > 0
-        else:
-            metrics = [
-                build_metric(cfg.metrics[metric]) for metric in args.eval
-            ]
-    else:
-        metrics = [build_metric(cfg.metrics[metric]) for metric in cfg.metrics]
-
-    # get source domain and target domain
-    target_domain = args.target_domain
-    if target_domain is None:
-        target_domain = model.module._default_domain
-    source_domain = model.module.get_other_domains(target_domain)[0]
-
-    basic_table_info = dict(
-        train_cfg=os.path.basename(cfg._filename),
-        ckpt=ckpt,
-        sample_model=args.sample_model,
-        source_domain=source_domain,
-        target_domain=target_domain)
-
-    # build the dataloader
-    if len(metrics) == 0:
-        basic_table_info['num_samples'] = args.num_samples
-        data_loader = None
-    else:
-        basic_table_info['num_samples'] = -1
-        if cfg.data.get('test', None):
-            dataset = build_dataset(cfg.data.test)
-        else:
-            dataset = build_dataset(cfg.data.train)
-        data_loader = build_dataloader(
-            dataset,
-            samples_per_gpu=args.batch_size,
-            workers_per_gpu=cfg.data.get('val_workers_per_gpu',
-                                         cfg.data.workers_per_gpu),
-            dist=False,
-            shuffle=True)
-
-    if args.online:
-        single_gpu_online_evaluation(model, data_loader, metrics, logger,
-                                     basic_table_info, args.batch_size)
-    else:
-        single_gpu_evaluation(model, data_loader, metrics, logger,
-                              basic_table_info, args.batch_size,
-                              args.samples_path)
 
+    def __init__(self,
+                 *args,
+                 buffer_size=50,
+                 loss_config=dict(cycle_loss_weight=10., id_loss_weight=0.5),
+                 **kwargs):
+        super().__init__(*args, **kwargs)
+        # GAN image buffers
+        self.image_buffers = dict()
+        self.buffer_size = buffer_size
+        for domain in self._reachable_domains:
+            self.image_buffers[domain] = GANImageBuffer(self.buffer_size)
+
+        self.loss_config = loss_config
+
+    def forward_test(self, img, target_domain, **kwargs):
+        """Forward function for testing.
+
+        Args:
+            img (tensor): Input image tensor.
+            target_domain (str): Target domain of output image.
+            kwargs (dict): Other arguments.
+
+        Returns:
+            dict: Forward results.
+        """
+        # This is a trick for CycleGAN
+        # ref: https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix/blob/e1bdf46198662b0f4d0b318e24568205ec4d7aee/test.py#L54 # noqa
+        self.train()
+        target = self.translation(img, target_domain=target_domain, **kwargs)
+        results = dict(source=img.cpu(), target=target.cpu())
+        return results
+
+    def _get_disc_loss(self, outputs):
+        """Backward function for the discriminators.
+
+        Args:
+            outputs (dict): Dict of forward results.
+
+        Returns:
+            dict: Discriminators' loss and loss dict.
+        """
+        discriminators = self.get_module(self.discriminators)
+
+        log_vars_d = dict()
+        loss_d = 0
+
+        # GAN loss for discriminators['a']
+        for domain in self._reachable_domains:
+            losses = dict()
+            fake_img = self.image_buffers[domain].query(
+                outputs[f'fake_{domain}'])
+            fake_pred = discriminators[domain](fake_img.detach())
+            losses[f'loss_gan_d_{domain}_fake'] = F.mse_loss(
+                fake_pred, 0. * torch.ones_like(fake_pred))
+            real_pred = discriminators[domain](outputs[f'real_{domain}'])
+            losses[f'loss_gan_d_{domain}_real'] = F.mse_loss(
+                real_pred, 1. * torch.ones_like(real_pred))
+
+            _loss_d, _log_vars_d = self.parse_losses(losses)
+            _loss_d *= 0.5
+            loss_d += _loss_d
+            log_vars_d[f'loss_gan_d_{domain}'] = _log_vars_d['loss'] * 0.5
+
+        return loss_d, log_vars_d
+
+    def _get_gen_loss(self, outputs):
+        """Backward function for the generators.
+
+        Args:
+            outputs (dict): Dict of forward results.
+
+        Returns:
+            dict: Generators' loss and loss dict.
+        """
+        generators = self.get_module(self.generators)
+        discriminators = self.get_module(self.discriminators)
+
+        losses = dict()
+        # gan loss
+        for domain in self._reachable_domains:
+            # Identity reconstruction for generators
+            outputs[f'identity_{domain}'] = generators[domain](
+                outputs[f'real_{domain}'])
+            # GAN loss for generators
+            fake_pred = discriminators[domain](outputs[f'fake_{domain}'])
+            # LSGAN loss
+            losses[f'loss_gan_g_{domain}'] = F.mse_loss(
+                fake_pred, 1. * torch.ones_like(fake_pred))
+
+        # cycle loss
+        loss_weight = self.loss_config['cycle_loss_weight']
+        losses['cycle_loss'] = 0.
+        for domain in self._reachable_domains:
+            losses['cycle_loss'] += loss_weight * F.l1_loss(
+                outputs[f'cycle_{domain}'],
+                outputs[f'real_{domain}'],
+                reduction='mean')
+
+        # id loss
+        loss_weight = self.loss_config['id_loss_weight']
+        if loss_weight != 0.:
+            losses['id_loss'] = 0.
+            for domain in self._reachable_domains:
+                losses['id_loss'] += loss_weight * F.l1_loss(
+                    outputs[f'identity_{domain}'],
+                    outputs[f'real_{domain}'],
+                    reduction='mean')
+
+        loss_g, log_vars_g = self.parse_losses(losses)
+
+        return loss_g, log_vars_g
+
+    def _get_opposite_domain(self, domain):
+        for item in self._reachable_domains:
+            if item != domain:
+                return item
+        return None
+
+    def train_step(self, data: dict, optim_wrapper: OptimWrapperDict):
+        """Training step function.
+
+        Args:
+            data_batch (dict): Dict of the input data batch.
+            optimizer (dict[torch.optim.Optimizer]): Dict of optimizers for
+                the generators and discriminators.
+            ddp_reducer (:obj:`Reducer` | None, optional): Reducer from ddp.
+                It is used to prepare for ``backward()`` in ddp. Defaults to
+                None.
+            running_status (dict | None, optional): Contains necessary basic
+                information for training, e.g., iteration number. Defaults to
+                None.
+
+        Returns:
+            dict: Dict of loss, information for logger, the number of samples\
+                and results for visualization.
+        """
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
+        data = self.data_preprocessor(data, True)
+        disc_optimizer_wrapper = optim_wrapper['discriminators']
+
+        inputs_dict = data['inputs']
+        outputs, log_vars = dict(), dict()
+
+        # forward generators
+        with disc_optimizer_wrapper.optim_context(self.discriminators):
+            for target_domain in self._reachable_domains:
+                # fetch data by domain
+                source_domain = self.get_other_domains(target_domain)[0]
+                img = inputs_dict[f'img_{source_domain}']
+                # translation process
+                results = self(
+                    img, test_mode=False, target_domain=target_domain)
+                outputs[f'real_{source_domain}'] = results['source']
+                outputs[f'fake_{target_domain}'] = results['target']
+                # cycle process
+                results = self(
+                    results['target'],
+                    test_mode=False,
+                    target_domain=source_domain)
+                outputs[f'cycle_{source_domain}'] = results['target']
+
+            # update discriminators
+            disc_accu_iters = disc_optimizer_wrapper._accumulative_counts
+            loss_d, log_vars_d = self._get_disc_loss(outputs)
+            disc_optimizer_wrapper.update_params(loss_d)
+            log_vars.update(log_vars_d)
+
+        # generators, no updates to discriminator parameters.
+        if ((curr_iter + 1) % (self.discriminator_steps * disc_accu_iters) == 0
+                and curr_iter >= self.disc_init_steps):
+            set_requires_grad(self.discriminators, False)
+            # update generator
+            gen_optimizer_wrapper = optim_wrapper['generators']
+            with gen_optimizer_wrapper.optim_context(self.generators):
+                loss_g, log_vars_g = self._get_gen_loss(outputs)
+                gen_optimizer_wrapper.update_params(loss_g)
+                log_vars.update(log_vars_g)
+
+            set_requires_grad(self.discriminators, True)
+
+        return log_vars
+
+    def test_step(self, data: dict) -> ForwardOutputs:
+        """Gets the generated image of given data. Same as :meth:`val_step`.
+
+        Args:
+            data (dict): Data sampled from metric specific
+                sampler. More detials in `Metrics` and `Evaluator`.
+
+        Returns:
+            ForwardOutputs: Generated image or image dict.
+        """
+        data = self.data_preprocessor(data)
+        inputs_dict, data_samples = data['inputs'], data['data_samples']
+
+        outputs = {}
+        for src_domain in self._reachable_domains:
+            # Identity reconstruction for generators
+            target_domain = self.get_other_domains(src_domain)[0]
+            target = self.forward_test(
+                inputs_dict[f'img_{src_domain}'],
+                target_domain=target_domain)['target']
+            outputs[f'img_{target_domain}'] = target
+
+        batch_sample_list = []
+        num_batches = next(iter(outputs.values())).shape[0]
+        for idx in range(num_batches):
+            gen_sample = GenDataSample()
+            if data_samples:
+                gen_sample.update(data_samples[idx])
+
+            for src_domain in self._reachable_domains:
+                target_domain = self.get_other_domains(src_domain)[0]
+                setattr(gen_sample, f'gt_{src_domain}',
+                        PixelData(data=inputs_dict[f'img_{src_domain}'][idx]))
+                setattr(gen_sample, f'fake_{src_domain}',
+                        PixelData(data=outputs[f'img_{src_domain}'][idx]))
+
+            batch_sample_list.append(gen_sample)
+        return batch_sample_list
+
+    def val_step(self, data: dict) -> ForwardOutputs:
+        """Gets the generated image of given data. Same as :meth:`val_step`.
+
+        Args:
+            data (dict): Data sampled from metric specific
+                sampler. More detials in `Metrics` and `Evaluator`.
+
+        Returns:
+            ForwardOutputs: Generated image or image dict.
+        """
+        data = self.data_preprocessor(data)
+        inputs_dict, data_samples = data['inputs'], data['data_samples']
+
+        outputs = {}
+        for src_domain in self._reachable_domains:
+            # Identity reconstruction for generators
+            target_domain = self.get_other_domains(src_domain)[0]
+            target = self.forward_test(
+                inputs_dict[f'img_{src_domain}'],
+                target_domain=target_domain)['target']
+            outputs[f'img_{target_domain}'] = target
+
+        batch_sample_list = []
+        num_batches = next(iter(outputs.values())).shape[0]
+        for idx in range(num_batches):
+            gen_sample = GenDataSample()
+            if data_samples:
+                gen_sample.update(data_samples[idx])
+
+            for src_domain in self._reachable_domains:
+                target_domain = self.get_other_domains(src_domain)[0]
+                setattr(gen_sample, f'gt_{src_domain}',
+                        PixelData(data=inputs_dict[f'img_{src_domain}'][idx]))
+                setattr(gen_sample, f'fake_{src_domain}',
+                        PixelData(data=outputs[f'img_{src_domain}'][idx]))
 
-if __name__ == '__main__':
-    main()
+            batch_sample_list.append(gen_sample)
+        return batch_sample_list
```

### Comparing `mmgen-0.7.3/mmgen/__init__.py` & `mmgen-1.0.0rc0/mmgen/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,18 +12,18 @@
         elif x.find('rc') != -1:
             patch_version = x.split('rc')
             digit_version.append(int(patch_version[0]) - 1)
             digit_version.append(int(patch_version[1]))
     return digit_version
 
 
-mmcv_minimum_version = '1.3.0'
-mmcv_maximum_version = '1.8.0'
+mmcv_minimum_version = '2.0.0rc1'
+mmcv_maximum_version = '2.0.0'
 mmcv_version = digit_version(mmcv.__version__)
 
 
 assert (mmcv_version >= digit_version(mmcv_minimum_version)
         and mmcv_version <= digit_version(mmcv_maximum_version)), \
     f'MMCV=={mmcv.__version__} is used but incompatible. ' \
-    f'Please install mmcv>={mmcv_minimum_version}, <={mmcv_maximum_version}.'
+    f'Please install mmcv>={mmcv_minimum_version}, <{mmcv_maximum_version}.'
 
 __all__ = ['__version__', 'version_info', 'parse_version_info']
```

### Comparing `mmgen-0.7.3/mmgen/apis/inference.py` & `mmgen-1.0.0rc0/mmgen/apis/inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,40 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import mmcv
+import mmengine
 import torch
-from mmcv.parallel import collate, scatter
-from mmcv.runner import load_checkpoint
-from mmcv.utils import is_list_of
+from mmengine import is_list_of
+from mmengine.config import Config
+from mmengine.dataset import Compose
+from mmengine.runner import load_checkpoint
 
-from mmgen.datasets.pipelines import Compose
-from mmgen.models import BaseTranslationModel, build_model
+from mmgen.models import BaseTranslationModel
+from mmgen.registry import MODELS
+from mmgen.utils import register_all_modules
+
+register_all_modules()
+
+
+def set_random_seed(seed, deterministic=False, use_rank_shift=True):
+    """Set random seed.
+
+    In this function, we just modify the default behavior of the similar
+    function defined in MMCV.
+    Args:
+        seed (int): Seed to be used.
+        deterministic (bool): Whether to set the deterministic option for
+            CUDNN backend, i.e., set `torch.backends.cudnn.deterministic`
+            to True and `torch.backends.cudnn.benchmark` to False.
+            Default: False.
+        rank_shift (bool): Whether to add rank number to the random seed to
+            have different random seed in different threads. Default: True.
+    """
+    # TODO: refactor this  when refactor dir
+    # set_random_seed_mmcv(
+    #     seed, deterministic=deterministic, use_rank_shift=use_rank_shift)
+    return
 
 
 def init_model(config, checkpoint=None, device='cuda:0', cfg_options=None):
     """Initialize a detector from config file.
 
     Args:
         config (str or :obj:`mmcv.Config`): Config file path or the config
@@ -21,23 +45,22 @@
             config.
 
     Returns:
         nn.Module: The constructed unconditional model.
     """
 
     if isinstance(config, str):
-        config = mmcv.Config.fromfile(config)
-    elif not isinstance(config, mmcv.Config):
+        config = Config.fromfile(config)
+    elif not isinstance(config, Config):
         raise TypeError('config must be a filename or Config object, '
                         f'but got {type(config)}')
     if cfg_options is not None:
         config.merge_from_dict(cfg_options)
 
-    model = build_model(
-        config.model, train_cfg=config.train_cfg, test_cfg=config.test_cfg)
+    model = MODELS.build(config.model)
 
     if checkpoint is not None:
         load_checkpoint(model, checkpoint, map_location='cpu')
 
     model._cfg = config  # save the config in the model for convenience
     model.to(device)
     model.eval()
@@ -73,20 +96,19 @@
 
     if num_samples % num_batches > 0:
         batches_list.append(num_samples % num_batches)
     res_list = []
 
     # inference
     for batches in batches_list:
-        res = model.sample_from_noise(
-            None, num_batches=batches, sample_model=sample_model, **kwargs)
-        res_list.append(res.cpu())
-
-    results = torch.cat(res_list, dim=0)
+        res = model(
+            dict(num_batches=batches, sample_model=sample_model), **kwargs)
+        res_list.extend([item.fake_img.data.cpu() for item in res])
 
+    results = torch.stack(res_list, dim=0)
     return results
 
 
 @torch.no_grad()
 def sample_conditional_model(model,
                              num_samples=16,
                              num_batches=4,
@@ -164,24 +186,20 @@
         else:
             label_list.append(label[(n + 1) * num_batches:])
 
     res_list = []
 
     # inference
     for batches, labels in zip(batches_list, label_list):
-        res = model.sample_from_noise(
-            None,
-            num_batches=batches,
-            label=labels,
-            sample_model=sample_model,
+        res = model(
+            dict(
+                num_batches=batches, labels=labels, sample_model=sample_model),
             **kwargs)
-        res_list.append(res.cpu())
-
-    results = torch.cat(res_list, dim=0)
-
+        res_list.extend([item.fake_img.data.cpu() for item in res])
+    results = torch.stack(res_list, dim=0)
     return results
 
 
 def sample_img2img_model(model, image_path, target_domain=None, **kwargs):
     """Sampling from translation models.
 
     Args:
@@ -195,33 +213,31 @@
 
     # get source domain and target domain
     if target_domain is None:
         target_domain = model._default_domain
     source_domain = model.get_other_domains(target_domain)[0]
 
     cfg = model._cfg
-    device = next(model.parameters()).device  # model device
     # build the data pipeline
     test_pipeline = Compose(cfg.test_pipeline)
 
     # prepare data
     data = dict()
     # dirty code to deal with test data pipeline
     data['pair_path'] = image_path
     data[f'img_{source_domain}_path'] = image_path
     data[f'img_{target_domain}_path'] = image_path
 
-    data = test_pipeline(data)
-    if device.type == 'cpu':
-        data = collate([data], samples_per_gpu=1)
-        data['meta'] = []
-    else:
-        data = scatter(collate([data], samples_per_gpu=1), [device])[0]
+    data = [test_pipeline(data)]
+
+    data = model.data_preprocessor(data, False)
+    inputs_dict = data['inputs']
+
+    source_image = inputs_dict[f'img_{source_domain}']
 
-    source_image = data[f'img_{source_domain}']
     # forward the model
     with torch.no_grad():
         results = model(
             source_image,
             test_mode=True,
             target_domain=target_domain,
             **kwargs)
@@ -261,37 +277,36 @@
         batches_list.append(num_samples % num_batches)
 
     noise_batch = torch.randn(model.image_shape) if same_noise else None
 
     res_list = []
     # inference
     for idx, batches in enumerate(batches_list):
-        mmcv.print_log(
-            f'Start to sample batch [{idx+1} / '
-            f'{len(batches_list)}]', 'mmgen')
+        mmengine.print_log(f'Start to sample batch [{idx+1} / '
+                           f'{len(batches_list)}]')
         noise_batch_ = noise_batch[None, ...].expand(batches, -1, -1, -1) \
             if same_noise else None
 
-        res = model.sample_from_noise(
-            noise_batch_,
+        batch_input = dict(
+            noise=noise_batch_,
             num_batches=batches,
             sample_model=sample_model,
             show_pbar=True,
             **kwargs)
-        if isinstance(res, dict):
-            res = {k: v.cpu() for k, v in res.items()}
-        elif isinstance(res, torch.Tensor):
-            res = res.cpu()
-        else:
-            raise ValueError('Sample results should be \'dict\' or '
-                             f'\'torch.Tensor\', but receive \'{type(res)}\'')
-        res_list.append(res)
+        res = model(batch_input)
+        for idx in range(len(res)):
+            if res[idx].sample_model == 'ema/orig':
+                res_ = {
+                    'ema': res[idx].ema.fake_img.data.cpu(),
+                    'orig': res[idx].orig.fake_img.data.cpu()
+                }
+            else:
+                res_ = res[idx].fake_img.data.cpu()
+            res_list.append(res_)
 
     # gather the res_list
     if isinstance(res_list[0], dict):
         res_dict = dict()
-        for t in res_list[0].keys():
-            # num_samples x 3 x H x W
-            res_dict[t] = torch.cat([res[t] for res in res_list], dim=0)
+        for k in res_list[0].keys():
+            res_dict[k] = [res[k] for res in res_list]
         return res_dict
-    else:
-        return torch.cat(res_list, dim=0)
+    return res_list
```

### Comparing `mmgen-0.7.3/mmgen/core/evaluation/eval_hooks.py` & `mmgen-1.0.0rc0/mmgen/models/gans/progressive_growing_unconditional_gan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,524 +1,462 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import math
-import os
-import os.path as osp
-import sys
-import warnings
-from bisect import bisect_right
+from functools import partial
+from typing import Dict, List, Optional, Tuple, Union
 
 import mmcv
+import numpy as np
 import torch
-from mmcv.runner import HOOKS, Hook, get_dist_info
-
-from ..registry import build_metric
-
-
-@HOOKS.register_module()
-class GenerativeEvalHook(Hook):
-    """Evaluation Hook for Generative Models.
-
-    This evaluation hook can be used to evaluate unconditional and conditional
-    models. Note that only ``FID`` and ``IS`` metric are supported for the
-    distributed training now. In the future, we will support more metrics for
-    the evaluation during the training procedure.
-
-    In our config system, you only need to add `evaluation` with the detailed
-    configureations. Below is several usage cases for different situations.
-    What you need to do is to add these lines at the end of your config file.
-    Then, you can use this evaluation hook in the training procedure.
-
-    To be noted that, this evaluation hook support evaluation with dynamic
-    intervals for FID or other metrics may fluctuate frequently at the end of
-    the training process.
-
-    # TODO: fix the online doc
-
-    #. Only use FID for evaluation
-
-    .. code-block:: python
-        :linenos:
-
-        evaluation = dict(
-            type='GenerativeEvalHook',
-            interval=10000,
-            metrics=dict(
-                type='FID',
-                num_images=50000,
-                inception_pkl='work_dirs/inception_pkl/ffhq-256-50k-rgb.pkl',
-                bgr2rgb=True),
-            sample_kwargs=dict(sample_model='ema'))
-
-    #. Use FID and IS simultaneously and save the best checkpoints respectively
-
-    .. code-block:: python
-        :linenos:
-
-        evaluation = dict(
-            type='GenerativeEvalHook',
-            interval=10000,
-            metrics=[dict(
-                type='FID',
-                num_images=50000,
-                inception_pkl='work_dirs/inception_pkl/ffhq-256-50k-rgb.pkl',
-                bgr2rgb=True),
-                dict(type='IS',
-                num_images=50000)],
-            best_metric=['fid', 'is'],
-            sample_kwargs=dict(sample_model='ema'))
-
-    #. Use dynamic evaluation intervals
-
-    .. code-block:: python
-        :linenos:
-
-        # interval = 10000 if iter < 50000,
-        # interval = 4000, if 50000 <= iter < 750000,
-        # interval = 2000, if iter >= 750000
-
-        evaluation = dict(
-            type='GenerativeEvalHook',
-            interval=dict(milestones=[500000, 750000],
-                          interval=[10000, 4000, 2000])
-            metrics=[dict(
-                type='FID',
-                num_images=50000,
-                inception_pkl='work_dirs/inception_pkl/ffhq-256-50k-rgb.pkl',
-                bgr2rgb=True),
-                dict(type='IS',
-                num_images=50000)],
-            best_metric=['fid', 'is'],
-            sample_kwargs=dict(sample_model='ema'))
-
+import torch.autograd as autograd
+import torch.nn as nn
+import torch.nn.functional as F
+from mmengine import MessageHub
+from mmengine.dist import get_world_size
+from mmengine.model import is_model_wrapper
+from mmengine.optim import OptimWrapper, OptimWrapperDict
+from torch import Tensor
+
+from mmgen.registry import MODELS
+from mmgen.structures import GenDataSample, PixelData
+from mmgen.utils.typing import ForwardInputs
+from ..common import gather_log_vars, get_valid_num_batches, set_requires_grad
+from .base_gan import BaseGAN
+
+ModelType = Union[Dict, nn.Module]
+TrainInput = Union[dict, Tensor]
+
+
+# @MODELS.register_module('StyleGANV1')
+@MODELS.register_module('PGGAN')
+@MODELS.register_module()
+class ProgressiveGrowingGAN(BaseGAN):
+    """Progressive Growing Unconditional GAN.
+
+    In this GAN model, we implement progressive growing training schedule,
+    which is proposed in Progressive Growing of GANs for improved Quality,
+    Stability and Variation, ICLR 2018.
+
+    We highly recommend to use ``GrowScaleImgDataset`` for saving computational
+    load in data pre-processing.
+
+    Notes for **using PGGAN**:
+
+    #. In official implementation, Tero uses gradient penalty with
+       ``norm_mode="HWC"``
+    #. We do not implement ``minibatch_repeats`` where has been used in
+       official Tensorflow implementation.
+
+    Notes for resuming progressive growing GANs:
+    Users should specify the ``prev_stage`` in ``train_cfg``. Otherwise, the
+    model is possible to reset the optimizer status, which will bring
+    inferior performance. For example, if your model is resumed from the
+    `256` stage, you should set ``train_cfg=dict(prev_stage=256)``.
 
     Args:
-        dataloader (DataLoader): A PyTorch dataloader.
-        interval (int | dict): Evaluation interval. If int is passed,
-            ``eval_hook`` would run under given interval. If a dict is passed,
-            The key and value would be interpret as 'milestones' and 'interval'
-            of the evaluation.  Default: 1.
-        dist (bool, optional): Whether to use distributed evaluation.
-            Defaults to True.
-        metrics (dict | list[dict], optional): Configs for metrics that will be
-            used in evaluation hook. Defaults to None.
-        sample_kwargs (dict | None, optional): Additional keyword arguments for
-            sampling images. Defaults to None.
-        save_best_ckpt (bool, optional): Whether to save the best checkpoint
-            according to ``best_metric``. Defaults to ``True``.
-        best_metric (str | list, optional): Which metric to be used in saving
-            the best checkpoint. Multiple metrics have been supported by
-            inputing a list of metric names, e.g., ``['fid', 'is']``.
-            Defaults to ``'fid'``.
+        generator (dict): Config for generator.
+        discriminator (dict): Config for discriminator.
     """
-    rule_map = {'greater': lambda x, y: x > y, 'less': lambda x, y: x < y}
-    init_value_map = {'greater': -math.inf, 'less': math.inf}
-    greater_keys = ['acc', 'top', 'AR@', 'auc', 'precision', 'mAP', 'is']
-    less_keys = ['loss', 'fid']
-    _supported_best_metrics = ['fid', 'is']
 
     def __init__(self,
-                 dataloader,
-                 interval=1,
-                 dist=True,
-                 metrics=None,
-                 sample_kwargs=None,
-                 save_best_ckpt=True,
-                 best_metric='fid'):
-        assert metrics is not None
-        self.dataloader = dataloader
-        self.dist = dist
-        self.sample_kwargs = sample_kwargs if sample_kwargs else dict()
-        self.save_best_ckpt = save_best_ckpt
-        self.best_metric = best_metric
-
-        if isinstance(interval, int):
-            self.interval = interval
-        elif isinstance(interval, dict):
-            if 'milestones' not in interval or 'interval' not in interval:
-                raise KeyError(
-                    '`milestones` and `interval` must exist in interval dict '
-                    'if you want to use the dynamic interval evaluation '
-                    f'strategy. But receive [{[k for k in interval.keys()]}] '
-                    'in the interval dict.')
-
-            self.milestones = interval['milestones']
-            self.interval = interval['interval']
-            # check if length of interval match with the milestones
-            if len(self.interval) != len(self.milestones) + 1:
-                raise ValueError(
-                    f'Length of `interval`(={len(self.interval)}) cannot '
-                    f'match length of `milestones`(={len(self.milestones)}).')
-
-            # check if milestones is in order
-            for idx in range(len(self.milestones) - 1):
-                former, latter = self.milestones[idx], self.milestones[idx + 1]
-                if former >= latter:
-                    raise ValueError(
-                        'Elements in `milestones` should in ascending order.')
-        else:
-            raise TypeError('`interval` only support `int` or `dict`,'
-                            f'recieve {type(self.interval)} instead.')
+                 generator,
+                 discriminator,
+                 data_preprocessor,
+                 nkimgs_per_scale,
+                 noise_size=None,
+                 interp_real=None,
+                 transition_kimgs: int = 600,
+                 prev_stage: int = 0,
+                 ema_config: Optional[Dict] = None):
+        super().__init__(generator, discriminator, data_preprocessor, 1, 1,
+                         noise_size, ema_config)
+
+        # register necessary training status
+        self.register_buffer('shown_nkimg', torch.tensor(0.))
+        self.register_buffer('_curr_transition_weight', torch.tensor(1.))
+
+        if interp_real is None:
+            interp_real = dict(mode='bilinear', align_corners=True)
+        self.interp_real_to = partial(F.interpolate, **interp_real)
+
+        self.scales, self.nkimgs = [], []
+        for k, v in nkimgs_per_scale.items():
+            # support for different data types
+            if isinstance(k, str):
+                k = (int(k), int(k))
+            elif isinstance(k, int):
+                k = (k, k)
+            else:
+                assert mmcv.is_tuple_of(k, int)
 
-        if isinstance(best_metric, str):
-            self.best_metric = [self.best_metric]
+            # sanity check for the order of scales
+            assert len(self.scales) == 0 or k[0] > self.scales[-1][0]
+            self.scales.append(k)
+            self.nkimgs.append(v)
+
+        self.cum_nkimgs = np.cumsum(self.nkimgs)
+        self.curr_stage = 0
+        # dirty walkround for avoiding optimizer bug in resuming
+        self.prev_stage = prev_stage
+        # actually nkimgs shown at the end of per training stage
+        self._actual_nkimgs = []
+        # In each scale, transit from previous torgb layer to newer torgb layer
+        # with `transition_kimgs` imgs
+        self.transition_kimgs = transition_kimgs
+
+        # this buffer is used to resume model easily
+        self.register_buffer(
+            '_next_scale_int',
+            torch.tensor(self.scales[0][0], dtype=torch.int32))
+        # TODO: init it with the same value as `_next_scale_int`
+        # a dirty workaround for testing
+        self.register_buffer(
+            '_curr_scale_int',
+            torch.tensor(self.scales[-1][0], dtype=torch.int32))
+
+    def forward(self,
+                inputs: ForwardInputs,
+                data_samples: Optional[list] = None,
+                mode: Optional[str] = None):
+        """Sample images from noises by using the generator."""
+        if isinstance(inputs, Tensor):
+            noise = inputs
+            curr_scale = transition_weight = None
+        else:
+            noise = inputs.get('noise', None)
+            num_batches = get_valid_num_batches(inputs)
+            noise = self.noise_fn(noise, num_batches=num_batches)
+
+            curr_scale = inputs.get('curr_scale', None)
+            transition_weight = inputs.get('transition_weight', None)
+        num_batches = noise.shape[0]
+
+        # use `self.curr_scale` if curr_scale is None
+        if curr_scale is None:
+            # in training, 'curr_scale' will be set as attribute
+            if hasattr(self, 'curr_scale'):
+                curr_scale = self.curr_scale[0]
+            # in testing, adopt '_curr_scale_int' from buffer as testing scale
+            else:
+                curr_scale = self._curr_scale_int.item()
 
-        if self.save_best_ckpt:
-            not_supported = set(self.best_metric) - set(
-                self._supported_best_metrics)
-            assert len(not_supported) == 0, (
-                f'{not_supported} is not supported for saving best ckpt')
-
-        self.metrics = build_metric(metrics)
-
-        if isinstance(metrics, dict):
-            self.metrics = [self.metrics]
-
-        for metric in self.metrics:
-            metric.prepare()
-
-        # add support for saving best ckpt
-        if self.save_best_ckpt:
-            self.rule = {}
-            self.compare_func = {}
-            self._curr_best_score = {}
-            self._curr_best_ckpt_path = {}
-            for name in self.best_metric:
-                if name in self.greater_keys:
-                    self.rule[name] = 'greater'
-                else:
-                    self.rule[name] = 'less'
-                self.compare_func[name] = self.rule_map[self.rule[name]]
-                self._curr_best_score[name] = self.init_value_map[
-                    self.rule[name]]
-                self._curr_best_ckpt_path[name] = None
+        # use `self._curr_transition_weight` if `transition_weight` is None
+        if transition_weight is None:
+            transition_weight = self._curr_transition_weight.item()
 
-    def get_current_interval(self, runner):
-        """Get current evaluation interval.
+        sample_model = self._get_valid_model(inputs)
 
-        Args:
-            runner (``mmcv.runner.BaseRunner``): The runner.
-        """
-        if isinstance(self.interval, int):
-            return self.interval
+        if sample_model in ['ema', 'ema/orig']:
+            _model = self.generator_ema
         else:
-            curr_iter = runner.iter + 1
-            index = bisect_right(self.milestones, curr_iter)
-            return self.interval[index]
+            _model = self.generator
 
-    def before_run(self, runner):
-        """The behavior before running.
+        outputs = _model(
+            noise, curr_scale=curr_scale, transition_weight=transition_weight)
 
-        Args:
-            runner (``mmcv.runner.BaseRunner``): The runner.
-        """
-        if self.save_best_ckpt is not None:
-            if runner.meta is None:
-                warnings.warn('runner.meta is None. Creating an empty one.')
-                runner.meta = dict()
-            runner.meta.setdefault('hook_msgs', dict())
+        if sample_model == 'ema/orig':
+            _model = self.generator
+            outputs_orig = _model(
+                noise,
+                curr_scale=curr_scale,
+                transition_weight=transition_weight)
+            outputs = dict(ema=outputs, orig=outputs_orig)
+
+        batch_sample_list = []
+        for idx in range(num_batches):
+            gen_sample = GenDataSample()
+            if data_samples:
+                gen_sample.update(data_samples[idx])
+            if isinstance(outputs, dict):
+                gen_sample.ema = GenDataSample(
+                    fake_img=PixelData(data=outputs['ema'][idx]),
+                    sample_model='ema')
+                gen_sample.orig = GenDataSample(
+                    fake_img=PixelData(data=outputs['orig'][idx]),
+                    sample_model='orig')
+                gen_sample.sample_model = 'ema/orig'
+            else:
+                gen_sample.fake_img = PixelData(data=outputs[idx])
+                gen_sample.sample_model = sample_model
 
-    def after_train_iter(self, runner):
-        """The behavior after each train iteration.
+            # Append input condition (noise and sample_kwargs) to
+            # batch_sample_list
+            gen_sample.noise = noise
+            batch_sample_list.append(gen_sample)
+
+        return batch_sample_list
+
+    def train_discriminator(
+            self, inputs: Tensor, data_samples: List[GenDataSample],
+            optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        real_imgs = inputs
+        num_batches = real_imgs.shape[0]
+        noise_batch = self.noise_fn(num_batches=num_batches)
+
+        with torch.no_grad():
+            fake_imgs = self.generator(
+                noise_batch,
+                curr_scale=self.curr_scale[0],
+                transition_weight=self._curr_transition_weight,
+                return_noise=False)
+
+        disc_pred_fake = self.discriminator(
+            fake_imgs,
+            curr_scale=self.curr_scale[0],
+            transition_weight=self._curr_transition_weight)
+        disc_pred_real = self.discriminator(
+            real_imgs,
+            curr_scale=self.curr_scale[0],
+            transition_weight=self._curr_transition_weight)
+
+        parsed_loss, log_vars = self.disc_loss(disc_pred_fake, disc_pred_real,
+                                               fake_imgs, real_imgs)
+        optimizer_wrapper.update_params(parsed_loss)
+        return log_vars
+
+    def disc_loss(self, disc_pred_fake: Tensor, disc_pred_real: Tensor,
+                  fake_data: Tensor, real_data: Tensor) -> Tuple[Tensor, dict]:
+        r"""Get disc loss. PGGAN use WGAN-GP's loss and discriminator shift
+        loss to train the discriminator.
+
+        .. math:
+            L_{D} = \mathbb{E}_{z\sim{p_{z}}}D\left\(G\left\(z\right\)\right\)
+                - \mathbb{E}_{x\sim{p_{data}}}D\left\(x\right\) + L_{GP} \\
+            L_{GP} = \lambda\mathbb{E}(\Vert\nabla_{\tilde{x}}D(\tilde{x})
+                \Vert_2-1)^2 \\
+            \tilde{x} = \epsilon x + (1-\epsilon)G(z)
+            L_{shift} =
 
         Args:
-            runner (``mmcv.runner.BaseRunner``): The runner.
+            disc_pred_fake (Tensor): Discriminator's prediction of the fake
+                images.
+            disc_pred_real (Tensor): Discriminator's prediction of the real
+                images.
+            fake_data (Tensor): Generated images, used to calculate gradient
+                penalty.
+            real_data (Tensor): Real images, used to calculate gradient
+                penalty.
+
+        Returns:
+            Tuple[Tensor, dict]: Loss value and a dict of log variables.
         """
-        interval = self.get_current_interval(runner)
-        if not self.every_n_iters(runner, interval):
-            return
-
-        runner.model.eval()
-
-        batch_size = self.dataloader.batch_size
-        rank, ws = get_dist_info()
-        total_batch_size = batch_size * ws
-
-        # sample real images
-        max_real_num_images = max(metric.num_images - metric.num_real_feeded
-                                  for metric in self.metrics)
-        # define mmcv progress bar
-        if rank == 0 and max_real_num_images > 0:
-            mmcv.print_log(
-                f'Sample {max_real_num_images} real images for evaluation',
-                'mmgen')
-            pbar = mmcv.ProgressBar(max_real_num_images)
-
-        if max_real_num_images > 0:
-            for data in self.dataloader:
-                if 'real_img' in data:
-                    reals = data['real_img']
-                # key for conditional GAN
-                elif 'img' in data:
-                    reals = data['img']
-                else:
-                    raise KeyError('Cannot found key for images in data_dict. '
-                                   'Only support `real_img` for unconditional '
-                                   'datasets and `img` for conditional '
-                                   'datasets.')
-
-                if reals.shape[1] not in [1, 3]:
-                    raise RuntimeError('real images should have one or three '
-                                       'channels in the first, '
-                                       'not % d' % reals.shape[1])
-                if reals.shape[1] == 1:
-                    reals = reals.repeat(1, 3, 1, 1)
-
-                num_feed = 0
-                for metric in self.metrics:
-                    num_feed_ = metric.feed(reals, 'reals')
-                    num_feed = max(num_feed_, num_feed)
-
-                if num_feed <= 0:
-                    break
-
-                if rank == 0:
-                    pbar.update(num_feed)
-
-        max_num_images = max(metric.num_images for metric in self.metrics)
-        if rank == 0:
-            mmcv.print_log(
-                f'Sample {max_num_images} fake images for evaluation', 'mmgen')
-
-        # define mmcv progress bar
-        if rank == 0:
-            pbar = mmcv.ProgressBar(max_num_images)
-
-        # sampling fake images and directly send them to metrics
-        for _ in range(0, max_num_images, total_batch_size):
-
-            with torch.no_grad():
-                fakes = runner.model(
-                    None,
-                    num_batches=batch_size,
-                    return_loss=False,
-                    **self.sample_kwargs)
-
-                for metric in self.metrics:
-                    # feed in fake images
-                    metric.feed(fakes, 'fakes')
-
-            if rank == 0:
-                pbar.update(total_batch_size)
-
-        runner.log_buffer.clear()
-        # a dirty walkround to change the line at the end of pbar
-        if rank == 0:
-            sys.stdout.write('\n')
-            for metric in self.metrics:
-                with torch.no_grad():
-                    metric.summary()
-                for name, val in metric._result_dict.items():
-                    runner.log_buffer.output[name] = val
-
-                    # record best metric and save the best ckpt
-                    if self.save_best_ckpt and name in self.best_metric:
-                        self._save_best_ckpt(runner, val, name)
-
-            runner.log_buffer.ready = True
-        runner.model.train()
-
-        # clear all current states for next evaluation
-        for metric in self.metrics:
-            metric.clear()
 
-    def _save_best_ckpt(self, runner, new_score, metric_name):
-        """Save checkpoint with best metric score.
+        losses_dict = dict()
+        losses_dict['loss_disc_fake'] = disc_pred_fake.mean()
+        losses_dict['loss_disc_real'] = -disc_pred_real.mean()
+
+        # gradient penalty
+        batch_size = real_data.size(0)
+        alpha = torch.rand(batch_size, 1, 1, 1).to(real_data)
+
+        # interpolate between real_data and fake_data
+        interpolates = alpha * real_data + (1. - alpha) * fake_data
+        interpolates = autograd.Variable(interpolates, requires_grad=True)
+
+        disc_interpolates = self.discriminator(
+            interpolates,
+            curr_scale=self.curr_scale[0],
+            transition_weight=self._curr_transition_weight)
+        gradients = autograd.grad(
+            outputs=disc_interpolates,
+            inputs=interpolates,
+            grad_outputs=torch.ones_like(disc_interpolates),
+            create_graph=True,
+            retain_graph=True,
+            only_inputs=True)[0]
+        # norm_mode is 'HWC'
+        gradients_penalty = ((
+            gradients.reshape(batch_size, -1).norm(2, dim=1) - 1)**2).mean()
+        losses_dict['loss_gp'] = 10 * gradients_penalty
+        losses_dict['loss_disc_shift'] = 0.001 * 0.5 * (
+            disc_pred_fake**2 + disc_pred_real**2)
+
+        parsed_loss, log_vars = self.parse_losses(losses_dict)
+        return parsed_loss, log_vars
+
+    def train_generator(self, inputs: Tensor,
+                        data_samples: List[GenDataSample],
+                        optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        real_imgs = inputs
+        num_batches = real_imgs.shape[0]
+        noise_batch = self.noise_fn(num_batches=num_batches)
+
+        fake_imgs = self.generator(
+            noise_batch,
+            num_batches=num_batches,
+            curr_scale=self.curr_scale[0],
+            transition_weight=self._curr_transition_weight)
+        disc_pred_fake_g = self.discriminator(
+            fake_imgs,
+            curr_scale=self.curr_scale[0],
+            transition_weight=self._curr_transition_weight)
+
+        parsed_loss, log_vars = self.gen_loss(disc_pred_fake_g)
+        optimizer_wrapper.update_params(parsed_loss)
+        return log_vars
+
+    def gen_loss(self, disc_pred_fake: Tensor) -> Tuple[Tensor, dict]:
+        r"""Generator loss for PGGAN. PGGAN use WGAN's loss to train the
+        generator.
+
+        .. math:
+            L_{G} = -\mathbb{E}_{z\sim{p_{z}}}D\left\(G\left\(z\right\)\right\)
+                + L_{MSE}
 
         Args:
-            runner (``mmcv.runner.BaseRunner``): The runner.
-            new_score (float): New metric score.
-            metric_name (str): Name of metric.
-        """
-        curr_iter = f'iter_{runner.iter + 1}'
+            disc_pred_fake (Tensor): Discriminator's prediction of the fake
+                images.
+            recon_imgs (Tensor): Reconstructive images.
 
-        if self.compare_func[metric_name](new_score,
-                                          self._curr_best_score[metric_name]):
-            best_ckpt_name = f'best_{metric_name}_{curr_iter}.pth'
-            runner.meta['hook_msgs'][f'best_score_{metric_name}'] = new_score
-
-            if self._curr_best_ckpt_path[metric_name] and osp.isfile(
-                    self._curr_best_ckpt_path[metric_name]):
-                os.remove(self._curr_best_ckpt_path[metric_name])
-
-            self._curr_best_ckpt_path[metric_name] = osp.join(
-                runner.work_dir, best_ckpt_name)
-            runner.save_checkpoint(
-                runner.work_dir, best_ckpt_name, create_symlink=False)
-            runner.meta['hook_msgs'][
-                f'best_ckpt_{metric_name}'] = self._curr_best_ckpt_path[
-                    metric_name]
-
-            self._curr_best_score[metric_name] = new_score
-            runner.logger.info(
-                f'Now best checkpoint is saved as {best_ckpt_name}.')
-            runner.logger.info(f'Best {metric_name} is {new_score:0.4f} '
-                               f'at {curr_iter}.')
-
-
-@HOOKS.register_module()
-class TranslationEvalHook(GenerativeEvalHook):
-    """Evaluation Hook for Translation Models.
-
-    This evaluation hook can be used to evaluate translation models. Note
-    that only ``FID`` and ``IS`` metric are supported for the distributed
-    training now. In the future, we will support more metrics for the
-    evaluation during the training procedure.
-
-    In our config system, you only need to add `evaluation` with the detailed
-    configureations. Below is several usage cases for different situations.
-    What you need to do is to add these lines at the end of your config file.
-    Then, you can use this evaluation hook in the training procedure.
-
-    To be noted that, this evaluation hook support evaluation with dynamic
-    intervals for FID or other metrics may fluctuate frequently at the end of
-    the training process.
-
-    # TODO: fix the online doc
-
-    #. Only use FID for evaluation
-
-    .. code-blcok:: python
-        :linenos
-
-        evaluation = dict(
-            type='TranslationEvalHook',
-            target_domain='photo',
-            interval=10000,
-            metrics=dict(type='FID', num_images=106, bgr2rgb=True))
-
-    #. Use FID and IS simultaneously and save the best checkpoints respectively
-
-    .. code-block:: python
-        :linenos
-
-        evaluation = dict(
-            type='TranslationEvalHook',
-            target_domain='photo',
-            interval=10000,
-            metrics=[
-                dict(type='FID', num_images=106, bgr2rgb=True),
-                dict(
-                    type='IS',
-                    num_images=106,
-                    inception_args=dict(type='pytorch'))
-            ],
-            best_metric=['fid', 'is'])
-
-    #. Use dynamic evaluation intervals
-
-    .. code-block:: python
-        :linenos
-
-        # interval = 10000 if iter < 100000,
-        # interval = 4000, if 100000 <= iter < 200000,
-        # interval = 2000, if iter >= 200000
-
-        evaluation = dict(
-            type='TranslationEvalHook',
-            interval=dict(milestones=[100000, 200000],
-                          interval=[10000, 4000, 2000]),
-            target_domain='zebra',
-            metrics=[
-                dict(type='FID', num_images=140, bgr2rgb=True),
-                dict(type='IS', num_images=140)
-            ],
-            best_metric=['fid', 'is'])
+        Returns:
+            Tuple[Tensor, dict]: Loss value and a dict of log variables.
+        """
+        losses_dict = dict()
+        losses_dict['loss_gen'] = -disc_pred_fake.mean()
+        loss, log_vars = self.parse_losses(losses_dict)
+        return loss, log_vars
+
+    def train_step(self, data: dict, optim_wrapper: OptimWrapperDict):
+        """Train step function.
+
+        This function implements the standard training iteration for
+        asynchronous adversarial training. Namely, in each iteration, we first
+        update discriminator and then compute loss for generator with the newly
+        updated discriminator.
 
+        As for distributed training, we use the ``reducer`` from ddp to
+        synchronize the necessary params in current computational graph.
 
-    Args:
-        target_domain (str): Target domain of output image.
-    """
+        Args:
+            data_batch (dict): Input data from dataloader.
+            optimizer (dict): Dict contains optimizer for generator and
+                discriminator.
+            ddp_reducer (:obj:`Reducer` | None, optional): Reducer from ddp.
+                It is used to prepare for ``backward()`` in ddp. Defaults to
+                None.
+            running_status (dict | None, optional): Contains necessary basic
+                information for training, e.g., iteration number. Defaults to
+                None.
 
-    def __init__(self, *args, target_domain, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.target_domain = target_domain
+        Returns:
+            dict: Contains 'log_vars', 'num_samples', and 'results'.
+        """
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
 
-    def after_train_iter(self, runner):
-        """The behavior after each train iteration.
+        # update current stage
+        self.curr_stage = int(
+            min(
+                sum(self.cum_nkimgs <= self.shown_nkimg.item()),
+                len(self.scales) - 1))
+        self.curr_scale = self.scales[self.curr_stage]
+        self._curr_scale_int = self._next_scale_int.clone()
+
+        if self.curr_stage != self.prev_stage:
+            self.prev_stage = self.curr_stage
+            self._actual_nkimgs.append(self.shown_nkimg.item())
+
+        data = self.data_preprocessor(data, True)
+        inputs, data_sample = data['inputs'], data['data_samples']
+        if isinstance(inputs, dict):
+            real_imgs = inputs['img']
+        else:  # tensor
+            real_imgs = inputs
+
+        curr_scale = str(self.curr_scale[0])
+        disc_optimizer_wrapper: OptimWrapper = optim_wrapper[
+            f'discriminator_{curr_scale}']
+        gen_optimizer_wrapper: OptimWrapper = optim_wrapper[
+            f'generator_{curr_scale}']
+        disc_accu_iters = disc_optimizer_wrapper._accumulative_counts
+
+        # update training configs, like transition weight for torgb layers.
+        # get current transition weight for interpolating two torgb layers
+        if self.curr_stage == 0:
+            transition_weight = 1.
+        else:
+            transition_weight = (
+                self.shown_nkimg.item() -
+                self._actual_nkimgs[-1]) / self.transition_kimgs
+            # clip to [0, 1]
+            transition_weight = min(max(transition_weight, 0.), 1.)
+        self._curr_transition_weight = torch.tensor(transition_weight).to(
+            self._curr_transition_weight)
+
+        if real_imgs.shape[2:] == self.curr_scale:
+            pass
+        elif real_imgs.shape[2] >= self.curr_scale[0] and real_imgs.shape[
+                3] >= self.curr_scale[1]:
+            real_imgs = self.interp_real_to(real_imgs, size=self.curr_scale)
+        else:
+            raise RuntimeError(
+                f'The scale of real image {real_imgs.shape[2:]} is smaller '
+                f'than current scale {self.curr_scale}.')
+
+        # normal gan training process
+        with disc_optimizer_wrapper.optim_context(self.discriminator):
+            log_vars = self.train_discriminator(real_imgs, data_sample,
+                                                disc_optimizer_wrapper)
+
+        # add 1 to `curr_iter` because iter is updated in train loop.
+        # Whether to update the generator. We update generator with
+        # discriminator is fully updated for `self.n_discriminator_steps`
+        # iterations. And one full updating for discriminator contains
+        # `disc_accu_counts` times of grad accumulations.
+        if (curr_iter + 1) % (self.discriminator_steps * disc_accu_iters) == 0:
+            set_requires_grad(self.discriminator, False)
+            gen_accu_iters = gen_optimizer_wrapper._accumulative_counts
+
+            log_vars_gen_list = []
+            # init optimizer wrapper status for generator manually
+            gen_optimizer_wrapper.initialize_count_status(
+                self.generator, 0, self.generator_steps * gen_accu_iters)
+            for _ in range(self.generator_steps * gen_accu_iters):
+                with gen_optimizer_wrapper.optim_context(self.generator):
+                    log_vars_gen = self.train_generator(
+                        real_imgs, data_sample, gen_optimizer_wrapper)
+
+                log_vars_gen_list.append(log_vars_gen)
+            log_vars_gen = gather_log_vars(log_vars_gen_list)
+            log_vars_gen.pop('loss', None)  # remove 'loss' from gen logs
+
+            set_requires_grad(self.discriminator, True)
+
+            # only do ema after generator update
+            if self.with_ema_gen and (curr_iter + 1) >= (
+                    self.ema_start * self.discriminator_steps *
+                    disc_accu_iters):
+                self.generator_ema.update_parameters(
+                    self.generator.module
+                    if is_model_wrapper(self.generator) else self.generator)
+                # if not update buffer, copy buffer from orig model
+                if not self.generator_ema.update_buffers:
+                    self.generator_ema.sync_buffers(
+                        self.generator.module if is_model_wrapper(
+                            self.generator) else self.generator)
+            elif self.with_ema_gen:
+                # before ema, copy weights from orig
+                self.generator_ema.sync_parameters(
+                    self.generator.module
+                    if is_model_wrapper(self.generator) else self.generator)
+
+            log_vars.update(log_vars_gen)
+
+        # add batch size info to log_vars
+        _batch_size = real_imgs.shape[0] * get_world_size()
+        self.shown_nkimg += (_batch_size / 1000.)
+
+        log_vars.update(
+            dict(
+                shown_nkimg=self.shown_nkimg.item(),
+                curr_scale=self.curr_scale[0],
+                transition_weight=transition_weight))
+
+        # check if a new scale will be added in the next iteration
+        _curr_stage = int(
+            min(
+                sum(self.cum_nkimgs <= self.shown_nkimg.item()),
+                len(self.scales) - 1))
+        # in the next iteration, we will switch to a new scale
+        if _curr_stage != self.curr_stage:
+            # `self._next_scale_int` is updated at the end of `train_step`
+            self._next_scale_int = self._next_scale_int * 2
 
-        Args:
-            runner (``mmcv.runner.BaseRunner``): The runner.
-        """
-        interval = self.get_current_interval(runner)
-        if not self.every_n_iters(runner, interval):
-            return
-
-        runner.model.eval()
-        source_domain = runner.model.module.get_other_domains(
-            self.target_domain)[0]
-        # feed real images
-        max_num_images = max(metric.num_images for metric in self.metrics)
-        for metric in self.metrics:
-            if metric.num_real_feeded >= metric.num_real_need:
-                continue
-            mmcv.print_log(f'Feed reals to {metric.name} metric.', 'mmgen')
-            # feed in real images
-            for data in self.dataloader:
-                # key for translation model
-                if f'img_{self.target_domain}' in data:
-                    reals = data[f'img_{self.target_domain}']
-                # key for conditional GAN
-                else:
-                    raise KeyError(
-                        'Cannot found key for images in data_dict. ')
-                num_feed = metric.feed(reals, 'reals')
-                if num_feed <= 0:
-                    break
-
-        mmcv.print_log(f'Sample {max_num_images} fake images for evaluation',
-                       'mmgen')
-
-        rank, ws = get_dist_info()
-
-        # define mmcv progress bar
-        if rank == 0:
-            pbar = mmcv.ProgressBar(max_num_images)
-
-        # feed in fake images
-        for data in self.dataloader:
-            # key for translation model
-            if f'img_{source_domain}' in data:
-                with torch.no_grad():
-                    output_dict = runner.model(
-                        data[f'img_{source_domain}'],
-                        test_mode=True,
-                        target_domain=self.target_domain,
-                        **self.sample_kwargs)
-                fakes = output_dict['target']
-            # key Error
-            else:
-                raise KeyError('Cannot found key for images in data_dict. ')
-            # sampling fake images and directly send them to metrics
-            # pbar update number for one proc
-            num_update = 0
-            for metric in self.metrics:
-                if metric.num_fake_feeded >= metric.num_fake_need:
-                    continue
-                num_feed = metric.feed(fakes, 'fakes')
-                num_update = max(num_update, num_feed)
-                if num_feed <= 0:
-                    break
-
-            if rank == 0:
-                if num_update > 0:
-                    pbar.update(num_update * ws)
-
-        runner.log_buffer.clear()
-        # a dirty walkround to change the line at the end of pbar
-        if rank == 0:
-            sys.stdout.write('\n')
-            for metric in self.metrics:
-                with torch.no_grad():
-                    metric.summary()
-                for name, val in metric._result_dict.items():
-                    runner.log_buffer.output[name] = val
-
-                    # record best metric and save the best ckpt
-                    if self.save_best_ckpt and name in self.best_metric:
-                        self._save_best_ckpt(runner, val, name)
-
-            runner.log_buffer.ready = True
-        runner.model.train()
-
-        # clear all current states for next evaluation
-        for metric in self.metrics:
-            metric.clear()
+        return log_vars
```

### Comparing `mmgen-0.7.3/mmgen/core/evaluation/metric_utils.py` & `mmgen-1.0.0rc0/mmgen/models/gans/mspie_stylegan2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,283 +1,210 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import sys
+from copy import deepcopy
+from typing import Dict, List, Union
 
-import mmcv
 import numpy as np
 import torch
+import torch.distributed as dist
+import torch.nn as nn
 import torch.nn.functional as F
-from mmcv.parallel import is_module_wrapper
+from mmengine import MessageHub
+from mmengine.logging import MMLogger
+from mmengine.model import is_model_wrapper
+from mmengine.optim import OptimWrapper, OptimWrapperDict
+from torch import Tensor
+
+from mmgen.registry import MODELS
+from mmgen.structures import GenDataSample
+from ..common import gather_log_vars, set_requires_grad
+from ..gans.stylegan2 import StyleGAN2
+
+ModelType = Union[Dict, nn.Module]
+TrainInput = Union[dict, Tensor]
+
+
+@MODELS.register_module()
+class MSPIEStyleGAN2(StyleGAN2):
+    """MS-PIE StyleGAN2.
+
+    In this GAN, we adopt the MS-PIE training schedule so that multi-scale
+    images can be generated with a single generator. Details can be found in:
+    Positional Encoding as Spatial Inductive Bias in GANs, CVPR2021.
+
+    Args:
+        train_settings (dict): Config for training settings.
+            Defaults to `dict()`.
+    """
+
+    def __init__(self, *args, train_settings=dict(), **kwargs):
+        super().__init__(*args, **kwargs)
+        self.train_settings = deepcopy(train_settings)
+        # set the number of upsampling blocks. This value will be used to
+        # calculate the current result size according to the size of the input
+        # feature map, e.g., positional encoding map
+        self.num_upblocks = self.train_settings.get('num_upblocks', 6)
+
+        # multiple input scales (a list of int) that will be added to the
+        # original starting scale.
+        self.multi_input_scales = self.train_settings.get('multi_input_scales')
+        self.multi_scale_probability = self.train_settings.get(
+            'multi_scale_probability')
+
+    def train_step(self, data: dict,
+                   optim_wrapper: OptimWrapperDict) -> Dict[str, Tensor]:
+        """Train GAN model. In the training of GAN models, generator and
+        discriminator are updated alternatively. In MMGeneration's design,
+        `self.train_step` is called with data input. Therefore we always update
+        discriminator, whose updating is relay on real data, and then determine
+        if the generator needs to be updated based on the current number of
+        iterations. More details about whether to update generator can be found
+        in :meth:`should_gen_update`.
+
+        Args:
+            data (dict): Data sampled from dataloader.
+            optim_wrapper (OptimWrapperDict): OptimWrapperDict instance
+                contains OptimWrapper of generator and discriminator.
+
+        Returns:
+            Dict[str, torch.Tensor]: A ``dict`` of tensor for logging.
+        """
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
+        data = self.data_preprocessor(data, True)
+
+        disc_optimizer_wrapper: OptimWrapper = optim_wrapper['discriminator']
+        disc_accu_iters = disc_optimizer_wrapper._accumulative_counts
+
+        with disc_optimizer_wrapper.optim_context(self.discriminator):
+            log_vars = self.train_discriminator(
+                **data, optimizer_wrapper=disc_optimizer_wrapper)
+
+        # add 1 to `curr_iter` because iter is updated in train loop.
+        # Whether to update the generator. We update generator with
+        # discriminator is fully updated for `self.n_discriminator_steps`
+        # iterations. And one full updating for discriminator contains
+        # `disc_accu_counts` times of grad accumulations.
+        if (curr_iter + 1) % (self.discriminator_steps * disc_accu_iters) == 0:
+            set_requires_grad(self.discriminator, False)
+            gen_optimizer_wrapper = optim_wrapper['generator']
+            gen_accu_iters = gen_optimizer_wrapper._accumulative_counts
+
+            log_vars_gen_list = []
+            # init optimizer wrapper status for generator manually
+            gen_optimizer_wrapper.initialize_count_status(
+                self.generator, 0, self.generator_steps * gen_accu_iters)
+            for _ in range(self.generator_steps * gen_accu_iters):
+                with gen_optimizer_wrapper.optim_context(self.generator):
+                    log_vars_gen = self.train_generator(
+                        **data, optimizer_wrapper=gen_optimizer_wrapper)
+
+                log_vars_gen_list.append(log_vars_gen)
+            log_vars_gen = gather_log_vars(log_vars_gen_list)
+            log_vars_gen.pop('loss', None)  # remove 'loss' from gen logs
+
+            set_requires_grad(self.discriminator, True)
+
+            # only do ema after generator update
+            if self.with_ema_gen and (curr_iter + 1) >= (
+                    self.ema_start * self.discriminator_steps *
+                    disc_accu_iters):
+                self.generator_ema.update_parameters(
+                    self.generator.module
+                    if is_model_wrapper(self.generator) else self.generator)
+                # if not update buffer, copy buffer from orig model
+                if not self.generator_ema.update_buffers:
+                    self.generator_ema.sync_buffers(
+                        self.generator.module if is_model_wrapper(
+                            self.generator) else self.generator)
+            elif self.with_ema_gen:
+                # before ema, copy weights from orig
+                self.generator_ema.sync_parameters(
+                    self.generator.module
+                    if is_model_wrapper(self.generator) else self.generator)
+
+            log_vars.update(log_vars_gen)
+
+        return log_vars
+
+    def train_generator(self, inputs: dict, data_samples: List[GenDataSample],
+                        optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        """Train generator.
+
+        Args:
+            inputs (TrainInput): Inputs from dataloader.
+            data_samples (List[GenDataSample]): Data samples from dataloader.
+                Do not used in generator's training.
+            optim_wrapper (OptimWrapper): OptimWrapper instance used to update
+                model parameters.
+
+        Returns:
+            Dict[str, Tensor]: A ``dict`` of tensor for logging.
+        """
+        # num_batches = inputs['real_imgs'].shape[0]
+        num_batches = inputs['img'].shape[0]
+
+        noise = self.noise_fn(num_batches=num_batches)
+        fake_imgs = self.generator(
+            noise, return_noise=False, chosen_scale=self.chosen_scale)
+
+        disc_pred_fake = self.discriminator(fake_imgs)
+        parsed_loss, log_vars = self.gen_loss(disc_pred_fake, num_batches)
+
+        optimizer_wrapper.update_params(parsed_loss)
+        return log_vars
+
+    def train_discriminator(
+            self, inputs: dict, data_samples: List[GenDataSample],
+            optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        """Train discriminator.
+
+        Args:
+            inputs (TrainInput): Inputs from dataloader.
+            data_samples (List[GenDataSample]): Data samples from dataloader.
+            optim_wrapper (OptimWrapper): OptimWrapper instance used to update
+                model parameters.
+        Returns:
+            Dict[str, Tensor]: A ``dict`` of tensor for logging.
+        """
+        real_imgs = inputs['img']
+
+        if dist.is_initialized():
+            # randomly sample a scale for current training iteration
+            chosen_scale = np.random.choice(self.multi_input_scales, 1,
+                                            self.multi_scale_probability)[0]
+
+            chosen_scale = torch.tensor(chosen_scale, dtype=torch.int).cuda()
+            dist.broadcast(chosen_scale, 0)
+            chosen_scale = int(chosen_scale.item())
 
-from mmgen.models.architectures.common import get_module_device
-
-
-@torch.no_grad()
-def extract_inception_features(dataloader,
-                               inception,
-                               num_samples,
-                               inception_style='pytorch'):
-    """Extract inception features for FID metric.
-
-    Args:
-        dataloader (:obj:`DataLoader`): Dataloader for images.
-        inception (nn.Module): Inception network.
-        num_samples (int): The number of samples to be extracted.
-        inception_style (str): The style of Inception network, "pytorch" or
-            "stylegan". Defaults to "pytorch".
-
-    Returns:
-        torch.Tensor: Inception features.
-    """
-    batch_size = dataloader.batch_size
-    num_iters = num_samples // batch_size
-    if num_iters * batch_size < num_samples:
-        num_iters += 1
-    # define mmcv progress bar
-    pbar = mmcv.ProgressBar(num_iters)
-
-    feature_list = []
-    curr_iter = 1
-    for data in dataloader:
-        # a dirty walkround to support multiple datasets (mainly for the
-        # unconditional dataset and conditional dataset). In our
-        # implementation, unconditioanl dataset will return real images with
-        # the key "real_img". However, the conditional dataset contains a key
-        # "img" denoting the real images.
-        if 'real_img' in data:
-            # Mainly for the unconditional dataset in our MMGeneration
-            img = data['real_img']
         else:
-            # Mainly for conditional dataset in MMClassification
-            img = data['img']
-        pbar.update()
-
-        # the inception network is not wrapped with module wrapper.
-        if not is_module_wrapper(inception):
-            # put the img to the module device
-            img = img.to(get_module_device(inception))
-
-        if inception_style == 'stylegan':
-            img = (img * 127.5 + 128).clamp(0, 255).to(torch.uint8)
-            feature = inception(img, return_features=True)
-        else:
-            feature = inception(img)[0].view(img.shape[0], -1)
-        feature_list.append(feature.to('cpu'))
-
-        if curr_iter >= num_iters:
-            break
-        curr_iter += 1
-
-    # Attention: the number of features may be different as you want.
-    features = torch.cat(feature_list, 0)
-
-    assert features.shape[0] >= num_samples
-    features = features[:num_samples]
-
-    # to change the line after pbar
-    sys.stdout.write('\n')
-    return features
-
-
-def _hox_downsample(img):
-    r"""Downsample images with factor equal to 0.5.
-
-    Ref: https://github.com/tkarras/progressive_growing_of_gans/blob/master/metrics/ms_ssim.py  # noqa
-
-    Args:
-        img (ndarray): Images with order "NHWC".
-
-    Returns:
-        ndarray: Downsampled images with order "NHWC".
-    """
-    return (img[:, 0::2, 0::2, :] + img[:, 1::2, 0::2, :] +
-            img[:, 0::2, 1::2, :] + img[:, 1::2, 1::2, :]) * 0.25
-
-
-def _f_special_gauss(size, sigma):
-    r"""Return a circular symmetric gaussian kernel.
-
-    Ref: https://github.com/tkarras/progressive_growing_of_gans/blob/master/metrics/ms_ssim.py  # noqa
-
-    Args:
-        size (int): Size of Gaussian kernel.
-        sigma (float): Standard deviation for Gaussian blur kernel.
-
-    Returns:
-        ndarray: Gaussian kernel.
-    """
-    radius = size // 2
-    offset = 0.0
-    start, stop = -radius, radius + 1
-    if size % 2 == 0:
-        offset = 0.5
-        stop -= 1
-    x, y = np.mgrid[offset + start:stop, offset + start:stop]
-    assert len(x) == size
-    g = np.exp(-((x**2 + y**2) / (2.0 * sigma**2)))
-    return g / g.sum()
-
-
-# Gaussian blur kernel
-def get_gaussian_kernel():
-    kernel = np.array([[1, 4, 6, 4, 1], [4, 16, 24, 16, 4], [6, 24, 36, 24, 6],
-                       [4, 16, 24, 16, 4], [1, 4, 6, 4, 1]],
-                      np.float32) / 256.0
-    gaussian_k = torch.as_tensor(kernel.reshape(1, 1, 5, 5))
-    return gaussian_k
-
-
-def get_pyramid_layer(image, gaussian_k, direction='down'):
-    gaussian_k = gaussian_k.to(image.device)
-    if direction == 'up':
-        image = F.interpolate(image, scale_factor=2)
-    multiband = [
-        F.conv2d(
-            image[:, i:i + 1, :, :],
-            gaussian_k,
-            padding=2,
-            stride=1 if direction == 'up' else 2) for i in range(3)
-    ]
-    image = torch.cat(multiband, dim=1)
-    return image
-
-
-def gaussian_pyramid(original, n_pyramids, gaussian_k):
-    x = original
-    # pyramid down
-    pyramids = [original]
-    for _ in range(n_pyramids):
-        x = get_pyramid_layer(x, gaussian_k)
-        pyramids.append(x)
-    return pyramids
-
-
-def laplacian_pyramid(original, n_pyramids, gaussian_k):
-    """Calculate Laplacian pyramid.
-
-    Ref: https://github.com/koshian2/swd-pytorch/blob/master/swd.py
-
-    Args:
-        original (Tensor): Batch of Images with range [0, 1] and order "NCHW"
-        n_pyramids (int): Levels of pyramids minus one.
-        gaussian_k (Tensor): Gaussian kernel with shape (1, 1, 5, 5).
-
-    Return:
-        list[Tensor]. Laplacian pyramids of original.
-    """
-    # create gaussian pyramid
-    pyramids = gaussian_pyramid(original, n_pyramids, gaussian_k)
-
-    # pyramid up - diff
-    laplacian = []
-    for i in range(len(pyramids) - 1):
-        diff = pyramids[i] - get_pyramid_layer(pyramids[i + 1], gaussian_k,
-                                               'up')
-        laplacian.append(diff)
-    # Add last gaussian pyramid
-    laplacian.append(pyramids[len(pyramids) - 1])
-    return laplacian
-
-
-def get_descriptors_for_minibatch(minibatch, nhood_size, nhoods_per_image):
-    r"""Get descriptors of one level of pyramids.
-
-    Ref: https://github.com/tkarras/progressive_growing_of_gans/blob/master/metrics/sliced_wasserstein.py  # noqa
-
-    Args:
-        minibatch (Tensor): Pyramids of one level with order "NCHW".
-        nhood_size (int): Pixel neighborhood size.
-        nhoods_per_image (int): The number of descriptors per image.
-
-    Return:
-        Tensor: Descriptors of images from one level batch.
-    """
-    S = minibatch.shape  # (minibatch, channel, height, width)
-    assert len(S) == 4 and S[1] == 3
-    N = nhoods_per_image * S[0]
-    H = nhood_size // 2
-    nhood, chan, x, y = np.ogrid[0:N, 0:3, -H:H + 1, -H:H + 1]
-    img = nhood // nhoods_per_image
-    x = x + np.random.randint(H, S[3] - H, size=(N, 1, 1, 1))
-    y = y + np.random.randint(H, S[2] - H, size=(N, 1, 1, 1))
-    idx = ((img * S[1] + chan) * S[2] + y) * S[3] + x
-    return minibatch.view(-1)[idx]
-
-
-def finalize_descriptors(desc):
-    r"""Normalize and reshape descriptors.
-
-    Ref: https://github.com/tkarras/progressive_growing_of_gans/blob/master/metrics/sliced_wasserstein.py  # noqa
-
-    Args:
-        desc (list or Tensor): List of descriptors of one level.
-
-    Return:
-        Tensor: Descriptors after normalized along channel and flattened.
-    """
-    if isinstance(desc, list):
-        desc = torch.cat(desc, dim=0)
-    assert desc.ndim == 4  # (neighborhood, channel, height, width)
-    desc -= torch.mean(desc, dim=(0, 2, 3), keepdim=True)
-    desc /= torch.std(desc, dim=(0, 2, 3), keepdim=True)
-    desc = desc.reshape(desc.shape[0], -1)
-    return desc
-
-
-def compute_pr_distances(row_features,
-                         col_features,
-                         num_gpus,
-                         rank,
-                         col_batch_size=10000):
-    r"""Compute distances between real images and fake images.
-
-    This function is used for calculate Precision and Recall metric.
-    Refer to:https://github.com/NVlabs/stylegan2-ada-pytorch/blob/main/metrics/precision_recall.py  # noqa
-    """
-    assert 0 <= rank < num_gpus
-    num_cols = col_features.shape[0]
-    num_batches = ((num_cols - 1) // col_batch_size // num_gpus + 1) * num_gpus
-    col_batches = torch.nn.functional.pad(
-        col_features, [0, 0, 0, -num_cols % num_batches]).chunk(num_batches)
-    dist_batches = []
-    for col_batch in col_batches[rank::num_gpus]:
-        dist_batch = torch.cdist(
-            row_features.unsqueeze(0), col_batch.unsqueeze(0))[0]
-        for src in range(num_gpus):
-            dist_broadcast = dist_batch.clone()
-            if num_gpus > 1:
-                torch.distributed.broadcast(dist_broadcast, src=src)
-            dist_batches.append(dist_broadcast.cpu() if rank == 0 else None)
-    return torch.cat(dist_batches, dim=1)[:, :num_cols] if rank == 0 else None
-
-
-def normalize(a):
-    """L2 normalization.
-
-    Args:
-        a (Tensor): Tensor with shape [N, C].
-
-    Returns:
-        Tensor: Tensor after L2 normalization per-instance.
-    """
-    return a / torch.norm(a, dim=1, keepdim=True)
-
-
-def slerp(a, b, percent):
-    """Spherical linear interpolation between two unnormalized vectors.
-
-    Args:
-        a (Tensor): Tensor with shape [N, C].
-        b (Tensor): Tensor with shape [N, C].
-        percent (float|Tensor): A float or tensor with shape broadcastable to
-            the shape of input Tensors.
-
-    Returns:
-        Tensor: Spherical linear interpolation result with shape [N, C].
-    """
-    a = normalize(a)
-    b = normalize(b)
-    d = (a * b).sum(-1, keepdim=True)
-    p = percent * torch.acos(d)
-    c = normalize(b - d * a)
-    d = a * torch.cos(p) + c * torch.sin(p)
-
-    return normalize(d)
+            logger = MMLogger.get_current_instance()
+            logger.info(
+                'Distributed training has not been initialized. Degrade to '
+                'the standard stylegan2')
+            chosen_scale = 0
+
+        curr_size = (4 + chosen_scale) * (2**self.num_upblocks)
+        # adjust the shape of images
+        if real_imgs.shape[-2:] != (curr_size, curr_size):
+            real_imgs = F.interpolate(
+                real_imgs,
+                size=(curr_size, curr_size),
+                mode='bilinear',
+                align_corners=True)
+
+        num_batches = real_imgs.shape[0]
+
+        noise_batch = self.noise_fn(num_batches=num_batches)
+        with torch.no_grad():
+            fake_imgs = self.generator(
+                noise_batch, return_noise=False, chosen_scale=chosen_scale)
+        # store chosen scale for training generator
+        setattr(self, 'chosen_scale', chosen_scale)
+
+        disc_pred_fake = self.discriminator(fake_imgs)
+        disc_pred_real = self.discriminator(real_imgs)
+
+        parsed_losses, log_vars = self.disc_loss(disc_pred_fake,
+                                                 disc_pred_real, real_imgs)
+        optimizer_wrapper.update_params(parsed_losses)
+        return log_vars
```

### Comparing `mmgen-0.7.3/mmgen/core/hooks/pickle_data_hook.py` & `mmgen-1.0.0rc0/mmgen/engine/hooks/pickle_data_hook.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+
 import logging
 import os
 import pickle
+from typing import List, Optional, Sequence, Tuple
 
-import mmcv
+import numpy as np
 import torch
-from mmcv.runner import HOOKS, Hook
-from mmcv.runner.dist_utils import master_only
+from mmengine import is_list_of, mkdir_or_exist, print_log
+from mmengine.dist import master_only
+from mmengine.hooks import Hook
+from mmengine.runner import Runner
+from torch import Tensor
+
+from mmgen.registry import HOOKS
+
+DATA_BATCH = Optional[Sequence[dict]]
 
 
 @HOOKS.register_module()
 class PickleDataHook(Hook):
     """Pickle Useful Data Hook.
 
     This hook will be used in SinGAN training for saving some important data
     that will be used in testing or inference.
 
     Args:
         output_dir (str): The output path for saving pickled data.
         data_name_list (list[str]): The list contains the name of results in
             outputs dict.
         interval (int): The interval of calling this hook. If set to -1,
-            the visualization hook will not be called. Default: -1.
+            the PickleDataHook will not be called during training. Default: -1.
         before_run (bool, optional): Whether to save before running.
             Defaults to False.
         after_run (bool, optional): Whether to save after running.
             Defaults to False.
         filename_tmpl (str, optional): Format string used to save images. The
             output file name will be formatted as this args.
             Defaults to 'iter_{}.pkl'.
@@ -34,15 +43,15 @@
     def __init__(self,
                  output_dir,
                  data_name_list,
                  interval=-1,
                  before_run=False,
                  after_run=False,
                  filename_tmpl='iter_{}.pkl'):
-        assert mmcv.is_list_of(data_name_list, str)
+        assert is_list_of(data_name_list, str)
         self.output_dir = output_dir
         self.data_name_list = data_name_list
         self.interval = interval
         self.filename_tmpl = filename_tmpl
         self._before_run = before_run
         self._after_run = after_run
 
@@ -63,50 +72,76 @@
         Args:
             runner (object): The runner.
         """
         if self._before_run:
             self._pickle_data(runner)
 
     @master_only
-    def after_train_iter(self, runner):
+    def after_train_iter(self,
+                         runner,
+                         batch_idx: int,
+                         data_batch: DATA_BATCH = None,
+                         outputs: Optional[dict] = None):
         """The behavior after each train iteration.
 
         Args:
-            runner (object): The runner.
+            runner (Runner): The runner of the training process.
+            batch_idx (int): The index of the current batch in the train loop.
+            data_batch (Sequence[dict], optional): Data from dataloader.
+                Defaults to None.
+            outputs (dict, optional): Outputs from model.
+                Defaults to None.
         """
-        if not self.every_n_iters(runner, self.interval):
+        if not self.every_n_train_iters(runner, self.interval):
             return
         self._pickle_data(runner)
 
-    def _pickle_data(self, runner):
+    def _pickle_data(self, runner: Runner):
+        """Save target data to pickle file.
+
+        Args:
+            runner (Runner): The runner of the training process.
+        """
         filename = self.filename_tmpl.format(runner.iter + 1)
         if not hasattr(self, '_out_dir'):
             self._out_dir = os.path.join(runner.work_dir, self.output_dir)
-        mmcv.mkdir_or_exist(self._out_dir)
+        mkdir_or_exist(self._out_dir)
         file_path = os.path.join(self._out_dir, filename)
         with open(file_path, 'wb') as f:
-            data = runner.outputs['results']
+            module = runner.model
+            if hasattr(module, 'module'):
+                module = module.module
             not_find_keys = []
             data_dict = {}
             for k in self.data_name_list:
-                if k in data.keys():
-                    data_dict[k] = self._get_numpy_data(data[k])
+                if hasattr(module, k):
+                    data_dict[k] = self._get_numpy_data(getattr(module, k))
                 else:
                     not_find_keys.append(k)
             pickle.dump(data_dict, f)
-            mmcv.print_log(f'Pickle data in {filename}', 'mmgen')
+            print_log(f'Pickle data in {filename}', 'current')
 
             if len(not_find_keys) > 0:
-                mmcv.print_log(
+                print_log(
                     f'Cannot find keys for pickling: {not_find_keys}',
-                    'mmgen',
+                    'current',
                     level=logging.WARN)
             f.flush()
 
-    def _get_numpy_data(self, data):
+    def _get_numpy_data(
+        self, data: Tuple[List[Tensor], Tensor, int]
+    ) -> Tuple[List[np.ndarray], np.ndarray, int]:
+        """Convert tensor or list of tensor to numpy or list of numpy.
+
+        Args:
+            data (Tuple[List[Tensor], Tensor, int]): Data to be converted.
+
+        Returns:
+            Tuple[List[np.ndarray], np.ndarray, int]: Converted data.
+        """
         if isinstance(data, list):
             return [self._get_numpy_data(x) for x in data]
 
         if isinstance(data, torch.Tensor):
             return data.cpu().numpy()
 
         return data
```

### Comparing `mmgen-0.7.3/mmgen/core/hooks/visualize_training_samples.py` & `mmgen-1.0.0rc0/mmgen/models/gans/ggan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,122 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import os.path as osp
+from typing import Dict, List, Tuple
 
-import mmcv
 import torch
-from mmcv.runner import HOOKS, Hook
-from mmcv.runner.dist_utils import master_only
-from torchvision.utils import save_image
-
-
-@HOOKS.register_module()
-class VisualizeUnconditionalSamples(Hook):
-    """Visualization hook for unconditional GANs.
-
-    In this hook, we use the official api `save_image` in torchvision to save
-    the visualization results.
-
-    Args:
-        output_dir (str): The file path to store visualizations.
-        fixed_noise (bool, optional): Whether to use fixed noises in sampling.
-            Defaults to True.
-        num_samples (int, optional): The number of samples to show in
-            visualization. Defaults to 16.
-        interval (int): The interval of calling this hook. If set to -1,
-            the visualization hook will not be called. Default: -1.
-        filename_tmpl (str): Format string used to save images. The output file
-            name will be formatted as this args. Default: 'iter_{}.png'.
-        rerange (bool): Whether to rerange the output value from [-1, 1] to
-            [0, 1]. We highly recommend users should preprocess the
-            visualization results on their own. Here, we just provide a simple
-            interface. Default: True.
-        bgr2rgb (bool): Whether to reformat the channel dimension from BGR to
-            RGB. The final image we will save is following RGB style.
-            Default: True.
-        nrow (int): The number of samples in a row. Default: 1.
-        padding (int): The number of padding pixels between each samples.
-            Default: 4.
-        kwargs (dict | None, optional): Key-word arguments for sampling
-            function. Defaults to None.
+import torch.nn.functional as F
+from mmengine.optim import OptimWrapper
+from torch import Tensor
+
+from mmgen.registry import MODELS
+from mmgen.structures import GenDataSample
+from .base_gan import BaseGAN
+
+
+@MODELS.register_module()
+class GGAN(BaseGAN):
+    """Impelmentation of ``.
+
+    Paper link:
     """
 
-    def __init__(self,
-                 output_dir,
-                 fixed_noise=True,
-                 num_samples=16,
-                 interval=-1,
-                 filename_tmpl='iter_{}.png',
-                 rerange=True,
-                 bgr2rgb=True,
-                 nrow=4,
-                 padding=0,
-                 kwargs=None):
-        self.output_dir = output_dir
-        self.fixed_noise = fixed_noise
-        self.num_samples = num_samples
-        self.interval = interval
-        self.filename_tmpl = filename_tmpl
-        self.bgr2rgb = bgr2rgb
-        self.rerange = rerange
-        self.nrow = nrow
-        self.padding = padding
-
-        # the sampling noise will be initialized by the first sampling.
-        self.sampling_noise = None
-
-        self.kwargs = kwargs if kwargs is not None else dict()
-
-    @master_only
-    def after_train_iter(self, runner):
-        """The behavior after each train iteration.
+    def disc_loss(self, disc_pred_fake: Tensor,
+                  disc_pred_real: Tensor) -> Tuple:
+        r"""Get disc loss. GGAN use hinge loss to train
+        the discriminator.
+
+        .. math:
+            L_{D} = -\mathbb{E}_{\left(x, y\right)\sim{p}_{data}}
+                \left[\min\left(0, -1 + D\left(x, y\right)\right)\right]
+                -\mathbb{E}_{z\sim{p_{z}}, y\sim{p_{data}}}\left[\min
+                \left(0, -1 - D\left(G\left(z\right), y\right)\right)\right]
+
+        Args:
+            disc_pred_fake (Tensor): Discriminator's prediction of the fake
+                images.
+            disc_pred_real (Tensor): Discriminator's prediction of the real
+                images.
+
+        Returns:
+            tuple[Tensor, dict]: Loss value and a dict of log variables.
+        """
+        losses_dict = dict()
+        losses_dict['loss_disc_fake'] = F.relu(1 + disc_pred_fake).mean()
+        losses_dict['loss_disc_real'] = F.relu(1 - disc_pred_real).mean()
+
+        loss, log_var = self.parse_losses(losses_dict)
+        return loss, log_var
+
+    def gen_loss(self, disc_pred_fake):
+        r"""Get disc loss. GGAN use hinge loss to train
+        the generator.
+
+        .. math:
+            L_{G} = -\mathbb{E}_{z\sim{p_{z}}, y\sim{p_{data}}}
+                D\left(G\left(z\right), y\right)
+
+        Args:
+            disc_pred_fake (Tensor): Discriminator's prediction of the fake
+                images.
+
+        Returns:
+            tuple[Tensor, dict]: Loss value and a dict of log variables.
+        """
+        losses_dict = dict()
+        losses_dict['loss_gen'] = -disc_pred_fake.mean()
+        loss, log_var = self.parse_losses(losses_dict)
+        return loss, log_var
+
+    def train_discriminator(
+            self, inputs: dict, data_samples: List[GenDataSample],
+            optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        """Train discriminator.
 
         Args:
-            runner (object): The runner.
+            inputs (dict): Inputs from dataloader.
+            data_samples (List[GenDataSample]): Data samples from dataloader.
+            optim_wrapper (OptimWrapper): OptimWrapper instance used to update
+                model parameters.
+        Returns:
+            Dict[str, Tensor]: A ``dict`` of tensor for logging.
         """
-        if not self.every_n_iters(runner, self.interval):
-            return
-        # eval mode
-        runner.model.eval()
-        # no grad in sampling
+        real_imgs = inputs['img']
+
+        num_batches = real_imgs.shape[0]
+
+        noise_batch = self.noise_fn(num_batches=num_batches)
         with torch.no_grad():
-            outputs_dict = runner.model(
-                self.sampling_noise,
-                return_loss=False,
-                num_batches=self.num_samples,
-                return_noise=True,
-                **self.kwargs)
-            imgs = outputs_dict['fake_img']
-            noise_ = outputs_dict['noise_batch']
-        # initialize samling noise with the first returned noise
-        if self.sampling_noise is None and self.fixed_noise:
-            self.sampling_noise = noise_
-
-        # train mode
-        runner.model.train()
-
-        filename = self.filename_tmpl.format(runner.iter + 1)
-        if self.rerange:
-            imgs = ((imgs + 1) / 2)
-        if self.bgr2rgb and imgs.size(1) == 3:
-            imgs = imgs[:, [2, 1, 0], ...]
-        if imgs.size(1) == 1:
-            imgs = torch.cat([imgs, imgs, imgs], dim=1)
-        imgs = imgs.clamp_(0, 1)
-
-        mmcv.mkdir_or_exist(osp.join(runner.work_dir, self.output_dir))
-        save_image(
-            imgs,
-            osp.join(runner.work_dir, self.output_dir, filename),
-            nrow=self.nrow,
-            padding=self.padding)
+            fake_imgs = self.generator(noise=noise_batch, return_noise=False)
+
+        disc_pred_fake = self.discriminator(fake_imgs)
+        disc_pred_real = self.discriminator(real_imgs)
+
+        parsed_losses, log_vars = self.disc_loss(disc_pred_fake,
+                                                 disc_pred_real)
+        optimizer_wrapper.update_params(parsed_losses)
+        return log_vars
+
+    def train_generator(self, inputs: dict, data_samples: List[GenDataSample],
+                        optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        """Train generator.
+
+        Args:
+            inputs (dict): Inputs from dataloader.
+            data_samples (List[GenDataSample]): Data samples from dataloader.
+                Do not used in generator's training.
+            optim_wrapper (OptimWrapper): OptimWrapper instance used to update
+                model parameters.
+
+        Returns:
+            Dict[str, Tensor]: A ``dict`` of tensor for logging.
+        """
+        # num_batches = inputs['real_imgs'].shape[0]
+        num_batches = inputs['img'].shape[0]
+
+        # >>> new setting
+        noise = self.noise_fn(num_batches=num_batches)
+        fake_imgs = self.generator(noise=noise, return_noise=False)
+
+        disc_pred_fake = self.discriminator(fake_imgs)
+        parsed_loss, log_vars = self.gen_loss(disc_pred_fake)
+
+        optimizer_wrapper.update_params(parsed_loss)
+        return log_vars
```

### Comparing `mmgen-0.7.3/mmgen/core/registry.py` & `mmgen-1.0.0rc0/mmgen/models/builder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from mmcv.utils import Registry, build_from_cfg
+import torch.nn as nn
+from mmengine.registry import build_from_cfg
 
-METRICS = Registry('metric')
+from mmgen.registry import MODELS, MODULES
 
 
 def build(cfg, registry, default_args=None):
     """Build a module.
 
     Args:
         cfg (dict, list[dict]): The config of modules, is is either a dict
@@ -16,15 +17,20 @@
     Returns:
         nn.Module: A built nn module.
     """
     if isinstance(cfg, list):
         modules = [
             build_from_cfg(cfg_, registry, default_args) for cfg_ in cfg
         ]
-        return modules
+        return nn.ModuleList(modules)
 
     return build_from_cfg(cfg, registry, default_args)
 
 
-def build_metric(cfg):
-    """Build a metric calculator."""
-    return build(cfg, METRICS)
+def build_model(cfg, train_cfg=None, test_cfg=None):
+    """Build model (GAN)."""
+    return build(cfg, MODELS, dict(train_cfg=train_cfg, test_cfg=test_cfg))
+
+
+def build_module(cfg, default_args=None):
+    """Build a module or modules from a list."""
+    return build(cfg, MODULES, default_args)
```

### Comparing `mmgen-0.7.3/mmgen/core/runners/fp16_utils.py` & `mmgen-1.0.0rc0/mmgen/engine/runners/fp16_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import functools
 from collections import abc
 from inspect import getfullargspec
 
 import numpy as np
 import torch
 import torch.nn as nn
-from mmcv.utils import TORCH_VERSION
+from mmengine.utils.dl_utils import TORCH_VERSION
 
 try:
     # If PyTorch version >= 1.6.0, torch.cuda.amp.autocast would be imported
     # and used; otherwise, auto fp16 will adopt mmcv's implementation.
     from torch.cuda.amp import autocast
 except ImportError:
     pass
```

### Comparing `mmgen-0.7.3/mmgen/datasets/__init__.py` & `mmgen-1.0.0rc0/mmgen/datasets/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from .builder import build_dataloader, build_dataset
 from .dataset_wrappers import RepeatDataset
 from .grow_scale_image_dataset import GrowScaleImgDataset
 from .paired_image_dataset import PairedImageDataset
-from .pipelines import (Collect, Compose, Flip, ImageToTensor,
-                        LoadImageFromFile, Normalize, Resize, ToTensor)
 from .quick_test_dataset import QuickTestImageDataset
 from .samplers import DistributedSampler
 from .singan_dataset import SinGANDataset
+from .transforms import (FixedCrop, Flip, LoadImageFromFile, PackGenInputs,
+                         Resize)
 from .unconditional_image_dataset import UnconditionalImageDataset
 from .unpaired_image_dataset import UnpairedImageDataset
 
 __all__ = [
     'build_dataloader', 'build_dataset', 'LoadImageFromFile',
-    'DistributedSampler', 'UnconditionalImageDataset', 'Compose', 'ToTensor',
-    'ImageToTensor', 'Collect', 'Flip', 'Resize', 'RepeatDataset', 'Normalize',
-    'GrowScaleImgDataset', 'SinGANDataset', 'PairedImageDataset',
-    'UnpairedImageDataset', 'QuickTestImageDataset'
+    'DistributedSampler', 'UnconditionalImageDataset', 'Flip', 'Resize',
+    'RepeatDataset', 'GrowScaleImgDataset', 'SinGANDataset',
+    'PairedImageDataset', 'UnpairedImageDataset', 'QuickTestImageDataset',
+    'PackGenInputs', 'FixedCrop'
 ]
```

### Comparing `mmgen-0.7.3/mmgen/datasets/dataset_wrappers.py` & `mmgen-1.0.0rc0/mmgen/datasets/dataset_wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from .builder import DATASETS
+from mmgen.registry import DATASETS
 
 
 @DATASETS.register_module()
 class RepeatDataset:
     """A wrapper of repeated dataset.
 
     The length of repeated dataset will be `times` larger than the original
```

### Comparing `mmgen-0.7.3/mmgen/datasets/grow_scale_image_dataset.py` & `mmgen-1.0.0rc0/mmgen/datasets/grow_scale_image_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import os.path as osp
+from typing import Optional, Union
 
-import mmcv
-from torch.utils.data import Dataset
+from mmengine import FileClient, print_log
+from mmengine.dataset import BaseDataset
 
-from .builder import DATASETS
-from .pipelines import Compose
+from mmgen.registry import DATASETS
+from .utils import infer_io_backend
 
 
 @DATASETS.register_module()
-class GrowScaleImgDataset(Dataset):
+class GrowScaleImgDataset(BaseDataset):
     """Grow Scale Unconditional Image Dataset.
 
     This dataset is similar with ``UnconditionalImageDataset``, but offer
     more dynamic functionalities for the supporting complex algorithms, like
     PGGAN.
 
     Highlight functionalities:
@@ -45,62 +45,83 @@
             kept. Defaults to 1e6.
         gpu_samples_per_scale (dict | None, optional): Dict contains
             ``samples_per_gpu`` for each scale. For example, ``{'32': 4}`` will
             set the scale of 32 with ``samples_per_gpu=4``, despite other scale
             with ``samples_per_gpu=self.gpu_samples_base``.
         gpu_samples_base (int, optional): Set default ``samples_per_gpu`` for
             each scale. Defaults to 32.
+        io_backend (str, optional): The storage backend type. Options are
+            "disk", "ceph", "memcached", "lmdb", "http" and "petrel".
+            Default: None.
         test_mode (bool, optional): If True, the dataset will work in test
             mode. Otherwise, in train mode. Default to False.
     """
 
     _VALID_IMG_SUFFIX = ('.jpg', '.png', '.jpeg', '.JPEG')
 
     def __init__(self,
-                 imgs_roots,
+                 data_roots: dict,
                  pipeline,
                  len_per_stage=int(1e6),
                  gpu_samples_per_scale=None,
                  gpu_samples_base=32,
+                 io_backend: Optional[str] = None,
+                 file_lists: Optional[Union[str, dict]] = None,
                  test_mode=False):
-        super().__init__()
-        assert isinstance(imgs_roots, dict)
-        self.imgs_roots = imgs_roots
-        self._img_scales = sorted([int(x) for x in imgs_roots.keys()])
+
+        assert isinstance(data_roots, dict)
+        self.data_roots = data_roots
+        self._img_scales = sorted([int(x) for x in data_roots.keys()])
         self._curr_scale = self._img_scales[0]
         self._actual_curr_scale = self._curr_scale
-        self.imgs_root = self.imgs_roots[str(self._curr_scale)]
-        self.pipeline = Compose(pipeline)
-        self.test_mode = test_mode
+        self.data_root = self.data_roots[str(self._curr_scale)]
 
         # len_per_stage = -1, keep the original length
         self.len_per_stage = len_per_stage
         self.curr_stage = 0
         self.gpu_samples_per_scale = gpu_samples_per_scale
         if self.gpu_samples_per_scale is not None:
             assert isinstance(self.gpu_samples_per_scale, dict)
         else:
             self.gpu_samples_per_scale = dict()
         self.gpu_samples_base = gpu_samples_base
-        self.load_annotations()
+
+        if io_backend is None:
+            data_root_ = list(data_roots.values())[0]
+            io_backend = infer_io_backend(data_root_)
+        self.file_client = FileClient(backend=io_backend)
+
+        # use current data root to initialize and do not support
+        # `serialize_data`
+        super().__init__(
+            data_root=self.data_root,
+            pipeline=pipeline,
+            test_mode=test_mode,
+            serialize_data=False)
 
         # print basic dataset information to check the validity
-        mmcv.print_log(repr(self), 'mmgen')
+        print_log(repr(self), 'current')
 
-    def load_annotations(self):
+    def load_data_list(self):
         """Load annotations."""
         # recursively find all of the valid images from imgs_root
-        imgs_list = mmcv.scandir(
-            self.imgs_root, self._VALID_IMG_SUFFIX, recursive=True)
-        self.imgs_list = [osp.join(self.imgs_root, x) for x in imgs_list]
+        data_list = self.file_client.list_dir_or_file(
+            self.data_root,
+            list_dir=False,
+            suffix=self._VALID_IMG_SUFFIX,
+            recursive=True)
+        self.data_list = [
+            self.file_client.join_path(self.data_root, x) for x in data_list
+        ]
 
         if self.len_per_stage > 0:
             self.concat_imgs_list_to(self.len_per_stage)
         self.samples_per_gpu = self.gpu_samples_per_scale.get(
             str(self._actual_curr_scale), self.gpu_samples_base)
+        return self.data_list
 
     def update_annotations(self, curr_scale):
         """Update annotations.
 
         Args:
             curr_scale (int): Current image scale.
 
@@ -114,66 +135,64 @@
             if curr_scale <= scale:
                 self._curr_scale = scale
                 break
             if scale == self._img_scales[-1]:
                 assert RuntimeError(
                     f'Cannot find a suitable scale for {curr_scale}')
         self._actual_curr_scale = curr_scale
-        self.imgs_root = self.imgs_roots[str(self._curr_scale)]
-        self.load_annotations()
+        self.data_root = self.data_roots[str(self._curr_scale)]
+        self.load_data_list()
         # print basic dataset information to check the validity
-        mmcv.print_log('Update Dataset: ' + repr(self), 'mmgen')
+        print_log('Update Dataset: ' + repr(self), 'current')
         return True
 
     def concat_imgs_list_to(self, num):
         """Concat image list to specified length.
 
         Args:
             num (int): The length of the concatenated image list.
         """
-        if num <= len(self.imgs_list):
-            self.imgs_list = self.imgs_list[:num]
+
+        if num <= len(self.data_list):
+            self.data_list = self.data_list[:num]
             return
 
-        concat_factor = (num // len(self.imgs_list)) + 1
-        imgs = self.imgs_list * concat_factor
-        self.imgs_list = imgs[:num]
+        concat_factor = (num // len(self.data_list)) + 1
+        imgs = self.data_list * concat_factor
+        self.data_list = imgs[:num]
 
     def prepare_train_data(self, idx):
         """Prepare training data.
 
         Args:
             idx (int): Index of current batch.
 
         Returns:
             dict: Prepared training data batch.
         """
-        results = dict(real_img_path=self.imgs_list[idx])
+        results = dict(img_path=self.data_list[idx])
         return self.pipeline(results)
 
     def prepare_test_data(self, idx):
         """Prepare testing data.
 
         Args:
             idx (int): Index of current batch.
 
         Returns:
             dict: Prepared training data batch.
         """
-        results = dict(real_img_path=self.imgs_list[idx])
+        results = dict(img_path=self.data_list[idx])
         return self.pipeline(results)
 
-    def __len__(self):
-        return len(self.imgs_list)
-
     def __getitem__(self, idx):
         if not self.test_mode:
             return self.prepare_train_data(idx)
 
         return self.prepare_test_data(idx)
 
     def __repr__(self):
         dataset_name = self.__class__
-        imgs_root = self.imgs_root
+        imgs_root = self.data_root
         num_imgs = len(self)
         return (f'dataset_name: {dataset_name}, total {num_imgs} images in '
                 f'imgs_root: {imgs_root}')
```

### Comparing `mmgen-0.7.3/mmgen/datasets/pipelines/augmentation.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/ddpm/modules.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,438 +1,419 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import mmcv
-import numpy as np
-from mmcls.datasets import PIPELINES as CLS_PIPELINE
+from copy import deepcopy
+from functools import partial
 
-from ..builder import PIPELINES
+import mmengine
+import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from mmcv.cnn.bricks import build_norm_layer
+from mmengine.model import constant_init
+from mmengine.utils.dl_utils import TORCH_VERSION
+from mmengine.utils.version_utils import digit_version
+
+from mmgen.models.builder import build_module
+from mmgen.registry import MODELS, MODULES
+
+
+class EmbedSequential(nn.Sequential):
+    """A sequential module that passes timestep embeddings to the children that
+    support it as an extra input.
 
+    Modified from
+    https://github.com/openai/improved-diffusion/blob/main/improved_diffusion/unet.py#L35
+    """
 
-@PIPELINES.register_module()
-class Flip:
-    """Flip the input data with a probability.
+    def forward(self, x, y):
+        for layer in self:
+            if isinstance(layer, DenoisingResBlock):
+                x = layer(x, y)
+            else:
+                x = layer(x)
+        return x
 
-    Reverse the order of elements in the given data with a specific direction.
-    The shape of the data is preserved, but the elements are reordered.
-    Required keys are the keys in attributes "keys", added or modified keys are
-    "flip", "flip_direction" and the keys in attributes "keys".
-    It also supports flipping a list of images with the same flip.
 
+@MODELS.register_module()
+class SiLU(nn.Module):
+    r"""Applies the Sigmoid Linear Unit (SiLU) function, element-wise.
+    The SiLU function is also known as the swish function.
     Args:
-        keys (list[str]): The images to be flipped.
-        flip_ratio (float): The propability to flip the images.
-        direction (str): Flip images horizontally or vertically. Options are
-            "horizontal" | "vertical". Default: "horizontal".
+        input (bool, optional): Use inplace operation or not.
+            Defaults to `False`.
     """
-    _directions = ['horizontal', 'vertical']
-
-    def __init__(self, keys, flip_ratio=0.5, direction='horizontal'):
-        if direction not in self._directions:
-            raise ValueError(f'Direction {direction} is not supported.'
-                             f'Currently support ones are {self._directions}')
-        self.keys = keys
-        self.flip_ratio = flip_ratio
-        self.direction = direction
 
-    def __call__(self, results):
-        """Call function.
+    def __init__(self, inplace=False):
+        super().__init__()
+        if digit_version(TORCH_VERSION) <= digit_version('1.6.0') and inplace:
+            mmengine.print_log(
+                'Inplace version of \'SiLU\' is not supported for '
+                f'torch < 1.6.0, found \'{torch.version}\'.')
+        self.inplace = inplace
 
+    def forward(self, x):
+        """Forward function for SiLU.
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            x (torch.Tensor): Input tensor.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            torch.Tensor: Tensor after activation.
         """
-        flip = np.random.random() < self.flip_ratio
 
-        if flip:
-            for key in self.keys:
-                if isinstance(results[key], list):
-                    for v in results[key]:
-                        mmcv.imflip_(v, self.direction)
-                else:
-                    mmcv.imflip_(results[key], self.direction)
-
-        results['flip'] = flip
-        results['flip_direction'] = self.direction
-
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += (f'(keys={self.keys}, flip_ratio={self.flip_ratio}, '
-                     f'direction={self.direction})')
-        return repr_str
-
-
-@PIPELINES.register_module()
-class Resize:
-    """Resize data to a specific size for training or resize the images to fit
-    the network input regulation for testing.
-
-    When used for resizing images to fit network input regulation, the case is
-    that a network may have several downsample and then upsample operation,
-    then the input height and width should be divisible by the downsample
-    factor of the network.
-    For example, the network would downsample the input for 5 times with
-    stride 2, then the downsample factor is 2^5 = 32 and the height
-    and width should be divisible by 32.
-
-    Required keys are the keys in attribute "keys", added or modified keys are
-    "keep_ratio", "scale_factor", "interpolation" and the
-    keys in attribute "keys".
+        if digit_version(TORCH_VERSION) <= digit_version('1.6.0'):
+            return x * torch.sigmoid(x)
 
-    All keys in "keys" should have the same shape. "test_trans" is used to
-    record the test transformation to align the input's shape.
+        return F.silu(x, inplace=self.inplace)
+
+
+@MODULES.register_module()
+class MultiHeadAttention(nn.Module):
+    """An attention block allows spatial position to attend to each other.
+
+    Originally ported from here, but adapted to the N-d case.
+    https://github.com/hojonathanho/diffusion/blob/1e0dceb3b3495bbe19116a5e1b3596cd0706c543/diffusion_tf/models/unet.py#L66.  # noqa
 
     Args:
-        keys (list[str]): The images to be resized.
-        scale (float | Tuple[int]): If scale is Tuple(int), target spatial
-            size (h, w). Otherwise, target spatial size is scaled by input
-            size. If any of scale is -1, we will rescale short edge.
-            Note that when it is used, `size_factor` and `max_size` are
-            useless. Default: None
-        keep_ratio (bool): If set to True, images will be resized without
-            changing the aspect ratio. Otherwise, it will resize images to a
-            given size. Default: False.
-            Note that it is used togher with `scale`.
-        size_factor (int): Let the output shape be a multiple of size_factor.
-            Default:None.
-            Note that when it is used, `scale` should be set to None and
-            `keep_ratio` should be set to False.
-        max_size (int): The maximum size of the longest side of the output.
-            Default:None.
-            Note that it is used togher with `size_factor`.
-        interpolation (str): Algorithm used for interpolation:
-            "nearest" | "bilinear" | "bicubic" | "area" | "lanczos".
-            Default: "bilinear".
-        backend (str | None): The image resize backend type. Options are `cv2`,
-            `pillow`, `None`. If backend is None, the global imread_backend
-            specified by ``mmcv.use_backend()`` will be used. Default: None.
+        in_channels (int): Channels of the input feature map.
+        num_heads (int, optional): Number of heads in the attention.
+        norm_cfg (dict, optional): Config for normalization layer. Default
+            to ``dict(type='GN', num_groups=32)``
     """
 
     def __init__(self,
-                 keys,
-                 scale=None,
-                 keep_ratio=False,
-                 size_factor=None,
-                 max_size=None,
-                 interpolation='bilinear',
-                 backend=None):
-        assert keys, 'Keys should not be empty.'
-        if size_factor:
-            assert scale is None, ('When size_factor is used, scale should ',
-                                   f'be None. But received {scale}.')
-            assert keep_ratio is False, ('When size_factor is used, '
-                                         'keep_ratio should be False.')
-        if max_size:
-            assert size_factor is not None, (
-                'When max_size is used, '
-                f'size_factor should also be set. But received {size_factor}.')
-        if isinstance(scale, float):
-            if scale <= 0:
-                raise ValueError(f'Invalid scale {scale}, must be positive.')
-        elif mmcv.is_tuple_of(scale, int):
-            max_long_edge = max(scale)
-            max_short_edge = min(scale)
-            if max_short_edge == -1:
-                # assign np.inf to long edge for rescaling short edge later.
-                scale = (np.inf, max_long_edge)
-        elif scale is not None:
-            raise TypeError(
-                f'Scale must be None, float or tuple of int, but got '
-                f'{type(scale)}.')
-        self.keys = keys
-        self.scale = scale
-        self.size_factor = size_factor
-        self.max_size = max_size
-        self.keep_ratio = keep_ratio
-        self.interpolation = interpolation
-        self.backend = backend
+                 in_channels,
+                 num_heads=1,
+                 norm_cfg=dict(type='GN', num_groups=32)):
+        super().__init__()
+        self.num_heads = num_heads
+        _, self.norm = build_norm_layer(norm_cfg, in_channels)
+        self.qkv = nn.Conv1d(in_channels, in_channels * 3, 1)
+        self.proj = nn.Conv1d(in_channels, in_channels, 1)
+        self.init_weights()
+
+    @staticmethod
+    def QKVAttention(qkv):
+        channel = qkv.shape[1] // 3
+        q, k, v = torch.chunk(qkv, 3, dim=1)
+        scale = 1 / np.sqrt(np.sqrt(channel))
+        weight = torch.einsum('bct,bcs->bts', q * scale, k * scale)
+        weight = torch.softmax(weight.float(), dim=-1).type(weight.dtype)
+        weight = torch.einsum('bts,bcs->bct', weight, v)
+        return weight
 
-    def _resize(self, img, scale):
-        """Resize given image with corresponding scale.
+    def forward(self, x):
+        """Forward function for multi head attention.
         Args:
-            img (np.array): Image to be resized.
-            scale (float | Tuple[int]): Scale used in resize process.
+            x (torch.Tensor): Input feature map.
 
         Returns:
-            tuple: Tuple contains resized image and scale factor in resize
-                process.
+            torch.Tensor: Feature map after attention.
         """
-        if self.keep_ratio:
-            img, scale_factor = mmcv.imrescale(
-                img,
-                scale,
-                return_scale=True,
-                interpolation=self.interpolation,
-                backend=self.backend)
+        b, c, *spatial = x.shape
+        x = x.reshape(b, c, -1)
+        qkv = self.qkv(self.norm(x))
+        qkv = qkv.reshape(b * self.num_heads, -1, qkv.shape[2])
+        h = self.QKVAttention(qkv)
+        h = h.reshape(b, -1, h.shape[-1])
+        h = self.proj(h)
+        return (h + x).reshape(b, c, *spatial)
+
+    def init_weights(self):
+        constant_init(self.proj, 0)
+
+
+@MODULES.register_module()
+class TimeEmbedding(nn.Module):
+    """Time embedding layer, reference to Two level embedding. First embedding
+    time by an embedding function, then feed to neural networks.
+
+    Args:
+        in_channels (int): The channel number of the input feature map.
+        embedding_channels (int): The channel number of the output embedding.
+        embedding_mode (str, optional): Embedding mode for the time embedding.
+            Defaults to 'sin'.
+        embedding_cfg (dict, optional): Config for time embedding.
+            Defaults to None.
+        act_cfg (dict, optional): Config for activation layer. Defaults to
+            ``dict(type='SiLU', inplace=False)``.
+    """
+
+    def __init__(self,
+                 in_channels,
+                 embedding_channels,
+                 embedding_mode='sin',
+                 embedding_cfg=None,
+                 act_cfg=dict(type='SiLU', inplace=False)):
+        super().__init__()
+        self.blocks = nn.Sequential(
+            nn.Linear(in_channels, embedding_channels), MODELS.build(act_cfg),
+            nn.Linear(embedding_channels, embedding_channels))
+
+        # add `dim` to embedding config
+        embedding_cfg_ = dict(dim=in_channels)
+        if embedding_cfg is not None:
+            embedding_cfg_.update(embedding_cfg)
+        if embedding_mode.upper() == 'SIN':
+            self.embedding_fn = partial(self.sinusodial_embedding,
+                                        **embedding_cfg_)
         else:
-            img, w_scale, h_scale = mmcv.imresize(
-                img,
-                scale,
-                return_scale=True,
-                interpolation=self.interpolation,
-                backend=self.backend)
-            scale_factor = np.array((w_scale, h_scale), dtype=np.float32)
-        return img, scale_factor
+            raise ValueError('Only support `SIN` for time embedding, '
+                             f'but receive {embedding_mode}.')
 
-    def __call__(self, results):
-        """Call function.
+    @staticmethod
+    def sinusodial_embedding(timesteps, dim, max_period=10000):
+        """Create sinusoidal timestep embeddings.
 
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            timesteps (torch.Tensor): Timestep to embedding. 1-D tensor shape
+                as ``[bz, ]``,  one per batch element.
+            dim (int): The dimension of the embedding.
+            max_period (int, optional): Controls the minimum frequency of the
+                embeddings. Defaults to ``10000``.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            torch.Tensor: Embedding results shape as `[bz, dim]`.
         """
-        if self.size_factor:
-            h, w = results[self.keys[0]].shape[:2]
-            new_h = h - (h % self.size_factor)
-            new_w = w - (w % self.size_factor)
-            if self.max_size:
-                new_h = min(self.max_size - (self.max_size % self.size_factor),
-                            new_h)
-                new_w = min(self.max_size - (self.max_size % self.size_factor),
-                            new_w)
-            scale = (new_w, new_h)
-        elif isinstance(self.scale, tuple) and (np.inf in self.scale):
-            # find inf in self.scale, calculate ``scale`` manually
-            h, w = results[self.keys[0]].shape[:2]
-            if h < w:
-                scale = (int(self.scale[-1] / h * w), self.scale[-1])
-            else:
-                scale = (self.scale[-1], int(self.scale[-1] / w * h))
-        else:
-            # direct use the given ones
-            scale = self.scale
-
-        # here we assume all images in self.keys have the same input size
-        for key in self.keys:
-            results[key], scale_factor = self._resize(results[key], scale)
-            if len(results[key].shape) == 2:
-                results[key] = np.expand_dims(results[key], axis=2)
-
-        results['scale_factor'] = scale_factor
-        results['keep_ratio'] = self.keep_ratio
-        results['interpolation'] = self.interpolation
-
-        return results
 
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += (
-            f'(keys={self.keys}, scale={self.scale}, '
-            f'keep_ratio={self.keep_ratio}, size_factor={self.size_factor}, '
-            f'max_size={self.max_size},interpolation={self.interpolation})')
-        return repr_str
+        half = dim // 2
+        freqs = torch.exp(
+            -np.log(max_period) *
+            torch.arange(start=0, end=half, dtype=torch.float32) /
+            half).to(device=timesteps.device)
+        args = timesteps[:, None].float() * freqs[None]
+        embedding = torch.cat([torch.cos(args), torch.sin(args)], dim=-1)
+        if dim % 2:
+            embedding = torch.cat(
+                [embedding, torch.zeros_like(embedding[:, :1])], dim=-1)
+        return embedding
 
+    def forward(self, t):
+        """Forward function for time embedding layer.
+        Args:
+            t (torch.Tensor): Input timesteps.
 
-@PIPELINES.register_module()
-class NumpyPad:
-    """Numpy Padding.
-
-    In this augmentation, numpy padding is adopted to customize padding
-    augmentation. Please carefully read the numpy manual in:
-    https://numpy.org/doc/stable/reference/generated/numpy.pad.html
-
-    If you just hope a single dimension to be padded, you must set ``padding``
-    like this:
+        Returns:
+            torch.Tensor: Timesteps embedding.
 
-    ::
+        """
+        return self.blocks(self.embedding_fn(t))
 
-        padding = ((2, 2), (0, 0), (0, 0))
 
-    In this case, if you adopt an input with three dimension, only the first
-    diemansion will be padded.
+@MODULES.register_module()
+class DenoisingResBlock(nn.Module):
+    """Resblock for the denoising network. If `in_channels` not equals to
+    `out_channels`, a learnable shortcut with conv layers will be added.
 
     Args:
-        keys (list[str]): The images to be resized.
-        padding (int | tuple(int)): Please refer to the args ``pad_width`` in
-            ``numpy.pad``.
+        in_channels (int): Number of channels of the input feature map.
+        embedding_channels (int): Number of channels of the input embedding.
+        use_scale_shift_norm (bool): Whether use scale-shift-norm in
+            `NormWithEmbedding` layer.
+        dropout (float): Probability of the dropout layers.
+        out_channels (int, optional): Number of output channels of the
+            ResBlock. If not defined, the output channels will equal to the
+            `in_channels`. Defaults to `None`.
+        norm_cfg (dict, optional): The config for the normalization layers.
+            Defaults too ``dict(type='GN', num_groups=32)``.
+        act_cfg (dict, optional): The config for the activation layers.
+            Defaults to ``dict(type='SiLU', inplace=False)``.
+        shortcut_kernel_size (int, optional): The kernel size for the shortcut
+            conv. Defaults to ``1``.
     """
 
-    def __init__(self, keys, padding, **kwargs):
-        self.keys = keys
-        self.padding = padding
-        self.kwargs = kwargs
+    def __init__(self,
+                 in_channels,
+                 embedding_channels,
+                 use_scale_shift_norm,
+                 dropout,
+                 out_channels=None,
+                 norm_cfg=dict(type='GN', num_groups=32),
+                 act_cfg=dict(type='SiLU', inplace=False),
+                 shortcut_kernel_size=1):
+        super().__init__()
+        out_channels = in_channels if out_channels is None else out_channels
+
+        _norm_cfg = deepcopy(norm_cfg)
+
+        _, norm_1 = build_norm_layer(_norm_cfg, in_channels)
+        conv_1 = [
+            norm_1,
+            MODELS.build(act_cfg),
+            nn.Conv2d(in_channels, out_channels, 3, padding=1)
+        ]
+        self.conv_1 = nn.Sequential(*conv_1)
+
+        norm_with_embedding_cfg = dict(
+            in_channels=out_channels,
+            embedding_channels=embedding_channels,
+            use_scale_shift=use_scale_shift_norm,
+            norm_cfg=_norm_cfg)
+        self.norm_with_embedding = build_module(
+            dict(type='NormWithEmbedding'),
+            default_args=norm_with_embedding_cfg)
+
+        conv_2 = [
+            MODELS.build(act_cfg),
+            nn.Dropout(dropout),
+            nn.Conv2d(out_channels, out_channels, 3, padding=1)
+        ]
+        self.conv_2 = nn.Sequential(*conv_2)
+
+        assert shortcut_kernel_size in [
+            1, 3
+        ], ('Only support `1` and `3` for `shortcut_kernel_size`, but '
+            f'receive {shortcut_kernel_size}.')
+
+        self.learnable_shortcut = out_channels != in_channels
+
+        if self.learnable_shortcut:
+            shortcut_padding = 1 if shortcut_kernel_size == 3 else 0
+            self.shortcut = nn.Conv2d(
+                in_channels,
+                out_channels,
+                shortcut_kernel_size,
+                padding=shortcut_padding)
+        self.init_weights()
+
+    def forward_shortcut(self, x):
+        if self.learnable_shortcut:
+            return self.shortcut(x)
+        return x
 
-    def __call__(self, results):
-        """Call function.
+    def forward(self, x, y):
+        """Forward function.
 
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            x (torch.Tensor): Input feature map tensor.
+            y (torch.Tensor): Shared time embedding or shared label embedding.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            torch.Tensor : Output feature map tensor.
         """
-
-        for k in self.keys:
-            results[k] = np.pad(results[k], self.padding, **self.kwargs)
-
-        return results
-
-    def __repr__(self) -> str:
-        repr_str = self.__class__.__name__
-        repr_str += (
-            f'(keys={self.keys}, padding={self.padding}, kwargs={self.kwargs})'
-        )
-        return repr_str
-
-
-@CLS_PIPELINE.register_module()
-@PIPELINES.register_module()
-class RandomImgNoise:
-    """Add random noise with specific distribution and range to the input
-    image.
+        shortcut = self.forward_shortcut(x)
+        x = self.conv_1(x)
+        x = self.norm_with_embedding(x, y)
+        x = self.conv_2(x)
+        return x + shortcut
+
+    def init_weights(self):
+        # apply zero init to last conv layer
+        constant_init(self.conv_2[-1], 0)
+
+
+@MODULES.register_module()
+class NormWithEmbedding(nn.Module):
+    """Nornalization with embedding layer. If `use_scale_shift == True`,
+    embedding results will be chunked and used to re-shift and re-scale
+    normalization results. Otherwise, embedding results will directly add to
+    input of normalization layer.
 
     Args:
-        keys (list[str]): The images to be added random noise.
-        lower_bound (float, optional): The lower bound of the noise.
-            Default to ``0.``.
-        upper_bound (float, optional): The upper bound of the noise.
-            Default to ``1 / 128.``.
-        distribution (str, optional): The probability distribution of the
-            noise. Default to 'uniform'.
+        in_channels (int): Number of channels of the input feature map.
+        embedding_channels (int) Number of channels of the input embedding.
+        norm_cfg (dict, optional): Config for the normalization operation.
+            Defaults to `dict(type='GN', num_groups=32)`.
+        act_cfg (dict, optional): Config for the activation layer. Defaults
+            to `dict(type='SiLU', inplace=False)`.
+        use_scale_shift (bool): If True, the output of Embedding layer will be
+            split to 'scale' and 'shift' and map the output of normalization
+            layer to ``out * (1 + scale) + shift``. Otherwise, the output of
+            Embedding layer will be added with the input before normalization
+            operation. Defaults to True.
     """
 
     def __init__(self,
-                 keys,
-                 lower_bound=0,
-                 upper_bound=1 / 128.,
-                 distribution='uniform'):
-        assert keys, 'Keys should not be empty.'
-
-        self.keys = keys
-        self.lower_bound = lower_bound
-        self.upper_bound = upper_bound
-
-        if distribution not in ['uniform', 'normal']:
-            raise KeyError('Only support \'uniform\' distribution and '
-                           '\'normal\' distribution, receive '
-                           f'{distribution}.')
-        self.distribution = distribution
+                 in_channels,
+                 embedding_channels,
+                 norm_cfg=dict(type='GN', num_groups=32),
+                 act_cfg=dict(type='SiLU', inplace=False),
+                 use_scale_shift=True):
+        super().__init__()
+        self.use_scale_shift = use_scale_shift
+        _, self.norm = build_norm_layer(norm_cfg, in_channels)
+
+        embedding_output = in_channels * 2 if use_scale_shift else in_channels
+        self.embedding_layer = nn.Sequential(
+            MODELS.build(act_cfg),
+            nn.Linear(embedding_channels, embedding_output))
 
-    def __call__(self, results):
-        """Call function.
+    def forward(self, x, y):
+        """Forward function.
 
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            x (torch.Tensor): Input feature map tensor.
+            y (torch.Tensor): Shared time embedding or shared label embedding.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            torch.Tensor : Output feature map tensor.
         """
-        if self.distribution == 'uniform':
-            dist_fn = np.random.rand
-        else:  # self.distribution == 'normal
-            dist_fn = np.random.randn
-
-        for key in self.keys:
-            img_size = results[key].shape
-            noise = dist_fn(*img_size)
-            scale = noise.max() - noise.min()
-            noise = noise - noise.min()
-            noise = noise / scale * (self.upper_bound - self.lower_bound)
-            noise = noise + self.lower_bound
-            results[key] += noise
-
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += (f'(keys={self.keys}, lower_bound={self.lower_bound}, '
-                     f'upper_bound={self.upper_bound})')
-        return repr_str
-
-
-@CLS_PIPELINE.register_module()
-@PIPELINES.register_module()
-class RandomCropLongEdge:
-    """Random crop the given image by the long edge.
+        embedding = self.embedding_layer(y)[:, :, None, None]
+        if self.use_scale_shift:
+            scale, shift = torch.chunk(embedding, 2, dim=1)
+            x = self.norm(x)
+            x = x * (1 + scale) + shift
+        else:
+            x = self.norm(x + embedding)
+        return x
+
+
+@MODULES.register_module()
+class DenoisingDownsample(nn.Module):
+    """Downsampling operation used in the denoising network. Support average
+    pooling and convolution for downsample operation.
 
     Args:
-        keys (list[str]): The images to be cropped.
+        in_channels (int): Number of channels of the input feature map to be
+            downsampled.
+        with_conv (bool, optional): Whether use convolution operation for
+            downsampling.  Defaults to `True`.
     """
 
-    def __init__(self, keys):
-        assert keys, 'Keys should not be empty.'
-        self.keys = keys
-
-    def __call__(self, results):
-        """Call function.
+    def __init__(self, in_channels, with_conv=True):
+        super().__init__()
+        if with_conv:
+            self.downsample = nn.Conv2d(in_channels, in_channels, 3, 2, 1)
+        else:
+            self.downsample = nn.AvgPool2d(stride=2)
 
+    def forward(self, x):
+        """Forward function for downsampling operation.
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            x (torch.Tensor): Feature map to downsample.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            torch.Tensor: Feature map after downsampling.
         """
+        return self.downsample(x)
+
 
-        for key in self.keys:
-            img = results[key]
-            img_height, img_width = img.shape[:2]
-            crop_size = min(img_height, img_width)
-            y1 = 0 if img_height == crop_size else \
-                np.random.randint(0, img_height - crop_size)
-            x1 = 0 if img_width == crop_size else \
-                np.random.randint(0, img_width - crop_size)
-            y2, x2 = y1 + crop_size - 1, x1 + crop_size - 1
-
-            img = mmcv.imcrop(img, bboxes=np.array([x1, y1, x2, y2]))
-            results[key] = img
-
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += (f'(keys={self.keys})')
-        return repr_str
-
-
-@CLS_PIPELINE.register_module()
-@PIPELINES.register_module()
-class CenterCropLongEdge:
-    """Center crop the given image by the long edge.
+@MODULES.register_module()
+class DenoisingUpsample(nn.Module):
+    """Upsampling operation used in the denoising network. Allows users to
+    apply an additional convolution layer after the nearest interpolation
+    operation.
 
     Args:
-        keys (list[str]): The images to be cropped.
+        in_channels (int): Number of channels of the input feature map to be
+            downsampled.
+        with_conv (bool, optional): Whether apply an additional convolution
+            layer after upsampling.  Defaults to `True`.
     """
 
-    def __init__(self, keys):
-        assert keys, 'Keys should not be empty.'
-        self.keys = keys
-
-    def __call__(self, results):
-        """Call function.
+    def __init__(self, in_channels, with_conv=True):
+        super().__init__()
+        if with_conv:
+            self.with_conv = True
+            self.conv = nn.Conv2d(in_channels, in_channels, 3, 1, 1)
 
+    def forward(self, x):
+        """Forward function for upsampling operation.
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            x (torch.Tensor): Feature map to upsample.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            torch.Tensor: Feature map after upsampling.
         """
-
-        for key in self.keys:
-            img = results[key]
-            img_height, img_width = img.shape[:2]
-            crop_size = min(img_height, img_width)
-            y1 = 0 if img_height == crop_size else \
-                int(round(img_height - crop_size) / 2)
-            x1 = 0 if img_width == crop_size else \
-                int(round(img_width - crop_size) / 2)
-            y2 = y1 + crop_size - 1
-            x2 = x1 + crop_size - 1
-
-            img = mmcv.imcrop(img, bboxes=np.array([x1, y1, x2, y2]))
-            results[key] = img
-
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += (f'(keys={self.keys})')
-        return repr_str
+        x = F.interpolate(x, scale_factor=2, mode='nearest')
+        if self.with_conv:
+            x = self.conv(x)
+        return x
```

### Comparing `mmgen-0.7.3/mmgen/datasets/pipelines/loading.py` & `mmgen-1.0.0rc0/mmgen/datasets/transforms/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from typing import Optional
+
 import mmcv
 import numpy as np
-from mmcv.fileio import FileClient
+from mmengine import FileClient
 
-from ..builder import PIPELINES
+from mmgen.registry import TRANSFORMS
+from ..utils import infer_io_backend
 
 
-@PIPELINES.register_module()
+@TRANSFORMS.register_module()
 class LoadImageFromFile:
     """Load image from file.
 
     Args:
-        io_backend (str): io backend where images are store. Default: 'disk'.
+        io_backend (Optional[str]): io backend where images are store. If not
+            passed, try to infer the io backend by file path. Default: None.
         key (str): Keys in results to find corresponding path. Default: 'gt'.
         flag (str): Loading flag for images. Default: 'color'.
         channel_order (str): Order of channel, candidates are 'bgr' and 'rgb'.
             Default: 'bgr'.
         backend (str | None): The image decoding backend type. Options are
             `cv2`, `pillow`, `turbojpeg`, `None`. If backend is None, the
             global imread_backend specified by ``mmcv.use_backend()`` will be
             used. Default: None.
         save_original_img (bool): If True, maintain a copy of the image in
             ``results`` dict with name of ``f'ori_{key}'``. Default: False.
         kwargs (dict): Args for file client.
     """
 
     def __init__(self,
-                 io_backend='disk',
+                 io_backend: Optional[str] = None,
                  key='gt',
                  flag='color',
                  channel_order='bgr',
                  backend=None,
                  save_original_img=False,
                  **kwargs):
         self.io_backend = io_backend
@@ -48,17 +52,19 @@
         Args:
             results (dict): A dict containing the necessary information and
                 data for augmentation.
 
         Returns:
             dict: A dict containing the processed data and information.
         """
+        filepath = str(results[f'{self.key}_path'])
         if self.file_client is None:
+            if self.io_backend is None:
+                self.io_backend = infer_io_backend(filepath)
             self.file_client = FileClient(self.io_backend, **self.kwargs)
-        filepath = str(results[f'{self.key}_path'])
         img_bytes = self.file_client.get(filepath)
         img = mmcv.imfrombytes(
             img_bytes,
             flag=self.flag,
             channel_order=self.channel_order,
             backend=self.backend)  # HWC
 
@@ -74,15 +80,15 @@
         repr_str = self.__class__.__name__
         repr_str += (
             f'(io_backend={self.io_backend}, key={self.key}, '
             f'flag={self.flag}, save_original_img={self.save_original_img})')
         return repr_str
 
 
-@PIPELINES.register_module()
+@TRANSFORMS.register_module()
 class LoadPairedImageFromFile(LoadImageFromFile):
     """Load a pair of images from file.
 
     Each sample contains a pair of images, which are concatenated in the w
     dimension (a|b). This is a special loading class for generation paired
     dataset. It loads a pair of images as the common loader does and crops
     it into two images with the same shape in different domains.
@@ -90,30 +96,31 @@
     Required key is "pair_path". Added or modified keys are "pair",
     "pair_ori_shape", "ori_pair", "img_{domain_a}", "img_{domain_b}",
     "img_{domain_a}_path", "img_{domain_b}_path", "img_{domain_a}_ori_shape",
     "img_{domain_b}_ori_shape", "ori_img_{domain_a}" and
     "ori_img_{domain_b}".
 
     Args:
-        io_backend (str): io backend where images are store. Default: 'disk'.
+        io_backend (str, optional): io backend where images are store. Defaults
+            to None.
         key (str): Keys in results to find corresponding path. Default: 'gt'.
         domain_a (str, optional): One of the paired image domain.
             Defaults to None.
         domain_b (str, optional): The other image domain.
             Defaults to None.
         flag (str): Loading flag for images. Default: 'color'.
         channel_order (str): Order of channel, candidates are 'bgr' and 'rgb'.
             Default: 'bgr'.
         save_original_img (bool): If True, maintain a copy of the image in
             `results` dict with name of `f'ori_{key}'`. Default: False.
         kwargs (dict): Args for file client.
     """
 
     def __init__(self,
-                 io_backend='disk',
+                 io_backend: Optional[str] = None,
                  key='pair',
                  domain_a=None,
                  domain_b=None,
                  flag='color',
                  channel_order='bgr',
                  backend=None,
                  save_original_img=False,
@@ -137,17 +144,19 @@
         Args:
             results (dict): A dict containing the necessary information and
                 data for augmentation.
 
         Returns:
             dict: A dict containing the processed data and information.
         """
+        filepath = str(results[f'{self.key}_path'])
         if self.file_client is None:
+            if self.io_backend is None:
+                self.io_backend = infer_io_backend(filepath)
             self.file_client = FileClient(self.io_backend, **self.kwargs)
-        filepath = str(results[f'{self.key}_path'])
         img_bytes = self.file_client.get(filepath)
         img = mmcv.imfrombytes(img_bytes, flag=self.flag)  # HWC, BGR
         if img.ndim == 2:
             img = np.expand_dims(img, axis=2)
 
         results[self.key] = img
         results[f'{self.key}_path'] = filepath
```

### Comparing `mmgen-0.7.3/mmgen/datasets/pipelines/normalize.py` & `mmgen-1.0.0rc0/mmgen/datasets/transforms/formatting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,75 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import mmcv
+from typing import Optional, Sequence
+
 import numpy as np
+from mmcv.transforms import BaseTransform, to_tensor
+from mmengine import is_list_of
 
-from ..builder import PIPELINES
+from mmgen.registry import TRANSFORMS
+from mmgen.structures import GenDataSample
 
 
-@PIPELINES.register_module()
-class Normalize:
-    """Normalize images with the given mean and std value.
+@TRANSFORMS.register_module()
+class PackGenInputs(BaseTransform):
+    """Pack the inputs data for the image generation.
 
-    Required keys are the keys in attribute "keys", added or modified keys are
-    the keys in attribute "keys" and these keys with postfix '_norm_cfg'.
-    It also supports normalizing a list of images.
     Args:
-        keys (Sequence[str]): The images to be normalized.
-        mean (np.ndarray): Mean values of different channels.
-        std (np.ndarray): Std values of different channels.
-        to_rgb (bool): Whether to convert channels from BGR to RGB.
+        keys (str): Target keys to pack. Defaults to 'img'.
+        pack_all (bool): If true all keys will be packed. Defaults to False.
+        meta_keys (Sequence[str], optional): Meta keys to be converted to
+            ``mmcv.DataContainer`` and collected in ``data[img_metas]``.
+            Default: ``('img_id', 'img_path', 'ori_shape', 'img_shape',
+            'scale_factor', 'flip', 'flip_direction')``
     """
 
-    def __init__(self, keys, mean, std, to_rgb=False):
-        self.keys = keys
-        self.mean = np.array(mean, dtype=np.float32)
-        self.std = np.array(std, dtype=np.float32)
-        self.to_rgb = to_rgb
-
-    def __call__(self, results):
-        """Call function.
-
-        Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
-        Returns:
-            dict: A dict containing the processed data and information.
-        """
-        for key in self.keys:
-            if isinstance(results[key], list):
-                results[key] = [
-                    mmcv.imnormalize(v, self.mean, self.std, self.to_rgb)
-                    for v in results[key]
-                ]
+    def __init__(self,
+                 keys: str = 'img',
+                 pack_all: bool = False,
+                 meta_keys: Optional[Sequence[str]] = None):
+        self.pack_all = pack_all
+        if not self.pack_all:
+            if isinstance(keys, str):
+                self.keys = [keys]
+            elif is_list_of(keys, str):
+                self.keys = keys
             else:
-                results[key] = mmcv.imnormalize(results[key], self.mean,
-                                                self.std, self.to_rgb)
-
-        results['img_norm_cfg'] = dict(
-            mean=self.mean, std=self.std, to_rgb=self.to_rgb)
-        return results
-
-    def __repr__(self):
-        repr_str = self.__class__.__name__
-        repr_str += (f'(keys={self.keys}, mean={self.mean}, std={self.std}, '
-                     f'to_rgb={self.to_rgb})')
-
-        return repr_str
+                raise TypeError(
+                    'keys is supported to be a string or a list of string')
+        self.meta_keys = [] if meta_keys is None else meta_keys
 
-
-@PIPELINES.register_module()
-class RescaleToZeroOne:
-    """Transform the images into a range between 0 and 1.
-
-    Required keys are the keys in attribute "keys", added or modified keys are
-    the keys in attribute "keys".
-    It also supports rescaling a list of images.
-
-    Args:
-        keys (Sequence[str]): The images to be transformed.
-    """
-
-    def __init__(self, keys):
-        self.keys = keys
-
-    def __call__(self, results):
-        """Call function.
+    def transform(self, results: dict) -> dict:
+        """Method to pack the input data.
 
         Args:
-            results (dict): A dict containing the necessary information and
-                data for augmentation.
+            results (dict): Result dict from the data pipeline.
 
         Returns:
-            dict: A dict containing the processed data and information.
+            dict:
+
+            - 'inputs' (obj:`torch.Tensor`): The forward data of models.
+            - 'data_sample' (obj:`DetDataSample`): The annotation info of the
+                sample.
         """
-        for key in self.keys:
-            if isinstance(results[key], list):
-                results[key] = [
-                    v.astype(np.float32) / 255. for v in results[key]
-                ]
-            else:
-                results[key] = results[key].astype(np.float32) / 255.
-        return results
+        packed_results = dict(inputs=dict())
+        pack_keys = results.keys() if self.pack_all else self.keys
+        for key in pack_keys:
+            if key in results:
+                img = results[key]
+                if len(img.shape) < 3:
+                    img = np.expand_dims(img, -1)
+                img = np.ascontiguousarray(img.transpose(2, 0, 1))
+                packed_results['inputs'][key] = to_tensor(img)
+
+        data_sample = GenDataSample()
+
+        img_meta = {}
+        for key in self.meta_keys:
+            img_meta[key] = results[key]
+        data_sample.set_metainfo(img_meta)
+        packed_results['data_samples'] = data_sample
+
+        return packed_results
 
     def __repr__(self):
-        return self.__class__.__name__ + f'(keys={self.keys})'
+        return self.__class__.__name__ + (
+            f'(key={self.keys}, meta_keys={self.meta_keys})')
```

### Comparing `mmgen-0.7.3/mmgen/datasets/quick_test_dataset.py` & `mmgen-1.0.0rc0/mmgen/datasets/quick_test_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch
 from torch.utils.data import Dataset
 
-from .builder import DATASETS
+from mmgen.registry import DATASETS
 
 
 @DATASETS.register_module()
 class QuickTestImageDataset(Dataset):
     """Dataset for quickly testing the correctness.
 
     Args:
```

### Comparing `mmgen-0.7.3/mmgen/datasets/samplers/distributed_sampler.py` & `mmgen-1.0.0rc0/mmgen/datasets/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/datasets/singan_dataset.py` & `mmgen-1.0.0rc0/mmgen/datasets/singan_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import mmcv
 import numpy as np
-import torch
-from torch.utils.data import Dataset
+from mmengine.dataset import BaseDataset
 
-from .builder import DATASETS
+from mmgen.registry import DATASETS
 
 
 def create_real_pyramid(real, min_size, max_size, scale_factor_init):
     """Create image pyramid.
 
     This function is modified from the official implementation:
     https://github.com/tamarott/SinGAN/blob/master/SinGAN/functions.py#L221
@@ -55,15 +54,15 @@
         curr_real = mmcv.imrescale(real, scale)
         reals.append(curr_real)
 
     return reals, scale_factor, stop_scale
 
 
 @DATASETS.register_module()
-class SinGANDataset(Dataset):
+class SinGANDataset(BaseDataset):
     """SinGAN Dataset.
 
     In this dataset, we create an image pyramid and save it in the cache.
 
     Args:
         img_path (str): Path to the single image file.
         min_size (int): Min size of the image pyramid. Here, the number will be
@@ -73,49 +72,66 @@
         scale_factor_init (float): Rescale factor. Note that the actual factor
             we use may be a little bit different from this value.
         num_samples (int, optional): The number of samples (length) in this
             dataset. Defaults to -1.
     """
 
     def __init__(self,
-                 img_path,
+                 data_root,
                  min_size,
                  max_size,
                  scale_factor_init,
+                 pipeline,
                  num_samples=-1):
-        self.img_path = img_path
-        assert mmcv.is_filepath(self.img_path)
-        self.load_annotations(min_size, max_size, scale_factor_init)
+        self.min_size = min_size
+        self.max_size = max_size
+        self.scale_factor_init = scale_factor_init
         self.num_samples = num_samples
+        super().__init__(data_root=data_root, pipeline=pipeline)
 
-    def load_annotations(self, min_size, max_size, scale_factor_init):
+    def full_init(self):
+        """Skip the full init process for SinGANDataset."""
+
+        self.load_data_list(self.min_size, self.max_size,
+                            self.scale_factor_init)
+
+    def load_data_list(self, min_size, max_size, scale_factor_init):
         """Load annatations for SinGAN Dataset.
 
         Args:
             min_size (int): The minimum size for the image pyramid.
             max_size (int): The maximum size for the image pyramid.
             scale_factor_init (float): The initial scale factor.
         """
-        real = mmcv.imread(self.img_path)
+        real = mmcv.imread(self.data_root)
         self.reals, self.scale_factor, self.stop_scale = create_real_pyramid(
             real, min_size, max_size, scale_factor_init)
 
         self.data_dict = {}
 
         for i, real in enumerate(self.reals):
-            self.data_dict[f'real_scale{i}'] = self._img2tensor(real)
+            self.data_dict[f'real_scale{i}'] = real
 
-        self.data_dict['input_sample'] = torch.zeros_like(
-            self.data_dict['real_scale0'])
+        self.data_dict['input_sample'] = np.zeros_like(
+            self.data_dict['real_scale0']).astype(np.float32)
 
-    def _img2tensor(self, img):
-        img = torch.from_numpy(img).to(torch.float32).permute(2, 0,
-                                                              1).contiguous()
-        img = (img / 255 - 0.5) * 2
+    def __getitem__(self, index):
+        """Get `:attr:self.data_dict`. For SinGAN, we use single image with
+        different resolution to train the model.
 
-        return img
+        Args:
+            idx (int): This will be ignored in `:class:SinGANDataset`.
 
-    def __getitem__(self, index):
-        return self.data_dict
+        Returns:
+            dict: Dict contains input image in different resolution.
+            ``self.pipeline``.
+        """
+        return self.pipeline(self.data_dict)
 
     def __len__(self):
+        """Get the length of filtered dataset and automatically call
+        ``full_init`` if the  dataset has not been fully init.
+
+        Returns:
+            int: The length of filtered dataset.
+        """
         return int(1e6) if self.num_samples < 0 else self.num_samples
```

### Comparing `mmgen-0.7.3/mmgen/datasets/unpaired_image_dataset.py` & `mmgen-1.0.0rc0/mmgen/datasets/unpaired_image_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import os.path as osp
-from pathlib import Path
+from typing import Optional
 
 import numpy as np
-from mmcv import scandir
-from torch.utils.data import Dataset
+from mmengine import FileClient
+from mmengine.dataset import BaseDataset
 
-from .builder import DATASETS
-from .pipelines import Compose
+from mmgen.registry import DATASETS
+from .utils import infer_io_backend
 
 IMG_EXTENSIONS = ('.jpg', '.JPG', '.jpeg', '.JPEG', '.png', '.PNG', '.ppm',
                   '.PPM', '.bmp', '.BMP', '.tif', '.TIF', '.tiff', '.TIFF')
 
 
 @DATASETS.register_module()
-class UnpairedImageDataset(Dataset):
+class UnpairedImageDataset(BaseDataset):
     """General unpaired image folder dataset for image generation.
 
     It assumes that the training directory of images from domain A is
     '/path/to/data/trainA', and that from domain B is '/path/to/data/trainB',
     respectively. '/path/to/data' can be initialized by args 'dataroot'.
     During test time, the directory is '/path/to/data/testA' and
     '/path/to/data/testB', respectively.
 
     Args:
         dataroot (str | :obj:`Path`): Path to the folder root of unpaired
             images.
         pipeline (List[dict | callable]): A sequence of data transformations.
+        io_backend (str, optional): The storage backend type. Options are
+            "disk", "ceph", "memcached", "lmdb", "http" and "petrel".
+            Default: None.
         test_mode (bool): Store `True` when building test dataset.
             Default: `False`.
         domain_a (str, optional): Domain of images in trainA / testA.
             Defaults to None.
         domain_b (str, optional): Domain of images in trainB / testB.
             Defaults to None.
     """
 
     def __init__(self,
-                 dataroot,
+                 data_root,
                  pipeline,
+                 io_backend: Optional[str] = None,
                  test_mode=False,
                  domain_a=None,
                  domain_b=None):
-        super().__init__()
         phase = 'test' if test_mode else 'train'
-        self.dataroot_a = osp.join(str(dataroot), phase + 'A')
-        self.dataroot_b = osp.join(str(dataroot), phase + 'B')
-        self.data_infos_a = self.load_annotations(self.dataroot_a)
-        self.data_infos_b = self.load_annotations(self.dataroot_b)
+        self.dataroot_a = osp.join(str(data_root), phase + 'A')
+        self.dataroot_b = osp.join(str(data_root), phase + 'B')
+
+        if io_backend is None:
+            io_backend = infer_io_backend(data_root)
+        self.file_client = FileClient(backend=io_backend)
+
+        super().__init__(
+            data_root=data_root,
+            pipeline=pipeline,
+            test_mode=test_mode,
+            serialize_data=False)
         self.len_a = len(self.data_infos_a)
         self.len_b = len(self.data_infos_b)
         self.test_mode = test_mode
-        self.pipeline = Compose(pipeline)
         assert isinstance(domain_a, str)
         assert isinstance(domain_b, str)
         self.domain_a = domain_a
         self.domain_b = domain_b
 
-    def load_annotations(self, dataroot):
+    def load_data_list(self):
+        self.data_infos_a = self._load_domain_data_list(self.dataroot_a)
+        self.data_infos_b = self._load_domain_data_list(self.dataroot_b)
+        return [self.data_infos_a, self.data_infos_b]
+
+    def _load_domain_data_list(self, dataroot):
         """Load unpaired image paths of one domain.
 
         Args:
             dataroot (str): Path to the folder root for unpaired images of
                 one domain.
 
         Returns:
@@ -104,33 +119,26 @@
         results[f'img_{self.domain_a}_path'] = img_a_path
         results[f'img_{self.domain_b}_path'] = img_b_path
         return self.pipeline(results)
 
     def __len__(self):
         return max(self.len_a, self.len_b)
 
-    @staticmethod
-    def scan_folder(path):
+    def scan_folder(self, path):
         """Obtain image path list (including sub-folders) from a given folder.
 
         Args:
             path (str | :obj:`Path`): Folder path.
 
         Returns:
             list[str]: Image list obtained from the given folder.
         """
-
-        if isinstance(path, (str, Path)):
-            path = str(path)
-        else:
-            raise TypeError("'path' must be a str or a Path object, "
-                            f'but received {type(path)}.')
-
-        images = scandir(path, suffix=IMG_EXTENSIONS, recursive=True)
-        images = [osp.join(path, v) for v in images]
+        imgs_list = self.file_client.list_dir_or_file(
+            path, list_dir=False, suffix=IMG_EXTENSIONS, recursive=True)
+        images = [self.file_client.join_path(path, img) for img in imgs_list]
         assert images, f'{path} has no valid image file.'
         return images
 
     def __getitem__(self, idx):
         """Get item at each call.
 
         Args:
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/__init__.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .lpips import PerceptualLoss
 from .lsgan import LSGANDiscriminator, LSGANGenerator
 from .pggan import (EqualizedLR, EqualizedLRConvDownModule,
                     EqualizedLRConvModule, EqualizedLRConvUpModule,
                     EqualizedLRLinearModule, MiniBatchStddevLayer,
                     PGGANDiscriminator, PGGANGenerator, PGGANNoiseTo2DFeat,
                     PixelNorm, equalized_lr)
-from .pix2pix import PatchDiscriminator, generation_init_weights
+from .pix2pix import PatchDiscriminator, UnetGenerator, generation_init_weights
 from .positional_encoding import CatersianGrid, SinusoidalPositionalEmbedding
 from .singan import SinGANMultiScaleDiscriminator, SinGANMultiScaleGenerator
 from .sngan_proj import ProjDiscriminator, SNGANGenerator
 from .stylegan import (MSStyleGAN2Discriminator, MSStyleGANv2Generator,
                        StyleGAN1Discriminator, StyleGAN2Discriminator,
                        StyleGANv1Generator, StyleGANv2Generator,
                        StyleGANv3Generator)
@@ -34,9 +34,9 @@
     'StyleGANv2Generator', 'StyleGANv1Generator', 'StyleGAN1Discriminator',
     'MSStyleGAN2Discriminator', 'MSStyleGANv2Generator',
     'generation_init_weights', 'PatchDiscriminator', 'ResnetGenerator',
     'PerceptualLoss', 'WGANGPDiscriminator', 'WGANGPGenerator',
     'LSGANDiscriminator', 'LSGANGenerator', 'ProjDiscriminator',
     'SNGANGenerator', 'BigGANGenerator', 'SNConvModule', 'BigGANDiscriminator',
     'BigGANDeepGenerator', 'BigGANDeepDiscriminator', 'DenoisingUnet',
-    'StyleGANv3Generator', 'IDLossModel'
+    'StyleGANv3Generator', 'IDLossModel', 'UnetGenerator'
 ]
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/arcface/helpers.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/arcface/helpers.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/arcface/id_loss.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/arcface/id_loss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import mmcv
+import mmengine
 import torch
 from torch import nn
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODULES
 from .model_irse import Backbone
 
 
 @MODULES.register_module('ArcFace')
 class IDLossModel(nn.Module):
     # ir se50 weight download link
     _ir_se50_url = 'https://gg0ltg.by.files.1drv.com/y4m3fNNszG03z9n8JQ7EhdtQKW8tQVQMFBisPVRgoXi_UfP8pKSSqv8RJNmHy2JampcPmEazo_Mx6NTFSqBpZmhPniROm9uNoghnzaavvYpxkCfiNmDH9YyIF3g-0nwt6bsjk2X80JDdL5z88OAblSDmB-kuQkWSWvA9BM3Xt8DHMCY8lO4HOQCZ5YWUtFyPAVwEyzTGDM-JRA5EJoN2bF1cg'  # noqa
 
     def __init__(self, ir_se50_weights=None, device='cuda'):
         super(IDLossModel, self).__init__()
-        mmcv.print_log('Loading ResNet ArcFace', 'mmgen')
+        mmengine.print_log('Loading ResNet ArcFace', 'current')
         self.facenet = Backbone(
             input_size=112, num_layers=50, drop_ratio=0.6, mode='ir_se')
         if ir_se50_weights is None:
             ir_se50_weights = self._ir_se50_url
         self.facenet.load_state_dict(
             torch.hub.load_state_dict_from_url(ir_se50_weights))
         self.pool = torch.nn.AdaptiveAvgPool2d((256, 256))
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/arcface/model_irse.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/arcface/model_irse.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/biggan/__init__.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/biggan/__init__.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/biggan/biggan_snmodule.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/biggan/biggan_snmodule.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/biggan/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/biggan/generator_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
-import mmcv
+import mmengine
 import torch
 import torch.nn as nn
-from mmcv.cnn import normal_init, xavier_init
-from mmcv.cnn.bricks import build_activation_layer
-from mmcv.runner import load_checkpoint
-from mmcv.runner.checkpoint import _load_checkpoint_with_prefix
+from mmengine.logging import MMLogger
+from mmengine.model import normal_init, xavier_init
+from mmengine.runner import load_checkpoint
+from mmengine.runner.checkpoint import _load_checkpoint_with_prefix
 from torch.nn.utils import spectral_norm
 
-from mmgen.models.builder import MODULES, build_module
-from mmgen.utils import get_root_logger
+from mmgen.models.builder import MODELS, MODULES, build_module
 from ..common import get_module_device
 from .biggan_snmodule import SNEmbedding, SNLinear
 from .modules import SelfAttentionBlock, SNConvModule
 
 
 @MODULES.register_module()
 class BigGANGenerator(nn.Module):
@@ -415,26 +414,26 @@
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif isinstance(pretrained, dict):
             ckpt_path = pretrained.get('ckpt_path', None)
             assert ckpt_path is not None
             prefix = pretrained.get('prefix', '')
             map_location = pretrained.get('map_location', 'cpu')
             strict = pretrained.get('strict', True)
             state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                       map_location)
             self.load_state_dict(state_dict, strict=strict)
-            mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+            mmengine.print_log(f'Load pretrained model from {ckpt_path}')
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, (nn.Conv2d, nn.Linear, nn.Embedding)):
                     if init_type == 'ortho':
                         nn.init.orthogonal_(m.weight)
                     elif init_type == 'N02':
                         normal_init(m, 0.0, 0.02)
@@ -557,15 +556,15 @@
                 self.conv_blocks.append(
                     SelfAttentionBlock(
                         out_ch,
                         with_spectral_norm=with_spectral_norm,
                         sn_eps=sn_eps,
                         sn_style=sn_style))
 
-        self.activate = build_activation_layer(act_cfg)
+        self.activate = MODELS.build(act_cfg)
 
         self.decision = nn.Linear(self.arch['out_channels'][-1], out_channels)
         if with_spectral_norm:
             if sn_style == 'torch':
                 self.decision = spectral_norm(self.decision, eps=sn_eps)
             elif sn_style == 'ajbrock':
                 self.decision = SNLinear(
@@ -673,26 +672,26 @@
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
 
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif isinstance(pretrained, dict):
             ckpt_path = pretrained.get('ckpt_path', None)
             assert ckpt_path is not None
             prefix = pretrained.get('prefix', '')
             map_location = pretrained.get('map_location', 'cpu')
             strict = pretrained.get('strict', True)
             state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                       map_location)
             self.load_state_dict(state_dict, strict=strict)
-            mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+            mmengine.print_log(f'Load pretrained model from {ckpt_path}')
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, (nn.Conv2d, nn.Linear, nn.Embedding)):
                     if init_type == 'ortho':
                         nn.init.orthogonal_(m.weight)
                     elif init_type == 'N02':
                         normal_init(m, 0.0, 0.02)
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/biggan/generator_discriminator_deep.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/biggan/generator_discriminator_deep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
-import mmcv
+import mmengine
 import torch
 import torch.nn as nn
-from mmcv.cnn import normal_init, xavier_init
-from mmcv.cnn.bricks import build_activation_layer
-from mmcv.runner import load_checkpoint
-from mmcv.runner.checkpoint import _load_checkpoint_with_prefix
+from mmengine.logging import MMLogger
+from mmengine.model import normal_init, xavier_init
+from mmengine.runner import load_checkpoint
+from mmengine.runner.checkpoint import _load_checkpoint_with_prefix
 from torch.nn.utils import spectral_norm
 
-from mmgen.models.builder import MODULES, build_module
-from mmgen.utils import get_root_logger
+from mmgen.models.builder import MODELS, MODULES, build_module
 from ..common import get_module_device
 from .biggan_snmodule import SNEmbedding, SNLinear
 from .modules import SelfAttentionBlock, SNConvModule
 
 
 @MODULES.register_module()
 class BigGANDeepGenerator(nn.Module):
@@ -430,26 +429,26 @@
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif isinstance(pretrained, dict):
             ckpt_path = pretrained.get('ckpt_path', None)
             assert ckpt_path is not None
             prefix = pretrained.get('prefix', '')
             map_location = pretrained.get('map_location', 'cpu')
             strict = pretrained.get('strict', True)
             state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                       map_location)
             self.load_state_dict(state_dict, strict=strict)
-            mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+            mmengine.print_log(f'Load pretrained model from {ckpt_path}')
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, (nn.Conv2d, nn.Linear, nn.Embedding)):
                     if init_type == 'ortho':
                         nn.init.orthogonal_(m.weight)
                     elif init_type == 'N02':
                         normal_init(m, 0.0, 0.02)
@@ -591,15 +590,15 @@
                 self.conv_blocks.append(
                     SelfAttentionBlock(
                         out_ch,
                         with_spectral_norm=with_spectral_norm,
                         sn_eps=sn_eps,
                         sn_style=sn_style))
 
-        self.activate = build_activation_layer(act_cfg)
+        self.activate = MODELS.build(act_cfg)
 
         self.decision = nn.Linear(self.arch['out_channels'][-1], out_channels)
         if with_spectral_norm:
             if sn_style == 'torch':
                 self.decision = spectral_norm(self.decision, eps=sn_eps)
             elif sn_style == 'ajbrock':
                 self.decision = SNLinear(
@@ -707,26 +706,26 @@
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
             init_type (str, optional): The name of an initialization method:
                 ortho | N02 | xavier. Defaults to 'ortho'.
         """
 
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif isinstance(pretrained, dict):
             ckpt_path = pretrained.get('ckpt_path', None)
             assert ckpt_path is not None
             prefix = pretrained.get('prefix', '')
             map_location = pretrained.get('map_location', 'cpu')
             strict = pretrained.get('strict', True)
             state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                       map_location)
             self.load_state_dict(state_dict, strict=strict)
-            mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+            mmengine.print_log(f'Load pretrained model from {ckpt_path}')
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, (nn.Conv2d, nn.Linear, nn.Embedding)):
                     if init_type == 'ortho':
                         nn.init.orthogonal_(m.weight)
                     elif init_type == 'N02':
                         normal_init(m, 0.0, 0.02)
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/biggan/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/biggan/modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from copy import deepcopy
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
 from mmcv.cnn import ConvModule
-from mmcv.cnn.bricks import build_activation_layer, build_upsample_layer
 from torch.nn import Parameter
 from torch.nn.modules.batchnorm import SyncBatchNorm
 from torch.nn.utils import spectral_norm
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODELS, MODULES
 from .biggan_snmodule import SNConv2d, SNLinear
 
 
 class SNConvModule(ConvModule):
     """Spectral Normalization ConvModule.
 
     In this module, we inherit default ``mmcv.cnn.ConvModule`` and adopt
@@ -98,19 +97,19 @@
                  upsample_cfg=dict(type='nearest', scale_factor=2),
                  sn_eps=1e-6,
                  sn_style='ajbrock',
                  with_spectral_norm=True,
                  input_is_label=False,
                  auto_sync_bn=True):
         super().__init__()
-        self.activation = build_activation_layer(act_cfg)
+        self.activation = MODELS.build(act_cfg)
         self.upsample_cfg = deepcopy(upsample_cfg)
         self.with_upsample = upsample_cfg is not None
         if self.with_upsample:
-            self.upsample_layer = build_upsample_layer(self.upsample_cfg)
+            self.upsample_layer = MODELS.build(self.upsample_cfg)
         self.learnable_sc = in_channels != out_channels or self.with_upsample
         if self.learnable_sc:
             self.shortcut = SNConvModule(
                 in_channels=in_channels,
                 out_channels=out_channels,
                 kernel_size=1,
                 stride=1,
@@ -410,15 +409,15 @@
                  act_cfg=dict(type='ReLU', inplace=False),
                  sn_eps=1e-6,
                  sn_style='ajbrock',
                  with_downsample=True,
                  with_spectral_norm=True,
                  is_head_block=False):
         super().__init__()
-        self.activation = build_activation_layer(act_cfg)
+        self.activation = MODELS.build(act_cfg)
         self.with_downsample = with_downsample
         self.is_head_block = is_head_block
         if self.with_downsample:
             self.downsample = nn.AvgPool2d(kernel_size=2, stride=2)
         self.learnable_sc = in_channels != out_channels or self.with_downsample
         if self.learnable_sc:
             self.shortcut = SNConvModule(
@@ -540,19 +539,19 @@
                  input_is_label=False,
                  auto_sync_bn=True,
                  channel_ratio=4):
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.hidden_channels = self.in_channels // channel_ratio
-        self.activation = build_activation_layer(act_cfg)
+        self.activation = MODELS.build(act_cfg)
         self.upsample_cfg = deepcopy(upsample_cfg)
         self.with_upsample = upsample_cfg is not None
         if self.with_upsample:
-            self.upsample_layer = build_upsample_layer(self.upsample_cfg)
+            self.upsample_layer = MODELS.build(self.upsample_cfg)
         # Here in_channels of BigGANGenResBlock equal to num_features of
         # BigGANConditionBN
         self.bn1 = BigGANConditionBN(
             in_channels,
             dim_after_concat,
             sn_eps=sn_eps,
             sn_style=sn_style,
@@ -702,15 +701,15 @@
                  sn_style='ajbrock',
                  with_downsample=True,
                  with_spectral_norm=True):
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.hidden_channels = self.out_channels // channel_ratio
-        self.activation = build_activation_layer(act_cfg)
+        self.activation = MODELS.build(act_cfg)
         self.with_downsample = with_downsample
 
         if self.with_downsample:
             self.downsample = nn.AvgPool2d(kernel_size=2, stride=2)
 
         self.learnable_sc = (in_channels != out_channels)
         if self.learnable_sc:
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/common.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/common.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/cyclegan/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/cyclegan/generator_discriminator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 from mmcv.cnn import ConvModule
-from mmcv.runner import load_checkpoint
+from mmengine.logging import MMLogger
+from mmengine.runner import load_checkpoint
 
 from mmgen.models.architectures.pix2pix import generation_init_weights
 from mmgen.models.builder import MODULES
-from mmgen.utils import get_root_logger
 from .modules import ResidualBlockWithDropout
 
 
 @MODULES.register_module()
 class ResnetGenerator(nn.Module):
     """Construct a Resnet-based generator that consists of residual blocks
     between a few downsampling/upsampling operations.
@@ -138,15 +138,15 @@
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Default: None.
             strict (bool, optional): Whether to allow different params for the
                 model and checkpoint. Default: True.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=strict, logger=logger)
         elif pretrained is None:
             generation_init_weights(
                 self, init_type=self.init_type, init_gain=self.init_gain)
         else:
             raise TypeError("'pretrained' must be a str or None. "
                             f'But received {type(pretrained)}.')
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/cyclegan/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/cyclegan/modules.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/dcgan/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/dcgan/generator_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 import torch.nn as nn
-from mmcv.cnn import ConvModule, normal_init
-from mmcv.runner import load_checkpoint
-from mmcv.utils.parrots_wrapper import _BatchNorm
+from mmcv.cnn import ConvModule
+from mmengine.logging import MMLogger
+from mmengine.model import normal_init
+from mmengine.runner import load_checkpoint
+from mmengine.utils.dl_utils.parrots_wrapper import _BatchNorm
 
 from mmgen.models.builder import MODULES
-from mmgen.utils import get_root_logger
 from ..common import get_module_device
 
 
 @MODULES.register_module()
 class DCGANGenerator(nn.Module):
     """Generator for DCGAN.
 
@@ -172,15 +173,15 @@
         We just use the initialization method proposed in the original paper.
 
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Defaults to None.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, (nn.Conv2d, nn.ConvTranspose2d)):
                     normal_init(m, 0, 0.02)
                 elif isinstance(m, _BatchNorm):
                     nn.init.normal_(m.weight.data)
@@ -238,14 +239,15 @@
         self.base_channels = base_channels
 
         # the number of times for downsampling
         self.num_downsamples = int(np.log2(input_scale // output_scale))
 
         # build up downsampling backbone (excluding the output layer)
         downsamples = []
+        curr_channels = in_channels
         for i in range(self.num_downsamples):
             # remove norm for the first conv
             norm_cfg_ = None if i == 0 else default_norm_cfg
             in_ch = in_channels if i == 0 else base_channels * 2**(i - 1)
 
             downsamples.append(
                 ConvModule(
@@ -297,15 +299,15 @@
         We just use the initialization method proposed in the original paper.
 
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Defaults to None.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, (nn.Conv2d, nn.ConvTranspose2d)):
                     normal_init(m, 0, 0.02)
                 elif isinstance(m, _BatchNorm):
                     nn.init.normal_(m.weight.data)
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/ddpm/denoising.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/ddpm/denoising.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import torch
 import torch.nn as nn
-from mmcv.cnn import constant_init
 from mmcv.cnn.bricks.conv_module import ConvModule
-from mmcv.runner import load_checkpoint
+from mmengine.logging import MMLogger
+from mmengine.model import constant_init
+from mmengine.runner import load_checkpoint
 
 from mmgen.models.builder import MODULES, build_module
-from mmgen.utils import get_root_logger
 from .modules import EmbedSequential, TimeEmbedding
 
 
 @MODULES.register_module()
 class DenoisingUnet(nn.Module):
     """Denoising Unet. This network receives a diffused image ``x_t`` and
     current timestep ``t``, and returns a ``output_dict`` corresponding to the
@@ -108,17 +108,17 @@
         attention_cfg (dict, optional): Config for attention operation.
             Defaults to ``dict(type='MultiHeadAttention')``.
         upsample_conv (bool, optional): Whether use conv in upsample block.
             Defaults to ``True``.
         downsample_conv (bool, optional): Whether use conv operation in
             downsample block.  Defaults to ``True``.
         upsample_cfg (dict, optional): Config for upsample blocks.
-            Defaults to ``dict(type='DenoisingUpsample')``.
-        downsample_cfg (dict, optional): Config for downsample blocks.
             Defaults to ``dict(type='DenoisingDownsample')``.
+        downsample_cfg (dict, optional): Config for downsample blocks.
+            Defaults to ``dict(type='DenoisingUpsample')``.
         attention_res (int | list[int], optional): Resolution of feature maps
             to apply attention operation. Defaults to ``[16, 8]``.
         pretrained (str | dict, optional): Path for the pretrained model or
             dict containing information for pretained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict.  Defaults to None.
     """
@@ -398,15 +398,15 @@
         We just use the initialization method proposed in the original paper.
 
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Defaults to None.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif pretrained is None:
             # As Improved-DDPM, we apply zero-initialization to
             #   second conv block in ResBlock (keywords: conv_2)
             #   the output layer of the Unet (keywords: 'out' but
             #     not 'out_blocks')
             #   projection layer in Attention layer (keywords: proj)
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/fid_inception.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/fid_inception.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/lpips/networks_basic.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/lpips/perceptual_loss.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/lpips/perceptual_loss.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/lpips/pretrained_networks.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/lsgan/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/lsgan/generator_discriminator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 import torch.nn as nn
 from mmcv.cnn import ConvModule
-from mmcv.cnn.bricks import build_activation_layer
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODELS, MODULES
 from ..common import get_module_device
 
 
 @MODULES.register_module()
 class LSGANGenerator(nn.Module):
     """Generator for LSGAN.
 
@@ -66,16 +65,16 @@
         self.input_scale = input_scale
         self.noise_size = noise_size
 
         self.noise2feat_head = nn.Sequential(
             nn.Linear(noise_size, input_scale * input_scale * base_channels))
         self.noise2feat_tail = nn.Sequential(nn.BatchNorm2d(base_channels))
         if default_act_cfg is not None:
-            self.noise2feat_tail.add_module(
-                'act', build_activation_layer(default_act_cfg))
+            self.noise2feat_tail.add_module('act',
+                                            MODELS.build(default_act_cfg))
 
         # the number of times for upsampling
         self.num_upsamples = int(np.log2(output_scale // input_scale)) - 2
 
         # build up convolution backbone (excluding the output layer)
         self.conv_blocks = nn.ModuleList()
         for _ in range(self.num_upsamples):
@@ -272,15 +271,15 @@
             curr_channels = curr_channels * 2
 
         # output layer
         self.decision = nn.Sequential(
             nn.Linear(output_scale * output_scale * curr_channels,
                       out_channels))
         if self.with_out_activation:
-            self.out_activation = build_activation_layer(out_act_cfg)
+            self.out_activation = MODELS.build(out_act_cfg)
 
     def forward(self, x):
         """Forward function.
 
         Args:
             x (torch.Tensor): Fake or real image tensor.
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/pggan/__init__.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/pggan/__init__.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/pggan/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/pggan/generator_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from copy import deepcopy
 from functools import partial
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mmcv.cnn.bricks.upsample import build_upsample_layer
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODELS, MODULES
 from ..common import get_module_device
 from .modules import (EqualizedLRConvDownModule, EqualizedLRConvModule,
                       EqualizedLRConvUpModule, MiniBatchStddevLayer,
                       PGGANDecisionHead, PGGANNoiseTo2DFeat)
 
 
 @MODULES.register_module()
@@ -112,15 +111,15 @@
             # setup torgb layers
             self.torgb_layers.append(
                 self._get_torgb_layer(self._num_out_channels(s - 1)))
             # setup upconv or conv blocks
             self.conv_blocks.extend(self._get_upconv_block(in_ch, s))
 
         # build upsample layer for residual path
-        self.upsample_layer = build_upsample_layer(self.upsample_cfg)
+        self.upsample_layer = MODELS.build(self.upsample_cfg)
 
     def _get_torgb_layer(self, in_channels):
         return EqualizedLRConvModule(
             in_channels,
             3,
             kernel_size=1,
             stride=1,
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/pggan/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/pggan/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mmcv.cnn.bricks import (NORM_LAYERS, PLUGIN_LAYERS, ConvModule,
-                             build_activation_layer, build_norm_layer,
-                             build_upsample_layer)
-from mmcv.cnn.utils import normal_init
+from mmcv.cnn.bricks import ConvModule, build_norm_layer
+from mmengine.model import normal_init
 from torch.nn.init import _calculate_correct_fan
 
-from mmgen.models.builder import MODULES
 from mmgen.models.common import AllGatherLayer
+from mmgen.registry import MODELS, MODULES
 
 
 class EqualizedLR:
     r"""Equalized Learning Rate.
 
     This trick is proposed in:
     Progressive Growing of GANs for Improved Quality, Stability, and Variation
@@ -160,15 +158,15 @@
         norm = torch.norm(x, p=2, dim=1, keepdim=True)
     norm = norm / torch.sqrt(torch.tensor(x.shape[1]).to(x))
 
     return x / (norm + eps)
 
 
 @MODULES.register_module()
-@NORM_LAYERS.register_module()
+@MODELS.register_module()
 class PixelNorm(nn.Module):
     """Pixel Normalization.
 
     This module is proposed in:
     Progressive Growing of GANs for Improved Quality, Stability, and Variation
 
     Args:
@@ -189,15 +187,15 @@
 
         Returns:
             torch.Tensor: Normalized tensor.
         """
         return pixel_norm(x, self.eps)
 
 
-@PLUGIN_LAYERS.register_module()
+@MODELS.register_module()
 class EqualizedLRConvModule(ConvModule):
     r"""Equalized LR ConvModule.
 
     In this module, we inherit default ``mmcv.cnn.ConvModule`` and adopt
     equalized lr in convolution. The equalized learning rate is proposed in:
     Progressive Growing of GANs for Improved Quality, Stability, and Variation
 
@@ -219,15 +217,15 @@
             self._init_conv_weights()
 
     def _init_conv_weights(self):
         """Initialize conv weights as described in PGGAN."""
         normal_init(self.conv)
 
 
-@PLUGIN_LAYERS.register_module()
+@MODELS.register_module()
 class EqualizedLRConvUpModule(EqualizedLRConvModule):
     r"""Equalized LR (Upsample + Conv) Module.
 
     In this module, we inherit ``EqualizedLRConvModule`` and adopt
     upsampling before convolution. As for upsampling, in addition to the
     sampling layer in MMCV, we also offer the "fused_nn" type. "fused_nn"
     denotes fusing upsampling and convolution. The fusion is modified from
@@ -250,15 +248,15 @@
         self.with_upsample = upsample is not None
         if self.with_upsample:
             if upsample.get('type') == 'fused_nn':
                 assert isinstance(self.conv, nn.ConvTranspose2d)
                 self.conv.register_forward_pre_hook(
                     EqualizedLRConvUpModule.fused_nn_hook)
             else:
-                self.upsample_layer = build_upsample_layer(upsample)
+                self.upsample_layer = MODELS.build(upsample)
 
     def forward(self, x, **kwargs):
         """Forward function.
 
         Args:
             x (Tensor): Input tensor with shape (n, c, h, w).
 
@@ -276,15 +274,15 @@
         # pad the last two dimensions
         weight = F.pad(weight, (1, 1, 1, 1))
         weight = weight[..., 1:, 1:] + weight[..., 1:, :-1] + weight[
             ..., :-1, 1:] + weight[..., :-1, :-1]
         module.weight = weight
 
 
-@PLUGIN_LAYERS.register_module()
+@MODELS.register_module()
 class EqualizedLRConvDownModule(EqualizedLRConvModule):
     r"""Equalized LR (Conv + Downsample)  Module.
 
     In this module, we inherit ``EqualizedLRConvModule`` and adopt
     downsampling after convolution. As for downsampling, we provide two modes
     of "avgpool" and "fused_pool". "avgpool" denotes the commonly used average
     pooling operation, while "fused_pool" represents fusing downsampling and
@@ -339,15 +337,15 @@
         # pad the last two dimensions
         weight = F.pad(weight, (1, 1, 1, 1))
         weight = (weight[..., 1:, 1:] + weight[..., 1:, :-1] +
                   weight[..., :-1, 1:] + weight[..., :-1, :-1]) * 0.25
         module.weight = weight
 
 
-@PLUGIN_LAYERS.register_module()
+@MODELS.register_module()
 class EqualizedLRLinearModule(nn.Linear):
     r"""Equalized LR LinearModule.
 
     In this module, we adopt equalized lr in ``nn.Linear``. The equalized
     learning rate is proposed in:
     Progressive Growing of GANs for Improved Quality, Stability, and Variation
 
@@ -404,15 +402,15 @@
         self.linear = EqualizedLRLinearModule(
             noise_size,
             out_channels * 16,
             equalized_lr_cfg=dict(gain=np.sqrt(2) / 4),
             bias=False)
 
         if self.with_activation:
-            self.activation = build_activation_layer(act_cfg)
+            self.activation = MODELS.build(act_cfg)
 
         # add bias for reshaped 2D feature.
         self.register_parameter(
             'bias', nn.Parameter(torch.zeros(1, out_channels, 1, 1)))
 
         if self.with_norm:
             _, self.norm = build_norm_layer(norm_cfg, out_channels)
@@ -475,18 +473,18 @@
             self.mid_channels,
             self.out_channels,
             bias=bias,
             equalized_lr_cfg=equalized_lr_cfg)
 
         # setup activation layers
         if self.with_activation:
-            self.activation = build_activation_layer(act_cfg)
+            self.activation = MODELS.build(act_cfg)
 
         if self.with_out_activation:
-            self.out_activation = build_activation_layer(out_act)
+            self.out_activation = MODELS.build(out_act)
 
     def forward(self, x):
         """Forward function.
 
         Args:
             x (Tensor): Input tensor with shape (n, c, h, w).
 
@@ -504,15 +502,15 @@
         if self.with_out_activation:
             x = self.out_activation(x)
 
         return x
 
 
 @MODULES.register_module()
-@PLUGIN_LAYERS.register_module()
+@MODELS.register_module()
 class MiniBatchStddevLayer(nn.Module):
     """Minibatch standard deviation.
 
     Args:
         group_size (int, optional): The size of groups in batch dimension.
             Defaults to 4.
         eps (float, optional):  Epsilon value to avoid computation error.
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/pix2pix/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/pix2pix/generator_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 from mmcv.cnn import ConvModule, build_conv_layer
-from mmcv.runner import load_checkpoint
+from mmengine.logging import MMLogger
+from mmengine.runner import load_checkpoint
 
 from mmgen.models.builder import MODULES
-from mmgen.utils import get_root_logger
 from .modules import UnetSkipConnectionBlock, generation_init_weights
 
 
 @MODULES.register_module()
 class UnetGenerator(nn.Module):
     """Construct the Unet-based generator from the innermost layer to the
     outermost layer, which is a recursive process.
@@ -112,15 +112,15 @@
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Default: None.
             strict (bool, optional): Whether to allow different params for the
                 model and checkpoint. Default: True.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=strict, logger=logger)
         elif pretrained is None:
             generation_init_weights(
                 self, init_type=self.init_type, init_gain=self.init_gain)
         else:
             raise TypeError("'pretrained' must be a str or None. "
                             f'But received {type(pretrained)}.')
@@ -238,15 +238,15 @@
         """Initialize weights for the model.
 
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Default: None.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif pretrained is None:
             generation_init_weights(
                 self, init_type=self.init_type, init_gain=self.init_gain)
         else:
             raise TypeError("'pretrained' must be a str or None. "
                             f'But received {type(pretrained)}.')
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/pix2pix/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/pix2pix/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.nn as nn
-from mmcv.cnn import ConvModule, kaiming_init, normal_init, xavier_init
+from mmcv.cnn import ConvModule
+from mmengine.model import kaiming_init, normal_init, xavier_init
 from torch.nn import init
 
 
 def generation_init_weights(module, init_type='normal', init_gain=0.02):
     """Default initialization of network weights for image generation.
 
     By default, we use normal init, but xavier and kaiming might work
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/positional_encoding.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/positional_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 import torch.nn as nn
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODULES
 
 
 @MODULES.register_module('SPE')
 @MODULES.register_module('SPE2d')
 class SinusoidalPositionalEmbedding(nn.Module):
     """Sinusoidal Positional Embedding 1D or 2D (SPE/SPE2d).
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/singan/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/singan/generator_discriminator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from functools import partial
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mmcv.runner import load_state_dict
-from mmcv.utils import print_log
+from mmengine import print_log
+from mmengine.logging import MMLogger
+# from mmcv.runner import load_state_dict
+from mmengine.runner import load_state_dict
 
 from mmgen.models.builder import MODULES
-from mmgen.utils import get_root_logger
 from .modules import DiscriminatorBlock, GeneratorBlock
 
 
 @MODULES.register_module()
 class SinGANMultiScaleGenerator(nn.Module):
     """Multi-Scale Generator used in SinGAN.
 
@@ -154,35 +155,37 @@
                 h_next, w_next = fixed_noises[stage + 1].shape[-2:]
                 g_res = self.upsample(g_res, (h_next, w_next))
 
         if get_prev_res or return_noise:
             output_dict = dict(
                 fake_img=g_res,
                 prev_res_list=prev_res_list,
-                noise_batch=noise_list)
+                # noise_batch=noise_list
+            )
             return output_dict
 
         return g_res
 
     def check_and_load_prev_weight(self, curr_scale):
+        logger = MMLogger.get_current_instance()
         if curr_scale == 0:
             return
         prev_ch = self.blocks[curr_scale - 1].base_channels
         curr_ch = self.blocks[curr_scale].base_channels
 
         prev_in_ch = self.blocks[curr_scale - 1].in_channels
         curr_in_ch = self.blocks[curr_scale].in_channels
         if prev_ch == curr_ch and prev_in_ch == curr_in_ch:
             load_state_dict(
                 self.blocks[curr_scale],
                 self.blocks[curr_scale - 1].state_dict(),
-                logger=get_root_logger())
-            print_log('Successfully load pretrianed model from last scale.')
+                logger=MMLogger.get_current_instance())
+            logger.info('Successfully load pretrianed model from last scale.')
         else:
-            print_log(
+            logger.info(
                 'Cannot load pretrained model from last scale since'
                 f' prev_ch({prev_ch}) != curr_ch({curr_ch})'
                 f' or prev_in_ch({prev_in_ch}) != curr_in_ch({curr_in_ch})')
 
 
 @MODULES.register_module()
 class SinGANMultiScaleDiscriminator(nn.Module):
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/singan/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/singan/modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
-from mmcv.cnn import ConvModule, constant_init, normal_init
-from mmcv.runner import load_checkpoint
-from mmcv.utils.parrots_wrapper import _BatchNorm
-
-from mmgen.utils import get_root_logger
+from mmcv.cnn import ConvModule
+from mmengine.logging import MMLogger
+from mmengine.model import constant_init, normal_init
+from mmengine.runner import load_checkpoint
+from mmengine.utils.dl_utils.parrots_wrapper import _BatchNorm
 
 
 class GeneratorBlock(nn.Module):
     """Generator block used in SinGAN.
 
     Args:
         in_channels (int): Input channels.
@@ -109,15 +109,15 @@
         if self.allow_no_residual and x.shape[1] != prev.shape[1]:
             return x
 
         return x + prev
 
     def init_weights(self, pretrained=None):
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, nn.Conv2d):
                     normal_init(m, 0, 0.02)
                 elif isinstance(m, (_BatchNorm, nn.InstanceNorm2d)):
                     constant_init(m, 1)
@@ -213,15 +213,15 @@
         x = self.tail(x)
 
         return x
 
     # TODO: study the effects of init functions
     def init_weights(self, pretrained=None):
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=False, logger=logger)
         elif pretrained is None:
             for m in self.modules():
                 if isinstance(m, nn.Conv2d):
                     normal_init(m, 0, 0.02)
                 elif isinstance(m, (_BatchNorm, nn.InstanceNorm2d)):
                     constant_init(m, 1)
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/singan/positional_encoding.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/singan/positional_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 
 In this module, we provide necessary components to conduct experiments
 mentioned in the paper: Positional Encoding as Spatial Inductive Bias in GANs.
 More details can be found in: https://arxiv.org/pdf/2012.05217.pdf
 """
 from functools import partial
 
-import mmcv
+import mmengine
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from mmgen.models.builder import MODULES, build_module
+from mmgen.models.builder import build_module
+from mmgen.registry import MODULES
 from .generator_discriminator import SinGANMultiScaleGenerator
 from .modules import GeneratorBlock
 
 
 @MODULES.register_module()
 class SinGANMSGeneratorPE(SinGANMultiScaleGenerator):
     """Multi-Scale Generator used in SinGAN with positional encoding.
@@ -127,15 +128,15 @@
             self.noise_padding_layer = nn.ZeroPad2d(self.pad_head)
             self.img_padding_layer = nn.ZeroPad2d(self.pad_head)
             self.mask_padding_layer = nn.ReflectionPad2d(self.pad_head)
         elif padding_mode == 'reflect':
             self.noise_padding_layer = nn.ReflectionPad2d(self.pad_head)
             self.img_padding_layer = nn.ReflectionPad2d(self.pad_head)
             self.mask_padding_layer = nn.ReflectionPad2d(self.pad_head)
-            mmcv.print_log('Using Reflection padding', 'mmgen')
+            mmengine.print_log('Using Reflection padding', 'current')
         else:
             raise NotImplementedError(
                 f'Padding mode {padding_mode} is not supported')
 
     def forward(self,
                 input_sample,
                 fixed_noises,
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/sngan_proj/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/sngan_proj/generator_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import numpy as np
 import torch
 import torch.nn as nn
-from mmcv.cnn import (ConvModule, build_activation_layer, constant_init,
-                      xavier_init)
-from mmcv.runner import load_checkpoint
-from mmcv.runner.checkpoint import _load_checkpoint_with_prefix
-from mmcv.utils import is_list_of
+from mmcv.cnn import ConvModule
+from mmengine import is_list_of
+from mmengine.logging import MMLogger
+from mmengine.model import constant_init, xavier_init
+from mmengine.runner import load_checkpoint
+from mmengine.runner.checkpoint import _load_checkpoint_with_prefix
 from torch.nn.init import xavier_uniform_
 from torch.nn.utils import spectral_norm
 
-from mmgen.models.builder import MODULES, build_module
+from mmgen.models.builder import build_module
+from mmgen.registry import MODELS, MODULES
 from mmgen.utils import check_dist_init
-from mmgen.utils.logger import get_root_logger
 from ..common import get_module_device
 
 
 @MODULES.register_module('SAGANGenerator')
 @MODULES.register_module()
 class SNGANGenerator(nn.Module):
     r"""Generator for SNGAN / Proj-GAN. The implementation refers to
@@ -102,14 +103,18 @@
             Defaults to `1e-12`.
         init_cfg (string, optional): Config for weight initialization.
             Defaults to ``dict(type='BigGAN')``.
         pretrained (str | dict, optional): Path for the pretrained model or
             dict containing information for pretained models whose necessary
             key is 'ckpt_path'. Besides, you can also provide 'prefix' to load
             the generator part from the whole state dict.  Defaults to None.
+        rgb_to_bgr (bool, optional): Whether to reformat the output channels
+                with order `bgr`. We provide several pre-trained BigGAN
+                weights whose output channels order is `rgb`. You can set
+                this argument to True to use the weights.
     """
 
     # default channel factors
     _default_channels_cfg = {
         32: [1, 1, 1],
         64: [16, 8, 4, 2],
         128: [16, 16, 8, 4, 2]
@@ -131,23 +136,25 @@
                  auto_sync_bn=True,
                  with_spectral_norm=False,
                  with_embedding_spectral_norm=None,
                  sn_style='torch',
                  norm_eps=1e-4,
                  sn_eps=1e-12,
                  init_cfg=dict(type='BigGAN'),
-                 pretrained=None):
+                 pretrained=None,
+                 rgb_to_bgr=False):
 
         super().__init__()
 
         self.input_scale = input_scale
         self.output_scale = output_scale
         self.noise_size = noise_size
         self.num_classes = num_classes
         self.init_type = init_cfg.get('type', None)
+        self.rgb_to_bgr = rgb_to_bgr
 
         self.blocks_cfg = deepcopy(blocks_cfg)
 
         self.blocks_cfg.setdefault('num_classes', num_classes)
         self.blocks_cfg.setdefault('act_cfg', act_cfg)
         self.blocks_cfg.setdefault('use_cbn', use_cbn)
         self.blocks_cfg.setdefault('auto_sync_bn', auto_sync_bn)
@@ -223,15 +230,15 @@
             stride=1,
             padding=1,
             bias=True,
             norm_cfg=to_rgb_norm_cfg,
             act_cfg=act_cfg,
             order=('norm', 'act', 'conv'),
             with_spectral_norm=with_spectral_norm)
-        self.final_act = build_activation_layer(dict(type='Tanh'))
+        self.final_act = MODELS.build(dict(type='Tanh'))
 
         self.init_weights(pretrained)
 
     def forward(self, noise, num_batches=0, label=None, return_noise=False):
         """Forward function.
 
         Args:
@@ -296,14 +303,17 @@
                 x = conv_block(x)
             else:
                 x = conv_block(x, label_batch)
 
         out_feat = self.to_rgb(x)
         out_img = self.final_act(out_feat)
 
+        if self.rgb_to_bgr:
+            out_img = out_img[:, [2, 1, 0], ...]
+
         if return_noise:
             return dict(
                 fake_img=out_img, noise_batch=noise_batch, label=label_batch)
         return out_img
 
     def init_weights(self, pretrained=None, strict=True):
         """Init weights for SNGAN-Proj and SAGAN. If ``pretrained=None``,
@@ -329,15 +339,15 @@
             pretrained (str | dict, optional): Path for the pretrained model or
                 dict containing information for pretained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=strict, logger=logger)
         elif isinstance(pretrained, dict):
             ckpt_path = pretrained.get('ckpt_path', None)
             assert ckpt_path is not None
             prefix = pretrained.get('prefix', '')
             map_location = pretrained.get('map_location', 'cpu')
             strict = pretrained.get('strict', True)
@@ -638,15 +648,15 @@
         # In this case, discriminator is designed for conditional synthesis.
         if num_classes > 0:
             self.proj_y = nn.Embedding(num_classes,
                                        factor_output * base_channels)
             if with_spectral_norm:
                 self.proj_y = spectral_norm(self.proj_y)
 
-        self.activate = build_activation_layer(act_cfg)
+        self.activate = MODELS.build(act_cfg)
         self.init_weights(pretrained)
 
     def forward(self, x, label=None):
         """Forward function. If `self.num_classes` is larger than 0, label
         projection would be used.
 
         Args:
@@ -694,15 +704,15 @@
             pretrained (str | dict, optional): Path for the pretrained model or
                 dict containing information for pretained models whose
                 necessary key is 'ckpt_path'. Besides, you can also provide
                 'prefix' to load the generator part from the whole state dict.
                 Defaults to None.
         """
         if isinstance(pretrained, str):
-            logger = get_root_logger()
+            logger = MMLogger.get_current_instance()
             load_checkpoint(self, pretrained, strict=strict, logger=logger)
         elif isinstance(pretrained, dict):
             ckpt_path = pretrained.get('ckpt_path', None)
             assert ckpt_path is not None
             prefix = pretrained.get('prefix', '')
             map_location = pretrained.get('map_location', 'cpu')
             strict = pretrained.get('strict', True)
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/sngan_proj/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/sngan_proj/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import numpy as np
 import torch.nn as nn
-from mmcv.cnn import (build_activation_layer, build_norm_layer,
-                      build_upsample_layer, constant_init, xavier_init)
+from mmcv.cnn import build_norm_layer
+from mmengine.model import constant_init, xavier_init
 from torch.nn.init import xavier_uniform_
 from torch.nn.utils import spectral_norm
 
 from mmgen.models.architectures.biggan.biggan_snmodule import SNEmbedding
 from mmgen.models.architectures.biggan.modules import SNConvModule
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODELS, MODULES
 from mmgen.utils import check_dist_init
 
 
 @MODULES.register_module()
 class SNGANGenResBlock(nn.Module):
     """ResBlock used in Generator of SNGAN / Proj-GAN.
 
@@ -85,20 +85,20 @@
                  init_cfg=dict(type='BigGAN')):
 
         super().__init__()
         self.learnable_sc = in_channels != out_channels or upsample
         self.with_upsample = upsample
         self.init_type = init_cfg.get('type', None)
 
-        self.activate = build_activation_layer(act_cfg)
+        self.activate = MODELS.build(act_cfg)
         hidden_channels = out_channels if hidden_channels is None \
             else hidden_channels
 
         if self.with_upsample:
-            self.upsample = build_upsample_layer(upsample_cfg)
+            self.upsample = MODELS.build(upsample_cfg)
 
         self.conv_cfg = deepcopy(self._default_conv_cfg)
         if conv_cfg is not None:
             self.conv_cfg.update(conv_cfg)
 
         # set `norm_spectral_norm` as `with_spectral_norm` if not defined
         with_embedding_spectral_norm = with_embedding_spectral_norm \
@@ -253,15 +253,15 @@
         self.with_downsample = downsample
         self.init_type = init_cfg.get('type', None)
 
         self.conv_cfg = deepcopy(self._default_conv_cfg)
         if conv_cfg is not None:
             self.conv_cfg.update(conv_cfg)
 
-        self.activate = build_activation_layer(act_cfg)
+        self.activate = MODELS.build(act_cfg)
 
         sn_cfg = dict(eps=sn_eps, sn_style=sn_style)
         self.conv_1 = SNConvModule(
             in_channels,
             hidden_channels,
             with_spectral_norm=with_spectral_norm,
             spectral_norm_cfg=sn_cfg,
@@ -390,15 +390,15 @@
         super().__init__()
 
         self.init_type = init_cfg.get('type', None)
         self.conv_cfg = deepcopy(self._default_conv_cfg)
         if conv_cfg is not None:
             self.conv_cfg.update(conv_cfg)
 
-        self.activate = build_activation_layer(act_cfg)
+        self.activate = MODELS.build(act_cfg)
 
         sn_cfg = dict(eps=sn_eps, sn_style=sn_style)
         self.conv_1 = SNConvModule(
             in_channels,
             out_channels,
             with_spectral_norm=with_spectral_norm,
             spectral_norm_cfg=sn_cfg,
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/__init__.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/__init__.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/generator_discriminator_v1.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/generator_discriminator_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import random
 
-import mmcv
+import mmengine
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from mmgen.models.architectures import PixelNorm
 from mmgen.models.architectures.common import get_module_device
 from mmgen.models.architectures.pggan import (EqualizedLRConvDownModule,
                                               EqualizedLRConvModule)
 from mmgen.models.architectures.stylegan.modules import Blur
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODULES
 from .. import MiniBatchStddevLayer
 from .modules.styleganv1_modules import StyleConv
 from .modules.styleganv2_modules import EqualLinearActModule
 from .utils import get_mean_latent, style_mixing
 
 
 @MODULES.register_module()
@@ -123,24 +123,22 @@
             shape = [1, 1, 2**res, 2**res]
             self.register_buffer(f'injected_noise_{layer_idx}',
                                  torch.randn(*shape))
 
     def train(self, mode=True):
         if mode:
             if self.default_style_mode != self._default_style_mode:
-                mmcv.print_log(
-                    f'Switch to train style mode: {self._default_style_mode}',
-                    'mmgen')
+                mmengine.print_log(
+                    f'Switch to train style mode: {self._default_style_mode}')
             self.default_style_mode = self._default_style_mode
 
         else:
             if self.default_style_mode != self.eval_style_mode:
-                mmcv.print_log(
-                    f'Switch to evaluation style mode: {self.eval_style_mode}',
-                    'mmgen')
+                mmengine.print_log(
+                    f'Switch to evaluation style mode: {self.eval_style_mode}')
             self.default_style_mode = self.eval_style_mode
 
         return super(StyleGANv1Generator, self).train(mode)
 
     def make_injected_noise(self):
         """make noises that will be injected into feature maps.
 
@@ -246,15 +244,15 @@
             torch.Tensor | dict: Generated image tensor or dictionary \
                 containing more data.
         """
         # receive noise and conduct sanity check.
         if isinstance(styles, torch.Tensor):
             assert styles.shape[1] == self.style_channels
             styles = [styles]
-        elif mmcv.is_seq_of(styles, torch.Tensor):
+        elif mmengine.is_seq_of(styles, torch.Tensor):
             for t in styles:
                 assert t.shape[-1] == self.style_channels
         # receive a noise generator and sample noise.
         elif callable(styles):
             device = get_module_device(self)
             noise_generator = styles
             assert num_batches > 0
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/generator_discriminator_v2.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/generator_discriminator_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import random
 
-import mmcv
+import mmengine
 import numpy as np
 import torch
 import torch.nn as nn
-from mmcv.runner.checkpoint import _load_checkpoint_with_prefix
+from mmengine.runner.amp import autocast
+from mmengine.runner.checkpoint import _load_checkpoint_with_prefix
 
-from mmgen.core.runners.fp16_utils import auto_fp16
 from mmgen.models.architectures import PixelNorm
 from mmgen.models.architectures.common import get_module_device
-from mmgen.models.builder import MODULES, build_module
+from mmgen.models.builder import build_module
+from mmgen.registry import MODULES
 from .ada.augment import AugmentPipe
 from .ada.misc import constant
 from .modules.styleganv2_modules import (ConstantInput, ConvDownLayer,
                                          EqualLinearActModule,
                                          ModMBStddevLayer, ModulatedStyleConv,
                                          ModulatedToRGB, ResBlock)
 from .utils import get_mean_latent, style_mixing
@@ -143,15 +144,16 @@
         self.constant_input = ConstantInput(self.channels[4])
         # 4x4 stage
         self.conv1 = ModulatedStyleConv(
             self.channels[4],
             self.channels[4],
             kernel_size=3,
             style_channels=style_channels,
-            blur_kernel=blur_kernel)
+            blur_kernel=blur_kernel,
+            fp16_enabled=fp16_enabled)
         self.to_rgb1 = ModulatedToRGB(
             self.channels[4],
             style_channels,
             upsample=False,
             fp16_enabled=fp16_enabled)
 
         # generator backbone (8x8 --> higher resolutions)
@@ -215,29 +217,27 @@
                                ckpt_path,
                                prefix='',
                                map_location='cpu',
                                strict=True):
         state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                   map_location)
         self.load_state_dict(state_dict, strict=strict)
-        mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+        mmengine.print_log(f'Load pretrained model from {ckpt_path}')
 
     def train(self, mode=True):
         if mode:
             if self.default_style_mode != self._default_style_mode:
-                mmcv.print_log(
-                    f'Switch to train style mode: {self._default_style_mode}',
-                    'mmgen')
+                mmengine.print_log(
+                    f'Switch to train style mode: {self._default_style_mode}')
             self.default_style_mode = self._default_style_mode
 
         else:
             if self.default_style_mode != self.eval_style_mode:
-                mmcv.print_log(
-                    f'Switch to evaluation style mode: {self.eval_style_mode}',
-                    'mmgen')
+                mmengine.print_log(
+                    f'Switch to evaluation style mode: {self.eval_style_mode}')
             self.default_style_mode = self.eval_style_mode
 
         return super(StyleGANv2Generator, self).train(mode)
 
     def make_injected_noise(self):
         """make noises that will be injected into feature maps.
 
@@ -277,15 +277,15 @@
             n_source=n_source,
             n_target=n_target,
             inject_index=inject_index,
             truncation=truncation,
             truncation_latent=truncation_latent,
             style_channels=self.style_channels)
 
-    @auto_fp16()
+    # @auto_fp16()
     def forward(self,
                 styles,
                 num_batches=-1,
                 return_noise=False,
                 return_latents=False,
                 inject_index=None,
                 truncation=1,
@@ -332,15 +332,15 @@
             torch.Tensor | dict: Generated image tensor or dictionary \
                 containing more data.
         """
         # receive noise and conduct sanity check.
         if isinstance(styles, torch.Tensor):
             assert styles.shape[1] == self.style_channels
             styles = [styles]
-        elif mmcv.is_seq_of(styles, torch.Tensor):
+        elif mmengine.is_seq_of(styles, torch.Tensor):
             for t in styles:
                 assert t.shape[-1] == self.style_channels
         # receive a noise generator and sample noise.
         elif callable(styles):
             device = get_module_device(self)
             noise_generator = styles
             assert num_batches > 0
@@ -363,80 +363,83 @@
                     torch.randn((num_batches, self.style_channels))
                     for _ in range(2)
                 ]
             else:
                 styles = [torch.randn((num_batches, self.style_channels))]
             styles = [s.to(device) for s in styles]
 
-        if not input_is_latent:
-            noise_batch = styles
-            styles = [self.style_mapping(s) for s in styles]
-        else:
-            noise_batch = None
-
-        if injected_noise is None:
-            if randomize_noise:
-                injected_noise = [None] * self.num_injected_noises
+        with autocast(enabled=self.fp16_enabled):
+            if not input_is_latent:
+                noise_batch = styles
+                styles = [self.style_mapping(s) for s in styles]
             else:
-                injected_noise = [
-                    getattr(self, f'injected_noise_{i}')
-                    for i in range(self.num_injected_noises)
-                ]
-        # use truncation trick
-        if truncation < 1:
-            style_t = []
-            # calculate truncation latent on the fly
-            if truncation_latent is None and not hasattr(
-                    self, 'truncation_latent'):
-                self.truncation_latent = self.get_mean_latent()
-                truncation_latent = self.truncation_latent
-            elif truncation_latent is None and hasattr(self,
-                                                       'truncation_latent'):
-                truncation_latent = self.truncation_latent
-
-            for style in styles:
-                style_t.append(truncation_latent + truncation *
-                               (style - truncation_latent))
-
-            styles = style_t
-        # no style mixing
-        if len(styles) < 2:
-            inject_index = self.num_latents
-
-            if styles[0].ndim < 3:
-                latent = styles[0].unsqueeze(1).repeat(1, inject_index, 1)
+                noise_batch = None
 
+            if injected_noise is None:
+                if randomize_noise:
+                    injected_noise = [None] * self.num_injected_noises
+                else:
+                    injected_noise = [
+                        getattr(self, f'injected_noise_{i}')
+                        for i in range(self.num_injected_noises)
+                    ]
+            # use truncation trick
+            if truncation < 1:
+                style_t = []
+                # calculate truncation latent on the fly
+                if truncation_latent is None and not hasattr(
+                        self, 'truncation_latent'):
+                    self.truncation_latent = self.get_mean_latent()
+                    truncation_latent = self.truncation_latent
+                elif truncation_latent is None and hasattr(
+                        self, 'truncation_latent'):
+                    truncation_latent = self.truncation_latent
+
+                for style in styles:
+                    style_t.append(truncation_latent + truncation *
+                                   (style - truncation_latent))
+
+                styles = style_t
+            # no style mixing
+            if len(styles) < 2:
+                inject_index = self.num_latents
+
+                if styles[0].ndim < 3:
+                    latent = styles[0].unsqueeze(1).repeat(1, inject_index, 1)
+
+                else:
+                    latent = styles[0]
+            # style mixing
             else:
-                latent = styles[0]
-        # style mixing
-        else:
-            if inject_index is None:
-                inject_index = random.randint(1, self.num_latents - 1)
+                if inject_index is None:
+                    inject_index = random.randint(1, self.num_latents - 1)
 
-            latent = styles[0].unsqueeze(1).repeat(1, inject_index, 1)
-            latent2 = styles[1].unsqueeze(1).repeat(
-                1, self.num_latents - inject_index, 1)
+                latent = styles[0].unsqueeze(1).repeat(1, inject_index, 1)
+                latent2 = styles[1].unsqueeze(1).repeat(
+                    1, self.num_latents - inject_index, 1)
 
-            latent = torch.cat([latent, latent2], 1)
+                latent = torch.cat([latent, latent2], 1)
 
-        # 4x4 stage
-        out = self.constant_input(latent)
-        out = self.conv1(out, latent[:, 0], noise=injected_noise[0])
-        skip = self.to_rgb1(out, latent[:, 1])
-
-        _index = 1
-
-        # 8x8 ---> higher resolutions
-        for up_conv, conv, noise1, noise2, to_rgb in zip(
-                self.convs[::2], self.convs[1::2], injected_noise[1::2],
-                injected_noise[2::2], self.to_rgbs):
-            out = up_conv(out, latent[:, _index], noise=noise1)
-            out = conv(out, latent[:, _index + 1], noise=noise2)
-            skip = to_rgb(out, latent[:, _index + 2], skip)
-            _index += 2
+            # 4x4 stage
+            out = self.constant_input(latent)
+            if self.fp16_enabled:
+                out = out.to(torch.float16)
+            out = self.conv1(out, latent[:, 0], noise=injected_noise[0])
+            skip = self.to_rgb1(out, latent[:, 1])
+
+            _index = 1
+
+            # 8x8 ---> higher resolutions
+            for up_conv, conv, noise1, noise2, to_rgb in zip(
+                    self.convs[::2], self.convs[1::2], injected_noise[1::2],
+                    injected_noise[2::2], self.to_rgbs):
+                out = up_conv(out, latent[:, _index], noise=noise1)
+                out = conv(out, latent[:, _index + 1], noise=noise2)
+                skip = to_rgb(out, latent[:, _index + 2], skip)
+                _index += 2
 
         # make sure the output image is torch.float32 to avoid RunTime Error
         # in other modules
         img = skip.to(torch.float32)
 
         if return_latents or return_noise:
             output_dict = dict(
@@ -567,15 +570,16 @@
 
             in_channels = out_channel
 
         self.convs = nn.Sequential(*convs)
 
         self.mbstd_layer = ModMBStddevLayer(**mbstd_cfg)
 
-        self.final_conv = ConvDownLayer(in_channels + 1, channels[4], 3)
+        self.final_conv = ConvDownLayer(
+            in_channels + 1, channels[4], 3, fp16_enabled=fp16_enabled)
         self.final_linear = nn.Sequential(
             EqualLinearActModule(
                 channels[4] * 4 * 4,
                 channels[4],
                 act_cfg=dict(type='fused_bias')),
             EqualLinearActModule(channels[4], 1),
         )
@@ -588,38 +592,42 @@
                                ckpt_path,
                                prefix='',
                                map_location='cpu',
                                strict=True):
         state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                   map_location)
         self.load_state_dict(state_dict, strict=strict)
-        mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+        mmengine.print_log(f'Load pretrained model from {ckpt_path}')
 
-    @auto_fp16()
     def forward(self, x):
         """Forward function.
 
         Args:
             x (torch.Tensor): Input image tensor.
 
         Returns:
             torch.Tensor: Predict score for the input image.
         """
         # This setting was used to finetune on converted weights
         if self.input_bgr2rgb:
             x = x[:, [2, 1, 0], ...]
 
+        # convs has own fp-16 controller, do not wrap here
         x = self.convs(x)
 
         x = self.mbstd_layer(x)
-        if not self.final_conv.fp16_enabled and self.convert_input_fp32:
-            x = x.to(torch.float32)
-        x = self.final_conv(x)
-        x = x.view(x.shape[0], -1)
-        x = self.final_linear(x)
+
+        fp16_enabled = (
+            self.final_conv.fp16_enabled or not self.convert_input_fp32)
+        with autocast(enabled=fp16_enabled):
+            if not fp16_enabled:
+                x = x.to(torch.float32)
+            x = self.final_conv(x)
+            x = x.view(x.shape[0], -1)
+            x = self.final_linear(x)
 
         return x
 
 
 @MODULES.register_module()
 class ADAStyleGAN2Discriminator(StyleGAN2Discriminator):
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/generator_discriminator_v3.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/generator_discriminator_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
-import mmcv
+import mmengine
 import torch
 import torch.nn as nn
-from mmcv.runner.checkpoint import _load_checkpoint_with_prefix
+from mmengine.runner.checkpoint import _load_checkpoint_with_prefix
 
 from mmgen.models.architectures.common import get_module_device
-from mmgen.models.builder import MODULES, build_module
+from mmgen.models.builder import build_module
+from mmgen.registry import MODULES
 from .utils import get_mean_latent
 
 
 @MODULES.register_module()
 class StyleGANv3Generator(nn.Module):
     """StyleGAN3 Generator.
 
@@ -78,15 +79,15 @@
                                ckpt_path,
                                prefix='',
                                map_location='cpu',
                                strict=True):
         state_dict = _load_checkpoint_with_prefix(prefix, ckpt_path,
                                                   map_location)
         self.load_state_dict(state_dict, strict=strict)
-        mmcv.print_log(f'Load pretrained model from {ckpt_path}', 'mmgen')
+        mmengine.print_log(f'Load pretrained model from {ckpt_path}')
 
     def forward(self,
                 noise,
                 num_batches=0,
                 input_is_latent=False,
                 truncation=1,
                 num_truncation_layer=None,
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/__init__.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/styleganv1_modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/styleganv1_modules.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/styleganv2_modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/styleganv2_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 from functools import partial
 
-import mmcv
+import mmengine
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from mmcv.cnn.bricks.activation import build_activation_layer
 from mmcv.ops.fused_bias_leakyrelu import (FusedBiasLeakyReLU,
                                            fused_bias_leakyrelu)
 from mmcv.ops.upfirdn2d import upfirdn2d
-from mmcv.runner.dist_utils import get_dist_info
+from mmengine.dist import get_dist_info
+from mmengine.runner.amp import autocast
 
-from mmgen.core.runners.fp16_utils import auto_fp16
 from mmgen.models.architectures.pggan import (EqualizedLRConvModule,
                                               EqualizedLRLinearModule,
                                               equalized_lr)
 from mmgen.models.common import AllGatherLayer
 from mmgen.ops import conv2d, conv_transpose2d
+from mmgen.registry import MODELS
 
 
 class _FusedBiasLeakyReLU(FusedBiasLeakyReLU):
     """Wrap FusedBiasLeakyReLU to support FP16 training."""
 
     def forward(self, x):
         """Forward function.
@@ -83,15 +83,15 @@
             act_cfg = deepcopy(act_cfg)
             if act_cfg['type'] == 'fused_bias':
                 self.act_type = act_cfg.pop('type')
                 assert self.bias is not None
                 self.activate = partial(fused_bias_leakyrelu, **act_cfg)
             else:
                 self.act_type = 'normal'
-                self.activate = build_activation_layer(act_cfg)
+                self.activate = MODELS.build(act_cfg)
         else:
             self.act_type = None
 
     def forward(self, x):
         """Forward function.
 
         Args:
@@ -284,21 +284,23 @@
             upsample=False,
             downsample=False,
             blur_kernel=[1, 3, 3, 1],
             equalized_lr_cfg=dict(mode='fan_in', lr_mul=1., gain=1.),
             style_mod_cfg=dict(bias_init=1.),
             style_bias=0.,
             padding=None,  # self define padding
-            eps=1e-8):
+            eps=1e-8,
+            fp16_enabled=False):
         super().__init__()
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.kernel_size = kernel_size
         self.style_channels = style_channels
         self.demodulate = demodulate
+        self.fp16_enabled = fp16_enabled
         # sanity check for kernel size
         assert isinstance(self.kernel_size,
                           int) and (self.kernel_size >= 1
                                     and self.kernel_size % 2 == 1)
         self.upsample = upsample
         self.downsample = downsample
         self.style_bias = style_bias
@@ -340,62 +342,67 @@
         self.padding = padding if padding else (kernel_size // 2)
 
     def forward(self, x, style, input_gain=None):
         n, c, h, w = x.shape
 
         weight = self.weight
         # Pre-normalize inputs to avoid FP16 overflow.
-        if x.dtype == torch.float16 and self.demodulate:
+        # if x.dtype == torch.float16 and self.demodulate:
+        if self.fp16_enabled and self.demodulate:
             weight = weight * (
                 1 / np.sqrt(
                     self.in_channels * self.kernel_size * self.kernel_size) /
                 weight.norm(float('inf'), dim=[1, 2, 3], keepdim=True)
             )  # max_Ikk
             style = style / style.norm(
                 float('inf'), dim=1, keepdim=True)  # max_I
 
-        # process style code
-        style = self.style_modulation(style).view(n, 1, c, 1,
-                                                  1) + self.style_bias
-        # combine weight and style
-        weight = weight * style
-        if self.demodulate:
-            demod = torch.rsqrt(weight.pow(2).sum([2, 3, 4]) + self.eps)
-            weight = weight * demod.view(n, self.out_channels, 1, 1, 1)
-
-        if input_gain is not None:
-            # input_gain shape [batch, in_ch]
-            input_gain = input_gain.expand(n, self.in_channels)
-            # weight shape [batch, out_ch, in_ch, kernel_size, kernel_size]
-            weight = weight * input_gain.unsqueeze(1).unsqueeze(3).unsqueeze(4)
-
-        weight = weight.view(n * self.out_channels, c, self.kernel_size,
-                             self.kernel_size)
+        with autocast(enabled=self.fp16_enabled):
+            # process style code
+            style = self.style_modulation(style).view(n, 1, c, 1,
+                                                      1) + self.style_bias
+            # combine weight and style
+            weight = weight * style
+            if self.demodulate:
+                demod = torch.rsqrt(weight.pow(2).sum([2, 3, 4]) + self.eps)
+                weight = weight * demod.view(n, self.out_channels, 1, 1, 1)
+
+            if input_gain is not None:
+                # input_gain shape [batch, in_ch]
+                input_gain = input_gain.expand(n, self.in_channels)
+                # weight shape [batch, out_ch, in_ch, kernel_size, kernel_size]
+                weight = weight * input_gain.unsqueeze(1).unsqueeze(
+                    3).unsqueeze(4)
 
-        weight = weight.to(x.dtype)
-        if self.upsample:
-            x = x.reshape(1, n * c, h, w)
-            weight = weight.view(n, self.out_channels, c, self.kernel_size,
+            weight = weight.view(n * self.out_channels, c, self.kernel_size,
                                  self.kernel_size)
-            weight = weight.transpose(1, 2).reshape(n * c, self.out_channels,
-                                                    self.kernel_size,
-                                                    self.kernel_size)
-            x = conv_transpose2d(x, weight, padding=0, stride=2, groups=n)
-            x = x.reshape(n, self.out_channels, *x.shape[-2:])
-            x = self.blur(x)
 
-        elif self.downsample:
-            x = self.blur(x)
-            x = x.view(1, n * self.in_channels, *x.shape[-2:])
-            x = conv2d(x, weight, stride=2, padding=0, groups=n)
-            x = x.view(n, self.out_channels, *x.shape[-2:])
-        else:
-            x = x.reshape(1, n * c, h, w)
-            x = conv2d(x, weight, stride=1, padding=self.padding, groups=n)
-            x = x.view(n, self.out_channels, *x.shape[-2:])
+            if self.fp16_enabled:
+                weight = weight.to(torch.float16)
+            if self.upsample:
+                x = x.reshape(1, n * c, h, w)
+                weight = weight.view(n, self.out_channels, c, self.kernel_size,
+                                     self.kernel_size)
+                weight = weight.transpose(1,
+                                          2).reshape(n * c, self.out_channels,
+                                                     self.kernel_size,
+                                                     self.kernel_size)
+                x = conv_transpose2d(x, weight, padding=0, stride=2, groups=n)
+                x = x.reshape(n, self.out_channels, *x.shape[-2:])
+                x = self.blur(x)
+
+            elif self.downsample:
+                x = self.blur(x)
+                x = x.view(1, n * self.in_channels, *x.shape[-2:])
+                x = conv2d(x, weight, stride=2, padding=0, groups=n)
+                x = x.view(n, self.out_channels, *x.shape[-2:])
+            else:
+                x = x.reshape(1, n * c, h, w)
+                x = conv2d(x, weight, stride=1, padding=self.padding, groups=n)
+                x = x.view(n, self.out_channels, *x.shape[-2:])
         return x
 
 
 class NoiseInjection(nn.Module):
     """Noise Injection Module.
 
     In StyleGAN2, they adopt this module to inject spatial random noise map in
@@ -445,15 +452,15 @@
             Defaults to 4.
     """
 
     def __init__(self, channel, size=4):
         super().__init__()
         if isinstance(size, int):
             size = [size, size]
-        elif mmcv.is_seq_of(size, int):
+        elif mmengine.is_seq_of(size, int):
             assert len(
                 size
             ) == 2, f'The length of size should be 2 but got {len(size)}'
         else:
             raise ValueError(f'Got invalid value in size, {size}')
 
         self.input = nn.Parameter(torch.randn(1, channel, *size))
@@ -712,50 +719,52 @@
             out_channels,
             kernel_size,
             style_channels,
             demodulate=demodulate,
             upsample=upsample,
             blur_kernel=blur_kernel,
             style_mod_cfg=style_mod_cfg,
-            style_bias=style_bias)
+            style_bias=style_bias,
+            fp16_enabled=fp16_enabled)
 
         self.noise_injector = NoiseInjection()
         self.activate = _FusedBiasLeakyReLU(out_channels)
 
         # if self.fp16_enabled:
         #     self.half()
 
-    @auto_fp16(apply_to=('x', 'noise'))
     def forward(self, x, style, noise=None, return_noise=False):
         """Forward Function.
 
         Args:
             x ([Tensor): Input features with shape of (N, C, H, W).
             style (Tensor): Style latent with shape of (N, C).
             noise (Tensor, optional): Noise for injection. Defaults to None.
             return_noise (bool, optional): Whether to return noise tensors.
                 Defaults to False.
 
         Returns:
             Tensor: Output features with shape of (N, C, H, W)
         """
-        out = self.conv(x, style)
+        with autocast(enabled=self.fp16_enabled):
+            out = self.conv(x, style)
 
-        if return_noise:
-            out, noise = self.noise_injector(
-                out, noise=noise, return_noise=return_noise)
-        else:
-            out = self.noise_injector(
-                out, noise=noise, return_noise=return_noise)
+            if return_noise:
+                out, noise = self.noise_injector(
+                    out, noise=noise, return_noise=return_noise)
+            else:
+                out = self.noise_injector(
+                    out, noise=noise, return_noise=return_noise)
 
-        # TODO: FP16 in activate layers
-        out = self.activate(out)
+            # TODO: FP16 in activate layers
+            out = self.activate(out)
 
-        if self.fp16_enabled:
-            out = torch.clamp(out, min=-self.conv_clamp, max=self.conv_clamp)
+            if self.fp16_enabled:
+                out = torch.clamp(
+                    out, min=-self.conv_clamp, max=self.conv_clamp)
 
         if return_noise:
             return out, noise
 
         return out
 
 
@@ -892,43 +901,48 @@
         self.conv = ModulatedConv2d(
             in_channels,
             out_channels=out_channels,
             kernel_size=1,
             style_channels=style_channels,
             demodulate=False,
             style_mod_cfg=style_mod_cfg,
-            style_bias=style_bias)
+            style_bias=style_bias,
+            fp16_enabled=fp16_enabled)
 
         self.bias = nn.Parameter(torch.zeros(1, 3, 1, 1))
 
         # enforece the output to be fp32 (follow Tero's implementation)
         self.out_fp32 = out_fp32
 
-    @auto_fp16(apply_to=('x', 'style'))
+    # @auto_fp16(apply_to=('x', 'style'))
     def forward(self, x, style, skip=None):
         """Forward Function.
 
         Args:
             x ([Tensor): Input features with shape of (N, C, H, W).
             style (Tensor): Style latent with shape of (N, C).
             skip (Tensor, optional): Tensor for skip link. Defaults to None.
 
         Returns:
             Tensor: Output features with shape of (N, C, H, W)
         """
-        out = self.conv(x, style)
-        out = out + self.bias.to(x.dtype)
-
-        if self.fp16_enabled:
-            out = torch.clamp(out, min=-self.conv_clamp, max=self.conv_clamp)
-
-        # Here, Tero adopts FP16 at `skip`.
-        if skip is not None:
-            skip = self.upsample(skip)
-            out = out + skip
+        with autocast(enabled=self.fp16_enabled):
+            out = self.conv(x, style)
+            out = out + self.bias.to(x.dtype)
+
+            if self.fp16_enabled:
+                out = torch.clamp(
+                    out, min=-self.conv_clamp, max=self.conv_clamp)
+
+            # Here, Tero adopts FP16 at `skip`.
+            if skip is not None:
+                skip = self.upsample(skip)
+                out = out + skip
+        if self.out_fp32:
+            out = out.to(torch.float32)
         return out
 
 
 class ConvDownLayer(nn.Sequential):
     """Convolution and Downsampling layer.
 
     Args:
@@ -995,19 +1009,20 @@
                 act_cfg=conv_act_cfg,
                 equalized_lr_cfg=dict(mode='fan_in', gain=1.)))
         if self.with_fused_bias:
             layers.append(_FusedBiasLeakyReLU(out_channels))
 
         super(ConvDownLayer, self).__init__(*layers)
 
-    @auto_fp16(apply_to=('x', ))
+    # @auto_fp16(apply_to=('x', ))
     def forward(self, x):
-        x = super().forward(x)
-        if self.fp16_enabled:
-            x = torch.clamp(x, min=-self.conv_clamp, max=self.conv_clamp)
+        with autocast(enabled=self.fp16_enabled):
+            x = super().forward(x)
+            if self.fp16_enabled:
+                x = torch.clamp(x, min=-self.conv_clamp, max=self.conv_clamp)
         return x
 
 
 class ResBlock(nn.Module):
     """Residual block used in the discriminator of StyleGAN2.
 
     Args:
@@ -1047,33 +1062,35 @@
             out_channels,
             1,
             downsample=True,
             act_cfg=None,
             bias=False,
             blur_kernel=blur_kernel)
 
-    @auto_fp16()
+    # @auto_fp16()
     def forward(self, input):
         """Forward function.
 
         Args:
             input (Tensor): Input feature map with shape of (N, C, H, W).
 
         Returns:
             Tensor: Output feature map.
         """
         # TODO: study whether this explicit datatype transfer will harm the
         # apex training speed
-        if not self.fp16_enabled and self.convert_input_fp32:
-            input = input.to(torch.float32)
-        out = self.conv1(input)
-        out = self.conv2(out)
+        fp16_enabled = self.fp16_enabled and not self.convert_input_fp32
+        with autocast(enabled=fp16_enabled):
+            if not fp16_enabled:
+                input = input.to(torch.float32)
+            out = self.conv1(input)
+            out = self.conv2(out)
 
-        skip = self.skip(input)
-        out = (out + skip) / np.sqrt(2)
+            skip = self.skip(input)
+            out = (out + skip) / np.sqrt(2)
 
         return out
 
 
 class ModMBStddevLayer(nn.Module):
     """Modified MiniBatch Stddev Layer.
 
@@ -1110,15 +1127,15 @@
         self.channel_groups = channel_groups
         self.sync_std = sync_std
         self.sync_groups = group_size if sync_groups is None else sync_groups
 
         if self.sync_std:
             assert torch.distributed.is_initialized(
             ), 'Only in distributed training can the sync_std be activated.'
-            mmcv.print_log('Adopt synced minibatch stddev layer', 'mmgen')
+            mmengine.print_log('Adopt synced minibatch stddev layer', 'mmgen')
 
     def forward(self, x):
         """Forward function.
 
         Args:
             x (Tensor): Input feature map with shape of (N, C, H, W).
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/modules/styleganv3_modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/modules/styleganv3_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import scipy
 import torch
 import torch.nn as nn
+from mmengine.runner.amp import autocast
 
-from mmgen.models.builder import MODULES
 from mmgen.ops import bias_act, conv2d_gradfix, filtered_lrelu
+from mmgen.registry import MODULES
 
 
 def modulated_conv2d(
     x,
     w,
     s,
     demodulate=True,
@@ -491,39 +492,44 @@
         if self.is_torgb:
             weight_gain = 1 / np.sqrt(self.in_channels * (self.conv_kernel**2))
             styles = styles * weight_gain
 
         # Execute modulated conv2d.
         dtype = torch.float16 if (self.use_fp16 and not force_fp32 and
                                   x.device.type == 'cuda') else torch.float32
-        x = modulated_conv2d(
-            x=x.to(dtype),
-            w=self.weight,
-            s=styles,
-            padding=self.conv_kernel - 1,
-            demodulate=(not self.is_torgb),
-            input_gain=input_gain)
-
-        # Execute bias, filtered leaky ReLU, and clamping.
-        gain = 1 if self.is_torgb else np.sqrt(2)
-        slope = 1 if self.is_torgb else 0.2
-        x = filtered_lrelu.filtered_lrelu(
-            x=x,
-            fu=self.up_filter,
-            fd=self.down_filter,
-            b=self.bias.to(x.dtype),
-            up=self.up_factor,
-            down=self.down_factor,
-            padding=self.padding,
-            gain=gain,
-            slope=slope,
-            clamp=self.conv_clamp)
+        with autocast(enabled=dtype == torch.float16):
+            x = modulated_conv2d(
+                x=x.to(dtype),
+                w=self.weight,
+                s=styles,
+                padding=self.conv_kernel - 1,
+                demodulate=(not self.is_torgb),
+                input_gain=input_gain)
+
+            # Execute bias, filtered leaky ReLU, and clamping.
+            gain = 1 if self.is_torgb else np.sqrt(2)
+            slope = 1 if self.is_torgb else 0.2
+            x = filtered_lrelu.filtered_lrelu(
+                x=x,
+                fu=self.up_filter,
+                fd=self.down_filter,
+                b=self.bias.to(x.dtype),
+                up=self.up_factor,
+                down=self.down_factor,
+                padding=self.padding,
+                gain=gain,
+                slope=slope,
+                clamp=self.conv_clamp)
 
         # Ensure correct shape and dtype.
-        assert x.dtype == dtype
+        try:
+            assert x.dtype == dtype
+        except Exception:
+            import ipdb
+            ipdb.set_trace()
         return x
 
     @staticmethod
     def design_lowpass_filter(numtaps, cutoff, width, fs, radial=False):
         """Design lowpass filter giving related arguments.
 
         Args:
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/stylegan/mspie.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/stylegan/mspie.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import random
 from copy import deepcopy
 
-import mmcv
+import mmengine
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from mmgen.models.architectures import PixelNorm
 from mmgen.models.architectures.common import get_module_device
-from mmgen.models.builder import MODULES, build_module
+from mmgen.models.builder import build_module
+from mmgen.registry import MODULES
 from .modules.styleganv2_modules import (ConstantInput, ConvDownLayer,
                                          EqualLinearActModule,
                                          ModMBStddevLayer,
                                          ModulatedPEStyleConv, ModulatedToRGB,
                                          ResBlock)
 from .utils import get_mean_latent, style_mixing
 
@@ -189,24 +190,22 @@
         for layer_idx in range(self.num_injected_noises):
             self.register_buffer(f'injected_noise_{layer_idx}',
                                  noises[layer_idx])
 
     def train(self, mode=True):
         if mode:
             if self.default_style_mode != self._default_style_mode:
-                mmcv.print_log(
-                    f'Switch to train style mode: {self._default_style_mode}',
-                    'mmgen')
+                mmengine.print_log(
+                    f'Switch to train style mode: {self._default_style_mode}')
             self.default_style_mode = self._default_style_mode
 
         else:
             if self.default_style_mode != self.eval_style_mode:
-                mmcv.print_log(
-                    f'Switch to evaluation style mode: {self.eval_style_mode}',
-                    'mmgen')
+                mmengine.print_log(
+                    f'Switch to evaluation style mode: {self.eval_style_mode}')
             self.default_style_mode = self.eval_style_mode
 
         return super(MSStyleGANv2Generator, self).train(mode)
 
     def make_injected_noise(self, chosen_scale=0):
         device = get_module_device(self)
 
@@ -309,15 +308,15 @@
             torch.Tensor | dict: Generated image tensor or dictionary \
                 containing more data.
         """
         # receive noise and conduct sanity check.
         if isinstance(styles, torch.Tensor):
             assert styles.shape[1] == self.style_channels
             styles = [styles]
-        elif mmcv.is_seq_of(styles, torch.Tensor):
+        elif mmengine.is_seq_of(styles, torch.Tensor):
             for t in styles:
                 assert t.shape[-1] == self.style_channels
         # receive a noise generator and sample noise.
         elif callable(styles):
             device = get_module_device(self)
             noise_generator = styles
             assert num_batches > 0
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/wgan_gp/generator_discriminator.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/wgan_gp/generator_discriminator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import numpy as np
 import torch
 import torch.nn as nn
 from mmcv.cnn import ConvModule
-from mmcv.cnn.bricks.upsample import build_upsample_layer
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODELS, MODULES
 from ..common import get_module_device
 from .modules import ConvLNModule, WGANDecisionHead, WGANNoiseTo2DFeat
 
 
 @MODULES.register_module()
 class WGANGPGenerator(nn.Module):
     r"""Generator for WGANGP.
@@ -74,16 +73,15 @@
             self.noise_size, self._default_channels_per_scale['4'])
         # set conv_blocks
         self.conv_blocks = nn.ModuleList()
         self.conv_blocks.append(ConvModule(512, 512, **self.conv_module_cfg))
 
         log2scale = int(np.log2(self.out_scale))
         for i in range(3, log2scale + 1):
-            self.conv_blocks.append(
-                build_upsample_layer(self._default_upsample_cfg))
+            self.conv_blocks.append(MODELS.build(self._default_upsample_cfg))
             self.conv_blocks.append(
                 ConvModule(self._default_channels_per_scale[str(2**(i - 1))],
                            self._default_channels_per_scale[str(2**i)],
                            **self.conv_module_cfg))
             self.conv_blocks.append(
                 ConvModule(self._default_channels_per_scale[str(2**i)],
                            self._default_channels_per_scale[str(2**i)],
```

### Comparing `mmgen-0.7.3/mmgen/models/architectures/wgan_gp/modules.py` & `mmgen-1.0.0rc0/mmgen/models/architectures/wgan_gp/modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import torch
 import torch.nn as nn
-from mmcv.cnn import (PLUGIN_LAYERS, ConvModule, build_activation_layer,
-                      build_norm_layer, constant_init)
+from mmcv.cnn import ConvModule, build_norm_layer
+from mmengine.model import constant_init
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODELS, MODULES
 
 
 @MODULES.register_module()
 class WGANNoiseTo2DFeat(nn.Module):
     """Module used in WGAN-GP to transform 1D noise tensor in order [N, C] to
     2D shape feature tensor in order [N, C, H, W].
 
@@ -42,15 +42,15 @@
         assert len(order) == 3 and set(order) == set(['linear', 'act', 'norm'])
 
         # w/o bias, because the bias is added after reshaping the tensor to
         # 2D feature
         self.linear = nn.Linear(noise_size, out_channels * 16, bias=False)
 
         if self.with_activation:
-            self.activation = build_activation_layer(act_cfg)
+            self.activation = MODELS.build(act_cfg)
 
         # add bias for reshaped 2D feature.
         self.register_parameter(
             'bias', nn.Parameter(torch.zeros(1, out_channels, 1, 1)))
 
         if self.with_norm:
             _, self.norm = build_norm_layer(norm_cfg, out_channels)
@@ -130,15 +130,15 @@
             norm_cfg=norm_cfg,
             order=('conv', 'norm', 'act'))
         # setup linear layer
         self.linear = nn.Linear(
             self.mid_channels, self.out_channels, bias=bias)
 
         if self.with_out_activation:
-            self.out_activation = build_activation_layer(out_act)
+            self.out_activation = MODELS.build(out_act)
 
         self._init_weight()
 
     def forward(self, x):
         """Forward function.
 
         Args:
@@ -156,15 +156,15 @@
 
     def _init_weight(self):
         """Initialize weights for the model."""
         nn.init.normal_(self.linear.weight, 0., 1.)
         nn.init.constant_(self.linear.bias, 0.)
 
 
-@PLUGIN_LAYERS.register_module()
+@MODELS.register_module()
 class ConvLNModule(ConvModule):
     r"""ConvModule with Layer Normalization.
 
     In this module, we inherit default ``mmcv.cnn.ConvModule`` and deal with
     the situation that 'norm_cfg' is 'LN2d' or 'GN'. We adopt 'GN' as a
     replacement for layer normalization referring to:
     https://github.com/LynnHo/DCGAN-LSGAN-WGAN-GP-DRAGAN-Pytorch/blob/master/module.py # noqa
```

### Comparing `mmgen-0.7.3/mmgen/models/common/dist_utils.py` & `mmgen-1.0.0rc0/mmgen/models/common/dist_utils.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/diffusions/sampler.py` & `mmgen-1.0.0rc0/mmgen/models/diffusions/sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 
-from ..builder import MODULES
+from mmgen.registry import MODULES
 
 
 @MODULES.register_module()
 class UniformTimeStepSampler:
     """Timestep sampler for DDPM-based models. This sampler sample all
     timesteps with the same probabilistic.
```

### Comparing `mmgen-0.7.3/mmgen/models/gans/basic_conditional_gan.py` & `mmgen-1.0.0rc0/mmgen/models/gans/stylegan2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,368 +1,322 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
+from typing import Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
-from torch.nn.parallel.distributed import _find_tensors
-
-from ..builder import MODELS, build_module
-from ..common import set_requires_grad
+import torch.nn.functional as F
+from mmengine import Config, MessageHub
+from mmengine.model import BaseModel, is_model_wrapper
+from mmengine.optim import OptimWrapper, OptimWrapperDict
+from torch import Tensor
+
+from mmgen.registry import MODELS, MODULES
+from mmgen.structures import GenDataSample
+from ..common import gather_log_vars, set_requires_grad
+from ..losses import gen_path_regularizer, r1_gradient_penalty_loss
 from .base_gan import BaseGAN
 
+ModelType = Union[Dict, nn.Module]
 
-@MODELS.register_module('BasiccGAN')
-@MODELS.register_module()
-class BasicConditionalGAN(BaseGAN):
-    """Basic conditional GANs.
 
-    This is the conditional GAN model containing standard adversarial training
-    schedule. To fulfill the requirements of various GAN algorithms,
-    ``disc_auxiliary_loss`` and ``gen_auxiliary_loss`` are provided to
-    customize auxiliary losses, e.g., gradient penalty loss, and discriminator
-    shift loss. In addition, ``train_cfg`` and ``test_cfg`` aims at setuping
-    training schedule.
+@MODELS.register_module()
+class StyleGAN2(BaseGAN):
+    """Impelmentation of `Analyzing and Improving the Image Quality of
+    Stylegan`. # noqa.
+
+    Paper link: https://openaccess.thecvf.com/content_CVPR_2020/html/Karras_Analyzing_and_Improving_the_Image_Quality_of_StyleGAN_CVPR_2020_paper.html. # noqa
+
+    :class:~`mmgen.models.architectures.stylegan.generator_discriminator_v2.StyleGANv2Generator`  # noqa
+    and
+    :class:~`mmgen.models.architectures.stylegan.generator_discriminator_v2.StyleGAN2Discriminator`  # noqa
 
     Args:
-        generator (dict): Config for generator.
-        discriminator (dict): Config for discriminator.
-        gan_loss (dict): Config for generative adversarial loss.
-        disc_auxiliary_loss (dict): Config for auxiliary loss to
-            discriminator.
-        gen_auxiliary_loss (dict | None, optional): Config for auxiliary loss
-            to generator. Defaults to None.
-        train_cfg (dict | None, optional): Config for training schedule.
-            Defaults to None.
-        test_cfg (dict | None, optional): Config for testing schedule. Defaults
-            to None.
-        num_classes (int | None, optional): The number of conditional classes.
-            Defaults to None.
+        generator (ModelType): The config or model of the generator.
+        discriminator (Optional[ModelType]): The config or model of the
+            discriminator. Defaults to None.
+        data_preprocessor (Optional[Union[dict, Config]]): The pre-process
+            config or :class:`~mmgen.models.GANDataPreprocessor`.
+        generator_steps (int): The number of times the generator is completely
+            updated before the discriminator is updated. Defaults to 1.
+        discriminator_steps (int): The number of times the discriminator is
+            completely updated before the generator is updated. Defaults to 1.
+        ema_config (Optional[Dict]): The config for generator's exponential
+            moving average setting. Defaults to None.
     """
 
     def __init__(self,
-                 generator,
-                 discriminator,
-                 gan_loss,
-                 disc_auxiliary_loss=None,
-                 gen_auxiliary_loss=None,
-                 train_cfg=None,
-                 test_cfg=None,
-                 num_classes=None):
-        super().__init__()
-        self.num_classes = num_classes
-        self._gen_cfg = deepcopy(generator)
-        self.generator = build_module(
-            generator, default_args=dict(num_classes=num_classes))
-
-        # support no discriminator in testing
-        if discriminator is not None:
-            self.discriminator = build_module(
-                discriminator, default_args=dict(num_classes=num_classes))
+                 generator: ModelType,
+                 discriminator: Optional[ModelType] = None,
+                 data_preprocessor: Optional[Union[dict, Config]] = None,
+                 generator_steps: int = 1,
+                 discriminator_steps: int = 1,
+                 ema_config: Optional[Dict] = None,
+                 loss_config=dict()):
+        BaseModel.__init__(self, data_preprocessor=data_preprocessor)
+
+        # build generator
+        if isinstance(generator, dict):
+            self._gen_cfg = deepcopy(generator)
+            generator = MODULES.build(generator)
+        self.generator = generator
+
+        # get valid noise_size
+        self.noise_size = getattr(self.generator, 'style_channels', 512)
+
+        # build discriminator
+        if discriminator:
+            if isinstance(discriminator, dict):
+                self._disc_cfg = deepcopy(discriminator)
+                # build discriminator with default `num_classes`
+                disc_args = dict()
+                if hasattr(self, 'num_classes'):
+                    disc_args['num_classes'] = self.num_classes
+                discriminator = MODULES.build(
+                    discriminator, default_args=disc_args)
+        self.discriminator = discriminator
+
+        self._gen_steps = generator_steps
+        self._disc_steps = discriminator_steps
+
+        if ema_config is None:
+            self._ema_config = None
+            self._with_ema_gen = False
         else:
-            self.discriminator = None
+            self._ema_config = deepcopy(ema_config)
+            self._init_ema_model(self._ema_config)
+            self._with_ema_gen = True
+
+        # loss config
+        self.loss_config = deepcopy(loss_config)
+        # r1 settings
+        self.r1_loss_weight = self.loss_config.get('r1_loss_weight', 80.0)
+        self.r1_interval = self.loss_config.get('r1_interval', 16)
+        self.norm_mode = self.loss_config.get('norm_mode', 'pixel')
+        self.r1_use_apex_amp = self.loss_config.get('r1_use_apex_amp', False)
+        self.scale_r1_loss = self.loss_config.get('scale_r1_loss', False)
+        # gen path reg settings
+        self.g_reg_interval = self.loss_config.get('g_reg_interval', 4)
+        self.g_reg_weight = self.loss_config.get('g_reg_weight', 8.)
+        self.pl_batch_shrink = self.loss_config.get('pl_batch_shrink', 2)
+        self.g_reg_use_apex_amp = self.loss_config.get('g_reg_use_apex_amp',
+                                                       False)
+        self.register_buffer('mean_path_length', torch.tensor(0.))
+
+    def disc_loss(self, disc_pred_fake: Tensor, disc_pred_real: Tensor,
+                  real_imgs: Tensor) -> Tuple:
+        r"""Get disc loss. StyleGANv2 use the non-saturating loss and R1
+            gradient penalty to train the discriminator.
 
-        # support no gan_loss in testing
-        if gan_loss is not None:
-            self.gan_loss = build_module(gan_loss)
-        else:
-            self.gan_loss = None
-
-        if disc_auxiliary_loss:
-            self.disc_auxiliary_losses = build_module(disc_auxiliary_loss)
-            if not isinstance(self.disc_auxiliary_losses, nn.ModuleList):
-                self.disc_auxiliary_losses = nn.ModuleList(
-                    [self.disc_auxiliary_losses])
-        else:
-            self.disc_auxiliary_loss = None
+        Args:
+            disc_pred_fake (Tensor): Discriminator's prediction of the fake
+                images.
+            disc_pred_real (Tensor): Discriminator's prediction of the real
+                images.
+            real_imgs (Tensor): Input real images.
 
-        if gen_auxiliary_loss:
-            self.gen_auxiliary_losses = build_module(gen_auxiliary_loss)
-            if not isinstance(self.gen_auxiliary_losses, nn.ModuleList):
-                self.gen_auxiliary_losses = nn.ModuleList(
-                    [self.gen_auxiliary_losses])
-        else:
-            self.gen_auxiliary_losses = None
+        Returns:
+            tuple[Tensor, dict]: Loss value and a dict of log variables.
+        """
 
-        self.train_cfg = deepcopy(train_cfg) if train_cfg else None
-        self.test_cfg = deepcopy(test_cfg) if test_cfg else None
+        losses_dict = dict()
+        # no-saturating gan loss
+        losses_dict['loss_disc_fake'] = F.softplus(disc_pred_fake).mean()
+        losses_dict['loss_disc_real'] = F.softplus(-disc_pred_real).mean()
+        # R1 Gradient Penalty
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
+        if curr_iter % self.r1_interval == 0:
+            losses_dict[
+                'loss_r1_gp'] = self.r1_loss_weight * r1_gradient_penalty_loss(
+                    self.discriminator,
+                    real_imgs,
+                    norm_mode=self.norm_mode,
+                    use_apex_amp=self.r1_use_apex_amp)
+
+        loss, log_var = self.parse_losses(losses_dict)
+        return loss, log_var
+
+    def gen_loss(self, disc_pred_fake: Tensor, batch_size: int) -> Tuple:
+        """Get gen loss. StyleGANv2 use the non-saturating loss and generator
+        path regularization to train the generator.
 
-        self._parse_train_cfg()
-        if test_cfg is not None:
-            self._parse_test_cfg()
-
-    def _parse_train_cfg(self):
-        """Parsing train config and set some attributes for training."""
-        if self.train_cfg is None:
-            self.train_cfg = dict()
-        # control the work flow in train step
-        self.disc_steps = self.train_cfg.get('disc_steps', 1)
-        self.gen_steps = self.train_cfg.get('gen_steps', 1)
-
-        # add support for accumulating gradients within multiple steps. This
-        # feature aims to simulate large `batch_sizes` (but may have some
-        # detailed differences in BN). Note that `self.disc_steps` should be
-        # set according to the batch accumulation strategy.
-        # In addition, in the detailed implementation, there is a difference
-        # between the batch accumulation in the generator and discriminator.
-        self.batch_accumulation_steps = self.train_cfg.get(
-            'batch_accumulation_steps', 1)
-
-        # whether to use exponential moving average for training
-        self.use_ema = self.train_cfg.get('use_ema', False)
-        if self.use_ema:
-            # use deepcopy to guarantee the consistency
-            self.generator_ema = deepcopy(self.generator)
-
-    def _parse_test_cfg(self):
-        """Parsing test config and set some attributes for testing."""
-        if self.test_cfg is None:
-            self.test_cfg = dict()
-
-        # basic testing information
-        self.batch_size = self.test_cfg.get('batch_size', 1)
-
-        # whether to use exponential moving average for testing
-        self.use_ema = self.test_cfg.get('use_ema', False)
-        # TODO: finish ema part
-
-    def train_step(self,
-                   data_batch,
-                   optimizer,
-                   ddp_reducer=None,
-                   loss_scaler=None,
-                   use_apex_amp=False,
-                   running_status=None):
-        """Train step function.
-
-        This function implements the standard training iteration for
-        asynchronous adversarial training. Namely, in each iteration, we first
-        update discriminator and then compute loss for generator with the newly
-        updated discriminator.
+        Args:
+            disc_pred_fake (Tensor): Discriminator's prediction of the fake
+                images.
+            batch_size (int): Batch size for generating fake images.
 
-        As for distributed training, we use the ``reducer`` from ddp to
-        synchronize the necessary params in current computational graph.
+        Returns:
+            tuple[Tensor, dict]: Loss value and a dict of log variables.
+        """
+        losses_dict = dict()
+        # no-saturating gan loss
+        losses_dict['loss_gen'] = F.softplus(-disc_pred_fake).mean()
+
+        # Generator Path Regularizer
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
+        if curr_iter % self.g_reg_interval == 0:
+            path_penalty, self.mean_path_length, _ = gen_path_regularizer(
+                self.generator,
+                batch_size,
+                self.mean_path_length,
+                pl_batch_shrink=self.pl_batch_shrink,
+                use_apex_amp=self.g_reg_use_apex_amp)
+            losses_dict['loss_path_regular'] = self.g_reg_weight * path_penalty
+        loss, log_var = self.parse_losses(losses_dict)
+        return loss, log_var
+
+    def train_discriminator(
+            self, inputs: dict, data_samples: List[GenDataSample],
+            optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        """Train discriminator.
 
         Args:
-            data_batch (dict): Input data from dataloader.
-            optimizer (dict): Dict contains optimizer for generator and
-                discriminator.
-            ddp_reducer (:obj:`Reducer` | None, optional): Reducer from ddp.
-                It is used to prepare for ``backward()`` in ddp. Defaults to
-                None.
-            loss_scaler (:obj:`torch.cuda.amp.GradScaler` | None, optional):
-                The loss/gradient scaler used for auto mixed-precision
-                training. Defaults to ``None``.
-            use_apex_amp (bool, optional). Whether to use apex.amp. Defaults to
-                ``False``.
-            running_status (dict | None, optional): Contains necessary basic
-                information for training, e.g., iteration number. Defaults to
-                None.
-
+            inputs (dict): Inputs from dataloader.
+            data_samples (List[GenDataSample]): Data samples from dataloader.
+            optim_wrapper (OptimWrapper): OptimWrapper instance used to update
+                model parameters.
         Returns:
-            dict: Contains 'log_vars', 'num_samples', and 'results'.
+            Dict[str, Tensor]: A ``dict`` of tensor for logging.
         """
-        # get data from data_batch
-        real_imgs = data_batch['img']
-        # get the ground-truth label, torch.Tensor (N, )
-        gt_label = data_batch['gt_label']
-        # If you adopt ddp, this batch size is local batch size for each GPU.
-        # If you adopt dp, this batch size is the global batch size as usual.
-        batch_size = real_imgs.shape[0]
-
-        # get running status
-        if running_status is not None:
-            curr_iter = running_status['iteration']
-        else:
-            # dirty walkround for not providing running status
-            if not hasattr(self, 'iteration'):
-                self.iteration = 0
-            curr_iter = self.iteration
-
-        # disc training
-        set_requires_grad(self.discriminator, True)
-
-        # do not `zero_grad` during batch accumulation
-        if curr_iter % self.batch_accumulation_steps == 0:
-            optimizer['discriminator'].zero_grad()
-        # TODO: add noise sampler to customize noise sampling
+        real_imgs = inputs['img']
+
+        num_batches = real_imgs.shape[0]
+
+        noise_batch = self.noise_fn(num_batches=num_batches)
         with torch.no_grad():
-            fake_data = self.generator(
-                None, num_batches=batch_size, label=None, return_noise=True)
-            # fake_label should be in the same data type with the gt_label
-            fake_imgs, fake_label = fake_data['fake_img'], fake_data['label']
-
-        # disc pred for fake imgs and real_imgs
-        disc_pred_fake = self.discriminator(fake_imgs, label=fake_label)
-        disc_pred_real = self.discriminator(real_imgs, label=gt_label)
-        # get data dict to compute losses for disc
-        data_dict_ = dict(
-            gen=self.generator,
-            disc=self.discriminator,
-            disc_pred_fake=disc_pred_fake,
-            disc_pred_real=disc_pred_real,
-            fake_imgs=fake_imgs,
-            real_imgs=real_imgs,
-            iteration=curr_iter,
-            batch_size=batch_size,
-            gt_label=gt_label,
-            fake_label=fake_label,
-            loss_scaler=loss_scaler)
-
-        loss_disc, log_vars_disc = self._get_disc_loss(data_dict_)
-        loss_disc = loss_disc / float(self.batch_accumulation_steps)
-
-        # prepare for backward in ddp. If you do not call this function before
-        # back propagation, the ddp will not dynamically find the used params
-        # in current computation.
-        if ddp_reducer is not None:
-            ddp_reducer.prepare_for_backward(_find_tensors(loss_disc))
-
-        if loss_scaler:
-            # add support for fp16
-            loss_scaler.scale(loss_disc).backward()
-        elif use_apex_amp:
-            from apex import amp
-            with amp.scale_loss(
-                    loss_disc, optimizer['discriminator'],
-                    loss_id=0) as scaled_loss_disc:
-                scaled_loss_disc.backward()
-        else:
-            loss_disc.backward()
+            fake_imgs = self.generator(noise_batch, return_noise=False)
 
-        if (curr_iter + 1) % self.batch_accumulation_steps == 0:
-            if loss_scaler:
-                loss_scaler.unscale_(optimizer['discriminator'])
-                # note that we do not contain clip_grad procedure
-                loss_scaler.step(optimizer['discriminator'])
-                # loss_scaler.update will be called in runner.train()
-            else:
-                optimizer['discriminator'].step()
-
-        # skip generator training if only train discriminator for current
-        # iteration
-        if (curr_iter + 1) % self.disc_steps != 0:
-            results = dict(
-                fake_imgs=fake_imgs.cpu(), real_imgs=real_imgs.cpu())
-            outputs = dict(
-                log_vars=log_vars_disc,
-                num_samples=batch_size,
-                results=results)
-            if hasattr(self, 'iteration'):
-                self.iteration += 1
-            return outputs
-
-        # generator training
-        set_requires_grad(self.discriminator, False)
-        # allow for training the generator with multiple steps
-        for _ in range(self.gen_steps):
-            optimizer['generator'].zero_grad()
-            for _ in range(self.batch_accumulation_steps):
-                # TODO: add noise sampler to customize noise sampling
-                fake_data = self.generator(
-                    None, num_batches=batch_size, return_noise=True)
-                # fake_label should be in the same data type with the gt_label
-                fake_imgs, fake_label = fake_data['fake_img'], fake_data[
-                    'label']
-                disc_pred_fake_g = self.discriminator(
-                    fake_imgs, label=fake_label)
-
-                data_dict_ = dict(
-                    gen=self.generator,
-                    disc=self.discriminator,
-                    fake_imgs=fake_imgs,
-                    disc_pred_fake_g=disc_pred_fake_g,
-                    iteration=curr_iter,
-                    batch_size=batch_size,
-                    fake_label=fake_label,
-                    loss_scaler=loss_scaler)
-
-                loss_gen, log_vars_g = self._get_gen_loss(data_dict_)
-                loss_gen = loss_gen / float(self.batch_accumulation_steps)
-
-                # prepare for backward in ddp. If you do not call this function
-                # before back propagation, the ddp will not dynamically find
-                # the used params in current computation.
-                if ddp_reducer is not None:
-                    ddp_reducer.prepare_for_backward(_find_tensors(loss_gen))
-
-                if loss_scaler:
-                    loss_scaler.scale(loss_gen).backward()
-                elif use_apex_amp:
-                    from apex import amp
-                    with amp.scale_loss(
-                            loss_gen, optimizer['generator'],
-                            loss_id=1) as scaled_loss_disc:
-                        scaled_loss_disc.backward()
-                else:
-                    loss_gen.backward()
-
-            if loss_scaler:
-                loss_scaler.unscale_(optimizer['generator'])
-                # note that we do not contain clip_grad procedure
-                loss_scaler.step(optimizer['generator'])
-                # loss_scaler.update will be called in runner.train()
-            else:
-                optimizer['generator'].step()
-
-        log_vars = {}
-        log_vars.update(log_vars_g)
-        log_vars.update(log_vars_disc)
-
-        results = dict(fake_imgs=fake_imgs.cpu(), real_imgs=real_imgs.cpu())
-        outputs = dict(
-            log_vars=log_vars, num_samples=batch_size, results=results)
-
-        if hasattr(self, 'iteration'):
-            self.iteration += 1
-        return outputs
-
-    def sample_from_noise(self,
-                          noise,
-                          num_batches=0,
-                          sample_model='ema/orig',
-                          label=None,
-                          **kwargs):
-        """Sample images from noises by using the generator.
+        disc_pred_fake = self.discriminator(fake_imgs)
+        disc_pred_real = self.discriminator(real_imgs)
+
+        parsed_losses, log_vars = self.disc_loss(disc_pred_fake,
+                                                 disc_pred_real, real_imgs)
+        optimizer_wrapper.update_params(parsed_losses)
+        # save ada info
+        message_hub = MessageHub.get_current_instance()
+        message_hub.update_info('disc_pred_real', disc_pred_real)
+        return log_vars
+
+    def train_generator(self, inputs: dict, data_samples: List[GenDataSample],
+                        optimizer_wrapper: OptimWrapper) -> Dict[str, Tensor]:
+        """Train generator.
 
         Args:
-            noise (torch.Tensor | callable | None): You can directly give a
-                batch of noise through a ``torch.Tensor`` or offer a callable
-                function to sample a batch of noise data. Otherwise, the
-                ``None`` indicates to use the default noise sampler.
-            num_batches (int, optional): The number of batch size.
-                Defaults to 0.
-            sampel_model (str, optional): Use which model to sample fake
-                images. Defaults to `'ema/orig'`.
-            label (torch.Tensor | None , optional): The conditional label.
-                Defaults to None.
+            inputs (dict): Inputs from dataloader.
+            data_samples (List[GenDataSample]): Data samples from dataloader.
+                Do not used in generator's training.
+            optim_wrapper (OptimWrapper): OptimWrapper instance used to update
+                model parameters.
 
         Returns:
-            torch.Tensor | dict: The output may be the direct synthesized
-                images in ``torch.Tensor``. Otherwise, a dict with queried
-                data, including generated images, will be returned.
+            Dict[str, Tensor]: A ``dict`` of tensor for logging.
         """
-        if sample_model == 'ema':
-            assert self.use_ema
-            _model = self.generator_ema
-        elif sample_model == 'ema/orig' and self.use_ema:
-            _model = self.generator_ema
-        else:
-            _model = self.generator
+        # num_batches = inputs['real_imgs'].shape[0]
+        num_batches = inputs['img'].shape[0]
+
+        # >>> new setting
+        noise = self.noise_fn(num_batches=num_batches)
+        fake_imgs = self.generator(noise, return_noise=False)
+
+        disc_pred_fake = self.discriminator(fake_imgs)
+        parsed_loss, log_vars = self.gen_loss(disc_pred_fake, num_batches)
+
+        optimizer_wrapper.update_params(parsed_loss)
+        return log_vars
+
+    def train_step(self, data: dict,
+                   optim_wrapper: OptimWrapperDict) -> Dict[str, Tensor]:
+        """Train GAN model. In the training of GAN models, generator and
+        discriminator are updated alternatively. In MMGeneration's design,
+        `self.train_step` is called with data input. Therefore we always update
+        discriminator, whose updating is relay on real data, and then determine
+        if the generator needs to be updated based on the current number of
+        iterations. More details about whether to update generator can be found
+        in :meth:`should_gen_update`.
 
-        outputs = _model(noise, num_batches=num_batches, label=label, **kwargs)
+        Args:
+            data (dict): Data sampled from dataloader.
+            optim_wrapper (OptimWrapperDict): OptimWrapperDict instance
+                contains OptimWrapper of generator and discriminator.
 
-        if isinstance(outputs, dict) and 'noise_batch' in outputs:
-            noise = outputs['noise_batch']
-            label = outputs['label']
-
-        if sample_model == 'ema/orig' and self.use_ema:
-            _model = self.generator
-            outputs_ = _model(
-                noise, num_batches=num_batches, label=label, **kwargs)
-
-            if isinstance(outputs_, dict):
-                outputs['fake_img'] = torch.cat(
-                    [outputs['fake_img'], outputs_['fake_img']], dim=0)
-            else:
-                outputs = torch.cat([outputs, outputs_], dim=0)
+        Returns:
+            Dict[str, torch.Tensor]: A ``dict`` of tensor for logging.
+        """
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
+        data = self.data_preprocessor(data, True)
+        inputs_dict, data_samples = data['inputs'], data['data_samples']
+
+        disc_optimizer_wrapper: OptimWrapper = optim_wrapper['discriminator']
+        disc_accu_iters = disc_optimizer_wrapper._accumulative_counts
+
+        # NOTE: Do not use context manager of optim_wrapper. Because
+        # in mixed-precision training, StyleGAN2 only enable fp16 in
+        # specified blocks (refers to `:attr:enable_fp16` in
+        # :class:~`StyleGANv2Generator` and :class:~`StyleGAN2Discriminator`
+        # for more details), but in :func:~`AmpOptimWrapper.optim_context`,
+        # fp16 is applied to all modules. This may slow down gradient
+        # accumulation because `no_sycn` in
+        # :func:~`OptimWrapper.optim_context` will not be called any more.
+        log_vars = self.train_discriminator(inputs_dict, data_samples,
+                                            disc_optimizer_wrapper)
+
+        # add 1 to `curr_iter` because iter is updated in train loop.
+        # Whether to update the generator. We update generator with
+        # discriminator is fully updated for `self.n_discriminator_steps`
+        # iterations. And one full updating for discriminator contains
+        # `disc_accu_counts` times of grad accumulations.
+        if (curr_iter + 1) % (self.discriminator_steps * disc_accu_iters) == 0:
+            set_requires_grad(self.discriminator, False)
+            gen_optimizer_wrapper = optim_wrapper['generator']
+            gen_accu_iters = gen_optimizer_wrapper._accumulative_counts
+
+            log_vars_gen_list = []
+            # init optimizer wrapper status for generator manually
+            gen_optimizer_wrapper.initialize_count_status(
+                self.generator, 0, self.generator_steps * gen_accu_iters)
+            for _ in range(self.generator_steps * gen_accu_iters):
+                log_vars_gen = self.train_generator(inputs_dict, data_samples,
+                                                    gen_optimizer_wrapper)
+
+                log_vars_gen_list.append(log_vars_gen)
+            log_vars_gen = gather_log_vars(log_vars_gen_list)
+            log_vars_gen.pop('loss', None)  # remove 'loss' from gen logs
+
+            set_requires_grad(self.discriminator, True)
+
+            # only do ema after generator update
+            if self.with_ema_gen and (curr_iter + 1) >= (
+                    self.ema_start * self.discriminator_steps *
+                    disc_accu_iters):
+                self.generator_ema.update_parameters(
+                    self.generator.module
+                    if is_model_wrapper(self.generator) else self.generator)
+                # if not update buffer, copy buffer from orig model
+                if not self.generator_ema.update_buffers:
+                    self.generator_ema.sync_buffers(
+                        self.generator.module if is_model_wrapper(
+                            self.generator) else self.generator)
+            elif self.with_ema_gen:
+                # before ema, copy weights from orig
+                self.generator_ema.sync_parameters(
+                    self.generator.module
+                    if is_model_wrapper(self.generator) else self.generator)
+
+            log_vars.update(log_vars_gen)
+
+        batch_size = data['inputs']['img'].shape[0]
+        # update ada p
+        if hasattr(self.discriminator,
+                   'with_ada') and self.discriminator.with_ada:
+            self.discriminator.ada_aug.log_buffer[0] += batch_size
+            self.discriminator.ada_aug.log_buffer[1] += message_hub.get_info(
+                'disc_pred_real').sign().sum()
+
+            self.discriminator.ada_aug.update(
+                iteration=curr_iter, num_batches=batch_size)
+            log_vars['augment'] = (
+                self.discriminator.ada_aug.aug_pipeline.p.data.cpu())
 
-        return outputs
+        return log_vars
```

### Comparing `mmgen-0.7.3/mmgen/models/gans/singan.py` & `mmgen-1.0.0rc0/mmgen/engine/hooks/visualization_hook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,461 +1,407 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-import pickle
+import math
+import warnings
+from collections import defaultdict
 from copy import deepcopy
-from functools import partial
+from typing import Dict, List, Optional, Sequence, Tuple, Union
 
-import mmcv
-import numpy as np
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn.parallel import DataParallel, DistributedDataParallel
-from torch.nn.parallel.distributed import _find_tensors
-
-from mmgen.models.architectures.common import get_module_device
-from mmgen.models.builder import MODELS, build_module
-from mmgen.models.gans.base_gan import BaseGAN
-from ..common import set_requires_grad
-
-
-@MODELS.register_module()
-class SinGAN(BaseGAN):
-    """SinGAN.
-
-    This model implement the single image generative adversarial model proposed
-    in: Singan: Learning a Generative Model from a Single Natural Image,
-    ICCV'19.
-
-    Notes for training:
-
-    - This model should be trained with our dataset ``SinGANDataset``.
-    - In training, the ``total_iters`` arguments is related to the number of
-      scales in the image pyramid and ``iters_per_scale`` in the ``train_cfg``.
-      You should set it carefully in the training config file.
-
-    Notes for model architectures:
-
-    - The generator and discriminator need ``num_scales`` in initialization.
-      However, this arguments is generated by ``create_real_pyramid`` function
-      from the ``singan_dataset.py``. The last element in the returned list
-      (``stop_scale``) is the value for ``num_scales``. Pay attention that this
-      scale is counted from zero. Please see our tutorial for SinGAN to obtain
-      more details or our standard config for reference.
+from mmengine import MessageHub
+from mmengine.dist import master_only
+from mmengine.hooks import Hook
+from mmengine.runner import Runner
+from mmengine.structures import BaseDataElement
+from mmengine.utils import is_list_of
+from mmengine.visualization import Visualizer
+
+from mmgen.registry import HOOKS
+from mmgen.structures import GenDataSample, PixelData
+from mmgen.visualization.sampler import get_sampler
+
+
+@HOOKS.register_module()
+class GenVisualizationHook(Hook):
+    """Generation Visualization Hook. Used to visual output samples in
+    training, validation and testing. In this hook, we use a list called
+    `sample_kwargs_list` to control how to generate samples and how to
+    visualize them. Each element in `sample_kwargs_list`, called
+    `sample_kwargs`, may contains the following keywords:
+
+    - Required key words:
+        - 'type': Value must be string. Denotes what kind of sampler is used to
+            generate image. Refers to `:meth:~mmgen.core.sampler.get_sampler`.
+    - Optional key words (If not passed, will use the default value):
+        - 'n_rows': Value must be int. The number of images in one row.
+        - 'num_samples': Value must be int. The number of samples to visualize.
+        - 'vis_mode': Value must be string. How to visualize the generated
+            samples (e.g. image, gif).
+        - 'fixed_input': Value must be bool. Whether use the fixed input
+            during the loop.
+        - 'draw_gt': Value must be bool. Whether save the real images.
+        - 'target_keys': Value must be string or list of string. The keys of
+            the target image to visualize.
+        - 'name': Value must be string. If not passed, will use
+            `sample_kwargs['type']` as default.
+
+    For convenience, we also define a group of alias of samplers' type for
+    models supported in MMGeneration. Refers to
+    `:attr:self.SAMPLER_TYPE_MAPPING`.
+
+    Example:
+        >>> # for GAN models
+        >>> custom_hooks = [
+        >>>     dict(
+        >>>         type='GenVisualizationHook',
+        >>>         interval=1000,
+        >>>         fixed_input=True,
+        >>>         vis_kwargs_list=dict(type='GAN', name='fake_img'))]
+        >>> # for Translation models
+        >>> custom_hooks = [
+        >>>     dict(
+        >>>         type='GenVisualizationHook',
+        >>>         interval=10,
+        >>>         fixed_input=False,
+        >>>         vis_kwargs_list=[dict(type='Translation',
+        >>>                                  name='translation_train',
+        >>>                                  n_samples=6, draw_gt=True,
+        >>>                                  n_rows=3),
+        >>>                             dict(type='TranslationVal',
+        >>>                                  name='translation_val',
+        >>>                                  n_samples=16, draw_gt=True,
+        >>>                                  n_rows=4)])]
+
+    # NOTE: user-defined vis_kwargs > vis_kwargs_mapping > hook init args
 
     Args:
-        generator (dict): Config for generator.
-        discriminator (dict): Config for discriminator.
-        gan_loss (dict): Config for generative adversarial loss.
-        disc_auxiliary_loss (dict): Config for auxiliary loss to
-            discriminator.
-        gen_auxiliary_loss (dict | None, optional): Config for auxiliary loss
-            to generator. Defaults to None.
-        train_cfg (dict | None, optional): Config for training schedule.
-            Defaults to None.
-        test_cfg (dict | None, optional): Config for testing schedule. Defaults
-            to None.
+        interval (int): Visualization interval. Default: 1000.
+        sampler_kwargs_list (Tuple[List[dict], dict]): The list of sampling
+            behavior to generate images.
+        fixed_input (bool): The default action of whether use fixed input to
+            generate samples during the loop. Defaults to True.
+        n_samples (Optional[int]): The default value of number of samples to
+            visualize. Defaults to 64.
+        n_row (Optional[int]): The default value of number of images in each
+            row in the visualization results. Defaults to 8.
+        show (bool): Whether to display the drawn image. Default to False.
+        wait_time (float): The interval of show (s). Defaults to 0.
     """
 
-    def __init__(self,
-                 generator,
-                 discriminator,
-                 gan_loss,
-                 disc_auxiliary_loss,
-                 gen_auxiliary_loss=None,
-                 train_cfg=None,
-                 test_cfg=None):
-        super().__init__()
-        self._gen_cfg = deepcopy(generator)
-        self.generator = build_module(generator)
-
-        # support no discriminator in testing
-        if discriminator is not None:
-            self.discriminator = build_module(discriminator)
-        else:
-            self.discriminator = None
-
-        # support no gan_loss in testing
-        if gan_loss is not None:
-            self.gan_loss = build_module(gan_loss)
-        else:
-            self.gan_loss = None
+    priority = 'NORMAL'
 
-        if disc_auxiliary_loss:
-            self.disc_auxiliary_losses = build_module(disc_auxiliary_loss)
-            if not isinstance(self.disc_auxiliary_losses, nn.ModuleList):
-                self.disc_auxiliary_losses = nn.ModuleList(
-                    [self.disc_auxiliary_losses])
-        else:
-            self.disc_auxiliary_losses = None
+    VIS_KWARGS_MAPPING = dict(
+        GAN=dict(type='Noise'),
+        SinGAN=dict(type='Arguments', forward_kwargs=dict(mode='rand')),
+        Translation=dict(type='Data'),
+        TranslationVal=dict(type='ValData'),
+        TranslationTest=dict(type='TestData'),
+        DDPMDenoising=dict(
+            type='Arguments',
+            name='ddpm_sample',
+            n_samples=16,
+            n_row=4,
+            vis_mode='gif',
+            n_skip=100,
+            forward_kwargs=dict(
+                forward_mode='sampling',
+                sample_kwargs=dict(show_pbar=True, save_intermedia=True))))
 
-        if gen_auxiliary_loss:
-            self.gen_auxiliary_losses = build_module(gen_auxiliary_loss)
-            if not isinstance(self.gen_auxiliary_losses, nn.ModuleList):
-                self.gen_auxiliary_losses = nn.ModuleList(
-                    [self.gen_auxiliary_losses])
-        else:
-            self.gen_auxiliary_losses = None
+    def __init__(self,
+                 interval: int = 1000,
+                 vis_kwargs_list: Tuple[List[dict], dict] = None,
+                 fixed_input: bool = True,
+                 n_samples: Optional[int] = 64,
+                 n_row: Optional[int] = 8,
+                 message_hub_vis_kwargs: Optional[Tuple[str, dict, List[str],
+                                                        List[Dict]]] = None,
+                 save_at_test: bool = True,
+                 test_vis_keys: Optional[Union[str, List[str]]] = None,
+                 show: bool = False,
+                 wait_time: float = 0):
+
+        self._visualizer: Visualizer = Visualizer.get_current_instance()
+        self.interval = interval
+
+        self.vis_kwargs_list = deepcopy(vis_kwargs_list)
+        if isinstance(self.vis_kwargs_list, dict):
+            self.vis_kwargs_list = [self.vis_kwargs_list]
+
+        self.fixed_input = fixed_input
+        self.inputs_buffer = defaultdict(list)
+
+        self.n_samples = n_samples
+        self.n_row = n_row
+
+        self.show = show
+        if self.show:
+            # No need to think about vis backends.
+            self._visualizer._vis_backends = {}
+            warnings.warn('The show is True, it means that only '
+                          'the prediction results are visualized '
+                          'without storing data, so vis_backends '
+                          'needs to be excluded.')
+
+        self.wait_time = wait_time
+        self.save_at_test = save_at_test
+        self.test_vis_keys_list = test_vis_keys
+        self.message_vis_kwargs = message_hub_vis_kwargs
+
+    @master_only
+    def after_val_iter(self, runner: Runner, batch_idx: int, data_batch: dict,
+                       outputs) -> None:
+        """:class:`GenVisualizationHook` do not support visualize during
+        validation.
 
-        # register necessary training status
-        self.curr_stage = -1
-        self.noise_weights = [1]
-        self.fixed_noises = []
-        self.reals = []
-        self.train_cfg = deepcopy(train_cfg) if train_cfg else None
-        self.test_cfg = deepcopy(test_cfg) if test_cfg else None
-
-        self._parse_train_cfg()
-        if test_cfg is not None:
-            self._parse_test_cfg()
-
-    def _parse_train_cfg(self):
-        """Parsing train config and set some attributes for training."""
-        if self.train_cfg is None:
-            self.train_cfg = dict()
-
-        # whether to use exponential moving average for training
-        self.use_ema = self.train_cfg.get('use_ema', False)
-        if self.use_ema:
-            # use deepcopy to guarantee the consistency
-            self.generator_ema = deepcopy(self.generator)
-
-    def _parse_test_cfg(self):
-        if self.test_cfg.get('pkl_data', None) is not None:
-            with open(self.test_cfg.pkl_data, 'rb') as f:
-                data = pickle.load(f)
-                self.fixed_noises = self._from_numpy(data['fixed_noises'])
-                self.noise_weights = self._from_numpy(data['noise_weights'])
-                self.curr_stage = data['curr_stage']
-
-            mmcv.print_log(f'Load pkl data from {self.test_cfg.pkl_data}',
-                           'mmgen')
-
-    def _from_numpy(self, data):
-        if isinstance(data, list):
-            return [self._from_numpy(x) for x in data]
-
-        if isinstance(data, np.ndarray):
-            data = torch.from_numpy(data)
-            device = get_module_device(self.generator)
-            data = data.to(device)
-            return data
+        Args:
+            runner (Runner): The runner of the training process.
+            batch_idx (int): The index of the current batch in the test loop.
+            data_batch (Sequence[dict], optional): Data from dataloader.
+                Defaults to None.
+            outputs: outputs of the generation model
+        """
+        return
 
-        return data
+    @master_only
+    def after_test_iter(self, runner: Runner, batch_idx, data_batch: dict,
+                        outputs):
+        """Visualize samples after test iteraiton.
 
-    def get_module(self, model, module_name):
-        """Get an inner module from model.
+        Args:
+            runner (Runner): The runner of the training process.
+            batch_idx (int): The index of the current batch in the test loop.
+            data_batch (dict, optional): Data from dataloader.
+                Defaults to None.
+            outputs: outputs of the generation model Defaults to None.
+        """
+        if not self.save_at_test:
+            return
 
-        Since we will wrapper DDP for some model, we have to judge whether the
-        module can be indexed directly.
+        # get color order, mean and std
+        module = runner.model
+        if hasattr(module, 'module'):
+            module = module.module
+        data_preprocessor = module.data_preprocessor
+        if hasattr(data_preprocessor, 'output_color_order'):
+            output_color_order = data_preprocessor.output_color_order
+        else:
+            output_color_order = 'bgr'
+        mean = data_preprocessor.mean
+        std = data_preprocessor.std
+        for idx, sample in enumerate(outputs):
+            curr_idx = batch_idx * len(outputs) + idx
+            if self.test_vis_keys_list is None:
+                target_keys = [
+                    k for k, v in sample.items()
+                    if not k.startswith('_') and isinstance(v, PixelData)
+                ]
+                assert len(target_keys), (
+                    'Cannot found PixelData in outputs. Please specific '
+                    '\'vis_test_keys_list\'.')
+            elif isinstance(self.test_vis_keys_list, str):
+                target_keys = [self.test_vis_keys_list]
+            else:
+                assert is_list_of(self.test_vis_keys_list, str), (
+                    'test_vis_keys_list must be str or list of str or None.')
+                target_keys = self.test_vis_keys_list
+
+            for key in target_keys:
+                name = key.replace('.', '_')
+                self._visualizer.add_datasample(
+                    name=name,
+                    gen_samples=[sample],
+                    batch_idx=curr_idx,
+                    target_keys=key,
+                    n_row=1,
+                    color_order=output_color_order,
+                    target_mean=mean.cpu(),
+                    target_std=std.cpu())
+
+    @master_only
+    def after_train_iter(self,
+                         runner: Runner,
+                         batch_idx: int,
+                         data_batch: dict = None,
+                         outputs: Optional[dict] = None) -> None:
+        """Visualize samples after train iteration.
 
         Args:
-            model (nn.Module): This model may wrapped with DDP or not.
-            module_name (str): The name of specific module.
-
-        Return:
-            nn.Module: Returned sub module.
+            runner (Runner): The runner of the training process.
+            batch_idx (int): The index of the current batch in the train loop.
+            data_batch (dict): Data from dataloader.
+                Defaults to None.
+            outputs (dict, optional): Outputs from model. Defaults to None.
         """
-        if isinstance(model, (DataParallel, DistributedDataParallel)):
-            return getattr(model.module, module_name)
+        if self.every_n_inner_iters(batch_idx, self.interval):
+            self.vis_sample(runner, batch_idx, data_batch, outputs)
 
-        return getattr(model, module_name)
-
-    def sample_from_noise(self,
-                          noise,
-                          num_batches=0,
-                          curr_scale=None,
-                          sample_model='ema/orig',
-                          **kwargs):
-        """Sample images from noises by using the generator.
+    @torch.no_grad()
+    def vis_sample(self,
+                   runner: Runner,
+                   batch_idx: int,
+                   data_batch: dict,
+                   outputs: Optional[dict] = None) -> None:
+        """Visualize samples.
 
         Args:
-            noise (torch.Tensor | callable | None): You can directly give a
-                batch of noise through a ``torch.Tensor`` or offer a callable
-                function to sample a batch of noise data. Otherwise, the
-                ``None`` indicates to use the default noise sampler.
-            num_batches (int, optional):  The number of batch size.
-                Defaults to 0.
-
-        Returns:
-            torch.Tensor | dict: The output may be the direct synthesized \
-                images in ``torch.Tensor``. Otherwise, a dict with queried \
-                data, including generated images, will be returned.
+            runner (Runner): The runner conatians model to visualize.
+            batch_idx (int): The index of the current batch in loop.
+            data_batch (dict): Data from dataloader.
+                Defaults to None.
+            outputs (dict, optional): Outputs from model. Defaults to None.
         """
-        # use `self.curr_scale` if curr_scale is None
-        if curr_scale is None:
-            curr_scale = self.curr_stage
-
-        if sample_model == 'ema':
-            assert self.use_ema
-            _model = self.generator_ema
-        elif sample_model == 'ema/orig' and self.use_ema:
-            _model = self.generator_ema
-        else:
-            _model = self.generator
-
-        if not self.fixed_noises[0].is_cuda and torch.cuda.is_available():
-            self.fixed_noises = [
-                x.to(get_module_device(self)) for x in self.fixed_noises
-            ]
+        # this function will only called in training process
+        num_batches = runner.train_dataloader.batch_size
 
-        outputs = _model(
-            None,
-            fixed_noises=self.fixed_noises,
-            noise_weights=self.noise_weights,
-            rand_mode='rand',
-            num_batches=num_batches,
-            curr_scale=curr_scale,
-            **kwargs)
-
-        return outputs
-
-    def construct_fixed_noises(self):
-        """Construct the fixed noises list used in SinGAN."""
-        for i, real in enumerate(self.reals):
-            h, w = real.shape[-2:]
-            if i == 0:
-                noise = torch.randn(1, 1, h, w).to(real)
-                self.fixed_noises.append(noise)
+        module = runner.model
+        module.eval()
+        if hasattr(module, 'module'):
+            module = module.module
+
+        forward_func = module.val_step
+        # get color order, mean and std
+        data_preprocessor = module.data_preprocessor
+        if hasattr(data_preprocessor, 'output_color_order'):
+            output_color_order = data_preprocessor.output_color_order
+        else:
+            output_color_order = 'bgr'
+        mean = data_preprocessor.mean
+        std = data_preprocessor.std
+
+        for vis_kwargs in self.vis_kwargs_list:
+            # pop the sample-unrelated values
+            vis_kwargs_ = deepcopy(vis_kwargs)
+            sampler_type = vis_kwargs_['type']
+
+            # replace with alias
+            for alias in self.VIS_KWARGS_MAPPING.keys():
+                if alias.upper() == sampler_type.upper():
+                    sampler_alias = deepcopy(self.VIS_KWARGS_MAPPING[alias])
+                    vis_kwargs_['type'] = sampler_alias.pop('type')
+                    for default_k, default_v in sampler_alias.items():
+                        vis_kwargs_.setdefault(default_k, default_v)
+                    break
+            # sampler_type = vis_kwargs_.pop('type')
+
+            name = vis_kwargs_.pop('name', None)
+            if not name:
+                name = sampler_type.lower()
+
+            n_samples = vis_kwargs_.pop('n_samples', self.n_samples)
+            n_row = vis_kwargs_.pop('n_row', self.n_row)
+            n_row = min(n_row, n_samples)
+
+            num_iters = math.ceil(n_samples / num_batches)
+            vis_kwargs_['max_times'] = num_iters
+            vis_kwargs_['num_batches'] = num_batches
+            fixed_input = vis_kwargs_.pop('fixed_input', self.fixed_input)
+            target_keys = vis_kwargs_.pop('target_keys', None)
+            vis_mode = vis_kwargs_.pop('vis_mode', None)
+
+            output_list = []
+            if fixed_input and self.inputs_buffer[sampler_type]:
+                sampler = self.inputs_buffer[sampler_type]
             else:
-                noise = torch.zeros_like(real)
-                self.fixed_noises.append(noise)
+                sampler = get_sampler(vis_kwargs_, runner)
+            need_save = fixed_input and not self.inputs_buffer[sampler_type]
 
-    def train_step(self,
-                   data_batch,
-                   optimizer,
-                   ddp_reducer=None,
-                   running_status=None):
-        """Train step function.
-
-        This function implements the standard training iteration for
-        asynchronous adversarial training. Namely, in each iteration, we first
-        update discriminator and then compute loss for generator with the newly
-        updated discriminator.
+            for inputs in sampler:
+                output_list += [out for out in forward_func(inputs)]
 
-        As for distributed training, we use the ``reducer`` from ddp to
-        synchronize the necessary params in current computational graph.
+                # save inputs
+                if need_save:
+                    self.inputs_buffer[sampler_type].append(inputs)
+
+            self._visualizer.add_datasample(
+                name=name,
+                gen_samples=output_list[:n_samples],
+                target_keys=target_keys,
+                vis_mode=vis_mode,
+                n_row=n_row,
+                color_order=output_color_order,
+                target_mean=mean.cpu(),
+                target_std=std.cpu(),
+                show=self.show,
+                wait_time=self.wait_time,
+                step=batch_idx + 1,
+                **vis_kwargs_)
+
+        # save images in message_hub
+        self.vis_from_message_hub(batch_idx, output_color_order, mean, std)
+
+        module.train()
+
+    def vis_from_message_hub(self, batch_idx: int, color_order: str,
+                             target_mean: Sequence[Union[float, int]],
+                             target_std: Sequence[Union[float, int]]):
+        """Visualize samples from message hub.
 
         Args:
-            data_batch (dict): Input data from dataloader.
-            optimizer (dict): Dict contains optimizer for generator and
-                discriminator.
-            ddp_reducer (:obj:`Reducer` | None, optional): Reducer from ddp.
-                It is used to prepare for ``backward()`` in ddp. Defaults to
-                None.
-            running_status (dict | None, optional): Contains necessary basic
-                information for training, e.g., iteration number. Defaults to
-                None.
-
-        Returns:
-            dict: Contains 'log_vars', 'num_samples', and 'results'.
+            batch_idx (int): The index of the current batch in the test loop.
+            color_order (str): The color order of generated images.
+            target_mean (Sequence[Union[float, int]]): The original mean
+                of the image tensor before preprocessing. Image will be
+                re-shifted to ``target_mean`` before visualizing.
+            target_std (Sequence[Union[float, int]]): The original std of the
+                image tensor before preprocessing. Image will be re-scaled to
+                ``target_std`` before visualizing.
         """
+        if self.message_vis_kwargs is None:
+            return
 
-        # get running status
-        if running_status is not None:
-            curr_iter = running_status['iteration']
+        message_hub = MessageHub.get_current_instance()
+        if 'vis_results' not in message_hub.runtime_info:
+            raise RuntimeError('Cannot find \'vis_results\' in '
+                               '\'message_hub.runtime_info\'. Cannot perform '
+                               'visualization from messageHub.')
+
+        vis_results = message_hub.get_info('vis_results')
+        if isinstance(self.message_vis_kwargs, str):
+            target_keys, vis_modes = [self.message_vis_kwargs], [None]
+        elif isinstance(self.message_vis_kwargs, dict):
+            target_keys = [self.message_vis_kwargs['key']]
+            vis_modes = [self.message_vis_kwargs['vis_mode']]
+        elif is_list_of(self.message_vis_kwargs, str):
+            target_keys = self.message_vis_kwargs
+            vis_modes = [None for _ in range(len(target_keys))]
         else:
-            # dirty walkround for not providing running status
-            if not hasattr(self, 'iteration'):
-                self.iteration = 0
-            curr_iter = self.iteration
-
-        # init each scale
-        if curr_iter % self.train_cfg['iters_per_scale'] == 0:
-            self.curr_stage += 1
-            # load weights from prev scale
-            self.get_module(self.generator, 'check_and_load_prev_weight')(
-                self.curr_stage)
-            self.get_module(self.discriminator, 'check_and_load_prev_weight')(
-                self.curr_stage)
-            # build optimizer for each scale
-            g_module = self.get_module(self.generator, 'blocks')
-            param_list = g_module[self.curr_stage].parameters()
-
-            self.g_optim = torch.optim.Adam(
-                param_list, lr=self.train_cfg['lr_g'], betas=(0.5, 0.999))
-            d_module = self.get_module(self.discriminator, 'blocks')
-            self.d_optim = torch.optim.Adam(
-                d_module[self.curr_stage].parameters(),
-                lr=self.train_cfg['lr_d'],
-                betas=(0.5, 0.999))
-
-            self.optimizer = dict(
-                generator=self.g_optim, discriminator=self.d_optim)
-
-            self.g_scheduler = torch.optim.lr_scheduler.MultiStepLR(
-                optimizer=self.g_optim, **self.train_cfg['lr_scheduler_args'])
-            self.d_scheduler = torch.optim.lr_scheduler.MultiStepLR(
-                optimizer=self.d_optim, **self.train_cfg['lr_scheduler_args'])
-
-        optimizer = self.optimizer
-
-        # setup fixed noises and reals pyramid
-        if curr_iter == 0 or len(self.reals) == 0:
-            keys = [k for k in data_batch.keys() if 'real_scale' in k]
-            scales = len(keys)
-            self.reals = [data_batch[f'real_scale{s}'] for s in range(scales)]
-
-            # here we do not padding fixed noises
-            self.construct_fixed_noises()
-
-        # disc training
-        set_requires_grad(self.discriminator, True)
-        for _ in range(self.train_cfg['disc_steps']):
-            optimizer['discriminator'].zero_grad()
-            # TODO: add noise sampler to customize noise sampling
-            with torch.no_grad():
-                fake_imgs = self.generator(
-                    data_batch['input_sample'],
-                    self.fixed_noises,
-                    self.noise_weights,
-                    rand_mode='rand',
-                    curr_scale=self.curr_stage)
-
-            # disc pred for fake imgs and real_imgs
-            disc_pred_fake = self.discriminator(fake_imgs.detach(),
-                                                self.curr_stage)
-            disc_pred_real = self.discriminator(self.reals[self.curr_stage],
-                                                self.curr_stage)
-            # get data dict to compute losses for disc
-            data_dict_ = dict(
-                iteration=curr_iter,
-                gen=self.generator,
-                disc=self.discriminator,
-                disc_pred_fake=disc_pred_fake,
-                disc_pred_real=disc_pred_real,
-                fake_imgs=fake_imgs,
-                real_imgs=self.reals[self.curr_stage],
-                disc_partial=partial(
-                    self.discriminator, curr_scale=self.curr_stage))
-
-            loss_disc, log_vars_disc = self._get_disc_loss(data_dict_)
-
-            # prepare for backward in ddp. If you do not call this function
-            # before back propagation, the ddp will not dynamically find the
-            # used params in current computation.
-            if ddp_reducer is not None:
-                ddp_reducer.prepare_for_backward(_find_tensors(loss_disc))
-            loss_disc.backward()
-            optimizer['discriminator'].step()
-
-        log_vars_disc.update(dict(curr_stage=self.curr_stage))
-
-        # generator training
-        set_requires_grad(self.discriminator, False)
-        for _ in range(self.train_cfg['generator_steps']):
-            optimizer['generator'].zero_grad()
-
-            # TODO: add noise sampler to customize noise sampling
-            fake_imgs = self.generator(
-                data_batch['input_sample'],
-                self.fixed_noises,
-                self.noise_weights,
-                rand_mode='rand',
-                curr_scale=self.curr_stage)
-            disc_pred_fake_g = self.discriminator(
-                fake_imgs, curr_scale=self.curr_stage)
-
-            recon_imgs = self.generator(
-                data_batch['input_sample'],
-                self.fixed_noises,
-                self.noise_weights,
-                rand_mode='recon',
-                curr_scale=self.curr_stage)
-
-            data_dict_ = dict(
-                iteration=curr_iter,
-                gen=self.generator,
-                disc=self.discriminator,
-                fake_imgs=fake_imgs,
-                recon_imgs=recon_imgs,
-                real_imgs=self.reals[self.curr_stage],
-                disc_pred_fake_g=disc_pred_fake_g)
-
-            loss_gen, log_vars_g = self._get_gen_loss(data_dict_)
-
-            # prepare for backward in ddp. If you do not call this function
-            # before back propagation, the ddp will not dynamically find the
-            # used params in current computation.
-            if ddp_reducer is not None:
-                ddp_reducer.prepare_for_backward(_find_tensors(loss_gen))
-
-            loss_gen.backward()
-            optimizer['generator'].step()
-
-        # end of each scale
-        # calculate noise weight for next scale
-        if (curr_iter % self.train_cfg['iters_per_scale']
-                == 0) and (self.curr_stage < len(self.reals) - 1):
-
-            with torch.no_grad():
-                g_recon = self.generator(
-                    data_batch['input_sample'],
-                    self.fixed_noises,
-                    self.noise_weights,
-                    rand_mode='recon',
-                    curr_scale=self.curr_stage)
-                if isinstance(g_recon, dict):
-                    g_recon = g_recon['fake_img']
-                g_recon = F.interpolate(
-                    g_recon, self.reals[self.curr_stage + 1].shape[-2:])
-
-            mse = F.mse_loss(g_recon.detach(), self.reals[self.curr_stage + 1])
-            rmse = torch.sqrt(mse)
-            self.noise_weights.append(
-                self.train_cfg.get('noise_weight_init', 0.1) * rmse.item())
-
-            # try to release GPU memory.
-            torch.cuda.empty_cache()
-
-        log_vars = {}
-        log_vars.update(log_vars_g)
-        log_vars.update(log_vars_disc)
-
-        results = dict(
-            fake_imgs=fake_imgs.cpu(),
-            real_imgs=self.reals[self.curr_stage].cpu(),
-            recon_imgs=recon_imgs.cpu(),
-            curr_stage=self.curr_stage,
-            fixed_noises=self.fixed_noises,
-            noise_weights=self.noise_weights)
-        outputs = dict(log_vars=log_vars, num_samples=1, results=results)
-
-        # update lr scheduler
-        self.d_scheduler.step()
-        self.g_scheduler.step()
-
-        if hasattr(self, 'iteration'):
-            self.iteration += 1
-
-        return outputs
-
-
-@MODELS.register_module()
-class PESinGAN(SinGAN):
-    """Positional Encoding in SinGAN.
-
-    This modified SinGAN is used to reimplement the experiments in: Positional
-    Encoding as Spatial Inductive Bias in GANs, CVPR2021.
-    """
+            # list of dict
+            target_keys = [kwargs['key'] for kwargs in self.message_vis_kwargs]
+            vis_modes = [
+                kwargs.pop('vis_mode', None)
+                for kwargs in deepcopy(self.message_vis_kwargs)
+            ]
 
-    def _parse_train_cfg(self):
-        super(PESinGAN, self)._parse_train_cfg()
-        self.fixed_noise_with_pad = self.train_cfg.get('fixed_noise_with_pad',
-                                                       False)
-        self.first_fixed_noises_ch = self.train_cfg.get(
-            'first_fixed_noises_ch', 1)
-
-    def construct_fixed_noises(self):
-        """Construct the fixed noises list used in SinGAN."""
-        for i, real in enumerate(self.reals):
-            h, w = real.shape[-2:]
-            if self.fixed_noise_with_pad:
-                pad_ = self.get_module(self, 'generator').pad_head
-                h += 2 * pad_
-                w += 2 * pad_
-            if i == 0:
-                noise = torch.randn(1, self.first_fixed_noises_ch, h,
-                                    w).to(real)
-                self.fixed_noises.append(noise)
+        for key, vis_mode in zip(target_keys, vis_modes):
+            if key not in vis_results:
+                raise RuntimeError(
+                    f'Cannot find \'{key}\' in '
+                    'message_hub.runtime_info[\'vis_results\'].')
+
+            value = vis_results[key]
+            # pack to list of GenDataSample
+            if isinstance(value, torch.Tensor):
+                gen_samples = []
+                num_batches = value.shape[0]
+                for idx in range(num_batches):
+                    gen_sample = GenDataSample()
+                    setattr(gen_sample, key, PixelData(data=value[idx]))
+                    gen_samples.append(gen_sample)
+            elif is_list_of(value, BaseDataElement):
+                # already packed
+                gen_samples = value
+                num_batches = len(gen_samples)
             else:
-                noise = torch.zeros((1, 1, h, w)).to(real)
-                self.fixed_noises.append(noise)
+                raise TypeError(
+                    'Only support to visualize Tensor or list of DataSample '
+                    f'in MessageHub. But \'{key}\' is \'{type(value)}\'.')
+
+            self._visualizer.add_datasample(
+                name=f'train_{key}',
+                gen_samples=gen_samples,
+                target_keys=key,
+                vis_mode=vis_mode,
+                n_row=min(self.n_row, num_batches),
+                color_order=color_order,
+                target_mean=target_mean.cpu(),
+                target_std=target_std.cpu(),
+                show=self.show,
+                step=batch_idx)
```

### Comparing `mmgen-0.7.3/mmgen/models/losses/__init__.py` & `mmgen-1.0.0rc0/mmgen/models/losses/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from .ddpm_loss import DDPMVLBLoss
 from .disc_auxiliary_loss import (DiscShiftLoss, GradientPenaltyLoss,
                                   R1GradientPenalty, disc_shift_loss,
                                   gradient_penalty_loss,
                                   r1_gradient_penalty_loss)
 from .gan_loss import GANLoss
 from .gen_auxiliary_loss import (CLIPLoss, FaceIdLoss,
-                                 GeneratorPathRegularizer, PerceptualLoss,
+                                 GeneratorPathRegularizer,
                                  gen_path_regularizer)
 from .pixelwise_loss import (DiscretizedGaussianLogLikelihoodLoss,
                              GaussianKLDLoss, L1Loss, MSELoss,
                              discretized_gaussian_log_likelihood, gaussian_kld)
 
 __all__ = [
     'GANLoss', 'DiscShiftLoss', 'disc_shift_loss', 'gradient_penalty_loss',
     'GradientPenaltyLoss', 'R1GradientPenalty', 'r1_gradient_penalty_loss',
     'GeneratorPathRegularizer', 'gen_path_regularizer', 'MSELoss', 'L1Loss',
     'gaussian_kld', 'GaussianKLDLoss', 'DiscretizedGaussianLogLikelihoodLoss',
     'DDPMVLBLoss', 'discretized_gaussian_log_likelihood', 'FaceIdLoss',
-    'CLIPLoss', 'PerceptualLoss'
+    'CLIPLoss'
 ]
```

### Comparing `mmgen-0.7.3/mmgen/models/losses/ddpm_loss.py` & `mmgen-1.0.0rc0/mmgen/models/losses/ddpm_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from abc import abstractmethod
 from copy import deepcopy
 from functools import partial
 
-import mmcv
+import mmengine
 import torch
 import torch.distributed as dist
 import torch.nn as nn
-from mmcv.utils import digit_version
+from mmengine.utils.dl_utils import TORCH_VERSION
+from mmengine.utils.version_utils import digit_version
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODULES
 from .pixelwise_loss import (DiscretizedGaussianLogLikelihoodLoss,
                              GaussianKLDLoss, _reduction_modes, mse_loss)
 from .utils import reduce_loss
 
 
 class DDPMLoss(nn.Module):
     """Base module for DDPM losses. We support loss weight rescale and log
@@ -152,15 +153,15 @@
 
         self.log_fn_list = []
 
         log_cfgs_ = deepcopy(log_cfgs)
         if log_cfgs_ is not None:
             if not isinstance(log_cfgs_, list):
                 log_cfgs_ = [log_cfgs_]
-            assert mmcv.is_list_of(log_cfgs_, dict)
+            assert mmengine.is_list_of(log_cfgs_, dict)
             for log_cfg_ in log_cfgs_:
                 log_type = log_cfg_.pop('type')
                 log_collect_fn = f'{log_type}_log_collect'
                 assert hasattr(self, log_collect_fn)
                 log_collect_fn = getattr(self, log_collect_fn)
 
                 log_cfg_.setdefault('prefix_name', 'loss')
@@ -182,18 +183,18 @@
                 else:
                     assert weight is not None and isinstance(
                         weight, torch.Tensor), (
                             '\'weight\' or a \'sampler\' contains weight '
                             'attribute is must be \'torch.Tensor\' for '
                             '\'timestep_weight\' rescale_mode.')
 
-                mmcv.print_log(
+                mmengine.print_log(
                     'Apply \'timestep_weight\' rescale_mode for '
                     f'{self._loss_name}. Please make sure the passed weight '
-                    'can be updated by external functions.', 'mmgen')
+                    'can be updated by external functions.')
 
                 rescale_cfg = dict(weight=weight)
             self.rescale_fn = partial(
                 getattr(self, rescale_fn_name), **rescale_cfg)
 
     @staticmethod
     def constant_rescale(loss, timesteps, scale):
@@ -271,15 +272,15 @@
             prefix_name (str): Prefix want to show in logs.
             reduction (str, optional): Specifies the reduction to apply to the
                 output losses. Defaults to `mean`.
 
         Returns:
             dict: Collected log variables.
         """
-        if digit_version(torch.__version__) <= digit_version('1.6.0'):
+        if digit_version(TORCH_VERSION) <= digit_version('1.6.0'):
             # use true_divide in older torch version
             quartile = torch.true_divide(timesteps, total_timesteps) * 4
         else:
             quartile = (timesteps / total_timesteps * 4)
         quartile = quartile.type(torch.LongTensor)
 
         log_vars = dict()
```

### Comparing `mmgen-0.7.3/mmgen/models/losses/disc_auxiliary_loss.py` & `mmgen-1.0.0rc0/mmgen/models/losses/disc_auxiliary_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch
 import torch.autograd as autograd
 import torch.nn as nn
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODULES
 from .utils import weighted_loss
 
 
 @weighted_loss
 def disc_shift_loss(pred):
     """Disc Shift loss.
```

### Comparing `mmgen-0.7.3/mmgen/models/losses/gan_loss.py` & `mmgen-1.0.0rc0/mmgen/models/losses/gan_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import torch.nn as nn
 import torch.nn.functional as F
 
-from ..builder import MODULES
+from mmgen.registry import MODULES
 
 
 @MODULES.register_module()
 class GANLoss(nn.Module):
     """Define GAN loss.
 
     Args:
```

### Comparing `mmgen-0.7.3/mmgen/models/losses/pixelwise_loss.py` & `mmgen-1.0.0rc0/mmgen/models/losses/pixelwise_loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from mmgen.models.builder import MODULES
+from mmgen.registry import MODULES
 from .utils import weighted_loss
 
 _reduction_modes = ['none', 'mean', 'sum', 'batchmean', 'flatmean']
 
 
 @weighted_loss
 def l1_loss(pred, target):
```

### Comparing `mmgen-0.7.3/mmgen/models/losses/utils.py` & `mmgen-1.0.0rc0/mmgen/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/models/translation_models/base_translation_model.py` & `mmgen-1.0.0rc0/mmgen/models/translation_models/base_translation_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from abc import ABCMeta, abstractmethod
-from copy import deepcopy
 
-import torch.nn as nn
+from mmengine.model import BaseModel
 
-from ..builder import MODELS
+from mmgen.registry import MODELS
 
 
 @MODELS.register_module()
-class BaseTranslationModel(nn.Module, metaclass=ABCMeta):
+class BaseTranslationModel(BaseModel, metaclass=ABCMeta):
     """Base Translation Model.
 
     Translation models can transfer images from one domain to
     another. Domain information like `default_domain`,
     `reachable_domains` are needed to initialize the class.
     And we also provide query functions like `is_domain_reachable`,
     `get_other_domains`.
@@ -31,44 +30,36 @@
         reachable_domains (list[str]): Domains that can be generated by
             the model.
         related_domains (list[str]): Domains involved in training and
             testing. `reachable_domains` must be contained in
             `related_domains`. However, related_domains may contain
             source domains that are used to retrieve source images from
             data_batch but not in reachable_domains.
-        train_cfg (dict): Config for training. Default: None.
-        test_cfg (dict): Config for testing. Default: None.
+        discriminator_steps (int): The number of times the discriminator is
+            completely updated before the generator is updated. Defaults to 1.
+        disc_init_steps (int): The number of initial steps used only to train
+            discriminators.
     """
 
     def __init__(self,
                  default_domain,
                  reachable_domains,
                  related_domains,
-                 train_cfg=None,
-                 test_cfg=None):
+                 discriminator_steps=1,
+                 disc_init_steps=0,
+                 real_img_key='real_img'):
         self._default_domain = default_domain
         self._reachable_domains = reachable_domains
         self._related_domains = related_domains
         assert self._default_domain in self._reachable_domains
         assert set(self._reachable_domains) <= set(self._related_domains)
 
-        self.train_cfg = deepcopy(train_cfg) if train_cfg else None
-        self.test_cfg = deepcopy(test_cfg) if test_cfg else None
-
-        self._parse_train_cfg()
-        if test_cfg is not None:
-            self._parse_test_cfg()
-
-    @abstractmethod
-    def _parse_train_cfg(self):
-        """Parsing train config and set some attributes for training."""
-
-    @abstractmethod
-    def _parse_test_cfg(self):
-        """Parsing test config and set some attributes for testing."""
+        self.discriminator_steps = discriminator_steps
+        self.disc_init_steps = disc_init_steps
+        self.real_img_key = real_img_key
 
     def forward(self, img, test_mode=False, **kwargs):
         """Forward function.
 
         Args:
             img (tensor): Input image tensor.
             test_mode (bool): Whether in test mode or not. Default: False.
```

### Comparing `mmgen-0.7.3/mmgen/models/translation_models/cyclegan.py` & `mmgen-1.0.0rc0/mmgen/models/translation_models/pix2pix.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,211 +1,210 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from torch.nn.parallel.distributed import _find_tensors
-
-from mmgen.models.builder import MODELS
-from ..common import GANImageBuffer, set_requires_grad
+import torch
+import torch.nn.functional as F
+from mmengine import MessageHub
+
+from mmgen.registry import MODELS
+from mmgen.structures import GenDataSample, PixelData
+from mmgen.utils.typing import ForwardOutputs, ValTestStepInputs
+from ..common import set_requires_grad
 from .static_translation_gan import StaticTranslationGAN
 
 
 @MODELS.register_module()
-class CycleGAN(StaticTranslationGAN):
-    """CycleGAN model for unpaired image-to-image translation.
+class Pix2Pix(StaticTranslationGAN):
+    """Pix2Pix model for paired image-to-image translation.
 
     Ref:
-    Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial
-    Networks
+     Image-to-Image Translation with Conditional Adversarial Networks
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        # GAN image buffers
-        self.image_buffers = dict()
-        self.buffer_size = (50 if self.train_cfg is None else
-                            self.train_cfg.get('buffer_size', 50))
-        for domain in self._reachable_domains:
-            self.image_buffers[domain] = GANImageBuffer(self.buffer_size)
-
-        self.use_ema = False
 
     def forward_test(self, img, target_domain, **kwargs):
         """Forward function for testing.
 
         Args:
             img (tensor): Input image tensor.
             target_domain (str): Target domain of output image.
             kwargs (dict): Other arguments.
 
         Returns:
             dict: Forward results.
         """
-        # This is a trick for CycleGAN
-        # ref: https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix/blob/e1bdf46198662b0f4d0b318e24568205ec4d7aee/test.py#L54 # noqa
+        # This is a trick for Pix2Pix
+        # ref: https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix/blob/e1bdf46198662b0f4d0b318e24568205ec4d7aee/test.py#L54  # noqa
         self.train()
         target = self.translation(img, target_domain=target_domain, **kwargs)
         results = dict(source=img.cpu(), target=target.cpu())
         return results
 
     def _get_disc_loss(self, outputs):
-        """Backward function for the discriminators.
-
-        Args:
-            outputs (dict): Dict of forward results.
+        # GAN loss for the discriminator
+        losses = dict()
 
-        Returns:
-            dict: Discriminators' loss and loss dict.
-        """
         discriminators = self.get_module(self.discriminators)
+        target_domain = self._default_domain
+        source_domain = self.get_other_domains(target_domain)[0]
+        fake_ab = torch.cat((outputs[f'real_{source_domain}'],
+                             outputs[f'fake_{target_domain}']), 1)
+        fake_pred = discriminators[target_domain](fake_ab.detach())
+        losses['loss_gan_d_fake'] = F.binary_cross_entropy_with_logits(
+            fake_pred, 0. * torch.ones_like(fake_pred))
+        real_ab = torch.cat((outputs[f'real_{source_domain}'],
+                             outputs[f'real_{target_domain}']), 1)
+        real_pred = discriminators[target_domain](real_ab)
+        losses['loss_gan_d_real'] = F.binary_cross_entropy_with_logits(
+            real_pred, 1. * torch.ones_like(real_pred))
 
-        log_vars_d = dict()
-        loss_d = 0
-
-        # GAN loss for discriminators['a']
-        for domain in self._reachable_domains:
-            losses = dict()
-            fake_img = self.image_buffers[domain].query(
-                outputs[f'fake_{domain}'])
-            fake_pred = discriminators[domain](fake_img.detach())
-            losses[f'loss_gan_d_{domain}_fake'] = self.gan_loss(
-                fake_pred, target_is_real=False, is_disc=True)
-            real_pred = discriminators[domain](outputs[f'real_{domain}'])
-            losses[f'loss_gan_d_{domain}_real'] = self.gan_loss(
-                real_pred, target_is_real=True, is_disc=True)
-
-            _loss_d, _log_vars_d = self._parse_losses(losses)
-            _loss_d *= 0.5
-            loss_d += _loss_d
-            log_vars_d[f'loss_gan_d_{domain}'] = _log_vars_d['loss'] * 0.5
+        loss_d, log_vars_d = self.parse_losses(losses)
+        loss_d *= 0.5
 
         return loss_d, log_vars_d
 
     def _get_gen_loss(self, outputs):
-        """Backward function for the generators.
-
-        Args:
-            outputs (dict): Dict of forward results.
-
-        Returns:
-            dict: Generators' loss and loss dict.
-        """
-        generators = self.get_module(self.generators)
-        discriminators = self.get_module(self.discriminators)
-
+        target_domain = self._default_domain
+        source_domain = self.get_other_domains(target_domain)[0]
         losses = dict()
-        for domain in self._reachable_domains:
-            # Identity reconstruction for generators
-            outputs[f'identity_{domain}'] = generators[domain](
-                outputs[f'real_{domain}'])
-            # GAN loss for generators
-            fake_pred = discriminators[domain](outputs[f'fake_{domain}'])
-            losses[f'loss_gan_g_{domain}'] = self.gan_loss(
-                fake_pred, target_is_real=True, is_disc=False)
-
-        # gen auxiliary loss
-        if self.with_gen_auxiliary_loss:
-            for loss_module in self.gen_auxiliary_losses:
-                loss_ = loss_module(outputs)
-                if loss_ is None:
-                    continue
-                # the `loss_name()` function return name as 'loss_xxx'
-                if loss_module.loss_name() in losses:
-                    losses[loss_module.loss_name(
-                    )] = losses[loss_module.loss_name()] + loss_
-                else:
-                    losses[loss_module.loss_name()] = loss_
 
-        loss_g, log_vars_g = self._parse_losses(losses)
+        discriminators = self.get_module(self.discriminators)
+        # GAN loss for the generator
+        fake_ab = torch.cat((outputs[f'real_{source_domain}'],
+                             outputs[f'fake_{target_domain}']), 1)
+        fake_pred = discriminators[target_domain](fake_ab)
+        losses['loss_gan_g'] = F.binary_cross_entropy_with_logits(
+            fake_pred, 1. * torch.ones_like(fake_pred))
 
+        loss_g, log_vars_g = self.parse_losses(losses)
         return loss_g, log_vars_g
 
-    def _get_opposite_domain(self, domain):
-        for item in self._reachable_domains:
-            if item != domain:
-                return item
-        return None
-
-    def train_step(self,
-                   data_batch,
-                   optimizer,
-                   ddp_reducer=None,
-                   running_status=None):
+    def train_step(self, data, optim_wrapper=None):
         """Training step function.
 
         Args:
             data_batch (dict): Dict of the input data batch.
             optimizer (dict[torch.optim.Optimizer]): Dict of optimizers for
-                the generators and discriminators.
+                the generator and discriminator.
             ddp_reducer (:obj:`Reducer` | None, optional): Reducer from ddp.
                 It is used to prepare for ``backward()`` in ddp. Defaults to
                 None.
             running_status (dict | None, optional): Contains necessary basic
                 information for training, e.g., iteration number. Defaults to
                 None.
 
         Returns:
             dict: Dict of loss, information for logger, the number of samples\
                 and results for visualization.
         """
-        # get running status
-        if running_status is not None:
-            curr_iter = running_status['iteration']
-        else:
-            # dirty walkround for not providing running status
-            if not hasattr(self, 'iteration'):
-                self.iteration = 0
-            curr_iter = self.iteration
+        message_hub = MessageHub.get_current_instance()
+        curr_iter = message_hub.get_info('iter')
+        data = self.data_preprocessor(data, True)
+        inputs_dict = data['inputs']
+
+        disc_optimizer_wrapper = optim_wrapper['discriminators']
+        disc_accu_iters = disc_optimizer_wrapper._accumulative_counts
+
+        target_domain = self._default_domain
+        source_domain = self.get_other_domains(self._default_domain)[0]
+        source_image = inputs_dict[f'img_{source_domain}']
+        target_image = inputs_dict[f'img_{target_domain}']
 
-        # forward generators
+        # forward generator
         outputs = dict()
-        for target_domain in self._reachable_domains:
-            # fetch data by domain
-            source_domain = self.get_other_domains(target_domain)[0]
-            img = data_batch[f'img_{source_domain}']
-            # translation process
-            results = self(img, test_mode=False, target_domain=target_domain)
+        with disc_optimizer_wrapper.optim_context(self.discriminators):
+            results = self(
+                source_image,
+                target_domain=self._default_domain,
+                test_mode=False)
             outputs[f'real_{source_domain}'] = results['source']
             outputs[f'fake_{target_domain}'] = results['target']
-            # cycle process
-            results = self(
-                results['target'],
-                test_mode=False,
-                target_domain=source_domain)
-            outputs[f'cycle_{source_domain}'] = results['target']
-
-        log_vars = dict()
-
-        # discriminators
-        set_requires_grad(self.discriminators, True)
-        # optimize
-        optimizer['discriminators'].zero_grad()
-        loss_d, log_vars_d = self._get_disc_loss(outputs)
-        log_vars.update(log_vars_d)
-        if ddp_reducer is not None:
-            ddp_reducer.prepare_for_backward(_find_tensors(loss_d))
-        loss_d.backward()
-        optimizer['discriminators'].step()
+            outputs[f'real_{target_domain}'] = target_image
+            log_vars = dict()
 
-        # generators, no updates to discriminator parameters.
-        if (curr_iter % self.disc_steps == 0
+            # discriminator
+            set_requires_grad(self.discriminators, True)
+            # optimize
+            disc_optimizer_wrapper.zero_grad()
+            loss_d, log_vars_d = self._get_disc_loss(outputs)
+            log_vars.update(log_vars_d)
+            disc_optimizer_wrapper.backward(loss_d)
+            disc_optimizer_wrapper.step()
+
+        # generator, no updates to discriminator parameters.
+        gen_optimizer_wrapper = optim_wrapper['generators']
+        if ((curr_iter + 1) % (self.discriminator_steps * disc_accu_iters) == 0
                 and curr_iter >= self.disc_init_steps):
             set_requires_grad(self.discriminators, False)
             # optimize
-            optimizer['generators'].zero_grad()
-            loss_g, log_vars_g = self._get_gen_loss(outputs)
-            log_vars.update(log_vars_g)
-            if ddp_reducer is not None:
-                ddp_reducer.prepare_for_backward(_find_tensors(loss_g))
-            loss_g.backward()
-            optimizer['generators'].step()
-
-        if hasattr(self, 'iteration'):
-            self.iteration += 1
-
-        image_results = dict()
-        for domain in self._reachable_domains:
-            image_results[f'real_{domain}'] = outputs[f'real_{domain}'].cpu()
-            image_results[f'fake_{domain}'] = outputs[f'fake_{domain}'].cpu()
-        results = dict(
-            log_vars=log_vars,
-            num_samples=len(outputs[f'real_{domain}']),
-            results=image_results)
+            with gen_optimizer_wrapper.optim_context(self.generators):
+                gen_optimizer_wrapper.zero_grad()
+                loss_g, log_vars_g = self._get_gen_loss(outputs)
+                log_vars.update(log_vars_g)
+                gen_optimizer_wrapper.backward(loss_g)
+                gen_optimizer_wrapper.step()
 
-        return results
+        return log_vars
+
+    def test_step(self, data: ValTestStepInputs) -> ForwardOutputs:
+        """Gets the generated image of given data. Same as :meth:`val_step`.
+
+        Args:
+            data (ValTestStepInputs): Data sampled from metric specific
+                sampler. More detials in `Metrics` and `Evaluator`.
+
+        Returns:
+            ForwardOutputs: Generated image or image dict.
+        """
+        data = self.data_preprocessor(data)
+        inputs_dict, data_samples = data['inputs'], data['data_samples']
+        target_domain = self._reachable_domains[0]
+        source_domain = self.get_other_domains(target_domain)[0]
+        outputs = self.forward_test(
+            inputs_dict[f'img_{source_domain}'], target_domain=target_domain)
+
+        batch_sample_list = []
+        num_batches = next(iter(outputs.values())).shape[0]
+        for idx in range(num_batches):
+            gen_sample = GenDataSample()
+            if data_samples:
+                gen_sample.update(data_samples[idx])
+            setattr(gen_sample, f'gt_{target_domain}',
+                    PixelData(data=inputs_dict[f'img_{target_domain}'][idx]))
+            setattr(gen_sample, f'fake_{target_domain}',
+                    PixelData(data=outputs['target'][idx]))
+            setattr(gen_sample, f'gt_{source_domain}',
+                    PixelData(data=inputs_dict[f'img_{source_domain}'][idx]))
+            batch_sample_list.append(gen_sample)
+        return batch_sample_list
+
+    def val_step(self, data: ValTestStepInputs) -> ForwardOutputs:
+        """Gets the generated image of given data. Same as :meth:`val_step`.
+
+        Args:
+            data (ValTestStepInputs): Data sampled from metric specific
+                sampler. More detials in `Metrics` and `Evaluator`.
+
+        Returns:
+            ForwardOutputs: Generated image or image dict.
+        """
+        data = self.data_preprocessor(data)
+        inputs_dict, data_samples = data['inputs'], data['data_samples']
+        target_domain = self._reachable_domains[0]
+        source_domain = self.get_other_domains(target_domain)[0]
+        outputs = self.forward_test(
+            inputs_dict[f'img_{source_domain}'], target_domain=target_domain)
+
+        batch_sample_list = []
+        num_batches = next(iter(outputs.values())).shape[0]
+        for idx in range(num_batches):
+            gen_sample = GenDataSample()
+            if data_samples:
+                gen_sample.update(data_samples[idx])
+            setattr(gen_sample, f'gt_{target_domain}',
+                    PixelData(data=inputs_dict[f'img_{target_domain}'][idx]))
+            setattr(gen_sample, f'fake_{target_domain}',
+                    PixelData(data=outputs['target'][idx]))
+            setattr(gen_sample, f'gt_{source_domain}',
+                    PixelData(data=inputs_dict[f'img_{source_domain}'][idx]))
+            batch_sample_list.append(gen_sample)
+        return batch_sample_list
```

### Comparing `mmgen-0.7.3/mmgen/models/translation_models/static_translation_gan.py` & `mmgen-1.0.0rc0/mmgen/models/translation_models/static_translation_gan.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from copy import deepcopy
 
 import torch.nn as nn
-from mmcv.parallel import MMDistributedDataParallel
+from mmengine.model import (BaseModel, MMDistributedDataParallel,
+                            is_model_wrapper)
 
-from ..builder import MODELS, build_module
-from ..gans import BaseGAN
+from mmgen.registry import MODELS
+from ..builder import build_module
 from .base_translation_model import BaseTranslationModel
 
 
 @MODELS.register_module()
-class StaticTranslationGAN(BaseTranslationModel, BaseGAN):
+class StaticTranslationGAN(BaseTranslationModel, BaseModel):
     """Basic translation model based on static unconditional GAN.
 
     Args:
         generator (dict): Config for the generator.
         discriminator (dict): Config for the discriminator.
         gan_loss (dict): Config for the gan loss.
         pretrained (str | optional): Path for pretrained model.
@@ -24,21 +25,19 @@
         gen_auxiliary_loss (dict | optional): Config for auxiliary loss
             to generator. Defaults to None.
     """
 
     def __init__(self,
                  generator,
                  discriminator,
-                 gan_loss,
                  *args,
                  pretrained=None,
-                 disc_auxiliary_loss=None,
-                 gen_auxiliary_loss=None,
+                 data_preprocessor=dict(type='GANDataPreprocessor'),
                  **kwargs):
-        BaseGAN.__init__(self)
+        BaseModel.__init__(self, data_preprocessor=data_preprocessor)
         BaseTranslationModel.__init__(self, *args, **kwargs)
         # Building generators and discriminators
         self._gen_cfg = deepcopy(generator)
         # build domain generators
         self.generators = nn.ModuleDict()
         for domain in self._reachable_domains:
             self.generators[domain] = build_module(generator)
@@ -49,68 +48,36 @@
             self.discriminators = nn.ModuleDict()
             for domain in self._reachable_domains:
                 self.discriminators[domain] = build_module(discriminator)
         # support no discriminator in testing
         else:
             self.discriminators = None
 
-        # support no gan_loss in testing
-        if gan_loss is not None:
-            self.gan_loss = build_module(gan_loss)
-        else:
-            self.gan_loss = None
-
-        if disc_auxiliary_loss:
-            self.disc_auxiliary_losses = build_module(disc_auxiliary_loss)
-            if not isinstance(self.disc_auxiliary_losses, nn.ModuleList):
-                self.disc_auxiliary_losses = nn.ModuleList(
-                    [self.disc_auxiliary_losses])
-        else:
-            self.disc_auxiliary_loss = None
-
-        if gen_auxiliary_loss:
-            self.gen_auxiliary_losses = build_module(gen_auxiliary_loss)
-            if not isinstance(self.gen_auxiliary_losses, nn.ModuleList):
-                self.gen_auxiliary_losses = nn.ModuleList(
-                    [self.gen_auxiliary_losses])
-        else:
-            self.gen_auxiliary_losses = None
-
         self.init_weights(pretrained)
 
     def init_weights(self, pretrained=None):
         """Initialize weights for the model.
 
         Args:
             pretrained (str, optional): Path for pretrained weights. If given
                 None, pretrained weights will not be loaded. Default: None.
         """
         for domain in self._reachable_domains:
-            self.generators[domain].init_weights(pretrained=pretrained)
-            self.discriminators[domain].init_weights(pretrained=pretrained)
-
-    def _parse_train_cfg(self):
-        """Parsing train config and set some attributes for training."""
-        if self.train_cfg is None:
-            self.train_cfg = dict()
-        # control the work flow in train step
-        self.disc_steps = self.train_cfg.get('disc_steps', 1)
-
-        self.disc_init_steps = (0 if self.train_cfg is None else
-                                self.train_cfg.get('disc_init_steps', 0))
-
-        self.real_img_key = self.train_cfg.get('real_img_key', 'real_img')
-
-    def _parse_test_cfg(self):
-        """Parsing test config and set some attributes for testing."""
-        if self.test_cfg is None:
-            self.test_cfg = dict()
-
-        # basic testing information
-        self.batch_size = self.test_cfg.get('batch_size', 1)
+            if is_model_wrapper(self.generators):
+                self.generators.module[domain].init_weights(
+                    pretrained=pretrained)
+            else:
+                self.generators[domain].init_weights(pretrained=pretrained)
+            if self.discriminators is not None:
+                if is_model_wrapper(self.discriminators):
+                    self.discriminators.module[domain].init_weights(
+                        pretrained=pretrained)
+                else:
+                    self.discriminators[domain].init_weights(
+                        pretrained=pretrained)
 
     def get_module(self, module):
         """Get `nn.ModuleDict` to fit the `MMDistributedDataParallel`
         interface.
 
         Args:
             module (MMDistributedDataParallel | nn.ModuleDict): The input
```

### Comparing `mmgen-0.7.3/mmgen/ops/conv2d_gradfix.py` & `mmgen-1.0.0rc0/mmgen/ops/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/ops/stylegan3/custom_ops.py` & `mmgen-1.0.0rc0/mmgen/ops/stylegan3/custom_ops.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/ops/stylegan3/ops/bias_act.py` & `mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/bias_act.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/ops/stylegan3/ops/filtered_lrelu.py` & `mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/filtered_lrelu.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/ops/stylegan3/ops/upfirdn2d.py` & `mmgen-1.0.0rc0/mmgen/ops/stylegan3/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/mmgen/utils/collect_env.py` & `mmgen-1.0.0rc0/mmgen/utils/collect_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,32 @@
 import sys
 from collections import defaultdict
 
 import cv2
 import mmcv
 import torch
 import torchvision
-from mmcv.utils import get_build_config, get_git_hash
+from mmengine.utils import get_git_hash
+from mmengine.utils.dl_utils.parrots_wrapper import get_build_config
 
 import mmgen
 
 
 def collect_env():
     """Collect the information of the running environments."""
     env_info = {}
     env_info['sys.platform'] = sys.platform
     env_info['Python'] = sys.version.replace('\n', '')
 
     cuda_available = torch.cuda.is_available()
     env_info['CUDA available'] = cuda_available
 
     if cuda_available:
-        if mmcv.__version__ < '1.3.11':
-            from mmcv.utils.parrots_wrapper import CUDA_HOME
-        else:
-            from mmcv.utils.parrots_wrapper import _get_cuda_home
-            CUDA_HOME = _get_cuda_home()
+        from mmengine.utils.dl_utils.parrots_wrapper import _get_cuda_home
+        CUDA_HOME = _get_cuda_home()
 
         env_info['CUDA_HOME'] = CUDA_HOME
 
         if CUDA_HOME is not None and osp.isdir(CUDA_HOME):
             try:
                 nvcc = osp.join(CUDA_HOME, 'bin/nvcc')
                 nvcc = subprocess.check_output(
```

### Comparing `mmgen-0.7.3/mmgen/utils/dist_util.py` & `mmgen-1.0.0rc0/mmgen/utils/dist_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import numpy as np
 import torch
 import torch.distributed as dist
-from mmcv.runner import get_dist_info
+# from mmcv.runner import get_dist_info
+from mmengine.dist import get_dist_info
 
 
 def check_dist_init():
     return dist.is_available() and dist.is_initialized()
 
 
 def sync_random_seed(seed=None, device='cuda'):
```

### Comparing `mmgen-0.7.3/mmgen/utils/io_utils.py` & `mmgen-1.0.0rc0/mmgen/utils/io_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import hashlib
 import os
 
 import click
 import mmcv
 import requests
 import torch.distributed as dist
-from mmcv.runner import get_dist_info
+from mmengine.dist import get_dist_info
 from requests.exceptions import InvalidURL, RequestException, Timeout
 
 MMGEN_CACHE_DIR = os.path.expanduser('~') + '/.cache/openmmlab/mmgen/'
 
 
 def get_content_from_url(url, timeout=15, stream=False):
     """Get content from url.
```

### Comparing `mmgen-0.7.3/mmgen/version.py` & `mmgen-1.0.0rc0/mmgen/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.7.3'
+__version__ = '1.0.0rc0'
 
 
 def parse_version_info(version_str):
     """Parse version information.
 
     Args:
         version_str (str): Version string.
```

### Comparing `mmgen-0.7.3/mmgen.egg-info/PKG-INFO` & `mmgen-1.0.0rc0/mmgen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmgen
-Version: 0.7.3
+Version: 1.0.0rc0
 Summary: MMGeneration
 Home-page: https://github.com/open-mmlab/mmgen
 Author: MMGeneration Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
             <img src="https://user-images.githubusercontent.com/12726765/114528756-de55af80-9c7b-11eb-94d7-d3224ada1585.png" width="400"/>
@@ -24,58 +24,44 @@
                </a>
              </sup>
            </div>
            <div>&nbsp;</div>
         </div>
         
         [![PyPI](https://img.shields.io/pypi/v/mmgen)](https://pypi.org/project/mmgen)
-        [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmgeneration.readthedocs.io/en/latest/)
+        [![docs](https://img.shields.io/badge/docs-latest-blue)](https://mmgeneration.readthedocs.io/en/1.x/)
         [![badge](https://github.com/open-mmlab/mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/mmgeneration/actions)
-        [![codecov](https://codecov.io/gh/open-mmlab/mmgeneration/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmgeneration)
-        [![license](https://img.shields.io/github/license/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/master/LICENSE)
+        [![codecov](https://codecov.io/gh/open-mmlab/mmgeneration/branch/1.x/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmgeneration)
+        [![license](https://img.shields.io/github/license/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/1.x/LICENSE)
         [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
         [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
         
-        [📘Documentation](https://mmgeneration.readthedocs.io/en/latest/) |
-        [🛠️Installation](https://mmgeneration.readthedocs.io/en/latest/get_started.html#installation) |
-        [👀Model Zoo](https://mmgeneration.readthedocs.io/en/latest/modelzoo_statistics.html) |
-        [🆕Update News](https://github.com/open-mmlab/mmgeneration/blob/master/docs/en/changelog.md) |
+        [📘Documentation](https://mmgeneration.readthedocs.io/en/1.x/) |
+        [🛠️Installation](https://mmgeneration.readthedocs.io/en/1.x/get_started.html#installation) |
+        [👀Model Zoo](https://mmgeneration.readthedocs.io/en/1.x/modelzoo_statistics.html) |
+        [🆕Update News](https://github.com/open-mmlab/mmgeneration/blob/1.x/docs/en/notes/changelog.md) |
         [🚀Ongoing Projects](https://github.com/open-mmlab/mmgeneration/projects) |
         [🤔Reporting Issues](https://github.com/open-mmlab/mmgeneration/issues)
         
         English | [简体中文](README_zh-CN.md)
         
-        ## What's New
-        
-        MMGeneration has been merged in [MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x). And we have supported new generation tasks and models. We highlight the following new features:
-        
-        - 🌟 Text2Image
-        
-          - ✅ [GLIDE](https://github.com/open-mmlab/mmediting/tree/1.x/projects/glide/configs/README.md)
-          - ✅ [Disco-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/disco_diffusion/README.md)
-          - ✅ [Stable-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/stable_diffusion/README.md)
-        
-        - 🌟 3D-aware Generation
-        
-          - ✅ [EG3D](https://github.com/open-mmlab/mmediting/tree/1.x/configs/eg3d/README.md)
-        
         ## Introduction
         
-        MMGeneration is a powerful toolkit for generative models, especially for GANs now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv). The master branch works with **PyTorch 1.5+**.
+        MMGeneration is a powerful toolkit for generative models, especially for GANs now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x). The master branch works with **PyTorch 1.5+**.
         
         <div align="center">
             <img src="https://user-images.githubusercontent.com/12726765/114534478-9a65a900-9c81-11eb-8087-de8b6816eed8.png" width="800"/>
         </div>
         
         ## Major Features
         
-        - **High-quality Training Performance:** We currently support training on Unconditional GANs, Internal GANs, and Image Translation Models. Support for conditional models will come soon.
-        - **Powerful Application Toolkit:** A plentiful toolkit containing multiple applications in GANs is provided to users. GAN interpolation, GAN projection, and GAN manipulations are integrated into our framework. It's time to play with your GANs! ([Tutorial for applications](docs/en/tutorials/applications.md))
-        - **Efficient Distributed Training for Generative Models:** For the highly dynamic training in generative models, we adopt a new way to train dynamic models with `MMDDP`. ([Tutorial for DDP](docs/en/tutorials/ddp_train_gans.md))
-        - **New Modular Design for Flexible Combination:** A new design for complex loss modules is proposed for customizing the links between modules, which can achieve flexible combination among different modules. ([Tutorial for new modular design](docs/en/tutorials/customize_losses.md))
+        - **High-quality Training Performance:** MMGeneration currently support training on Unconditional GANs, Conditional GANs, Internal GANs, Image Translation Models, and Diffusion Models.
+        - **Powerful Application Toolkit:** A toolkit that provides plentiful applications to users. MMGeneration supports GAN interpolation, GAN projection, GAN manipulations and many other popular GAN's applications. It's time to play with your GANs! ([Tutorial for applications](docs/en/advanced_guides/applications.md))
+        - **Efficient Distributed Training for Generative Models:** With support of [MMSeparateDistributedDataParallel](https://github.com/open-mmlab/mmengine/blob/main/mmengine/model/wrappers/seperate_distributed.py), distributed training for dynamic architectures can be easily implemented.
+        - **New Modular Design for Flexible Combination:** A new design for complex loss modules is proposed for customizing the links between modules, which can achieve flexible combination among different modules.(Tutorial for [losses](docs/en/advanced_guides/losses.md))
         
         <table>
         <thead>
           <tr>
             <td>
         <div align="center">
           <b> Training Visualization</b>
@@ -106,53 +92,63 @@
         
         ## Highlight
         
         - **Positional Encoding as Spatial Inductive Bias in GANs (CVPR2021)** has been released in `MMGeneration`.  [\[Config\]](configs/positional_encoding_in_gans/README.md), [\[Project Page\]](https://nbei.github.io/gan-pos-encoding.html)
         - Conditional GANs have been supported in our toolkit. More methods and pre-trained weights will come soon.
         - Mixed-precision training (FP16) for StyleGAN2 has been supported. Please check [the comparison](configs/styleganv2/README.md) between different implementations.
         
-        ## Changelog
+        ## What's new
+        
+        v1.0.0rc0 was released in 31/8/2022.
+        
+        This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
+        to try according to [the documentation](https://mmgeneration.readthedocs.io/en/1.x/).
         
-        v0.7.3 was released on 14/04/2023. Please refer to [changelog.md](docs/en/changelog.md) for details and release history.
+        And there are some BC-breaking changes. Please check [the migration tutorial](https://mmgeneration.readthedocs.io/en/1.x/migration.html).
+        
+        The release candidate will last until the end of 2022, and during the release candidate, we will develop on the `1.x` branch. And we will still maintain 0.x version still at least the end of 2023.
+        
+        Please refer to [changelog.md](https://mmgeneration.readthedocs.io/en/1.x/notes/changelog.html) for more details and other release history.
         
         ## Installation
         
-        MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv).
+        MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x).
         Below are quick steps for installation.
         
         **Step 1.**
         Install PyTorch following [official instructions](https://pytorch.org/get-started/locally/), e.g.
         
         ```python
         pip3 install torch torchvision
         
         ```
         
         **Step 2.**
         Install MMCV with [MIM](https://github.com/open-mmlab/mim).
         
         ```
-        pip3 install openmim
-        mim install mmcv-full
+        pip install -U openmim
+        # wait for more pre-compiled pkgs to release
+        mim install 'mmcv>=2.0.0rc1'
         ```
         
         **Step 3.**
         Install MMGeneration from source.
         
         ```
-        git clone https://github.com/open-mmlab/mmgeneration.git
+        git clone -b 1.x https://github.com/open-mmlab/mmgeneration.git
         cd mmgeneration
-        pip3 install -e .
+        pip3 install -e .[all]
         ```
         
         Please refer to [get_started.md](docs/en/get_started.md) for more detailed instruction.
         
         ## Getting Started
         
-        Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration. [docs/en/quick_run.md](docs/en/quick_run.md) can offer full guidance for quick run. For other details and tutorials, please go to our [documentation](https://mmgeneration.readthedocs.io/).
+        Please see [get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration. For other details and tutorials, please go to our [documentation](https://mmgeneration.readthedocs.io/en/1.x/).
         
         ## ModelZoo
         
         These methods have been carefully studied and supported in our frameworks:
         
         <details open>
         <summary>Unconditional GANs (click to collapse)</summary>
@@ -176,21 +172,14 @@
         - ✅ [Projection GAN](configs/sngan_proj/README.md) (ICLR'2018)
         - ✅ [SAGAN](configs/sagan/README.md) (ICML'2019)
         - ✅ [BIGGAN/BIGGAN-DEEP](configs/biggan/README.md) (ICLR'2019)
         
         </details>
         
         <details open>
-        <summary>Tricks for GANs (click to collapse)</summary>
-        
-        - ✅ [ADA](configs/ada/README.md) (NeurIPS'2020)
-        
-        </details>
-        
-        <details open>
         <summary>Image2Image Translation (click to collapse)</summary>
         
         - ✅ [Pix2Pix](configs/pix2pix/README.md) (CVPR'2017)
         - ✅ [CycleGAN](configs/cyclegan/README.md) (ICCV'2017)
         
         </details>
         
@@ -210,15 +199,15 @@
         
         ## Related-Applications
         
         - ✅ [MMGEN-FaceStylor](https://github.com/open-mmlab/MMGEN-FaceStylor)
         
         ## Contributing
         
-        We appreciate all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/blob/master/CONTRIBUTING.md) in MMCV for more details about the contributing guideline.
+        We appreciate all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/tree/2.x/CONTRIBUTING.md) in MMCV and \[https://github.com/open-mmlab/mmengine/blob/main/CONTRIBUTING.md\] in MMEngine for more details about the contributing guideline.
         
         ## Citation
         
         If you find this project useful in your research, please consider cite:
         
         ```BibTeX
         @misc{2021mmgeneration,
@@ -229,34 +218,35 @@
         }
         ```
         
         ## License
         
         This project is released under the [Apache 2.0 license](LICENSE). Some operations in `MMGeneration` are with other licenses instead of Apache2.0. Please refer to [LICENSES.md](LICENSES.md) for the careful check, if you are using our code for commercial matters.
         
-        ## Projects in OpenMMLab
+        ## Projects in OpenMMLab 2.0
         
-        - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+        - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+        - [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x): OpenMMLab foundational library for computer vision.
         - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-        - [MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab image classification toolbox and benchmark.
-        - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-        - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-        - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-        - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-        - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-        - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+        - [MMClassification](https://github.com/open-mmlab/mmclassification/tree/1.x): OpenMMLab image classification toolbox and benchmark.
+        - [MMDetection](https://github.com/open-mmlab/mmdetection/tree/3.x): OpenMMLab detection toolbox and benchmark.
+        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d/tree/1.x): OpenMMLab's next-generation platform for general 3D object detection.
+        - [MMRotate](https://github.com/open-mmlab/mmrotate/tree/1.x): OpenMMLab rotated object detection toolbox and benchmark.
+        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation/tree/1.x): OpenMMLab semantic segmentation toolbox and benchmark.
+        - [MMOCR](https://github.com/open-mmlab/mmocr/tree/1.x): OpenMMLab text detection, recognition, and understanding toolbox.
+        - [MMPose](https://github.com/open-mmlab/mmpose/tree/1.x): OpenMMLab pose estimation toolbox and benchmark.
+        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d/tree/1.x): OpenMMLab 3D human parametric model toolbox and benchmark.
+        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup/tree/1.x): OpenMMLab self-supervised learning toolbox and benchmark.
+        - [MMRazor](https://github.com/open-mmlab/mmrazor/tree/1.x): OpenMMLab model compression toolbox and benchmark.
+        - [MMFewShot](https://github.com/open-mmlab/mmfewshot/tree/1.x): OpenMMLab fewshot learning toolbox and benchmark.
+        - [MMAction2](https://github.com/open-mmlab/mmaction2/tree/1.x): OpenMMLab's next-generation action understanding toolbox and benchmark.
+        - [MMTracking](https://github.com/open-mmlab/mmtracking/tree/1.x): OpenMMLab video perception toolbox and benchmark.
+        - [MMFlow](https://github.com/open-mmlab/mmflow/tree/1.x): OpenMMLab optical flow toolbox and benchmark.
+        - [MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x): OpenMMLab image and video editing toolbox.
+        - [MMGeneration](https://github.com/open-mmlab/mmgeneration/tree/1.x): OpenMMLab image and video generative models toolbox.
         - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,149 +1,152 @@
-Metadata-Version: 2.1 Name: mmgen Version: 0.7.3 Summary: MMGeneration Home-
+Metadata-Version: 2.1 Name: mmgen Version: 1.0.0rc0 Summary: MMGeneration Home-
 page: https://github.com/open-mmlab/mmgen Author: MMGeneration Contributors
 Author-email: openmmlab@gmail.com License: Apache License 2.0 Description:
  [https://user-images.githubusercontent.com/12726765/114528756-de55af80-9c7b-
                           11eb-94d7-d3224ada1585.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
 [![PyPI](https://img.shields.io/pypi/v/mmgen)](https://pypi.org/project/mmgen)
 [![docs](https://img.shields.io/badge/docs-latest-blue)](https://
-mmgeneration.readthedocs.io/en/latest/) [![badge](https://github.com/open-
-mmlab/mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/
+mmgeneration.readthedocs.io/en/1.x/) [![badge](https://github.com/open-mmlab/
+mmgeneration/workflows/build/badge.svg)](https://github.com/open-mmlab/
 mmgeneration/actions) [![codecov](https://codecov.io/gh/open-mmlab/
-mmgeneration/branch/master/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
+mmgeneration/branch/1.x/graph/badge.svg)](https://codecov.io/gh/open-mmlab/
 mmgeneration) [![license](https://img.shields.io/github/license/open-mmlab/
-mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/master/
-LICENSE) [![open issues](https://isitmaintained.com/badge/open/open-mmlab/
+mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/blob/1.x/LICENSE)
+[![open issues](https://isitmaintained.com/badge/open/open-mmlab/
 mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues) [![issue
 resolution](https://isitmaintained.com/badge/resolution/open-mmlab/
 mmgeneration.svg)](https://github.com/open-mmlab/mmgeneration/issues)
-[ðDocumentation](https://mmgeneration.readthedocs.io/en/latest/) |
-[ð ï¸Installation](https://mmgeneration.readthedocs.io/en/latest/
+[ðDocumentation](https://mmgeneration.readthedocs.io/en/1.x/) |
+[ð ï¸Installation](https://mmgeneration.readthedocs.io/en/1.x/
 get_started.html#installation) | [ðModel Zoo](https://
-mmgeneration.readthedocs.io/en/latest/modelzoo_statistics.html) | [ðUpdate
-News](https://github.com/open-mmlab/mmgeneration/blob/master/docs/en/
+mmgeneration.readthedocs.io/en/1.x/modelzoo_statistics.html) | [ðUpdate
+News](https://github.com/open-mmlab/mmgeneration/blob/1.x/docs/en/notes/
 changelog.md) | [ðOngoing Projects](https://github.com/open-mmlab/
 mmgeneration/projects) | [ð¤Reporting Issues](https://github.com/open-mmlab/
-mmgeneration/issues) English | [ç®ä½ä¸­æ](README_zh-CN.md) ## What's New
-MMGeneration has been merged in [MMEditing](https://github.com/open-mmlab/
-mmediting/tree/1.x). And we have supported new generation tasks and models. We
-highlight the following new features: - ð Text2Image - â [GLIDE](https://
-github.com/open-mmlab/mmediting/tree/1.x/projects/glide/configs/README.md) -
-â [Disco-Diffusion](https://github.com/open-mmlab/mmediting/tree/1.x/configs/
-disco_diffusion/README.md) - â [Stable-Diffusion](https://github.com/open-
-mmlab/mmediting/tree/1.x/configs/stable_diffusion/README.md) - ð 3D-aware
-Generation - â [EG3D](https://github.com/open-mmlab/mmediting/tree/1.x/
-configs/eg3d/README.md) ## Introduction MMGeneration is a powerful toolkit for
-generative models, especially for GANs now. It is based on PyTorch and [MMCV]
-(https://github.com/open-mmlab/mmcv). The master branch works with **PyTorch
-1.5+**.
+mmgeneration/issues) English | [ç®ä½ä¸­æ](README_zh-CN.md) ## Introduction
+MMGeneration is a powerful toolkit for generative models, especially for GANs
+now. It is based on PyTorch and [MMCV](https://github.com/open-mmlab/mmcv/tree/
+2.x). The master branch works with **PyTorch 1.5+**.
  [https://user-images.githubusercontent.com/12726765/114534478-9a65a900-9c81-
                           11eb-8087-de8b6816eed8.png]
-## Major Features - **High-quality Training Performance:** We currently support
-training on Unconditional GANs, Internal GANs, and Image Translation Models.
-Support for conditional models will come soon. - **Powerful Application
-Toolkit:** A plentiful toolkit containing multiple applications in GANs is
-provided to users. GAN interpolation, GAN projection, and GAN manipulations are
-integrated into our framework. It's time to play with your GANs! ([Tutorial for
-applications](docs/en/tutorials/applications.md)) - **Efficient Distributed
-Training for Generative Models:** For the highly dynamic training in generative
-models, we adopt a new way to train dynamic models with `MMDDP`. ([Tutorial for
-DDP](docs/en/tutorials/ddp_train_gans.md)) - **New Modular Design for Flexible
-Combination:** A new design for complex loss modules is proposed for
-customizing the links between modules, which can achieve flexible combination
-among different modules. ([Tutorial for new modular design](docs/en/tutorials/
-customize_losses.md))
+## Major Features - **High-quality Training Performance:** MMGeneration
+currently support training on Unconditional GANs, Conditional GANs, Internal
+GANs, Image Translation Models, and Diffusion Models. - **Powerful Application
+Toolkit:** A toolkit that provides plentiful applications to users.
+MMGeneration supports GAN interpolation, GAN projection, GAN manipulations and
+many other popular GAN's applications. It's time to play with your GANs! (
+[Tutorial for applications](docs/en/advanced_guides/applications.md)) -
+**Efficient Distributed Training for Generative Models:** With support of
+[MMSeparateDistributedDataParallel](https://github.com/open-mmlab/mmengine/
+blob/main/mmengine/model/wrappers/seperate_distributed.py), distributed
+training for dynamic architectures can be easily implemented. - **New Modular
+Design for Flexible Combination:** A new design for complex loss modules is
+proposed for customizing the links between modules, which can achieve flexible
+combination among different modules.(Tutorial for [losses](docs/en/
+advanced_guides/losses.md))
    Training Visualization          GAN Interpolation               GAN Projector                GAN Manipulation
        [https://user-                [https://user-                [https://user-                [https://user-
 images.githubusercontent.com/ images.githubusercontent.com/ images.githubusercontent.com/ images.githubusercontent.com/
 12726765/114509105-b6f4e780-  12726765/114679300-9fd4f900-  12726765/114524392-c11ee200-  12726765/114523716-20302700-
        9c67-11eb-8644-               9d3e-11eb-8f37-               9c77-11eb-8b6d-               9c77-11eb-804e-
       110b3cb01314.gif]             c36a018c02f7.gif]             37bc637f5626.gif]             327ae1ca0c5b.gif]
 ## Highlight - **Positional Encoding as Spatial Inductive Bias in GANs
 (CVPR2021)** has been released in `MMGeneration`. [\[Config\]](configs/
 positional_encoding_in_gans/README.md), [\[Project Page\]](https://
 nbei.github.io/gan-pos-encoding.html) - Conditional GANs have been supported in
 our toolkit. More methods and pre-trained weights will come soon. - Mixed-
 precision training (FP16) for StyleGAN2 has been supported. Please check [the
 comparison](configs/styleganv2/README.md) between different implementations. ##
-Changelog v0.7.3 was released on 14/04/2023. Please refer to [changelog.md]
-(docs/en/changelog.md) for details and release history. ## Installation
-MMGeneration depends on [PyTorch](https://pytorch.org/) and [MMCV](https://
-github.com/open-mmlab/mmcv). Below are quick steps for installation. **Step
-1.** Install PyTorch following [official instructions](https://pytorch.org/get-
-started/locally/), e.g. ```python pip3 install torch torchvision ``` **Step
-2.** Install MMCV with [MIM](https://github.com/open-mmlab/mim). ``` pip3
-install openmim mim install mmcv-full ``` **Step 3.** Install MMGeneration from
-source. ``` git clone https://github.com/open-mmlab/mmgeneration.git cd
-mmgeneration pip3 install -e . ``` Please refer to [get_started.md](docs/en/
-get_started.md) for more detailed instruction. ## Getting Started Please see
-[get_started.md](docs/en/get_started.md) for the basic usage of MMGeneration.
-[docs/en/quick_run.md](docs/en/quick_run.md) can offer full guidance for quick
-run. For other details and tutorials, please go to our [documentation](https://
-mmgeneration.readthedocs.io/). ## ModelZoo These methods have been carefully
-studied and supported in our frameworks:  Unconditional GANs (click to
-collapse) - â [DCGAN](configs/dcgan/README.md) (ICLR'2016) - â [WGAN-GP]
-(configs/wgan-gp/README.md) (NIPS'2017) - â [LSGAN](configs/lsgan/README.md)
-(ICCV'2017) - â [GGAN](configs/ggan/README.md) (arXiv'2017) - â [PGGAN]
-(configs/pggan/README.md) (ICLR'2018) - â [StyleGANV1](configs/styleganv1/
-README.md) (CVPR'2019) - â [StyleGANV2](configs/styleganv2/README.md)
-(CVPR'2020) - â [StyleGANV3](configs/styleganv3/README.md) (NeurIPS'2021) -
-â [Positional Encoding in GANs](configs/positional_encoding_in_gans/
-README.md) (CVPR'2021)   Conditional GANs (click to collapse) - â [SNGAN]
-(configs/sngan_proj/README.md) (ICLR'2018) - â [Projection GAN](configs/
-sngan_proj/README.md) (ICLR'2018) - â [SAGAN](configs/sagan/README.md)
-(ICML'2019) - â [BIGGAN/BIGGAN-DEEP](configs/biggan/README.md) (ICLR'2019)
-Tricks for GANs (click to collapse) - â [ADA](configs/ada/README.md)
-(NeurIPS'2020)   Image2Image Translation (click to collapse) - â [Pix2Pix]
-(configs/pix2pix/README.md) (CVPR'2017) - â [CycleGAN](configs/cyclegan/
-README.md) (ICCV'2017)   Internal Learning (click to collapse) - â [SinGAN]
-(configs/singan/README.md) (ICCV'2019)   Denoising Diffusion Probabilistic
-Models (click to collapse) - â [Improved DDPM](configs/improved_ddpm/
-README.md) (arXiv'2021)  ## Related-Applications - â [MMGEN-FaceStylor]
-(https://github.com/open-mmlab/MMGEN-FaceStylor) ## Contributing We appreciate
-all contributions to improve MMGeneration. Please refer to [CONTRIBUTING.md]
-(https://github.com/open-mmlab/mmcv/blob/master/CONTRIBUTING.md) in MMCV for
-more details about the contributing guideline. ## Citation If you find this
-project useful in your research, please consider cite: ```BibTeX @misc
-{2021mmgeneration, title={{MMGeneration}: OpenMMLab Generative Model Toolbox
-and Benchmark}, author={MMGeneration Contributors}, howpublished = {\url{https:
-//github.com/open-mmlab/mmgeneration}}, year={2021} } ``` ## License This
-project is released under the [Apache 2.0 license](LICENSE). Some operations in
-`MMGeneration` are with other licenses instead of Apache2.0. Please refer to
-[LICENSES.md](LICENSES.md) for the careful check, if you are using our code for
-commercial matters. ## Projects in OpenMMLab - [MMCV](https://github.com/open-
-mmlab/mmcv): OpenMMLab foundational library for computer vision. - [MIM](https:
-//github.com/open-mmlab/mim): MIM installs OpenMMLab packages. -
-[MMClassification](https://github.com/open-mmlab/mmclassification): OpenMMLab
-image classification toolbox and benchmark. - [MMDetection](https://github.com/
-open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark. -
-[MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-
-generation platform for general 3D object detection. - [MMRotate](https://
-github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and
-benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation):
-OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR](https://
-github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and
-understanding toolbox. - [MMPose](https://github.com/open-mmlab/mmpose):
-OpenMMLab pose estimation toolbox and benchmark. - [MMHuman3D](https://
-github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox
-and benchmark. - [MMSelfSup](https://github.com/open-mmlab/mmselfsup):
-OpenMMLab self-supervised learning toolbox and benchmark. - [MMRazor](https://
-github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and
-benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab
-fewshot learning toolbox and benchmark. - [MMAction2](https://github.com/open-
-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and
-benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
+What's new v1.0.0rc0 was released in 31/8/2022. This release introduced a brand
+new and flexible training & test engine, but it's still in progress. Welcome to
+try according to [the documentation](https://mmgeneration.readthedocs.io/en/
+1.x/). And there are some BC-breaking changes. Please check [the migration
+tutorial](https://mmgeneration.readthedocs.io/en/1.x/migration.html). The
+release candidate will last until the end of 2022, and during the release
+candidate, we will develop on the `1.x` branch. And we will still maintain 0.x
+version still at least the end of 2023. Please refer to [changelog.md](https://
+mmgeneration.readthedocs.io/en/1.x/notes/changelog.html) for more details and
+other release history. ## Installation MMGeneration depends on [PyTorch](https:
+//pytorch.org/) and [MMCV](https://github.com/open-mmlab/mmcv/tree/2.x). Below
+are quick steps for installation. **Step 1.** Install PyTorch following
+[official instructions](https://pytorch.org/get-started/locally/), e.g.
+```python pip3 install torch torchvision ``` **Step 2.** Install MMCV with
+[MIM](https://github.com/open-mmlab/mim). ``` pip install -U openmim # wait for
+more pre-compiled pkgs to release mim install 'mmcv>=2.0.0rc1' ``` **Step 3.**
+Install MMGeneration from source. ``` git clone -b 1.x https://github.com/open-
+mmlab/mmgeneration.git cd mmgeneration pip3 install -e .[all] ``` Please refer
+to [get_started.md](docs/en/get_started.md) for more detailed instruction. ##
+Getting Started Please see [get_started.md](docs/en/get_started.md) for the
+basic usage of MMGeneration. For other details and tutorials, please go to our
+[documentation](https://mmgeneration.readthedocs.io/en/1.x/). ## ModelZoo These
+methods have been carefully studied and supported in our frameworks:
+Unconditional GANs (click to collapse) - â [DCGAN](configs/dcgan/README.md)
+(ICLR'2016) - â [WGAN-GP](configs/wgan-gp/README.md) (NIPS'2017) - â
+[LSGAN](configs/lsgan/README.md) (ICCV'2017) - â [GGAN](configs/ggan/
+README.md) (arXiv'2017) - â [PGGAN](configs/pggan/README.md) (ICLR'2018) -
+â [StyleGANV1](configs/styleganv1/README.md) (CVPR'2019) - â [StyleGANV2]
+(configs/styleganv2/README.md) (CVPR'2020) - â [StyleGANV3](configs/
+styleganv3/README.md) (NeurIPS'2021) - â [Positional Encoding in GANs]
+(configs/positional_encoding_in_gans/README.md) (CVPR'2021)   Conditional GANs
+(click to collapse) - â [SNGAN](configs/sngan_proj/README.md) (ICLR'2018) -
+â [Projection GAN](configs/sngan_proj/README.md) (ICLR'2018) - â [SAGAN]
+(configs/sagan/README.md) (ICML'2019) - â [BIGGAN/BIGGAN-DEEP](configs/
+biggan/README.md) (ICLR'2019)   Image2Image Translation (click to collapse) -
+â [Pix2Pix](configs/pix2pix/README.md) (CVPR'2017) - â [CycleGAN](configs/
+cyclegan/README.md) (ICCV'2017)   Internal Learning (click to collapse) - â
+[SinGAN](configs/singan/README.md) (ICCV'2019)   Denoising Diffusion
+Probabilistic Models (click to collapse) - â [Improved DDPM](configs/
+improved_ddpm/README.md) (arXiv'2021)  ## Related-Applications - â [MMGEN-
+FaceStylor](https://github.com/open-mmlab/MMGEN-FaceStylor) ## Contributing We
+appreciate all contributions to improve MMGeneration. Please refer to
+[CONTRIBUTING.md](https://github.com/open-mmlab/mmcv/tree/2.x/CONTRIBUTING.md)
+in MMCV and \[https://github.com/open-mmlab/mmengine/blob/main/
+CONTRIBUTING.md\] in MMEngine for more details about the contributing
+guideline. ## Citation If you find this project useful in your research, please
+consider cite: ```BibTeX @misc{2021mmgeneration, title={{MMGeneration}:
+OpenMMLab Generative Model Toolbox and Benchmark}, author={MMGeneration
+Contributors}, howpublished = {\url{https://github.com/open-mmlab/
+mmgeneration}}, year={2021} } ``` ## License This project is released under the
+[Apache 2.0 license](LICENSE). Some operations in `MMGeneration` are with other
+licenses instead of Apache2.0. Please refer to [LICENSES.md](LICENSES.md) for
+the careful check, if you are using our code for commercial matters. ##
+Projects in OpenMMLab 2.0 - [MMEngine](https://github.com/open-mmlab/mmengine):
+OpenMMLab foundational library for training deep learning models. - [MMCV]
+(https://github.com/open-mmlab/mmcv/tree/2.x): OpenMMLab foundational library
+for computer vision. - [MIM](https://github.com/open-mmlab/mim): MIM installs
+OpenMMLab packages. - [MMClassification](https://github.com/open-mmlab/
+mmclassification/tree/1.x): OpenMMLab image classification toolbox and
+benchmark. - [MMDetection](https://github.com/open-mmlab/mmdetection/tree/3.x):
+OpenMMLab detection toolbox and benchmark. - [MMDetection3D](https://
+github.com/open-mmlab/mmdetection3d/tree/1.x): OpenMMLab's next-generation
+platform for general 3D object detection. - [MMRotate](https://github.com/open-
+mmlab/mmrotate/tree/1.x): OpenMMLab rotated object detection toolbox and
+benchmark. - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation/
+tree/1.x): OpenMMLab semantic segmentation toolbox and benchmark. - [MMOCR]
+(https://github.com/open-mmlab/mmocr/tree/1.x): OpenMMLab text detection,
+recognition, and understanding toolbox. - [MMPose](https://github.com/open-
+mmlab/mmpose/tree/1.x): OpenMMLab pose estimation toolbox and benchmark. -
+[MMHuman3D](https://github.com/open-mmlab/mmhuman3d/tree/1.x): OpenMMLab 3D
+human parametric model toolbox and benchmark. - [MMSelfSup](https://github.com/
+open-mmlab/mmselfsup/tree/1.x): OpenMMLab self-supervised learning toolbox and
+benchmark. - [MMRazor](https://github.com/open-mmlab/mmrazor/tree/1.x):
+OpenMMLab model compression toolbox and benchmark. - [MMFewShot](https://
+github.com/open-mmlab/mmfewshot/tree/1.x): OpenMMLab fewshot learning toolbox
+and benchmark. - [MMAction2](https://github.com/open-mmlab/mmaction2/tree/1.x):
+OpenMMLab's next-generation action understanding toolbox and benchmark. -
+[MMTracking](https://github.com/open-mmlab/mmtracking/tree/1.x): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMEditing]
-(https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing
-toolbox. - [MMGeneration](https://github.com/open-mmlab/mmgeneration):
-OpenMMLab image and video generative models toolbox. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
-Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
-License :: OSI Approved :: Apache Software License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
-Provides-Extra: all Provides-Extra: tests Provides-Extra: mim
+mmlab/mmflow/tree/1.x): OpenMMLab optical flow toolbox and benchmark. -
+[MMEditing](https://github.com/open-mmlab/mmediting/tree/1.x): OpenMMLab image
+and video editing toolbox. - [MMGeneration](https://github.com/open-mmlab/
+mmgeneration/tree/1.x): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown Provides-Extra: all Provides-Extra: tests Provides-Extra: mim
```

### Comparing `mmgen-0.7.3/setup.cfg` & `mmgen-1.0.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmgen-0.7.3/setup.py` & `mmgen-1.0.0rc0/setup.py`

 * *Files identical despite different names*

