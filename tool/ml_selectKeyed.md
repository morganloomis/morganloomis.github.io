---
layout: page
permalink: tool/ml_selectKeyed/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_selectKeyed.png) Select Keyed
Download [ml_selectKeyed.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_selectKeyed.py)

| Revision | 5 |
|---:|---|
| Last Update | 2014-03-01 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Select any node in an animated hierarchy, such as a puppet, and run the command to select all the nodes in the hierarchy that are keyed. If the selected object has a namespace, it will only return nodes in that namespace. The top node of the hierarchy is excluded.

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

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## Revision History

| Revision | Date | Note|
|---|---|---|
|3|2012-05-27|Added revision notes, changed primary function to main() for consistency|
|4|2012-06-10|Fixing small bug when selecting objects that aren't in a hierarchy.|
|5|2014-03-01|adding category|
