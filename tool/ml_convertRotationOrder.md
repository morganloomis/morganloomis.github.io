---
layout: page
permalink: tool/ml_convertRotationOrder/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_convertRotationOrder.png) Convert Rotation Order
Download [ml_convertRotationOrder.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_convertRotationOrder.py)

| Revision | 4 |
|---:|---|
| Last Update | 2014-03-01 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This is a tool for changing the rotation order of an object while preserving keyed poses, for when you want to change the rotation order after you've already done animation, or don't want to alter the pose of an object.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_convertRotationOrder.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_convertRotationOrder
ml_convertRotationOrder.ui()
```

## Usage

 Run the UI. Select the objects with rotation orders you want to change, and press the button for the desired rotation order.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2011-10-08|First publish.|
|2|2012-03-12|Updated to work with non-keyed objects, added the tips button.|
|3|2012-08-04|Fixing bug with potential duplicate temp name.|
|4|2014-03-01|adding category|
