---
layout: page
permalink: tool/ml_copyAnim/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_copyAnim.png) Copy Anim
Download [ml_copyAnim.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_copyAnim.py)

| Revision | 5 |
|---:|---|
| Last Update | 2017-07-19 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Copy animation curves either completely or in part from one node or hierarchy to another.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_copyAnim.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_copyAnim
ml_copyAnim.ui()
```

## Usage

 Select the source and destination node (or top node) and press the button to either copy the selected node only, or the whole hierarchy underneath. Highlight the timeline if you want to copy just that part of the animation. Use the Copy to New Layer option if you want the curves copied into a new animation layer, in order to preserve the original animation, or to blend.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<input type="checkbox" checked="yes"> Copy To New Layer|Create a new animation layer to copy the curves into, preserving the original animation.||
|---|---|---|
|<button type="button">Copy Single</button>|Copy animation from one object to another.|Right-click to create a shelf or hotkey|
|<button type="button">Copy Hierarchy</button>|Uses name matching to copy animation across hierarchies.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2012-03-14|First publish.|
|2|2012-11-06|Adding layer option.|
|3|2012-11-28|remove debug print|
|4|2014-03-01|Adding category and fixing bad argument name.|
|5|2017-07-19|support for non-namespaced hierarchies, transferring rotateOrder|
