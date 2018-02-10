---
layout: page
permalink: tool/ml_controlLibrary/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_controlLibrary.png) Control Library
Download [ml_controlLibrary.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_controlLibrary.py)

| Revision | 3 |
|---:|---|
| Last Update | 2016-08-11 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This tool is for exporting and then importing nurbs curves to be used as animation controls.

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

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


| |Right-click for more options||

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-07-31|First publish.|
|2|2016-08-02|fixing function order for correct header generation.|
|3|2016-08-11|documentation and dependency update|
