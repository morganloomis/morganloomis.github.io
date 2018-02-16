---
layout: page
permalink: tool/ml_parentShape/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_parentShape.png) Parent Shape
Download [ml_parentShape.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_parentShape.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Reparent shape nodes to a different transform, or unparent shape nodes to a new transform. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_parentShape.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_parentShape
ml_parentShape.ui()
```

## Usage

 For parenting shapes, select the child and then the parent, just as if you were parenting nodes normally, and run the command. For unparenting shapes, select any number of nodes and run the command, just as if you were unparenting nodes from a hierarchy. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_parentShape.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_parentShape ml_parentShape.ui() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Ui

 [Parent Shape] : Parent shape of the first selected object to the second 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">Parent Shape</button>|Parent shape of the first selected object to the second|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2014-03-02|First publish.|
|2|2018-02-17|Updating license to MIT.|