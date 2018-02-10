---
layout: page
permalink: tool/ml_breakdownDragger/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_breakdownDragger.png) Breakdown Dragger
Download [ml_breakdownDragger.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_breakdownDragger.py)

| Revision | 5 |
|---:|---|
| Last Update | 2014-10-10 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Blend a keyframe or pose with the next or previous keys, essentially creating a breakdown pose that is weighted one way or the other. The weight of the blend is controlled by dragging the mouse in the viewport.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_breakdownDragger.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_breakdownDragger
ml_breakdownDragger.drag()
```

## Usage

 Run the tool, and the cursor will turn into a hand. Left-click and hold in the viewport, and then drag either left or right to weight the key to the next or previous key. Alternately, press and hold the middle mouse button to weight the key toward or away from the average of the surrounding keys. If you have no keys selectd, the tool will act only on curves that are visibile in the graph editor. If there are no keys at the current frame, keys will be set.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## Video Tutorial
[![youtube](http://img.youtube.com/vi/D8yD4zbHTP8/0.jpg)](http://www.youtube.com/watch?v=D8yD4zbHTP8)
## Revision History

| Revision | Date | Note|
|---|---|---|
|1||First publish|
|4|2014-03-01|adding category|
|5|2014-10-10|Bug fixes|
