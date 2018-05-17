---
layout: page
permalink: tool/ml_lockAndHideAttributes/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_lockAndHideAttributes.png) Lock And Hide Attributes
Download [ml_lockAndHideAttributes.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_lockAndHideAttributes.py)

| Revision | 3 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Quickly set the locked and keyable state of attributes in the channel box. This tool is designed to be used as hotkeys for quickly locking and hiding attributes. It will operate on all visible attributes, unless specific channels are selected. When using to unhide attributes, it will unhide all standard transform attributes, and all user defined attributes. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_lockAndHideAttributes.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_lockAndHideAttributes
ml_lockAndHideAttributes.ui()
```

## Usage

 Run the UI, select channels in the channel box, and hit the appropriate button to lock, hide, unlock or unhide channels. Right click the buttons to create hotkeys or shelf buttons. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_lockAndHideAttributes.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_lockAndHideAttributes ml_lockAndHideAttributes.ui() 

## Ui

 [Lock] : Lock selected attributes. [Hide] : Hide selected attributes. [Lock and Hide] : Lock and hide selected attributes. [Unlock] : Unlock selected attributes. [Unhide] : Unhide all core attributes. [Unlock and Unhide] : Unlock and unhide selected attributes. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">Lock</button>|Lock selected attributes.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Hide</button>|Hide selected attributes.|Right-click to create a shelf or hotkey|
|<button type="button">Lock and Hide</button>|Lock and hide selected attributes.|Right-click to create a shelf or hotkey|
|<button type="button">Unlock</button>|Unlock selected attributes.|Right-click to create a shelf or hotkey|
|<button type="button">Unhide</button>|Unhide all core attributes.|Right-click to create a shelf or hotkey|
|<button type="button">Unlock and Unhide</button>|Unlock and unhide selected attributes.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2011-10-08|First publish.|
|2|2014-03-01|adding category|
|3|2018-02-17|Updating license to MIT.|
