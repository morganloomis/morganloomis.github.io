---
layout: page
permalink: tool/ml_centerOfMass/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_centerOfMass.png) Center Of Mass
Download [ml_centerOfMass.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_centerOfMass.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Create a locator that approximates the Center of Mass for the character. This locator can be live and simply used as reference, or you can transfer the root animation of your character to the center of mass, and then back again after you've adjusted any motion. This workflow is helpful for debugging action animation when a characters body needs to move in a believable way. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_centerOfMass.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_centerOfMass
ml_centerOfMass.ui()
```

## Usage

 Run the tool to launch the UI. Select the root control of your puppet. The tool may not error if you select something other than the root, but it may behave strangely, so it's up to you to choose the correct control. Then choose to either create a live COM node, or transfer your root animation to the center of mass. After transferring from Root to COM, you can then transfer back after editing. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_centerOfMass.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_centerOfMass ml_centerOfMass.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-12-05|First publish.|
|2|2018-02-17|Updating license to MIT.|
