---
title: scale pixels
date: 2022-12-04T02:19:02+01:00
id: scale-pixels
applicable-version: 3.2.1
tags:
working-color-space: RGB
view: darkroom
masking: false
---

Some cameras (such as the Nikon D1X) have rectangular instead of the usual square sensor cells. Without correction this would lead to distorted images. This module applies the required scaling.

Ansel detects images that need correction using their Exif data and automatically activates this module where required. For other images the module always remains disabled.

The module has no controls.
