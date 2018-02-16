---
layout: page
permalink: tool/ml_animCurveEditor/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_animCurveEditor.png) Anim Curve Editor
Download [ml_animCurveEditor.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_animCurveEditor.py)

| Revision | 4 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Various tools for editing animation curves, similar to video clip non-linear editing tools. Maya's tools for editing lots of keys can be slow or cumbersome, this is meant to be an alternative interface for editing lots of keyframes. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_animCurveEditor.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_animCurveEditor
ml_animCurveEditor.ui()
```

## Usage

 The "Act on Anim Curves In:" drop-down controls which animCurves are affected in the scene. The tabs organize the different types of tools: Offset: Slip curves in time. Cut: Cut sections of curves. Scale Time: Globally retime a curve Scale Value: Globally adjust the value of a curve. Clamp: Clamp keyframe values to a high or low value, for example to prevent a channel going below zero. Clean-Up: Tools for getting rid of keyframes that you may not want or need. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_animCurveEditor.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_animCurveEditor ml_animCurveEditor.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-02-29|First publish.|
|2|2016-05-01|Fixing command name typo.|
|3|2017-12-03|Adding "Insert Frame"|
|4|2018-02-17|Updating license to MIT.|
