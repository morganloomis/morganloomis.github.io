---
layout: page
title: ml_arcTracer
permalink: help/ml_arcTracer/
---

| ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_arcTracer.png) | [ml_arcTracer](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_arcTracer.py) |
|---:|---|
| Revision | 6 |
| Last Update | 2017-06-30 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This tool is a substitute for tracing arcs on your screen by hand with a marker. It creates a thick line to represent the path of an object, either as an overlay on your camera view, or in world space. It's a bake process; like a marker it doesn't update interactively. Lines are colored randomly, to distinguish between multiple traces. Frames are marked along the arc as black dots, with keyframes colored red, and the current frame is highlighted.

## Installation

Copy this file into your maya scripts directory, for example:
> C:/Documents and Settings/user/My Documents/maya/scripts/ml_arcTracer.py

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_arcTracer
ml_arcTracer.ui()
```

## Usage

 Run the UI, and press the buttons to choose the action.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


| x | y | z |
|---|---|---|
| <button type="button">Trace World</button> | Trace an arc in world space. | Right-click to create a shelf or hotkey |
| <button type="button">Retrace Previous</button> | Retrace the previously traced arc. | Right-click to create a shelf or hotkey |
| <button type="button">Clear Arcs</button> | Clear all arcs. | Right-click to create a shelf or hotkey |
## Video Tutorial
[![youtube](http://img.youtube.com/vi/xLA1aglvPYM/0.jpg)](http://www.youtube.com/watch?v=xLA1aglvPYM)
## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2011-05-01|First publish|
|2|2011-05-14|minor bug fix involving error with duplicate names|
|3|2011-05-14|Revision notes update.|
|4|2014-03-01|adding category|
|5|2016-12-10|removing euclid dependency|
|6|2017-06-30|Fixing bug with moving cameras, adding line width|
