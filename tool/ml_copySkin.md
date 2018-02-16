---
layout: page
permalink: tool/ml_copySkin/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_copySkin.png) Copy Skin
Download [ml_copySkin.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_copySkin.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Copy a skinCluster from one mesh to another, or to a selection of vertices. If no skin exists on the destination, one will be created with the same influences. Otherwise any missing influences will be added in order to copy accurate weights. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_copySkin.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_copySkin
ml_copySkin.ui()
```

## Usage

 Input a source mesh into the "Source Mesh" field by selecting a mesh and pressing the "Set Selected" button. Select destination meshes or vertices, and press the "Copy Skin" button. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_copySkin.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_copySkin ml_copySkin.ui() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Ui

 [Copy Skin] : Copy the Source Skin to selection. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">Copy Skin</button>|Copy the Source Skin to selection.||

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-10-31|First publish.|
|2|2018-02-17|Updating license to MIT.|
