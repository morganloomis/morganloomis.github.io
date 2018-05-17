---
layout: page
permalink: tool/ml_graphEditorMask/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_graphEditorMask.png) Graph Editor Mask
Download [ml_graphEditorMask.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_graphEditorMask.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Quickly mask the visible curves in the graph editor. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_graphEditorMask.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_graphEditorMask
ml_graphEditorMask.ui()
```

## Usage

 Works best as hotkeys or marking menus for quick masking. Select Translate to isolate all the translate channels of the nodes you have selected. Select X to further isolate all translateX curves. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_graphEditorMask.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_graphEditorMask ml_graphEditorMask.ui() 

## Ui

 [Channel Box] : Isolate curves based on channels highlighted in the channel box [Selected] : Isolate the selected curves [All] : Show all animation curves [Translate] : Isolate translation curves [Rotate] : Isolate rotation curves [Scale] : Isolate scale curves [X] : Isolate X axis curves [Y] : Isolate Y axis curves [Z] : Isolate Z axis curves [null] : Isolate Z axis curves [TRS] : Isolate Z axis curves [Custom] : Isolate Z axis curves 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">Channel Box</button>|Isolate curves based on channels highlighted in the channel box|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Selected</button>|Isolate the selected curves|Right-click to create a shelf or hotkey|
|<button type="button">All</button>|Show all animation curves|Right-click to create a shelf or hotkey|
|<button type="button">Translate</button>|Isolate translation curves|Right-click to create a shelf or hotkey|
|<button type="button">Rotate</button>|Isolate rotation curves|Right-click to create a shelf or hotkey|
|<button type="button">Scale</button>|Isolate scale curves|Right-click to create a shelf or hotkey|
|<button type="button">X</button>|Isolate X axis curves|Right-click to create a shelf or hotkey|
|<button type="button">Y</button>|Isolate Y axis curves|Right-click to create a shelf or hotkey|
|<button type="button">Z</button>|Isolate Z axis curves|Right-click to create a shelf or hotkey|
|<button type="button">null</button>|Isolate Z axis curves|Right-click to create a shelf or hotkey|
|<button type="button">TRS</button>|Isolate Z axis curves|Right-click to create a shelf or hotkey|
|<button type="button">Custom</button>|Isolate Z axis curves|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-05-31|First publish.|
|2|2018-02-17|Updating license to MIT.|
