---
layout: page
permalink: tool/ml_pivot/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_pivot.png) Pivot
Download [ml_pivot.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_pivot.py)

| Revision | 4 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Change the rotate pivot of animated nodes. This is not a pivot switcher, it changes the pivot for the whole animation but preserves position by baking translation on ones. Eventually I'd like to make it a bit smarter about how it bakes. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_pivot.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_pivot
ml_pivot.ui()
```

## Usage

 Run the UI. Select a node whose pivot you'd like to change, and press Edit Pivot. Your selection with change to handle, position this where you'd like the pivot to be and press Return. Or press ESC or select something else to cancel. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_pivot.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_pivot ml_pivot.ui() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Ui

 [Edit Pivot] : Creates a temporary node to positon for the new pivot. [Reset Pivot] : Rest the rotation pivot to zero. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">Edit Pivot</button>|Creates a temporary node to positon for the new pivot.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Reset Pivot</button>|Rest the rotation pivot to zero.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-06-21|First publish.|
|2|2017-06-26|update for pySide2, maya 2017|
|3|2017-07-17|initial support for attribute driven pivots|
|4|2018-02-17|Updating license to MIT.|
