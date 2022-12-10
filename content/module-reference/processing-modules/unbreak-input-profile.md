---
title: unbreak input profile
date: 2022-12-04T02:19:02+01:00
id: unbreak-input-profile
applicable-version: 3.2.1
tags:
working-color-space: RGB
view: darkroom
masking: true
---

Add a correction curve to image data. This is required if you have selected certain input profiles in the [_input color profile_](./input-color-profile.md) module.

If you decide to use an ICC profile from the camera manufacturer in the [_input color profile_](./input-color-profile.md) module, a correction curve frequently needs to be pre-applied to image data to prevent the final output from looking too dark. This extra processing is not required if you use Ansel's standard or enhanced color matrices.

The correction curve is defined with a linear part extending from the shadows to some upper limit and a gamma curve covering mid-tones and highlights. For further information please see Ansel's neighboring project [UFRaw](http://ufraw.sourceforge.net).

linear
: The upper limit for the region counted as shadows and where no gamma correction is performed. Typically values between 0.0 and 0.1 are required by the profile.

gamma
: The gamma value required to compensate the input profile. Often the required value is 0.45 (the reciprocal of the 2.2 gamma used by some manufacturer's profiles).
