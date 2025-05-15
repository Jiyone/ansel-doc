---
title: raw overexposed warning
date: 2022-12-04T02:19:02+01:00
id: raw-overexposed
applicable-version: 3.2.1
tags:
view: darkroom
---

Highlight areas of the image where color channels of the raw input file are clipped.

Clipped color channels imply an overexposed image with loss of information in the affected areas. Some of this information may be recoverable using the [_highlight reconstruction_](../darkroom/modules/highlight-reconstruction.md), [_color reconstruction_](../darkroom/modules/color-reconstruction.md) or [_filmic rgb_](../darkroom/modules/filmic-rgb.md) modules.

Click on the ![raw overexposed](raw-overexposed-icon.jpg) icon to show/hide the warning overlay. Right-click on the icon to open a dialog containing the following configuration parameters.

mode
: Choose how to mark clipped areas:

: - _mark with CFA color_: Display a pattern of the respective primary colors (red, green, and blue) to indicate which color channels are clipped.

: - _mark with solid color_: Mark clipped areas with a user defined solid color (see below) independent of the affected color channels.

: - _false color_: Set clipped color channels to zero in the affected areas.

color scheme
: Choose the solid color for the _mark with solid color_ mode.

clipping threshold
: Set the threshold defining what values are considered to be overexposed. You can safely leave this slider at its default value of 1.0 (white level) in most cases.
