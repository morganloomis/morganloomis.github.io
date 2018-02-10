---
layout: page
permalink: tool/ml_breakdown/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_breakdown.png) Breakdown
Download [ml_breakdown.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_breakdown.py)

| Revision | 2 |
|---:|---|
| Last Update | 2015-05-13 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Blend a keyframe or pose with the next or previous keys, essentially creating a breakdown pose that is weighted one way or the other.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_breakdown.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_breakdown
ml_breakdown.ui()
```

## Usage

 Press the "Breakdown Dragger" button to enter the dragger, and the cursor will turn into a hand. Left-click and hold in the viewport, and then drag either left or right to weight the key to the next or previous key. Press and hold the middle mouse button to weight the key toward or away from the average of the surrounding keys. Alternately, set the slider to the desired weight, and press the Next, Previous or Average buttons to increment the breakdown. Right click the buttons to assign to hotkeys. If you have no keys selected, the tool will act only on curves that are visibile in the graph editor. If there are no keys at the current frame, keys will be set.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<button type="button">Breakdown Dragger</button>|Drag in the viewport to weight a breakdown toward the next or previous frame.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button"><<</button>|Weight toward the previous frame.|Right-click to create a shelf or hotkey|
|<button type="button">Average</button>|Weight toward the average of the next and previous frame.|Right-click to create a shelf or hotkey|
|<button type="button">>></button>|Weight toward the next frame.|Right-click to create a shelf or hotkey|

## Video Tutorial
[![youtube](http://img.youtube.com/vi/D8yD4zbHTP8/0.jpg)](http://www.youtube.com/watch?v=D8yD4zbHTP8)
## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2015-05-13|First publish.|
|2|2015-05-13|Documentation updates.|
