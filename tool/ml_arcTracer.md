---
layout: page
permalink: tool/ml_arcTracer/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_arcTracer.png) Arc Tracer
Download [ml_arcTracer.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_arcTracer.py)

| Revision | 11 |
|---:|---|
| Last Update | 2018-05-13 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Create a line on screen which traces the path af an animated object. It's Substitute for tracing arcs on your screen by hand with a marker. It can be used either as an overlay on your camera view, or in world space. It's a bake process; like a marker it doesn't update interactively. Lines are colored to distinguish between multiple traces. Frames are marked along the arc as black dots, with keyframes colored red, and the current frame is highlighted. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_arcTracer.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_arcTracer
ml_arcTracer.ui()
```

## Usage

 Run the UI, and press the buttons to choose the action. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_arcTracer.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_arcTracer ml_arcTracer.ui() 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Video

 http://www.youtube.com/watch?v=xLA1aglvPYM 

## Ui

 [Trace Camera] : Trace an arc as an overlay over the current camera. [Trace World] : Trace an arc in world space. [Retrace Previous] : Retrace the previously traced arc. [Clear Arcs] : Clear all arcs. 

## UI Options


|<button type="button">Trace Camera</button>|Trace an arc as an overlay over the current camera.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Trace World</button>|Trace an arc in world space.|Right-click to create a shelf or hotkey|
|<button type="button">Retrace Previous</button>|Retrace the previously traced arc.|Right-click to create a shelf or hotkey|
|<button type="button">Clear Arcs</button>|Clear all arcs.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2011-05-01|First publish|
|2|2011-05-14|minor bug fix involving error with duplicate names|
|3|2011-05-14|Revision notes update.|
|4|2014-03-01|adding category|
|5|2016-12-10|removing euclid dependency|
|6|2017-06-30|Fixing bug with moving cameras, adding line width|
|7|2018-02-17|Updating license to MIT.|
|8|2018-04-09|Test for accuracy to determine whether the fast solution is accurate.|
|9|2018-05-05|Adding shelf support.|
|10|2018-05-06|Added marking menu.|
|11|2018-05-13|shelf support|
