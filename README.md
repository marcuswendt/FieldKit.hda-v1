```
      _____    __    _____    __       ____
     / ___/   / /   /____/   / /      /    \    FieldKit.hda
    / ___/   / /   /____/   / /__    /  /  /    (c) 2016, FIELD. All rights reserved.
   /_/      /_/   /____/   /____/   /_____/     http://www.field.io

```

A collection of digital assets for SideFX's Houdini animation and visual effects software.
This library combines frequently used tools and ideas derived from the generative design field as small modular assets: 3D animation, procedural modelling, simulation etc.

It's a more modern and hopefully better engineered version of https://github.com/field/FieldKit.otl for Houdini 15.0+


# Conventions

* Operators are usually implemented in the VEX language for best performance.
* Each operator is defined in ./hda/fd_<context>_<operator-name>.hda and should include a example + test file in ./example/<context>_<operator-name>.hip


# Installation

1. [Download](//github.com/field/FieldKit.hda/archive/master.zip) or clone the repository onto a local or network drive e.g. //your-server/your-share/FieldKit.hda/

2. Open ```houdini.env``` (Windows: ```$HOME/houdiniX.Y/houdini.env``` OS X: ```~/Library/Preferences/houdini/```) in a text editor and append the following lines:
```Bash
FIELDKIT = "<PATH TO YOUR GIT CLONE HERE>"
HOUDINI_OTLSCAN_PATH = "$FIELDKIT;$HFS/houdini/otls"
```

3. Relaunch Houdini and it should have picked up the assets. Use Windows> Operator Type Manager> Scanned OTL Libraries to check.



Credits
=======

Released under the BSD license.  Full details in the included LICENSE file.

(c) 2016, Marcus Wendt <marcus@field.io>
