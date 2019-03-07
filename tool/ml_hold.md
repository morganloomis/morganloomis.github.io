---
layout: page
permalink: tool/ml_hold/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_hold.png) Hold
Download [ml_hold.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/scripts/ml_hold.py)

| Revision | 8 |
|---:|---|
| Last Update | 2018-05-13 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Quickly create animation holds, either for individual poses or over a range of keys. Select a range of keys in the graph editor or the time slider, or match your current pose to the next or previous one. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_hold.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_hold
ml_hold.ui()
```

## Usage

 Run the UI. Press Next and Previous to match keys to the value of next or previous keyframes. Press Current or Average to turn a frame range into a hold. Current sets the hold to be the current value, and average sets the value to the average of all keys across the range. The range is determined by one of 3 things, in the following order: 1. Selected range in the time slider. 2. The highest and lowest selected keys in the graph editor. 3. If nothing is selected, the previous and next keys from the current time determine the range. If you have no keys selectd, all commands will operate only on curves that are visibile in the graph editor. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_hold.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_hold ml_hold.ui() 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Video

 http://www.youtube.com/watch?v=fOeDwGbuHFE 

## Ui

 [Hold Current] : Creates a hold for the selected range, or the surrounding keys, based on current frame. [Hold Average] : Creates a hold for the selected range, or the surrounding keys, based on average of keys. [<< Previous] : Matches selected key or current frame to the previous keyframe value. [Next >>] : Matches selected key or current frame to the next keyframe value. 

## UI Options


|<button type="button">Hold Current</button>|Creates a hold for the selected range, or the surrounding keys, based on current frame.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Hold Average</button>|Creates a hold for the selected range, or the surrounding keys, based on average of keys.|Right-click to create a shelf or hotkey|
|<button type="button"><< Previous</button>|Matches selected key or current frame to the previous keyframe value.|Right-click to create a shelf or hotkey|
|<button type="button">Next >></button>|Matches selected key or current frame to the next keyframe value.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1||First publish|
|4|2011-05-01|Updated to use ml_utilities|
|5|2014-03-01|adding category|
|6|2015-01-10|Fixed bug relating to KeySelection|
|7|2018-02-17|Updating license to MIT.|
|8|2018-05-13|shelf support|
