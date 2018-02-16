---
layout: page
permalink: tool/ml_selectKeyed/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_selectKeyed.png) Select Keyed
Download [ml_selectKeyed.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_selectKeyed.py)

| Revision | 6 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Select all keyed nodes within a puppet. Select any node in an animated hierarchy, such as a puppet, and run the command to select all the nodes in the hierarchy that are keyed. If the selected object has a namespace, it will only return nodes in that namespace. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_selectKeyed.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_selectKeyed
ml_selectKeyed.main()
```

## Usage

 Select a node in an animated hierarchy, and run the command directly, as a hotkey or shelf button. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_selectKeyed.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_selectKeyed ml_selectKeyed.main() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|3|2012-05-27|Added revision notes, changed primary function to main() for consistency|
|4|2012-06-10|Fixing small bug when selecting objects that aren't in a hierarchy.|
|5|2014-03-01|adding category|
|6|2018-02-17|Updating license to MIT.|
