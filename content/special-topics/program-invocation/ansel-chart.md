---
title: Ansel-chart
id: Ansel-chart
weight: 40
draft: false
author: "people"
---

The `Ansel-chart` binary is a dedicated utility to create styles out of pairs of images such as RAW+JPEG with in-camera processing. Details about its usage can be found in the [using Ansel-chart](../Ansel-chart/_index.md) section.

`Ansel-chart` can either start a GUI or be used as a command-line program.

```
Ansel-chart
              [--help]
              [<input Lab pfm file>]
              [<cht file>]
              [<reference cgats/it8 or Lab pfm file>]
```

All parameters are optional, however, if you want to supply the second file name you also need to supply the first one. Starting `Ansel-chart` this way opens a special GUI (details can be found in the [using Ansel-chart](../Ansel-chart/_index.md) section).

`--help`
: Provide usage information and terminate.

`<input Lab pfm file>`
: Open the utility with the given file as source image. The input file needs to be in Lab Portable Float Map format.

`<cht file>`
: Specify a chart file describing the layout of the used color reference chart.

`<reference cgats/it8 or Lab pfm file>`
: Specify the reference values, either as measured values according to the CGATS standard, or as a reference image in Lab Portable Float Map format.

Alternatively `Ansel-chart` can be used as a command line program to generate Ansel style files using previously saved CSV files.

```
Ansel-chart
              --csv
              <csv file>
              <number patches>
              <output dtstyle file>
```

All parameters are mandatory.

`<csv file>`
: A CSV file previously saved from within `Ansel-chart`.

`<number of patches>`
: The number of color patches to be used in the color look up table settings of the created style.

`<output dtstyle file>`
: The name of the style file to be created.
