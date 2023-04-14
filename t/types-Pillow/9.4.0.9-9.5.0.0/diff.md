# Comparing `tmp/types-Pillow-9.4.0.9.tar.gz` & `tmp/types-Pillow-9.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Pillow-9.4.0.9.tar", last modified: Thu Feb  9 09:16:51 2023, max compression
+gzip compressed data, was "types-Pillow-9.5.0.0.tar", last modified: Fri Apr 14 09:14:44 2023, max compression
```

## Comparing `types-Pillow-9.4.0.9.tar` & `types-Pillow-9.5.0.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 09:16:51.453737 types-Pillow-9.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-02-09 09:16:50.000000 types-Pillow-9.4.0.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-09 09:16:50.000000 types-Pillow-9.4.0.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 09:16:51.449737 types-Pillow-9.4.0.9/PIL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/BdfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/BlpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/BmpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/BufrStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ContainerIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/CurImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/DcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/DdsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/EpsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ExifTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/FitsStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/FliImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/FontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/FpxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/FtexImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/GbrImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/GdImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/GifImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/GimpGradientFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/GimpPaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/GribStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/Hdf5StubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/IcnsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/IcoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/Image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageChops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageCms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageColor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageDraw2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageEnhance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageFilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageFont.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageGrab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageMath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageMode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageMorph.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageOps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImagePalette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImagePath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageQt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageSequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageShow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageStat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageTk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageTransform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImageWin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/ImtImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/IptcImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/Jpeg2KImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/JpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/JpegPresets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-09 09:16:50.000000 types-Pillow-9.4.0.9/PIL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/McIdasImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/MicImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/MpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/MpoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/MspImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PSDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PalmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PcdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PcfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PdfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PdfParser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PixarImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PngImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PsdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/PyAccess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/SgiImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/SpiderImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/SunImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/TarIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/TgaImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/TiffImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/TiffTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/WalImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/WebPImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/WmfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/XVThumbImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/XbmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/XpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/_binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/_imaging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/_tkinter_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-09 09:16:28.000000 types-Pillow-9.4.0.9/PIL-stubs/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-09 09:16:51.453737 types-Pillow-9.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 09:16:51.453737 types-Pillow-9.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-02-09 09:16:50.000000 types-Pillow-9.4.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 09:16:51.453737 types-Pillow-9.4.0.9/types_Pillow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-09 09:16:51.000000 types-Pillow-9.4.0.9/types_Pillow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-09 09:16:51.000000 types-Pillow-9.4.0.9/types_Pillow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 09:16:51.000000 types-Pillow-9.4.0.9/types_Pillow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-09 09:16:51.000000 types-Pillow-9.4.0.9/types_Pillow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:44.250007 types-Pillow-9.5.0.0/PIL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BdfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BlpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BmpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/BufrStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ContainerIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/CurImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/DcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/DdsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/EpsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ExifTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FitsStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FliImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FpxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/FtexImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GbrImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GdImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GifImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GimpGradientFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GimpPaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/GribStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/Hdf5StubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/IcnsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/IcoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/Image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageChops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageCms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageColor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageDraw2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageEnhance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageFilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageFont.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageGrab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageMath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageMode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageMorph.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageOps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImagePalette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImagePath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageQt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageSequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageShow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageStat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageTk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageTransform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImageWin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/ImtImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/IptcImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/Jpeg2KImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/JpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/JpegPresets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/PIL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/McIdasImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MicImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MpoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/MspImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PSDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PalmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PcdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PcfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PdfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PdfParser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PixarImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PngImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PsdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/PyAccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/SgiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/SpiderImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/SunImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TarIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TgaImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TiffImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/TiffTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/WalImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/WebPImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/WmfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/XVThumbImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/XbmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/XpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_imaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_tkinter_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 09:14:29.000000 types-Pillow-9.5.0.0/PIL-stubs/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-14 09:14:42.000000 types-Pillow-9.5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:14:44.254007 types-Pillow-9.5.0.0/types_Pillow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 09:14:44.000000 types-Pillow-9.5.0.0/types_Pillow.egg-info/top_level.txt
```

### Comparing `types-Pillow-9.4.0.9/CHANGELOG.md` & `types-Pillow-9.5.0.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,64 @@
+## 9.5.0.0 (2023-04-14)
+
+Bump Pillow to 9.5.* (#10046)
+
+Release: https://pypi.org/pypi/Pillow/9.5.0
+Homepage: https://python-pillow.org
+Changelog: https://github.com/python-pillow/Pillow/blob/main/CHANGES.rst
+Diff: https://github.com/python-pillow/Pillow/compare/9.4.0...9.5.0
+
+## 9.4.0.19 (2023-03-28)
+
+Delete some unnecessary type aliases in tkinter (#9970)
+
+## 9.4.0.18 (2023-03-27)
+
+Add default values for third-party stubs beginning with 'P' (#9957)
+
+## 9.4.0.17 (2023-02-26)
+
+Improve many `__(a)exit__` annotations (#9696)
+
+## 9.4.0.16 (2023-02-22)
+
+Update `Unused` parameters in `stubs/` (#9704)
+
+* Update _Unused TypeAlias
+
+* Update `object | None` params
+
+* Replace unused `object` parameters with `Unused` alias
+
+## 9.4.0.15 (2023-02-21)
+
+Integrate requirements-stubtest.txt into METADATA.toml (#9778)
+
+## 9.4.0.14 (2023-02-21)
+
+Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
+
+If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
+
+## 9.4.0.13 (2023-02-18)
+
+Add types for PIL.ImageTk (#9733)
+
+## 9.4.0.12 (2023-02-15)
+
+Use `typing_extensions.Self` instead of `_typeshed.Self` (#9702)
+
+## 9.4.0.11 (2023-02-14)
+
+Add comments when subclassing Any (#9732)
+
+## 9.4.0.10 (2023-02-09)
+
+Pillow: Add missing enums from 9.1.0 (#9698)
+
 ## 9.4.0.9 (2023-02-09)
 
 Use `_typeshed.FileDescriptorOrPath` in stubs (#9695)
 
 ## 9.4.0.8 (2023-02-07)
 
 Enable flake8-pyi's Y037 (#9686)
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/DdsImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/DdsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/EpsImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/EpsImagePlugin.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from .ImageFile import ImageFile
 
 split: Any
 field: Any
 gs_windows_binary: Any
 
 def has_ghostscript(): ...
-def Ghostscript(tile, size, fp, scale: int = ..., transparency: bool = ...): ...
+def Ghostscript(tile, size, fp, scale: int = 1, transparency: bool = False): ...
 
 class PSFile:
     fp: Any
     char: Any
     def __init__(self, fp) -> None: ...
-    def seek(self, offset, whence=...) -> None: ...
+    def seek(self, offset, whence=0) -> None: ...
     def readline(self): ...
 
 class EpsImageFile(ImageFile):
     format: ClassVar[Literal["EPS"]]
     format_description: ClassVar[str]
     mode_map: Any
     im: Any
     mode: Any
     tile: Any
-    def load(self, scale: int = ..., transparency: bool = ...) -> None: ...
+    def load(self, scale: int = 1, transparency: bool = False) -> None: ...
     def load_seek(self, *args, **kwargs) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ExifTags.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ExifTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/FpxImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/FpxImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/GifImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/GifImagePlugin.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     im: Any
     def seek(self, frame) -> None: ...
     def tell(self): ...
 
 RAWMODE: Any
 
 def get_interlace(im): ...
-def getheader(im, palette: Incomplete | None = ..., info: Incomplete | None = ...): ...
-def getdata(im, offset=..., **params): ...
+def getheader(im, palette: Incomplete | None = None, info: Incomplete | None = None): ...
+def getdata(im, offset=(0, 0), **params): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/IcnsImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/IcnsImagePlugin.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     SIZES: Any
     dct: Any
     fobj: Any
     def __init__(self, fobj) -> None: ...
     def itersizes(self): ...
     def bestsize(self): ...
     def dataforsize(self, size): ...
-    def getimage(self, size: Incomplete | None = ...): ...
+    def getimage(self, size: Incomplete | None = None): ...
 
 class IcnsImageFile(ImageFile):
     format: ClassVar[Literal["ICNS"]]
     format_description: ClassVar[str]
     @property
     def size(self): ...
     @size.setter
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/IcoImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/IcoImagePlugin.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 class IcoFile:
     buf: Any
     entry: Any
     nb_items: Any
     def __init__(self, buf): ...
     def sizes(self): ...
-    def getentryindex(self, size, bpp: bool = ...): ...
-    def getimage(self, size, bpp: bool = ...): ...
+    def getentryindex(self, size, bpp: bool = False): ...
+    def getimage(self, size, bpp: bool = False): ...
     def frame(self, idx): ...
 
 class IcoImageFile(ImageFile):
     format: ClassVar[Literal["ICO"]]
     format_description: ClassVar[str]
     @property
     def size(self): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/Image.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/Image.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from _typeshed import Incomplete, Self, SupportsRead, SupportsWrite
+from _typeshed import Incomplete, SupportsRead, SupportsWrite, Unused
 from collections.abc import Callable, Iterable, Iterator, MutableMapping, Sequence
 from enum import IntEnum
 from pathlib import Path
 from typing import Any, ClassVar, Protocol, SupportsBytes
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import Literal, Self, TypeAlias
 
 from PIL.PyAccess import PyAccess
 
 from ._imaging import (
     DEFAULT_STRATEGY as DEFAULT_STRATEGY,
     FILTERED as FILTERED,
     FIXED as FIXED,
@@ -38,17 +38,17 @@
 CONTAINER: Literal[2]  # deprecated
 
 class DecompressionBombWarning(RuntimeWarning): ...
 class DecompressionBombError(Exception): ...
 
 MAX_IMAGE_PIXELS: int | None
 
-LINEAR: Literal[2]  # deprecated
-CUBIC: Literal[3]  # deprecated
-ANTIALIAS: Literal[1]  # deprecated
+LINEAR: Literal[Resampling.BILINEAR]  # deprecated
+CUBIC: Literal[Resampling.BICUBIC]  # deprecated
+ANTIALIAS: Literal[Resampling.LANCZOS]  # deprecated
 
 class Transpose(IntEnum):
     FLIP_LEFT_RIGHT: Literal[0]
     FLIP_TOP_BOTTOM: Literal[1]
     ROTATE_90: Literal[2]
     ROTATE_180: Literal[3]
     ROTATE_270: Literal[4]
@@ -167,132 +167,132 @@
     encoderconfig: tuple[Incomplete, ...]
     @property
     def width(self) -> int: ...
     @property
     def height(self) -> int: ...
     @property
     def size(self) -> tuple[int, int]: ...
-    def __enter__(self: Self) -> Self: ...
-    def __exit__(self, *args: object) -> None: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, *args: Unused) -> None: ...
     def close(self) -> None: ...
     def __eq__(self, other: object) -> bool: ...
     def __getstate__(self) -> _ImageState: ...
     def __setstate__(self, state: _ImageState) -> None: ...
-    def tobytes(self, encoder_name: str = ..., *args) -> bytes: ...
-    def tobitmap(self, name: str = ...) -> bytes: ...
-    def frombytes(self, data: bytes, decoder_name: str = ..., *args) -> None: ...
+    def tobytes(self, encoder_name: str = "raw", *args) -> bytes: ...
+    def tobitmap(self, name: str = "image") -> bytes: ...
+    def frombytes(self, data: bytes, decoder_name: str = "raw", *args) -> None: ...
     def load(self) -> None: ...
     def verify(self) -> None: ...
     def convert(
         self,
-        mode: _Mode | None = ...,
-        matrix: _ConversionMatrix | None = ...,
-        dither: int | None = ...,
+        mode: _Mode | None = None,
+        matrix: _ConversionMatrix | None = None,
+        dither: int | None = None,
         palette: Palette | Literal[0, 1] = ...,
-        colors: int = ...,
+        colors: int = 256,
     ) -> Image: ...
     def quantize(
         self,
-        colors: int = ...,
-        method: Literal[0, 1, 2, 3] | None = ...,
-        kmeans: int = ...,
-        palette: Image | None = ...,
+        colors: int = 256,
+        method: Quantize | Literal[0, 1, 2, 3] | None = None,
+        kmeans: int = 0,
+        palette: Image | None = None,
         dither: int = ...,
     ) -> Image: ...
     def copy(self) -> Image: ...
     __copy__ = copy
-    def crop(self, box: _Box | None = ...) -> Image: ...
+    def crop(self, box: _Box | None = None) -> Image: ...
     def draft(self, mode: _Mode, size: _Size) -> None: ...
     def filter(self, filter: Filter | Callable[[], Filter]) -> Image: ...
     def getbands(self) -> tuple[str, ...]: ...
     def getbbox(self) -> tuple[int, int, int, int] | None: ...
-    def getcolors(self, maxcolors: int = ...) -> list[tuple[int, int]]: ...
-    def getdata(self, band: int | None = ...): ...
+    def getcolors(self, maxcolors: int = 256) -> list[tuple[int, int]]: ...
+    def getdata(self, band: int | None = None): ...
     def getextrema(self): ...
     def getexif(self) -> Exif: ...
     def get_child_images(self) -> list[Image]: ...
     def getim(self): ...
-    def getpalette(self, rawmode: str | None = ...) -> list[int] | None: ...
+    def getpalette(self, rawmode: str | None = "RGB") -> list[int] | None: ...
     def getpixel(self, xy: tuple[int, int]): ...
     def getprojection(self) -> tuple[list[int], list[int]]: ...
-    def histogram(self, mask: Image | None = ..., extrema: tuple[int, int] | tuple[float, float] | None = ...) -> list[int]: ...
-    def entropy(self, mask: Image | None = ..., extrema: tuple[int, int] | tuple[float, float] | None = ...) -> float: ...
-    def paste(self, im: Image | _Color, box: tuple[int, int] | _Box | None = ..., mask: Image | None = ...) -> None: ...
-    def alpha_composite(self, im: Image, dest: tuple[int, int] = ..., source: tuple[int, int] = ...) -> None: ...
-    def point(self, lut, mode: _Mode | None = ...) -> Image: ...
+    def histogram(self, mask: Image | None = None, extrema: tuple[int, int] | tuple[float, float] | None = None) -> list[int]: ...
+    def entropy(self, mask: Image | None = None, extrema: tuple[int, int] | tuple[float, float] | None = None) -> float: ...
+    def paste(self, im: Image | _Color, box: tuple[int, int] | _Box | None = None, mask: Image | None = None) -> None: ...
+    def alpha_composite(self, im: Image, dest: tuple[int, int] = (0, 0), source: tuple[int, int] = (0, 0)) -> None: ...
+    def point(self, lut, mode: _Mode | None = None) -> Image: ...
     def putalpha(self, alpha: Image | int) -> None: ...
-    def putdata(self, data: Sequence[int], scale: float = ..., offset: float = ...) -> None: ...
-    def putpalette(self, data: ImagePalette | bytes | Iterable[int] | SupportsBytes, rawmode: _Mode | None = ...) -> None: ...
+    def putdata(self, data: Sequence[int], scale: float = 1.0, offset: float = 0.0) -> None: ...
+    def putpalette(self, data: ImagePalette | bytes | Iterable[int] | SupportsBytes, rawmode: _Mode | None = "RGB") -> None: ...
     def putpixel(self, xy: tuple[int, int], value: _Color | list[float]) -> None: ...
-    def remap_palette(self, dest_map: Iterable[int], source_palette: Sequence[int] | None = ...) -> Image: ...
+    def remap_palette(self, dest_map: Iterable[int], source_palette: Sequence[int] | None = None) -> Image: ...
     def resize(
         self,
         size: tuple[int, int],
-        resample: Resampling | _Resample | None = ...,
-        box: tuple[float, float, float, float] | None = ...,
-        reducing_gap: float | None = ...,
+        resample: Resampling | _Resample | None = None,
+        box: tuple[float, float, float, float] | None = None,
+        reducing_gap: float | None = None,
     ) -> Image: ...
-    def reduce(self, factor: int | tuple[int, int] | list[int], box: _Box | None = ...) -> Image: ...
+    def reduce(self, factor: int | tuple[int, int] | list[int], box: _Box | None = None) -> Image: ...
     def rotate(
         self,
         angle: float,
         resample: Resampling | _Resample = ...,
         expand: bool = ...,
-        center: tuple[float, float] | None = ...,
-        translate: tuple[float, float] | None = ...,
-        fillcolor: _Color | None = ...,
+        center: tuple[float, float] | None = None,
+        translate: tuple[float, float] | None = None,
+        fillcolor: _Color | None = None,
     ) -> Image: ...
     def save(
         self,
         fp: str | bytes | Path | _Writeable,
-        format: str | None = ...,
+        format: str | None = None,
         *,
         save_all: bool = ...,
         bitmap_format: Literal["bmp", "png"] = ...,  # for ICO files
         optimize: bool = ...,
         **params: Any,
     ) -> None: ...
     def seek(self, frame: int) -> None: ...
-    def show(self, title: str | None = ...) -> None: ...
+    def show(self, title: str | None = None) -> None: ...
     def split(self) -> tuple[Image, ...]: ...
     def getchannel(self, channel: int | str) -> Image: ...
     def tell(self) -> int: ...
-    def thumbnail(self, size: tuple[int, int], resample: Resampling | _Resample = ..., reducing_gap: float = ...) -> None: ...
+    def thumbnail(self, size: tuple[int, int], resample: Resampling | _Resample = ..., reducing_gap: float = 2.0) -> None: ...
     def transform(
         self,
         size: _Size,
         method: Transform | Literal[0, 1, 2, 3, 4],
-        data=...,
+        data=None,
         resample: Resampling | _Resample = ...,
-        fill: int = ...,
-        fillcolor: _Color | int | None = ...,
+        fill: int = 1,
+        fillcolor: _Color | int | None = None,
     ) -> Image: ...
     def transpose(self, method: Transpose | Literal[0, 1, 2, 3, 4, 5, 6]) -> Image: ...
     def effect_spread(self, distance: int) -> Image: ...
     def toqimage(self): ...
     def toqpixmap(self): ...
 
 class ImagePointHandler: ...
 class ImageTransformHandler: ...
 
-def new(mode: _Mode, size: tuple[int, int], color: _Color = ...) -> Image: ...
-def frombytes(mode: _Mode, size: tuple[int, int], data, decoder_name: str = ..., *args) -> Image: ...
-def frombuffer(mode: _Mode, size: tuple[int, int], data, decoder_name: str = ..., *args) -> Image: ...
-def fromarray(obj, mode: _Mode | None = ...) -> Image: ...
+def new(mode: _Mode, size: tuple[int, int], color: _Color = 0) -> Image: ...
+def frombytes(mode: _Mode, size: tuple[int, int], data, decoder_name: str = "raw", *args) -> Image: ...
+def frombuffer(mode: _Mode, size: tuple[int, int], data, decoder_name: str = "raw", *args) -> Image: ...
+def fromarray(obj, mode: _Mode | None = None) -> Image: ...
 def fromqimage(im) -> Image: ...
 def fromqpixmap(im) -> Image: ...
 def open(
-    fp: str | bytes | Path | SupportsRead[bytes], mode: Literal["r"] = ..., formats: list[str] | tuple[str, ...] | None = ...
+    fp: str | bytes | Path | SupportsRead[bytes], mode: Literal["r"] = "r", formats: list[str] | tuple[str, ...] | None = None
 ) -> Image: ...
 def alpha_composite(im1: Image, im2: Image) -> Image: ...
 def blend(im1: Image, im2: Image, alpha: float) -> Image: ...
 def composite(image1: Image, image2: Image, mask: Image) -> Image: ...
 def eval(image: Image, *args) -> Image: ...
 def merge(mode: _Mode, bands: Sequence[Image]) -> Image: ...
-def register_open(id: str, factory, accept=...) -> None: ...
+def register_open(id: str, factory, accept=None) -> None: ...
 def register_mime(id: str, mimetype: str) -> None: ...
 def register_save(id: str, driver) -> None: ...
 def register_save_all(id: str, driver) -> None: ...
 def register_extension(id: str, extension: str) -> None: ...
 def register_extensions(id: str, extensions: Iterable[str]) -> None: ...
 def registered_extensions() -> dict[str, str]: ...
 def register_decoder(name: str, decoder) -> None: ...
@@ -300,15 +300,15 @@
 def effect_mandelbrot(size: tuple[int, int], extent: tuple[float, float, float, float], quality: int) -> Image: ...
 def effect_noise(size: tuple[int, int], sigma: float) -> Image: ...
 def linear_gradient(mode: _Mode) -> Image: ...
 def radial_gradient(mode: _Mode) -> Image: ...
 
 class Exif(MutableMapping[int, Any]):
     def load(self, data: bytes) -> None: ...
-    def tobytes(self, offset: int = ...) -> bytes: ...
+    def tobytes(self, offset: int = 8) -> bytes: ...
     def get_ifd(self, tag: int): ...
     def hide_offsets(self) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, tag: int) -> Any: ...
     def __contains__(self, tag: object) -> bool: ...
     def __setitem__(self, tag: int, value: Any) -> None: ...
     def __delitem__(self, tag: int) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageChops.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageChops.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 def darker(image1: Image, image2: Image) -> Image: ...
 def difference(image1: Image, image2: Image) -> Image: ...
 def multiply(image1: Image, image2: Image) -> Image: ...
 def screen(image1: Image, image2: Image) -> Image: ...
 def soft_light(image1: Image, image2: Image) -> Image: ...
 def hard_light(image1: Image, image2: Image) -> Image: ...
 def overlay(image1: Image, image2: Image) -> Image: ...
-def add(image1: Image, image2: Image, scale: float = ..., offset: int = ...) -> Image: ...
-def subtract(image1: Image, image2: Image, scale: float = ..., offset: int = ...) -> Image: ...
+def add(image1: Image, image2: Image, scale: float = 1.0, offset: int = 0) -> Image: ...
+def subtract(image1: Image, image2: Image, scale: float = 1.0, offset: int = 0) -> Image: ...
 def add_modulo(image1: Image, image2: Image) -> Image: ...
 def subtract_modulo(image1: Image, image2: Image) -> Image: ...
 def logical_and(image1: Image, image2: Image) -> Image: ...
 def logical_or(image1: Image, image2: Image) -> Image: ...
 def logical_xor(image1: Image, image2: Image) -> Image: ...
 def blend(image1: Image, image2: Image, alpha: float) -> Image: ...
 def composite(image1: Image, image2: Image, mask: Image) -> Image: ...
-def offset(image: Image, xoffset: int, yoffset: int | None = ...) -> Image: ...
+def offset(image: Image, xoffset: int, yoffset: int | None = None) -> Image: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageCms.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageCms.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 from _typeshed import Incomplete
+from enum import IntEnum
 from typing import Any
+from typing_extensions import Literal
 
 from .Image import ImagePointHandler
 
 DESCRIPTION: str
 VERSION: str
 core: Any
-INTENT_PERCEPTUAL: int
-INTENT_RELATIVE_COLORIMETRIC: int
-INTENT_SATURATION: int
-INTENT_ABSOLUTE_COLORIMETRIC: int
-DIRECTION_INPUT: int
-DIRECTION_OUTPUT: int
-DIRECTION_PROOF: int
+
+class Intent(IntEnum):
+    PERCEPTUAL: int
+    RELATIVE_COLORIMETRIC: int
+    SATURATION: int
+    ABSOLUTE_COLORIMETRIC: int
+
+INTENT_PERCEPTUAL: Literal[Intent.PERCEPTUAL]
+INTENT_RELATIVE_COLORIMETRIC: Literal[Intent.RELATIVE_COLORIMETRIC]
+INTENT_SATURATION: Literal[Intent.SATURATION]
+INTENT_ABSOLUTE_COLORIMETRIC: Literal[Intent.ABSOLUTE_COLORIMETRIC]
+
+class Direction(IntEnum):
+    INPUT: int
+    OUTPUT: int
+    PROOF: int
+
+DIRECTION_INPUT: Literal[Direction.INPUT]
+DIRECTION_OUTPUT: Literal[Direction.OUTPUT]
+DIRECTION_PROOF: Literal[Direction.PROOF]
+
 FLAGS: Any
 
 class ImageCmsProfile:
     def __init__(self, profile) -> None: ...
     def tobytes(self): ...
 
 class ImageCmsTransform(ImagePointHandler):
@@ -27,46 +43,46 @@
     def __init__(
         self,
         input,
         output,
         input_mode,
         output_mode,
         intent=...,
-        proof: Incomplete | None = ...,
+        proof: Incomplete | None = None,
         proof_intent=...,
-        flags: int = ...,
+        flags: int = 0,
     ) -> None: ...
     def point(self, im): ...
-    def apply(self, im, imOut: Incomplete | None = ...): ...
+    def apply(self, im, imOut: Incomplete | None = None): ...
     def apply_in_place(self, im): ...
 
-def get_display_profile(handle: Incomplete | None = ...): ...
+def get_display_profile(handle: Incomplete | None = None): ...
 
 class PyCMSError(Exception): ...
 
 def profileToProfile(
     im,
     inputProfile,
     outputProfile,
     renderingIntent=...,
-    outputMode: Incomplete | None = ...,
-    inPlace: bool = ...,
-    flags: int = ...,
+    outputMode: Incomplete | None = None,
+    inPlace: bool = False,
+    flags: int = 0,
 ): ...
 def getOpenProfile(profileFilename): ...
-def buildTransform(inputProfile, outputProfile, inMode, outMode, renderingIntent=..., flags: int = ...): ...
+def buildTransform(inputProfile, outputProfile, inMode, outMode, renderingIntent=..., flags: int = 0): ...
 def buildProofTransform(
-    inputProfile, outputProfile, proofProfile, inMode, outMode, renderingIntent=..., proofRenderingIntent=..., flags=...
+    inputProfile, outputProfile, proofProfile, inMode, outMode, renderingIntent=..., proofRenderingIntent=..., flags=16384
 ): ...
 
 buildTransformFromOpenProfiles = buildTransform
 buildProofTransformFromOpenProfiles = buildProofTransform
 
-def applyTransform(im, transform, inPlace: bool = ...): ...
-def createProfile(colorSpace, colorTemp: int = ...): ...
+def applyTransform(im, transform, inPlace: bool = False): ...
+def createProfile(colorSpace, colorTemp: int = -1): ...
 def getProfileName(profile): ...
 def getProfileInfo(profile): ...
 def getProfileCopyright(profile): ...
 def getProfileManufacturer(profile): ...
 def getProfileModel(profile): ...
 def getProfileDescription(profile): ...
 def getDefaultIntent(profile): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageDraw.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageDraw.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -7,150 +7,152 @@
 from .ImageColor import _Ink
 from .ImageFont import _Font
 
 _XY: TypeAlias = Sequence[float | tuple[float, float]]
 _Outline: TypeAlias = Any
 
 class ImageDraw:
-    def __init__(self, im: Image, mode: str | None = ...) -> None: ...
+    def __init__(self, im: Image, mode: str | None = None) -> None: ...
     def getfont(self): ...
-    def arc(self, xy: _XY, start: float, end: float, fill: _Ink | None = ..., width: float = ...) -> None: ...
-    def bitmap(self, xy: _XY, bitmap: Image, fill: _Ink | None = ...) -> None: ...
+    def arc(self, xy: _XY, start: float, end: float, fill: _Ink | None = None, width: float = 1) -> None: ...
+    def bitmap(self, xy: _XY, bitmap: Image, fill: _Ink | None = None) -> None: ...
     def chord(
-        self, xy: _XY, start: float, end: float, fill: _Ink | None = ..., outline: _Ink | None = ..., width: float = ...
+        self, xy: _XY, start: float, end: float, fill: _Ink | None = None, outline: _Ink | None = None, width: float = 1
     ) -> None: ...
-    def ellipse(self, xy: _XY, fill: _Ink | None = ..., outline: _Ink | None = ..., width: float = ...) -> None: ...
-    def line(self, xy: _XY, fill: _Ink | None = ..., width: float = ..., joint: Literal["curve"] | None = ...) -> None: ...
-    def shape(self, shape: _Outline, fill: _Ink | None = ..., outline: _Ink | None = ...) -> None: ...
+    def ellipse(self, xy: _XY, fill: _Ink | None = None, outline: _Ink | None = None, width: float = 1) -> None: ...
+    def line(self, xy: _XY, fill: _Ink | None = None, width: float = 0, joint: Literal["curve"] | None = None) -> None: ...
+    def shape(self, shape: _Outline, fill: _Ink | None = None, outline: _Ink | None = None) -> None: ...
     def pieslice(
         self,
         xy: tuple[tuple[float, float], tuple[float, float]],
         start: float,
         end: float,
-        fill: _Ink | None = ...,
-        outline: _Ink | None = ...,
-        width: float = ...,
+        fill: _Ink | None = None,
+        outline: _Ink | None = None,
+        width: float = 1,
     ) -> None: ...
-    def point(self, xy: _XY, fill: _Ink | None = ...) -> None: ...
-    def polygon(self, xy: _XY, fill: _Ink | None = ..., outline: _Ink | None = ..., width: float = ...) -> None: ...
+    def point(self, xy: _XY, fill: _Ink | None = None) -> None: ...
+    def polygon(self, xy: _XY, fill: _Ink | None = None, outline: _Ink | None = None, width: float = 1) -> None: ...
     def regular_polygon(
         self,
         bounding_circle: tuple[float, float] | tuple[float, float, float] | list[int],
         n_sides: int,
-        rotation: float = ...,
-        fill: _Ink | None = ...,
-        outline: _Ink | None = ...,
+        rotation: float = 0,
+        fill: _Ink | None = None,
+        outline: _Ink | None = None,
     ) -> None: ...
     def rectangle(
         self,
         xy: tuple[float, float, float, float] | tuple[tuple[float, float], tuple[float, float]],
-        fill: _Ink | None = ...,
-        outline: _Ink | None = ...,
-        width: float = ...,
+        fill: _Ink | None = None,
+        outline: _Ink | None = None,
+        width: float = 1,
     ) -> None: ...
     def rounded_rectangle(
         self,
         xy: tuple[float, float, float, float] | tuple[tuple[float, float], tuple[float, float]],
-        radius: float = ...,
-        fill: _Ink | None = ...,
-        outline: _Ink | None = ...,
-        width: float = ...,
+        radius: float = 0,
+        fill: _Ink | None = None,
+        outline: _Ink | None = None,
+        width: float = 1,
+        *,
+        corners: tuple[bool, bool, bool, bool] | None = None,
     ) -> None: ...
     def text(
         self,
         xy: tuple[float, float],
         text: str | bytes,
-        fill: _Ink | None = ...,
-        font: _Font | None = ...,
-        anchor: str | None = ...,
-        spacing: float = ...,
-        align: Literal["left", "center", "right"] = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Sequence[str] | None = ...,
-        language: str | None = ...,
-        stroke_width: int = ...,
-        stroke_fill: _Ink | None = ...,
-        embedded_color: bool = ...,
+        fill: _Ink | None = None,
+        font: _Font | None = None,
+        anchor: str | None = None,
+        spacing: float = 4,
+        align: Literal["left", "center", "right"] = "left",
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Sequence[str] | None = None,
+        language: str | None = None,
+        stroke_width: int = 0,
+        stroke_fill: _Ink | None = None,
+        embedded_color: bool = False,
         *args,
         **kwargs,
     ) -> None: ...
     def multiline_text(
         self,
         xy: tuple[float, float],
         text: str | bytes,
-        fill: _Ink | None = ...,
-        font: _Font | None = ...,
-        anchor: str | None = ...,
-        spacing: float = ...,
-        align: Literal["left", "center", "right"] = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Incomplete | None = ...,
-        language: str | None = ...,
-        stroke_width: int = ...,
-        stroke_fill: _Ink | None = ...,
-        embedded_color: bool = ...,
+        fill: _Ink | None = None,
+        font: _Font | None = None,
+        anchor: str | None = None,
+        spacing: float = 4,
+        align: Literal["left", "center", "right"] = "left",
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Incomplete | None = None,
+        language: str | None = None,
+        stroke_width: int = 0,
+        stroke_fill: _Ink | None = None,
+        embedded_color: bool = False,
     ) -> None: ...
     def textsize(
         self,
         text: str | bytes,
-        font: _Font | None = ...,
-        spacing: float = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Sequence[str] | None = ...,
-        language: str | None = ...,
-        stroke_width: int = ...,
+        font: _Font | None = None,
+        spacing: float = 4,
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Sequence[str] | None = None,
+        language: str | None = None,
+        stroke_width: int = 0,
     ) -> tuple[int, int]: ...
     def multiline_textsize(
         self,
         text: str | bytes,
-        font: _Font | None = ...,
-        spacing: float = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Sequence[str] | None = ...,
-        language: str | None = ...,
-        stroke_width: int = ...,
+        font: _Font | None = None,
+        spacing: float = 4,
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Sequence[str] | None = None,
+        language: str | None = None,
+        stroke_width: int = 0,
     ) -> tuple[int, int]: ...
     def textlength(
         self,
         text: str | bytes,
-        font: _Font | None = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Sequence[str] | None = ...,
-        language: str | None = ...,
-        embedded_color: bool = ...,
+        font: _Font | None = None,
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Sequence[str] | None = None,
+        language: str | None = None,
+        embedded_color: bool = False,
     ) -> float: ...
     def textbbox(
         self,
         xy: tuple[float, float],
         text: str | bytes,
-        font: _Font | None = ...,
-        anchor: str | None = ...,
-        spacing: float = ...,
-        align: Literal["left", "center", "right"] = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Incomplete | None = ...,
-        language: str | None = ...,
-        stroke_width: int = ...,
-        embedded_color: bool = ...,
+        font: _Font | None = None,
+        anchor: str | None = None,
+        spacing: float = 4,
+        align: Literal["left", "center", "right"] = "left",
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Incomplete | None = None,
+        language: str | None = None,
+        stroke_width: int = 0,
+        embedded_color: bool = False,
     ) -> tuple[int, int, int, int]: ...
     def multiline_textbbox(
         self,
         xy: tuple[float, float],
         text: str | bytes,
-        font: _Font | None = ...,
-        anchor: str | None = ...,
-        spacing: float = ...,
-        align: Literal["left", "center", "right"] = ...,
-        direction: Literal["rtl", "ltr", "ttb"] | None = ...,
-        features: Incomplete | None = ...,
-        language: str | None = ...,
-        stroke_width: int = ...,
-        embedded_color: bool = ...,
+        font: _Font | None = None,
+        anchor: str | None = None,
+        spacing: float = 4,
+        align: Literal["left", "center", "right"] = "left",
+        direction: Literal["rtl", "ltr", "ttb"] | None = None,
+        features: Incomplete | None = None,
+        language: str | None = None,
+        stroke_width: int = 0,
+        embedded_color: bool = False,
     ) -> tuple[int, int, int, int]: ...
 
-def Draw(im: Image, mode: str | None = ...) -> ImageDraw: ...
+def Draw(im: Image, mode: str | None = None) -> ImageDraw: ...
 def Outline() -> _Outline: ...
 @overload
-def getdraw(im: None = ..., hints: Container[Literal["nicest"]] | None = ...) -> tuple[None, Any]: ...
+def getdraw(im: None = None, hints: Container[Literal["nicest"]] | None = None) -> tuple[None, Any]: ...
 @overload
-def getdraw(im: Image, hints: Container[Literal["nicest"]] | None = ...) -> tuple[Image, Any]: ...
-def floodfill(image: Image, xy: tuple[float, float], value, border=..., thresh: float = ...) -> None: ...
+def getdraw(im: Image, hints: Container[Literal["nicest"]] | None = None) -> tuple[Image, Any]: ...
+def floodfill(image: Image, xy: tuple[float, float], value, border=None, thresh: float = 0) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageDraw2.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageDraw2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from _typeshed import Incomplete
 from typing import Any
 
 class Pen:
     color: Any
     width: Any
-    def __init__(self, color, width: int = ..., opacity: int = ...) -> None: ...
+    def __init__(self, color, width: int = 1, opacity: int = 255) -> None: ...
 
 class Brush:
     color: Any
-    def __init__(self, color, opacity: int = ...) -> None: ...
+    def __init__(self, color, opacity: int = 255) -> None: ...
 
 class Font:
     color: Any
     font: Any
-    def __init__(self, color, file, size: int = ...) -> None: ...
+    def __init__(self, color, file, size: int = 12) -> None: ...
 
 class Draw:
     draw: Any
     image: Any
     transform: Any
-    def __init__(self, image, size: Incomplete | None = ..., color: Incomplete | None = ...) -> None: ...
+    def __init__(self, image, size: Incomplete | None = None, color: Incomplete | None = None) -> None: ...
     def flush(self): ...
-    def render(self, op, xy, pen, brush: Incomplete | None = ...) -> None: ...
+    def render(self, op, xy, pen, brush: Incomplete | None = None) -> None: ...
     def settransform(self, offset) -> None: ...
     def arc(self, xy, start, end, *options) -> None: ...
     def chord(self, xy, start, end, *options) -> None: ...
     def ellipse(self, xy, *options) -> None: ...
     def line(self, xy, *options) -> None: ...
     def pieslice(self, xy, start, end, *options) -> None: ...
     def polygon(self, xy, *options) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageEnhance.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageEnhance.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageFile.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageFile.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from _typeshed import Incomplete, Self
+from _typeshed import Incomplete, Unused
 from typing import Any, NoReturn
+from typing_extensions import Self
 
 from .Image import Image
 
 MAXBLOCK: int
 SAFEBLOCK: Any
 LOAD_TRUNCATED_IMAGES: bool
 ERRORS: Any
@@ -14,15 +15,15 @@
     custom_mimetype: Any
     tile: list[Incomplete] | None
     readonly: int
     decoderconfig: Any
     decodermaxblock: Any
     fp: Any
     filename: Any
-    def __init__(self, fp: Incomplete | None = ..., filename: Incomplete | None = ...) -> None: ...
+    def __init__(self, fp: Incomplete | None = None, filename: Incomplete | None = None) -> None: ...
     def get_format_mimetype(self): ...
     def verify(self) -> None: ...
     map: Any
     im: Any
     def load(self): ...
     def load_prepare(self) -> None: ...
     def load_end(self) -> None: ...
@@ -36,16 +37,16 @@
     data: Incomplete | None
     decoder: Incomplete | None
     offset: int
     finished: bool
     def reset(self) -> None: ...
     decode: Any
     def feed(self, data) -> None: ...
-    def __enter__(self: Self) -> Self: ...
-    def __exit__(self, *args: object) -> None: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, *args: Unused) -> None: ...
     def close(self) -> Image: ...
 
 class PyCodecState:
     xsize: int
     ysize: int
     xoff: int
     yoff: int
@@ -60,9 +61,9 @@
     args: Any
     def init(self, args) -> None: ...
     @property
     def pulls_fd(self): ...
     def decode(self, buffer) -> None: ...
     def cleanup(self) -> None: ...
     def setfd(self, fd) -> None: ...
-    def setimage(self, im, extents: Incomplete | None = ...) -> None: ...
-    def set_as_raw(self, data, rawmode: Incomplete | None = ...) -> None: ...
+    def setimage(self, im, extents: Incomplete | None = None) -> None: ...
+    def set_as_raw(self, data, rawmode: Incomplete | None = None) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageFilter.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageFilter.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from _typeshed import Incomplete, Self
+from _typeshed import Incomplete
 from collections.abc import Callable, Iterable, Sequence
 from typing import Any
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import Literal, Self, TypeAlias
 
 from .Image import Image
 
 _FilterArgs: TypeAlias = tuple[Sequence[int], int, int, Sequence[int]]
 
 # filter image parameters below are the C images, i.e. Image().im.
 
@@ -14,65 +14,65 @@
 
 class BuiltinFilter(MultibandFilter):
     def filter(self, image) -> Image: ...
 
 class Kernel(BuiltinFilter):
     name: str
     filterargs: _FilterArgs
-    def __init__(self, size: Sequence[int], kernel: Sequence[int], scale: Incomplete | None = ..., offset: int = ...) -> None: ...
+    def __init__(self, size: Sequence[int], kernel: Sequence[int], scale: Incomplete | None = None, offset: int = 0) -> None: ...
 
 class RankFilter(Filter):
     name: str
     size: int
     rank: int
     def __init__(self, size: int, rank: int) -> None: ...
     def filter(self, image) -> Image: ...
 
 class MedianFilter(RankFilter):
     name: str
     size: int
     rank: int
-    def __init__(self, size: int = ...) -> None: ...
+    def __init__(self, size: int = 3) -> None: ...
 
 class MinFilter(RankFilter):
     name: str
     size: int
     rank: int
-    def __init__(self, size: int = ...) -> None: ...
+    def __init__(self, size: int = 3) -> None: ...
 
 class MaxFilter(RankFilter):
     name: str
     size: int
     rank: int
-    def __init__(self, size: int = ...) -> None: ...
+    def __init__(self, size: int = 3) -> None: ...
 
 class ModeFilter(Filter):
     name: str
     size: int
-    def __init__(self, size: int = ...) -> None: ...
+    def __init__(self, size: int = 3) -> None: ...
     def filter(self, image) -> Image: ...
 
 class GaussianBlur(MultibandFilter):
     name: str
     radius: float
-    def __init__(self, radius: float = ...) -> None: ...
+    def __init__(self, radius: float = 2) -> None: ...
     def filter(self, image) -> Image: ...
 
 class BoxBlur(MultibandFilter):
     name: str
     radius: float
     def __init__(self, radius: float) -> None: ...
     def filter(self, image) -> Image: ...
 
 class UnsharpMask(MultibandFilter):
     name: str
     radius: float
     percent: int
     threshold: int
-    def __init__(self, radius: float = ..., percent: int = ..., threshold: int = ...) -> None: ...
+    def __init__(self, radius: float = 2, percent: int = 150, threshold: int = 3) -> None: ...
     def filter(self, image) -> Image: ...
 
 class BLUR(BuiltinFilter):
     name: str
     filterargs: _FilterArgs
 
 class CONTOUR(BuiltinFilter):
@@ -113,26 +113,24 @@
 
 class Color3DLUT(MultibandFilter):
     name: str
     size: list[int]
     channels: int
     mode: str | None
     table: Any
-    def __init__(
-        self, size: int | Iterable[int], table, channels: int = ..., target_mode: str | None = ..., **kwargs
-    ) -> None: ...
+    def __init__(self, size: int | Iterable[int], table, channels: int = 3, target_mode: str | None = None, **kwargs) -> None: ...
     @classmethod
     def generate(
-        cls: type[Self],
+        cls,
         size: int | tuple[int, int, int],
         callback: Callable[[float, float, float], Iterable[float]],
-        channels: int = ...,
-        target_mode: str | None = ...,
+        channels: int = 3,
+        target_mode: str | None = None,
     ) -> Self: ...
     def transform(
-        self: Self,
+        self,
         callback: Callable[..., Iterable[float]],
-        with_normals: bool = ...,
-        channels: Literal[3, 4] | None = ...,
-        target_mode: Incomplete | None = ...,
+        with_normals: bool = False,
+        channels: Literal[3, 4] | None = None,
+        target_mode: Incomplete | None = None,
     ) -> Self: ...
     def filter(self, image) -> Image: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageMath.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageMath.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from _typeshed import Incomplete
 from typing import Any
 
 class _Operand:
     im: Any
     def __init__(self, im) -> None: ...
-    def apply(self, op, im1, im2: Incomplete | None = ..., mode: Incomplete | None = ...): ...
+    def apply(self, op, im1, im2: Incomplete | None = None, mode: Incomplete | None = None): ...
     def __bool__(self) -> bool: ...
     def __abs__(self): ...
     def __pos__(self): ...
     def __neg__(self): ...
     def __add__(self, other): ...
     def __radd__(self, other): ...
     def __sub__(self, other): ...
@@ -43,8 +43,8 @@
 def imagemath_notequal(self, other): ...
 def imagemath_min(self, other): ...
 def imagemath_max(self, other): ...
 def imagemath_convert(self, mode): ...
 
 ops: Any
 
-def eval(expression, _dict=..., **kw): ...
+def eval(expression, _dict={}, **kw): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageMorph.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageMorph.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 LUT_SIZE: int
 ROTATION_MATRIX: list[int]
 MIRROR_MATRIX: list[int]
 
 class LutBuilder:
     patterns: list[str]
     lut: bytearray
-    def __init__(self, patterns: list[str] | None = ..., op_name: str | None = ...) -> None: ...
+    def __init__(self, patterns: list[str] | None = None, op_name: str | None = None) -> None: ...
     def add_patterns(self, patterns: list[str]) -> None: ...
     def build_default_lut(self) -> None: ...
     def get_lut(self) -> bytearray: ...
     def build_lut(self) -> bytearray: ...
 
 class MorphOp:
     lut: bytearray
-    def __init__(self, lut: bytearray | None = ..., op_name: str | None = ..., patterns: list[str] | None = ...) -> None: ...
+    def __init__(self, lut: bytearray | None = None, op_name: str | None = None, patterns: list[str] | None = None) -> None: ...
     def apply(self, image: Image) -> tuple[int, Image]: ...
     def match(self, image: Image) -> list[tuple[int, int]]: ...
     def get_on_pixels(self, image: Image) -> list[tuple[int, int]]: ...
     def load_lut(self, filename: StrOrBytesPath) -> None: ...
     def save_lut(self, filename: StrOrBytesPath) -> None: ...
     def set_lut(self, lut: bytearray) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageShow.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageShow.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from _typeshed import Incomplete
 from typing import Any
 from typing_extensions import Literal
 
-def register(viewer, order: int = ...) -> None: ...
-def show(image, title: Incomplete | None = ..., **options): ...
+def register(viewer, order: int = 1) -> None: ...
+def show(image, title: Incomplete | None = None, **options): ...
 
 class Viewer:
     def show(self, image, **options): ...
     format: Any
     options: Any
     def get_format(self, image): ...
     def get_command(self, file, **options) -> None: ...
     def save_image(self, image): ...
     def show_image(self, image, **options): ...
-    def show_file(self, path: Incomplete | None = ..., **options): ...
+    def show_file(self, path: Incomplete | None = None, **options): ...
 
 class WindowsViewer(Viewer):
     format: str
     options: Any
     def get_command(self, file, **options): ...
 
 class MacViewer(Viewer):
     format: str
     options: Any
     def get_command(self, file, **options): ...
-    def show_file(self, path: Incomplete | None = ..., **options): ...
+    def show_file(self, path: Incomplete | None = None, **options): ...
 
 class UnixViewer(Viewer):
     format: str
     options: Any
     def get_command(self, file, **options): ...
-    def show_file(self, path: Incomplete | None = ..., **options): ...
+    def show_file(self, path: Incomplete | None = None, **options): ...
 
 class XDGViewer(UnixViewer):
     def get_command_ex(self, file, **options) -> tuple[Literal["xdg-open"], Literal["xdg-open"]]: ...
 
 class DisplayViewer(UnixViewer):
-    def get_command_ex(self, file, title: str | None = ..., **options): ...
+    def get_command_ex(self, file, title: str | None = None, **options): ...
 
 class GmDisplayViewer(UnixViewer):
     def get_command_ex(self, file, **options): ...
 
 class EogViewer(UnixViewer):
     def get_command_ex(self, file, **options): ...
 
 class XVViewer(UnixViewer):
-    def get_command_ex(self, file, title: Incomplete | None = ..., **options): ...
+    def get_command_ex(self, file, title: Incomplete | None = None, **options): ...
 
 class IPythonViewer(Viewer):
     def show_image(self, image, **options): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/ImageWin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/ImageWin.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,29 @@
     def __init__(self, wnd) -> None: ...
     def __int__(self) -> int: ...
 
 class Dib:
     image: Any
     mode: Any
     size: Any
-    def __init__(self, image, size: Incomplete | None = ...) -> None: ...
+    def __init__(self, image, size: Incomplete | None = None) -> None: ...
     def expose(self, handle): ...
-    def draw(self, handle, dst, src: Incomplete | None = ...): ...
+    def draw(self, handle, dst, src: Incomplete | None = None): ...
     def query_palette(self, handle): ...
-    def paste(self, im, box: Incomplete | None = ...) -> None: ...
+    def paste(self, im, box: Incomplete | None = None) -> None: ...
     def frombytes(self, buffer): ...
     def tobytes(self): ...
 
 class Window:
     hwnd: Any
-    def __init__(self, title: str = ..., width: Incomplete | None = ..., height: Incomplete | None = ...) -> None: ...
+    def __init__(self, title: str = "PIL", width: Incomplete | None = None, height: Incomplete | None = None) -> None: ...
     def ui_handle_clear(self, dc, x0, y0, x1, y1) -> None: ...
     def ui_handle_damage(self, x0, y0, x1, y1) -> None: ...
     def ui_handle_destroy(self) -> None: ...
     def ui_handle_repair(self, dc, x0, y0, x1, y1) -> None: ...
     def ui_handle_resize(self, width, height) -> None: ...
     def mainloop(self) -> None: ...
 
 class ImageWindow(Window):
     image: Any
-    def __init__(self, image, title: str = ...) -> None: ...
+    def __init__(self, image, title: str = "PIL") -> None: ...
     def ui_handle_repair(self, dc, x0, y0, x1, y1) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/JpegImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/JpegImagePlugin.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 RAWMODE: Any
 zigzag_index: Any
 samplings: Any
 
 def convert_dict_qtables(qtables): ...
 def get_sampling(im): ...
-def jpeg_factory(fp: Incomplete | None = ..., filename: Incomplete | None = ...): ...
+def jpeg_factory(fp: Incomplete | None = None, filename: Incomplete | None = None): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/MicImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/MicImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/PSDraw.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/PSDraw.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from _typeshed import SupportsWrite
+from _typeshed import SupportsWrite, Unused
 
 from .Image import Image
 
 class PSDraw:
     fp: SupportsWrite[bytes]
-    def __init__(self, fp: SupportsWrite[bytes] | None = ...) -> None: ...
+    def __init__(self, fp: SupportsWrite[bytes] | None = None) -> None: ...
     isofont: dict[bytes, int]
-    def begin_document(self, id: object | None = ...) -> None: ...
+    def begin_document(self, id: Unused = None) -> None: ...
     def end_document(self) -> None: ...
     def setfont(self, font: str, size: int) -> None: ...
     def line(self, xy0: tuple[int, int], xy1: tuple[int, int]) -> None: ...
     def rectangle(self, box: tuple[int, int, int, int]) -> None: ...
     def text(self, xy: tuple[int, int], text: str) -> None: ...
-    def image(self, box: tuple[int, int, int, int], im: Image, dpi: float | None = ...) -> None: ...
+    def image(self, box: tuple[int, int, int, int], im: Image, dpi: float | None = None) -> None: ...
 
 EDROFF_PS: bytes
 VDI_PS: bytes
 ERROR_PS: bytes
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/PdfParser.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/PdfParser.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import collections
 from _typeshed import Incomplete
+from types import TracebackType
 from typing import Any
+from typing_extensions import Literal
 
 def encode_text(s: str) -> bytes: ...
 
 PDFDocEncoding: dict[int, str]
 
 def decode_text(b: bytes) -> str: ...
 
@@ -84,39 +86,41 @@
     orig_pages: Any
     pages_ref: Any
     last_xref_section_offset: Any
     trailer_dict: Any
     xref_table: Any
     def __init__(
         self,
-        filename: Incomplete | None = ...,
-        f: Incomplete | None = ...,
-        buf: Incomplete | None = ...,
-        start_offset: int = ...,
-        mode: str = ...,
+        filename: Incomplete | None = None,
+        f: Incomplete | None = None,
+        buf: Incomplete | None = None,
+        start_offset: int = 0,
+        mode: str = "rb",
     ) -> None: ...
     def __enter__(self): ...
-    def __exit__(self, exc_type, exc_value, traceback): ...
+    def __exit__(
+        self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: TracebackType | None
+    ) -> Literal[False]: ...
     def start_writing(self) -> None: ...
     def close_buf(self) -> None: ...
     def close(self) -> None: ...
     def seek_end(self) -> None: ...
     def write_header(self) -> None: ...
     def write_comment(self, s) -> None: ...
     def write_catalog(self): ...
     def rewrite_pages(self) -> None: ...
-    def write_xref_and_trailer(self, new_root_ref: Incomplete | None = ...) -> None: ...
+    def write_xref_and_trailer(self, new_root_ref: Incomplete | None = None) -> None: ...
     def write_page(self, ref, *objs, **dict_obj): ...
     def write_obj(self, ref, *objs, **dict_obj): ...
     def del_root(self) -> None: ...
     @staticmethod
     def get_buf_from_file(f): ...
     file_size_this: Any
     def read_pdf_info(self) -> None: ...
-    def next_object_id(self, offset: Incomplete | None = ...): ...
+    def next_object_id(self, offset: Incomplete | None = None): ...
     delimiter: bytes
     delimiter_or_ws: bytes
     whitespace: bytes
     whitespace_or_hex: bytes
     whitespace_optional: Any
     whitespace_mandatory: Any
     whitespace_optional_no_nl: bytes
@@ -130,15 +134,15 @@
     re_name: Any
     re_dict_start: Any
     re_dict_end: Any
     @classmethod
     def interpret_trailer(cls, trailer_data): ...
     re_hashes_in_name: Any
     @classmethod
-    def interpret_name(cls, raw, as_text: bool = ...): ...
+    def interpret_name(cls, raw, as_text: bool = False): ...
     re_null: Any
     re_true: Any
     re_false: Any
     re_int: Any
     re_real: Any
     re_array_start: Any
     re_array_end: Any
@@ -147,18 +151,18 @@
     re_indirect_reference: Any
     re_indirect_def_start: Any
     re_indirect_def_end: Any
     re_comment: Any
     re_stream_start: Any
     re_stream_end: Any
     @classmethod
-    def get_value(cls, data, offset, expect_indirect: Incomplete | None = ..., max_nesting: int = ...): ...
+    def get_value(cls, data, offset, expect_indirect: Incomplete | None = None, max_nesting: int = -1): ...
     re_lit_str_token: Any
     escaped_chars: Any
     @classmethod
     def get_literal_string(cls, data, offset): ...
     re_xref_section_start: Any
     re_xref_subsection_start: Any
     re_xref_entry: Any
     def read_xref_table(self, xref_section_offset): ...
-    def read_indirect(self, ref, max_nesting: int = ...): ...
-    def linearize_page_tree(self, node: Incomplete | None = ...): ...
+    def read_indirect(self, ref, max_nesting: int = -1): ...
+    def linearize_page_tree(self, node: Incomplete | None = None): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/PngImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/PngImagePlugin.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,62 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
+from enum import IntEnum
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
 from ._binary import o8 as o8
 from .ImageFile import ImageFile
 
 logger: Any
 is_cid: Any
 MAX_TEXT_CHUNK: Any
 MAX_TEXT_MEMORY: Any
-APNG_DISPOSE_OP_NONE: int
-APNG_DISPOSE_OP_BACKGROUND: int
-APNG_DISPOSE_OP_PREVIOUS: int
-APNG_BLEND_OP_SOURCE: int
-APNG_BLEND_OP_OVER: int
+
+class Disposal(IntEnum):
+    OP_NONE: int
+    OP_BACKGROUND: int
+    OP_PREVIOUS: int
+
+APNG_DISPOSE_OP_NONE: Literal[Disposal.OP_NONE]
+APNG_DISPOSE_OP_BACKGROUND: Literal[Disposal.OP_BACKGROUND]
+APNG_DISPOSE_OP_PREVIOUS: Literal[Disposal.OP_PREVIOUS]
+
+class Blend(IntEnum):
+    OP_SOURCE: int
+    OP_OVER: int
+
+APNG_BLEND_OP_SOURCE: Literal[Blend.OP_SOURCE]
+APNG_BLEND_OP_OVER: Literal[Blend.OP_OVER]
 
 class ChunkStream:
     fp: Any
     queue: Any
     def __init__(self, fp) -> None: ...
     def read(self): ...
     def __enter__(self): ...
-    def __exit__(self, *args) -> None: ...
+    def __exit__(self, *args: Unused) -> None: ...
     def close(self) -> None: ...
     def push(self, cid, pos, length) -> None: ...
     def call(self, cid, pos, length): ...
     def crc(self, cid, data) -> None: ...
     def crc_skip(self, cid, data) -> None: ...
-    def verify(self, endchunk: bytes = ...): ...
+    def verify(self, endchunk: bytes = b"IEND"): ...
 
 class iTXt(str):
     lang: Any
     tkey: Any
     @staticmethod
-    def __new__(cls, text, lang: Incomplete | None = ..., tkey: Incomplete | None = ...): ...
+    def __new__(cls, text, lang: Incomplete | None = None, tkey: Incomplete | None = None): ...
 
 class PngInfo:
     chunks: Any
     def __init__(self) -> None: ...
-    def add(self, cid, data, after_idat: bool = ...) -> None: ...
-    def add_itxt(self, key, value, lang: str = ..., tkey: str = ..., zip: bool = ...) -> None: ...
-    def add_text(self, key, value, zip: bool = ...): ...
+    def add(self, cid, data, after_idat: bool = False) -> None: ...
+    def add_itxt(self, key, value, lang: str = "", tkey: str = "", zip: bool = False) -> None: ...
+    def add_text(self, key, value, zip: bool = False): ...
 
 class PngStream(ChunkStream):
     im_info: Any
     im_text: Any
     im_size: Any
     im_mode: Any
     im_tile: Any
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/PyAccess.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/PyAccess.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 logger: Logger
 
 class PyAccess:
     readonly: Any
     image8: Any
     image32: Any
     image: Any
-    def __init__(self, img, readonly: bool = ...) -> None: ...
+    def __init__(self, img, readonly: bool = False) -> None: ...
     def __setitem__(self, xy, color) -> None: ...
     def __getitem__(self, xy): ...
     putpixel: Any
     getpixel: Any
     def check_xy(self, xy): ...
 
 class _PyAccess32_2(PyAccess):
@@ -55,8 +55,8 @@
 
 class _PyAccessF(PyAccess):
     def get_pixel(self, x, y): ...
     def set_pixel(self, x, y, color) -> None: ...
 
 mode_map: Any
 
-def new(img, readonly: bool = ...): ...
+def new(img, readonly: bool = False): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/SpiderImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/SpiderImagePlugin.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -18,12 +18,12 @@
     def n_frames(self): ...
     @property
     def is_animated(self): ...
     def tell(self): ...
     stkoffset: Any
     fp: Any
     def seek(self, frame) -> None: ...
-    def convert2byte(self, depth: int = ...): ...
+    def convert2byte(self, depth: int = 255): ...
     def tkPhotoImage(self): ...
 
-def loadImageSeries(filelist: Incomplete | None = ...): ...
+def loadImageSeries(filelist: Incomplete | None = None): ...
 def makeSpiderHeader(im): ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/TiffImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/TiffImagePlugin.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from _typeshed import Incomplete
 from collections.abc import MutableMapping
 from numbers import Rational
+from types import TracebackType
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
 from .ImageFile import ImageFile
 
 logger: Any
 READ_LIBTIFF: bool
@@ -50,15 +51,15 @@
 IMAGEJ_META_DATA: int
 COMPRESSION_INFO: Any
 COMPRESSION_INFO_REV: Any
 OPEN_INFO: Any
 PREFIXES: Any
 
 class IFDRational(Rational):
-    def __init__(self, value, denominator: int = ...) -> None: ...
+    def __init__(self, value, denominator: int = 1) -> None: ...
     @property
     def numerator(a): ...
     @property
     def denominator(a): ...
     def limit_rational(self, max_denominator): ...
     def __hash__(self) -> int: ...
     def __eq__(self, other): ...
@@ -88,41 +89,43 @@
     __ceil__: Any
     __floor__: Any
     __round__: Any
 
 class ImageFileDirectory_v2(MutableMapping[int, Any]):
     group: int | None
     tagtype: dict[int, int]
-    def __init__(self, ifh: bytes = ..., prefix: bytes | None = ..., group: int | None = ...) -> None: ...
+    def __init__(
+        self, ifh: bytes = b"II*\x00\x00\x00\x00\x00", prefix: bytes | None = None, group: int | None = None
+    ) -> None: ...
     @property
     def prefix(self) -> bytes: ...
     @property
     def offset(self) -> int | None: ...
     @property
     def legacy_api(self) -> bool: ...
     def reset(self) -> None: ...
     def named(self): ...
     def __len__(self) -> int: ...
     def __getitem__(self, tag): ...
     def __contains__(self, tag): ...
     def __setitem__(self, tag, value) -> None: ...
     def __delitem__(self, tag) -> None: ...
     def __iter__(self): ...
-    def load_byte(self, data, legacy_api: bool = ...): ...
+    def load_byte(self, data, legacy_api: bool = True): ...
     def write_byte(self, data): ...
-    def load_string(self, data, legacy_api: bool = ...): ...
+    def load_string(self, data, legacy_api: bool = True): ...
     def write_string(self, value: int | str | bytes) -> bytes: ...
-    def load_rational(self, data, legacy_api: bool = ...): ...
+    def load_rational(self, data, legacy_api: bool = True): ...
     def write_rational(self, *values): ...
-    def load_undefined(self, data, legacy_api: bool = ...): ...
+    def load_undefined(self, data, legacy_api: bool = True): ...
     def write_undefined(self, value): ...
-    def load_signed_rational(self, data, legacy_api: bool = ...): ...
+    def load_signed_rational(self, data, legacy_api: bool = True): ...
     def write_signed_rational(self, *values): ...
     def load(self, fp) -> None: ...
-    def tobytes(self, offset: int = ...): ...
+    def tobytes(self, offset: int = 0): ...
     def save(self, fp): ...
 
 class ImageFileDirectory_v1(ImageFileDirectory_v2):
     def __init__(self, *args, **kwargs) -> None: ...
     @property
     def tags(self): ...
     @property
@@ -140,15 +143,15 @@
 ImageFileDirectory = ImageFileDirectory_v1
 
 class TiffImageFile(ImageFile):
     format: ClassVar[Literal["TIFF", "MIC"]]
     format_description: ClassVar[str]
     tag_v2: Any
     tag: Any
-    def __init__(self, fp: Incomplete | None = ..., filename: Incomplete | None = ...) -> None: ...
+    def __init__(self, fp: Incomplete | None = None, filename: Incomplete | None = None) -> None: ...
     @property
     def n_frames(self): ...
     im: Any
     def seek(self, frame) -> None: ...
     def tell(self): ...
     def load(self): ...
     def load_end(self) -> None: ...
@@ -158,26 +161,28 @@
 class AppendingTiffWriter:
     fieldSizes: Any
     Tags: Any
     f: Any
     close_fp: bool
     name: Any
     beginning: Any
-    def __init__(self, fn, new: bool = ...) -> None: ...
+    def __init__(self, fn, new: bool = False) -> None: ...
     whereToWriteNewIFDOffset: Any
     offsetOfNewPage: int
     IIMM: Any
     isFirst: bool
     def setup(self) -> None: ...
     def finalize(self) -> None: ...
     def newFrame(self) -> None: ...
     def __enter__(self): ...
-    def __exit__(self, exc_type, exc_value, traceback): ...
+    def __exit__(
+        self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: TracebackType | None
+    ) -> Literal[False]: ...
     def tell(self): ...
-    def seek(self, offset, whence=...): ...
+    def seek(self, offset, whence=0): ...
     def goToEnd(self) -> None: ...
     endian: Any
     longFmt: Any
     shortFmt: Any
     tagFormat: Any
     def setEndian(self, endian) -> None: ...
     def skipIFDs(self) -> None: ...
@@ -187,8 +192,8 @@
     def rewriteLastShortToLong(self, value) -> None: ...
     def rewriteLastShort(self, value) -> None: ...
     def rewriteLastLong(self, value) -> None: ...
     def writeShort(self, value) -> None: ...
     def writeLong(self, value) -> None: ...
     def close(self) -> None: ...
     def fixIFD(self) -> None: ...
-    def fixOffsets(self, count, isShort: bool = ..., isLong: bool = ...) -> None: ...
+    def fixOffsets(self, count, isShort: bool = False, isLong: bool = False) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/TiffTags.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/TiffTags.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -8,23 +8,23 @@
     type: _TagType
     length: int
     enum: dict[str, int]
 
 class TagInfo(_TagInfo):
     def __new__(
         cls,
-        value: Incomplete | None = ...,
-        name: str = ...,
-        type: _TagType | None = ...,
-        length: int | None = ...,
-        enum: dict[str, int] | None = ...,
+        value: Incomplete | None = None,
+        name: str = "unknown",
+        type: _TagType | None = None,
+        length: int | None = None,
+        enum: dict[str, int] | None = None,
     ): ...
     def cvt_enum(self, value): ...
 
-def lookup(tag: int, group: int | None = ...) -> _TagInfo: ...
+def lookup(tag: int, group: int | None = None) -> _TagInfo: ...
 
 BYTE: Literal[1]
 ASCII: Literal[2]
 SHORT: Literal[3]
 LONG: Literal[4]
 RATIONAL: Literal[5]
 SIGNED_BYTE: Literal[6]
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/WmfImagePlugin.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/WmfImagePlugin.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         bbox: Any
         def open(self, im) -> None: ...
         def load(self, im): ...
 
 class WmfStubImageFile(StubImageFile):
     format: ClassVar[Literal["WMF"]]
     format_description: ClassVar[str]
-    def load(self, dpi: Incomplete | None = ...) -> None: ...
+    def load(self, dpi: Incomplete | None = None) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PIL-stubs/features.pyi` & `types-Pillow-9.5.0.0/PIL-stubs/features.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 def check_feature(feature): ...
 def version_feature(feature): ...
 def get_supported_features(): ...
 def check(feature): ...
 def version(feature): ...
 def get_supported(): ...
-def pilinfo(out: Incomplete | None = ..., supported_formats: bool = ...) -> None: ...
+def pilinfo(out: Incomplete | None = None, supported_formats: bool = True) -> None: ...
```

### Comparing `types-Pillow-9.4.0.9/PKG-INFO` & `types-Pillow-9.5.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.4.0.9
+Version: 9.5.0.0
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9ed39d879649426ba6ba67f4879e3fb814472bc7`.
+This package was generated from typeshed commit `f66769a6f5c1f335e566d48c67d179974996a352`.
```

### Comparing `types-Pillow-9.4.0.9/setup.py` & `types-Pillow-9.5.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9ed39d879649426ba6ba67f4879e3fb814472bc7`.
+This package was generated from typeshed commit `f66769a6f5c1f335e566d48c67d179974996a352`.
 '''.lstrip()
 
 setup(name=name,
-      version="9.4.0.9",
+      version="9.5.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md",
```

### Comparing `types-Pillow-9.4.0.9/types_Pillow.egg-info/PKG-INFO` & `types-Pillow-9.5.0.0/types_Pillow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.4.0.9
+Version: 9.5.0.0
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9ed39d879649426ba6ba67f4879e3fb814472bc7`.
+This package was generated from typeshed commit `f66769a6f5c1f335e566d48c67d179974996a352`.
```

### Comparing `types-Pillow-9.4.0.9/types_Pillow.egg-info/SOURCES.txt` & `types-Pillow-9.5.0.0/types_Pillow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

