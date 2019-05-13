---
title: WebGL Engine Examples
permalink: "/webengine-examples/"
nav_order: 3
---

# WebGL Engine Examples
{: .no_toc }

Here’s a curated collection of examples of how to use the [WWT WebGL Engine]
in your own web projects.

[WWT WebGL Engine]: https://worldwidetelescope.gitbook.io/webgl-engine-reference/

**Note:** *Due to limitations in our web infrastructure, these examples will
  only work if you access them through unencrypted HTTP, not secure HTTPS.
  Please ensure that you are not visiting this site over an HTTPS channel.*

The above limitation is also why these examples are stored independently from
the main [WebGL Engine Reference] manual. We hope to integrate the reference
manual and our library of examples more tightly in the future.

Your contributions are more than welcome! If you’d like to add an example,
please submit a pull request against the [wwt-web-examples repository] with
your addition.

[WebGL Engine Reference]: https://worldwidetelescope.gitbook.io/webgl-engine-reference/
[wwt-web-examples repository]: https://github.com/WorldWideTelescope/wwt-web-examples/

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Targeted Examples

{% for ex in site.data.webengine_examples %}

----

### {{ ex.title }}

{{ ex.summary }}

- [View it live in the browser!](./{{ex.id}}/)
- [View the source code on GitHub](https://github.com/WorldWideTelescope/wwt-web-examples/tree/master/webengine-examples/{{ex.id}}/)

By: [{{ ex.author_name }}](https://github.com/{{ ex.author_github }}).

{% endfor %}


## Examples on the Main Website

There are a few additional examples integrated into the main WWT website:

- [ImportImage] (implemented in [ImportImage.js])
- [Spectroscopy] (implemented in [Spectroscopy.js])
- [Great Observatories] (implemented in [Observatories.js])
- [Planet Explorer] (implemented in [PlanetExplorer.js])

[ImportImage]: http://www.worldwidetelescope.org/GetInvolved/ImportImage
[Spectroscopy]: http://www.worldwidetelescope.org/GetInvolved/Spectrum
[Great Observatories]: http://www.worldwidetelescope.org/GetInvolved/GreatObservatories
[Planet Explorer]: http://www.worldwidetelescope.org/GetInvolved/PlanetExplorer

[ImportImage.js]: https://github.com/WorldWideTelescope/wwt-website/blob/master/WWTMVC5/Scripts/pages/ImportImage.js
[Spectroscopy.js]: https://github.com/WorldWideTelescope/wwt-website/blob/master/WWTMVC5/Scripts/pages/Spectroscopy.js
[Observatories.js]: https://github.com/WorldWideTelescope/wwt-website/blob/master/WWTMVC5/Scripts/pages/Observatories.js
[PlanetExplorer.js]: https://github.com/WorldWideTelescope/wwt-website/blob/master/WWTMVC5/Scripts/pages/PlanetExplorer.js


## WebGL Engine in the Wild

Here are some folks that use the WebGL engine out “in the wild”! Not all of
these have source code on GitHub, but since it’s the web, you can always open
up these pages in “View Source” or your browser’s Developer Tools and start
exploring ...

Are you using the WebGL engine in a project of your own? We would love to hear
from you! Please [file a pull request] to add your project to this list.

[file a pull request]: https://github.com/WorldWideTelescope/wwt-web-examples/pull/new/master

---

### The WWT Webclient

Of course, the [WWT webclient] is powered by the WebGL engine! The source code
to the frontend is mixed between the [wwt-web-client] and [wwt-website]
repositories.

[WWT webclient]: http://www.worldwidetelescope.org/webclient/
[wwt-web-client]: https://github.com/WorldWideTelescope/wwt-web-client/
[wwt-website]: https://github.com/WorldWideTelescope/wwt-website/

---

### pywwt

Another official WWT project, the [pywwt] Python module allows you to embed
the WWT WebGL engine in [Jupyter notebooks] and [JupyterLab environments],
allowing researchers to seamlessly visualize spatial astronomical data in
context. Source code lives in the [pywwt repository].

[pywwt]: https://pywwt.readthedocs.io/
[Jupyter notebooks]: https://jupyter.org/
[JupyterLab environments]: https://jupyterlab.readthedocs.io/en/stable/
[pywwt repository]: https://github.com/WorldWideTelescope/pywwt/

---

### Chandra Source Catalog 2.0

[Version 2.0 of the Chandra Source Catalog] includes a
[WWT-powered interactive visualizer] of its survey data.

[Version 2.0 of the Chandra Source Catalog]: http://cxc.harvard.edu/csc2/
[WWT-powered interactive visualizer]: http://cxc.harvard.edu/csc2/wwt.html

---

### "What is Chandra Doing Now?"

[What is Chandra Doing Now?] is a real-time dashboard of the Chandra space
telescope’s activities. The “Interactive” view is powered by WWT. Its source
code is in the [doug_burke/chandraobs] repository on [BitBucket].

[What is Chandra Doing Now?]: http://chandraobservatory.herokuapp.com/index.html
[doug_burke/chandraobs]: https://bitbucket.org/doug_burke/chandraobs/
[BitBucket]: https://bitbucket.org/

---

### GLIMPSE360 Viewer

The [GLIMPSE360] project is an infrared panorama of the Milky Way made with
the [Spitzer space telescope]. You can explore the full dataset in their
[interactive explorer].

[GLIMPSE360]: http://www.spitzer.caltech.edu/glimpse360/
[Spitzer space telescope]: http://www.spitzer.caltech.edu/
[interactive explorer]: http://www.spitzer.caltech.edu/glimpse360/wwt

---

### ADS All Sky Survey

The [ADS](http://ui.adsabs.harvard.edu/)
[All Sky Survey](http://www.adsass.org/wwt/) maps papers from the astronomical
literature onto the sky. The [ADSASS WWT viewer] makes it possible to explore
and filter this dataset.

[ADSASS WWT viewer]: http://www.adsass.org/wwt/

---

### Interactive Planck Data Viewer

The [Planck] satellite observed the whole sky in a suite of microwave bands.
You can explore the data using — you guessed it —
[an interactive viewer powered by the WWT WebGL engine].

[Planck]: http://sci.esa.int/planck/
[an interactive viewer powered by the WWT WebGL engine]: http://planck.ipac.caltech.edu/wwt/

---

### Milky Way 3D

“MilkyWay3D.org is a tool intended to organize and curate links to information
about data sets relevant to our 3D understanding of the Milky Way.” The
[main milkyway3d.org page] features a WWT-powered data exploration interface.

[main milkyway3d.org page]: http://milkyway3d.org/

---

### Sky Banana Party!

An small (and unfinished) web app project aiming to show the localizations of
gravitational-wave events from [LIGO] and [VIRGO] immersively. View the
current status at <http://skybanana.party>. Source code in the
[sky-banana-party] repository.

[LIGO]: https://www.ligo.caltech.edu/
[VIRGO]: http://www.virgo-gw.eu/
[sky-banana-party]: https://github.com/WorldWideTelescope/sky-banana-party/
