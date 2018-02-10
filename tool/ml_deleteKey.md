---
layout: page
permalink: tool/ml_deleteKey/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_deleteKey.png) Delete Key
Download [ml_deleteKey.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_deleteKey.py)

| Revision | 7 |
|---:|---|
| Last Update | 2014-03-01 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This is a more robust tool for deleting keyframes in Maya, including deleting keys on the current frame and which are visible in the graph editor. Alternately, delete selected channels.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_deleteKey.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_deleteKey
ml_deleteKey.ui()
```

## Usage

 Run the tool, select the options, and press the Delete Key button. Set the options and right click the button to create a hotkey or shelf button. If selected keys is unchecked, it will delete keys on the current frame regardless of key selection. Delete sub-frames will include keys which fall within half a frame of the current time. The second button operates on entire channels, and it will delete the channels that are selected, or all the channels on an object.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<input type="checkbox" checked="yes"> Selected Keys|Delete the keys selected in the graph editor.||
|---|---|---|
|<input type="checkbox" checked="yes"> Selected Channels|Delete all the keys on selected channels. (Unless overridden above)||
|<input type="checkbox" checked="yes"> Visible in Graph Editor|Only delete keys that are visible in the graph editor. (Unless overridden above)||
|<input type="checkbox" checked="yes"> Current Frame|Delete the keys on the current frame. (Unless overridden above)||
|<input type="checkbox" checked="yes"> Delete Sub-Frames|Delete sub-frame keys surrounding the current frame.||
|<button type="button">Delete Keys</button>|Delete Keyframe.|Right-click to create a shelf or hotkey|
|<button type="button">Delete Channels</button>|Delete selected channels, or all keys on selected nodes.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2012-03-29|First publish.|
|2|2012-03-29|Fixing bugs, published first version too quickly!|
|3|2012-04-14|minor bug fix|
|4|2012-07-23|Split into keys and channels, updated to use latest ml_utilities scripts, bug fixes.|
|5|2012-07-23|Fixing argument for KeySelection|
|6|2012-11-19|updated to new KeySelection|
|7|2014-03-01|adding category|
