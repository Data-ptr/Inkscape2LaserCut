# Inkscape2LaserCut
Instructions on taking vectors created in Inkscape and Importing them into LaserCut

By: Jane Hacker
Jan. 17th, 2018


## Setup

* Open Inkscape (I'm using 0.48.5 r10040)


### Document Units (CRITICAL)

* Goto "File > Document Properties" (or Shift + Ctrl + D)
* On the "Page" Tab under the "General" heading change "Default units" to mm


### Orientation and Size (Personal Preference)

* While still in "Document Properties" and the "Page" Tab:
  * Set "Orientation" to "Landscape"
  * Under the "Custom Size" box change "Units" to mm
  * Enter a size that will work for your project


### Grid (Personal Preference)

* While still in "Document Properties" go to the "Grids" tab
  * Under the "Creation" header drop down to "Rectangular Grid" (this may already be selected by default)
  * click the "New" button next to that.
  * Under the "Defined Grids" heading change "Grid Units" to mm
  * Change "Spacing X" and "Spacing Y" to 0.5


## Make stuff (Kinda the point...)

* I may add some hints for making stuff later


### Setting up stroke

* Make "Fill" "None" (The "X" square)
* Under the "Stroke paint" Tab set "Stroke" to:
  * Select the square with the tool-tip (hover over) "Flat color"
  * Color to "255" in RED (defaut used for "cut" mode)
  * Alpha to full
  * Or RGBA: ff0000ff
* Under the "Stroke style" Tab set:
  * Size "0.25mm" (change "Unit" to reflect mm) (NOTE: This is the laser beam we can typicaly expect)


## Saving for exporting to LaserCut

### Get things ready for exporting (CRITIAL)

* Select all objetcs by going to "Edit > Select All" (or CTRL + A)
* Goto "Object > Group" (or CTRL + G)
* While everything is still selected
  * Goto "Path > Stroke to Path" (or CTRL+ALT+C) ----------------------> VERY VERY CRITICAL
* Goto "Edit > deselect" (for good measure ;)


### The saving/exporting step

* Goto "File > Save a copy"
* Under the drop-down for file type (bottom right for me, will likely have "Inkscape SVG (*.svg)" selected by default)
  * Select "Desktop Cutting Plotter (AutoCAD DXF R14) (*.dxf)" --------> VERY VERY CRITICAL
* Chnage the name and location as you wish
* Click "Save"
* A new diolog will appear with the title "Desktop Cutting Plotter"
  * Under the "Options" tab (should already be showing) change "Base Unit" to mm
  * Click "OK"
* We are done exporting!


## Importing to LaserCut

* Open LaserCut (I'm using 5.3)
* Goto "File > Import..." (Or CTRL + I)
* An "Open" dialog will appear, navigate to where you saved your file from InkScape and select your file.
* We are done importing!
