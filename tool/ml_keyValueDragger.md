---
layout: page
permalink: tool/ml_keyValueDragger/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_keyValueDragger.png) Key Value Dragger
Download [ml_keyValueDragger.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_keyValueDragger.py)

| Revision | 5 |
|---:|---|
| Last Update | 2018-05-14 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Scale keyframes to their default value by dragging in the viewport. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_keyValueDragger.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_keyValueDragger
ml_keyValueDragger.drag()
```

## Usage

 Run the tool, and the cursor will turn into a hand. Left-click and hold in the viewport, and then drag either left or right to scale the key value up or down. If you have no keys selectd, the tool will act only on curves that are visibile in the graph editor. If there are no keys at the current frame, keys will be set. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_keyValueDragger.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_keyValueDragger ml_keyValueDragger.drag() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|2|2014-03-01|Added revision notes, adding category|
|3|2016-05-01|Bug fix|
|4|2016-05-02|Actual bug fix|
|5|2018-05-14|Shelf support.|
