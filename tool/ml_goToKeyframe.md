---
layout: page
permalink: tool/ml_goToKeyframe/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_goToKeyframe.png) Go To Keyframe
Download [ml_goToKeyframe.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/scripts/ml_goToKeyframe.py)

| Revision | 5 |
|---:|---|
| Last Update | 2018-05-13 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 A more robust tool for navigating to the next or previous keyframe. It recognizes only keys that are visible in the graph editor, and has options to only navigate through selected keys, and to round to the nearest whole frame, if you don't like editing on sub-frames. Finally, it can look for keys in the whole hierarchy of the selected node, to help with keeping all a character's keys on the same frames. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_goToKeyframe.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_goToKeyframe
ml_goToKeyframe.ui()
```

## Usage

 Run the UI, select next or previous to advance to the next or previous visible or selected key times. Right click the buttons to create hotkeys. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_goToKeyframe.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_goToKeyframe ml_goToKeyframe.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2012-07-23|First publish.|
|2|2013-10-29|Added hierarchy search, select keyframes, and a couple more options.|
|3|2014-03-01|adding category.|
|4|2018-02-17|Updating license to MIT.|
|5|2018-05-13|shelf support|
