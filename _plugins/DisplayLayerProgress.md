---
layout: plugin

id: DisplayLayerProgress
title: DisplayLayerProgress 
description: Displays the current processing layer and the percentage in "Printer-Display" and in top "NavBar"
author: Olli
license: AGPLv3

date: 2018-04-09

homepage: https://github.com/OllisGit/OctoPrint-DisplayLayerProgress
source: https://github.com/OllisGit/OctoPrint-DisplayLayerProgress
archive: https://github.com/OllisGit/OctoPrint-DisplayLayerProgress/archive/master.zip

follow_dependency_links: false

tags:
- display
- lcd
- printer
- progress
- layer

screenshots:
- url: /assets/img/plugins/DisplayLayerProgress/example-navbar-display.jpg
  alt: Example of NavBar Display
  caption: Example of NavBar Display
- url: /assets/img/plugins/DisplayLayerProgress/example-printer-display.jpg
  alt: Example of Printer Display
  caption: Example of Printer Display
- url: /assets/img/plugins/DisplayLayerProgress/example-statebar.jpg
  alt: Example of State Bar output
  caption: Example of State Bar output
- url: /assets/img/plugins/DisplayLayerProgress/settings.jpg
  alt: Plugin Settings
  caption: Plugin Settings


featuredimage: /assets/img/plugins/DisplayLayerProgress/example-navbar-display.jpg

---

A OctoPrint-Plugin that sends the current progress of a print via M117 command to the printer-display and also to the top navigation bar.
It shows the percentage, the current layer and the total layer count:

- Printer Display: 50% 60 / 120
- NavBar: Layer: 60 / 120

**ATTENTION:** 
- The layer information output only works with "Cura"/"Simplify3D" generated G-Code, because these Slicer insert the layer information directly as comments in the file. 
If you want to use "slic3r", see [Enhancement #8](https://github.com/OllisGit/OctoPrint-DisplayLayerProgress/issues/8)
- If the layer comments couldn't found, only the percentage will be displayed
- You need to upload your G-Code after installation of the plugin again (if you want to reuse already stored models in OctoPrint), because while uploading the G-Code is modfied


For implementation details please visit the [homepage]({{ page.homepage | absolute_url }}).

