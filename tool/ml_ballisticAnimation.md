---
layout: page
permalink: tool/ml_ballisticAnimation/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_ballisticAnimation.png) Ballistic Animation
Download [ml_ballisticAnimation.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_ballisticAnimation.py)

| Revision | 1 |
|---:|---|
| Last Update | 2016-10-01 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Runs very simple gravity physics on the translation of an object, taking into account initial velocity.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_ballisticAnimation.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_ballisticAnimation
ml_ballisticAnimation.main()
```

## Usage

 Simply select a static or animated object, highlight or set your frame range, and run the script. If your object is already animated, the initial velocity will be calculated based on the position one frame before the frirst frame of the frame range.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-10-01|First publish.|
