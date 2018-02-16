---
layout: page
permalink: tool/ml_tangentWeight/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_tangentWeight.png) Tangent Weight
Download [ml_tangentWeight.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_tangentWeight.py)

| Revision | 4 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Scale keyframe tangents up or down incrementally without changing their angle. The result is basically increasing or decreasing the influence of a keyframe on the animCurve. Can also weight tangents toward the left or right, which increases influence on one side of the keyframe while reducing it on the other. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_tangentWeight.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_tangentWeight
ml_tangentWeight.ui()
```

## Usage

 Select Keyframes to affect, and press the desired button. To further affect the tangents, continue pressing the button to increment the weight until the desired weight is attained. This works well as a hotkey. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_tangentWeight.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_tangentWeight ml_tangentWeight.ui() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Ui

 [-] : Scale tangent down. [+] : Scale tangent up. [<] : Weight tangent toward the left. [>] : Weight tangent toward the right. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">-</button>|Scale tangent down.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">+</button>|Scale tangent up.|Right-click to create a shelf or hotkey|
|<button type="button"><</button>|Weight tangent toward the left.|Right-click to create a shelf or hotkey|
|<button type="button">></button>|Weight tangent toward the right.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-03-25|First publish.|
|2|2016-03-27|Fixed command name typo|
|3|2016-05-01|fixed error when nothing is selected.|
|4|2018-02-17|Updating license to MIT.|
