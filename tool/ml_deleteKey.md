---
layout: page
permalink: tool/ml_deleteKey/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_deleteKey.png) Delete Key
Download [ml_deleteKey.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_deleteKey.py)

| Revision | 8 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 A more robust tool for deleting keyframes in Maya, including deleting keys on the current frame and which are visible in the graph editor. Alternately, delete selected channels. 

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

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_deleteKey.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_deleteKey ml_deleteKey.ui() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Ui

 [] Selected Keys : Delete the keys selected in the graph editor. [] Selected Channels : Delete all the keys on selected channels. (Unless overridden above) [] Visible in Graph Editor : Only delete keys that are visible in the graph editor. (Unless overridden above) [] Current Frame : Delete the keys on the current frame. (Unless overridden above) [] Delete Sub-Frames : Delete sub-frame keys surrounding the current frame. [Delete Keys] : Delete Keyframe. [Delete Channels] : Delete selected channels, or all keys on selected nodes. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

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
|8|2018-02-17|Updating license to MIT.|
