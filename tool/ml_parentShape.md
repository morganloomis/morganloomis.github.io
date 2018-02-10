---
layout: page
permalink: tool/ml_parentShape/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_parentShape.png) Parent Shape
Download [ml_parentShape.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_parentShape.py)

| Revision | 1 |
|---:|---|
| Last Update | 2014-03-02 |
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

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<button type="button">Parent Shape</button>|Parent shape of the first selected object to the second|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2014-03-02|First publish.|
