Cycles Render Time Calculator
=============================

This is the readme to **Cycles Render Time Calculator** (**CRTC**), a [Python  application](http://www.python.org)
and [HTML/JavaScript website experiment](http://le717.github.io/CRTC) written by
[Triangle717](http://Triangle717.WordPress.com) and [rioforce](http://rioforce.WordPress.com)
to calculate approximate GPU render times when using the [Blender Cycles Engine](http://www.blender.org).

Why Was This Created
--------------------

It is said that "Necessity is the mother of invention". That can be said of this small tool.
Rioforce and I were always spending lots of time trying to figure out when his render would be completed,
and we were tired of it. We finally determined I should write a program to do this for us.
Thus **CRTC** was born.

In the third week of October 2013, I began rewriting **CRTC** in HTML/JavaScript form
as an experiment and learning project on how to create websites.

_Coming Soon._

How It Works
------------

**Cycles Render Time Calculator** supports both the Tile and Progressive Refine render methods
for both still images and animations, as well as a general animation render (render engine neutral).
Blender Internal is not supported, and if it were, this project would not be named the way it is. :stuck_out_tongue:

**NOTE:** _Approximate_ is the keyword here. While the render times are accurate if all system variables remain constant,
that is an impossible feat to achieve. Thus, the final render times will be different than the stated time.
For example, it calculated a 6.5 minute render time for me, and it really only took 5 minutes.

### Python ###

For tile render, simply enter the number of tiles it takes to render your image, and how long it takes (in seconds) to render a single tile (milliseconds
are supported). This info can easily be found in the Render Window. **CRTC** will then calculate an approximate render time. If you
are rendering an animation (AKA video or "multi-frame" animation), press 'y' when prompted, enter the number of frames your video has, and an approximate
animation render time will be calculated.

For progressive refine, enter the number of samples in your render, and how long it takes (in seconds) a single sample to render. Again, milliseconds are
supported. This info can also be found in the Render Window.

The animation render asks only two questions: number of frames, and the time it takes for a single frame to render.

In all modes, render time will be displayed in either seconds, minutes, or hours, depending on the input and the result of the calculations.

### Website ###

_Coming Soon._


Releases
--------

All downloads of **CRTC** are hosted on this project,
and are available on the [Releases page.](https://github.com/le717/CRTC/releases)

* Version 1.2.2 - May 21, 2013

> [Source Code](https://github.com/le717/Cycles-Render-Time-Calculator/tree/1.2.2)

> [Direct Download](https://github.com/le717/Cycles-Render-Time-Calculator/archive/1.2.2.zip)

* Version 1.1/1.2 Stable - February 26, 2013

> [Source Code](https://github.com/le717/Cycles-Render-Time-Calculator/tree/V1.1Stable) [**](#builds)

> [Direct Download](https://github.com/le717/Cycles-Render-Time-Calculator/archive/V1.1Stable.zip)

* Version 1.0 Beta 2 - February 16, 2013

> [Source Code](https://github.com/le717/Cycles-Render-Time-Calculator/tree/V1.0b2)

> [Direct Download](https://github.com/le717/Cycles-Render-Time-Calculator/archive/V1.0b2.zip)

Builds
------
* **Cycles Render Time Calculator** was originally written in Python 3.3, but in version 1.2, it was updated to run on both Python 2 and 3.
It was successfully tested on Python 3.3.0 and 2.7.4 with no errors. Further more, only the raw Python script of that was upgraded to 1.2.
The OS-specific builds are version 1.1, written with Python 3.3.0 only.

* Releases are compiled into Windows x86, x64 EXEs and Mac OS X application using [cx_freeze](http://cx-freeze.sourceforge.net).

* Windows build has been sucessfully tested on x64 Windows 7 and 8. However, Vista (and possibly XP) should be supported.

* Mac OS X build is provided courtesy of [@JrMasterModelBuilder](https://github.com/JrMasterModelBuilder). Minimum supported version is Mac OS X 10.7 Lion.

* **Cycles Render Time Calculator** has been successfully tested on Ubuntu 12.04.1 x86 running Python 3.2. It may run on other Unix distos, but has not been
tested.

License
-------

**Cycles Render Time Calculator** and all components were created 2013 Triangle717 and rioforce.
The Python version is licensed under the
[GNU General Public License Version 3](http://www.gnu.org/licenses/gpl.html),
while the HTML/JavaScript website experiment licensed under
[The MIT License](http://opensource.org/licenses/MIT).

**CRTC** makes use of the [**CSS Browser Selector**](https://github.com/verbatim/css_browser_selector) library,
originally created by [Rafael Lima] (http://rafael.adm.br) and licensed under the
[CC BY 2.5](http://creativecommons.org/licenses/by/2.5/).
