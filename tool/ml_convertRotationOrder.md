---
layout: page
permalink: tool/ml_convertRotationOrder/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_convertRotationOrder.png) Convert Rotation Order
Download [ml_convertRotationOrder.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_convertRotationOrder.py)

| Revision | 5 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Change the rotation order of an object while preserving animation. When you want to change the rotation order of a control after you've already animated, or don't want to alter the pose of an object. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_convertRotationOrder.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_convertRotationOrder
ml_convertRotationOrder.ui()
```

## Usage

 Run the UI. Select the objects with rotation orders you want to change, and press the button for the desired rotation order. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_convertRotationOrder.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_convertRotationOrder ml_convertRotationOrder.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2011-10-08|First publish.|
|2|2012-03-12|Updated to work with non-keyed objects, added the tips button.|
|3|2012-08-04|Fixing bug with potential duplicate temp name.|
|4|2014-03-01|adding category|
|5|2018-02-17|Updating license to MIT.|
