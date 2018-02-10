---
layout: page
permalink: tool/ml_setKey/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_setKey.png) Set Key
Download [ml_setKey.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_setKey.py)

| Revision | 9 |
|---:|---|
| Last Update | 2014-03-01 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This is a more robust tool for setting keyframes in Maya, including setting keys on selected channels, keyed channels, and several other options.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_setKey.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_setKey
ml_setKey.ui()
```

## Usage

 Run the tool, select the options, and press the Set Key button. Alternately, set the options and press the "Create Hotkey" button to turn the current functionality into a hotkey.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<input type="checkbox" checked="yes"> Selected Channels|Only key channels that are selected in the Channel Box||
|---|---|---|
|<input type="checkbox" checked="yes"> Visible in Graph Editor|Only key curves visible in Graph Editor||
|<input type="checkbox" checked="yes"> Key Only Keyed Channels|Only set keys on channels that are already keyed||
|<input type="checkbox" checked="yes"> Delete Sub-Frames|Delete sub-frame keys surrounding the current frame||
|<input type="checkbox" checked="yes"> Insert Key|Insert key (preserve tangents)||
|<input type="checkbox" checked="yes"> Key Shapes|Set keyframes on shapes||
|<button type="button">Set Key</button>|Set a keyframe.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|4|2012-03-11|Added revision notes, updated to use ml_utilities, fixed a bug where tangents weren't being preserved, and fixed middle-mouse dragging.|
|5|2012-03-26|Updated delete sub-frame option to work with other frame rates|
|6|2012-07-23|Bug fixes.|
|7|2012-08-07|Updating in parallel with ml_utilities to fix bug with keying keyed shapes.|
|8|2012-11-19|updating to new KeySelection|
|9|2014-03-01|adding category|
