# Inkscape2LaserCut
Instructions on taking vectors created in Inkscape and Importing them into LaserCut  

By: Jane Hacker  
Jan. 17th, 2018


## Setup

* Open Inkscape (I'm using `0.48.5 r10040`)  
I'm also running it on Linux :)


### Document Units (CRITICAL)

* Goto "File > Document Properties" (or Shift+Ctrl+D)
* On the "Page" tab under the "General" heading change "Default units" to mm


### Orientation and Size (Personal Preference)

* While still in "Document Properties" and the "Page" tab:
  * Set "Orientation" to "Landscape"
  * Under the "Custom Size" box change "Units" to mm
  * Enter a size that will work for your project


### Grid (Personal Preference)

* While still in "Document Properties" go to the "Grids" tab
  * Under the "Creation" heading, drop-down to "Rectangular Grid" (this may already be selected by default)
  * click the "New" button next to that.
  * Under the "Defined Grids" heading change "Grid Units" to mm
  * Change "Spacing X" and "Spacing Y" to 0.5


## Make stuff (The main event)

* I may add some hints for making stuff later


### Setting up stroke (Personal Preference-ish)

When you start making objects:

* With the object selected, goto "Object > Fill and Stroke" (or Shift+Ctrl+F)
* Under the "Fill" tab make "Fill" "No paint" (The "X" square in the upper-right corner)
* Under the "Stroke paint" Tab set "Stroke" to:
  * Select the square with the tool-tip (hover over) "Flat color"
  * Goto the "RGB" tab if you are not already
  * Set the color to "255" in RED (typically used for "cut" mode)
  * Alpha to full
    * Or RGBA: `#ff0000ff` for the above two steps
  * "Blur" to 0
  * "Opacity" to 100%
* Under the "Stroke style" tab set:
  * Size "0.25mm" (change "Unit" to reflect mm) (NOTE: This is the laser beam we can typicaly expect)


## Saving for exporting to LaserCut

### Get things ready for exporting (CRITIAL)

* Select all objetcs by going to "Edit > Select All" (or Ctrl+A)
* Goto "Object > Unroup" (or Shift+Ctrl+G) ----------------------> VERY CRITICAL if you have been grouping objects
* While everything is still selected
  * Goto "Path > Stroke to Path" (or Ctrl+Alt+C) ----------------------> VERY VERY CRITICAL
* Goto "Edit > Deselect" (for good measure ;)


### The saving/exporting step

* Goto "File > Save a copy"
* Under the drop-down for file type (bottom right for me, will likely have `Inkscape SVG (*.svg)` selected by default)
  * Select `Desktop Cutting Plotter (AutoCAD DXF R14) (*.dxf)` --------> VERY VERY CRITICAL
* Change the name and location as you wish
* Click "Save"
* A new diolog will appear with the title "Desktop Cutting Plotter"
  * Under the "Options" tab (should already be showing) change "Base Unit" to mm --------> VERY VERY CRITICAL
  * Click "OK"
* We are done exporting!


## Importing to LaserCut

* Open LaserCut (I'm using `LaserCut5.3`)
* Goto "File > Import..." (Or Ctrl+I)
* An "Open" dialog will appear, navigate to where you saved your file from Inkscape and select your file.
* We are done importing!
