---
layout: page
permalink: tool/ml_cameraDepthDragger/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_cameraDepthDragger.png) Camera Depth Dragger
Download [ml_cameraDepthDragger.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_cameraDepthDragger.py)

| Revision | 3 |
|---:|---|
| Last Update | 2016-12-10 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Move objects closer to or further from camera, such that they don't change location in screen space, just get larger or smaller in frame.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_cameraDepthDragger.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_cameraDepthDragger
ml_cameraDepthDragger.drag()
```

## Usage

 Run the tool, and then click and drag the mouse in the viewport to move selected objects closer or further from camera. When you release click, the tool will exit.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2012-03-12|First publish.|
|2|2014-03-01|adding category|
|3|2016-12-10|Removing euclid dependency|
