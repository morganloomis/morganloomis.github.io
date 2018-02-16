---
layout: page
permalink: tool/ml_controlLibrary/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_controlLibrary.png) Control Library
Download [ml_controlLibrary.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_controlLibrary.py)

| Revision | 4 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Export and import nurbs curves to be used as animation controls. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_controlLibrary.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_controlLibrary
ml_controlLibrary.ui()
```

## Usage

 Run the UI. The first time it is run, it will prompt to create a control repository directory if it doesn't find one. This is where control curves will be saved, and by default it will be in the same directory that the script is in. If you want them saved somewhere else, just set the REPOSITORY_PATH variable in this file. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_controlLibrary.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_controlLibrary ml_controlLibrary.ui() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Ui

 : Right-click for more options 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


| |Right-click for more options||

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-07-31|First publish.|
|2|2016-08-02|fixing function order for correct header generation.|
|3|2016-08-11|documentation and dependency update|
|4|2018-02-17|Updating license to MIT.|
