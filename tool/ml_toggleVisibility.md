---
layout: page
permalink: tool/ml_toggleVisibility/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_toggleVisibility.png) Toggle Visibility
Download [ml_toggleVisibility.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_toggleVisibility.py)

| Revision | 4 |
|---:|---|
| Last Update | 2018-05-12 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Toggle the visibility of an object off and on, regardless of the attribute's locked or keyable state. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_toggleVisibility.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_toggleVisibility
ml_toggleVisibility.main()
```

## Usage

 Select an object, and run the script. If the object is visible, it will be hidden, and vice-versa. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_toggleVisibility.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_toggleVisibility ml_toggleVisibility.main() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2015-05-14|Converted from mel.|
|3|2018-02-17|Updating license to MIT.|
|4|2018-05-12|Shelf support|
