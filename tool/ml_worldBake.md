---
layout: page
permalink: tool/ml_worldBake/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_worldBake.png) World Bake
Download [ml_worldBake.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_worldBake.py)

| Revision | 15 |
|---:|---|
| Last Update | 2018-07-18 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Temporarily bake animation to locators in world (or custom) space. Use this tool to preserve the worldspace position of animation when you need to make positional changes to an object's parent. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_worldBake.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_worldBake
ml_worldBake.ui()
```

## Usage

 Run the tool, select the objects, then press the "To Locators" button. When you're ready to bake back, select the locators and press the "From Locators" button. Checking "Bake on Ones" will bake every frame, otherwise the keytimes will be derived from the original animation. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_worldBake.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_worldBake ml_worldBake.ui() 

## Ui

 [Bake Selection To Locators] : Bake selected object to locators specified space. [Bake Selected Locators Back To Objects] : Bake from selected locators back to their source objects. [Re-Parent Animated] : Parent all selected nodes to the last selection. [Un-Parent Animated] : Parent all selected to world. [Bake Selected] : Bake from the first selected object directly to the second. [Bake Selected With Offset] : Bake from the first selected object directly to the second, maintaining offset. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## UI Options


|<button type="button">Bake Selection To Locators</button>|Bake selected object to locators specified space.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Bake Selected Locators Back To Objects</button>|Bake from selected locators back to their source objects.|Right-click to create a shelf or hotkey|
|<button type="button">Re-Parent Animated</button>|Parent all selected nodes to the last selection.|Right-click to create a shelf or hotkey|
|<button type="button">Un-Parent Animated</button>|Parent all selected to world.|Right-click to create a shelf or hotkey|
|<button type="button">Bake Selected</button>|Bake from the first selected object directly to the second.|Right-click to create a shelf or hotkey|
|<button type="button">Bake Selected With Offset</button>|Bake from the first selected object directly to the second, maintaining offset.|Right-click to create a shelf or hotkey|

## Revision History

| Revision | Date | Note|
|---|---|---|
|1||First publish|
|6||Updated to use ml_utilities. Changed from direct constraint to constrained duplicate node.|
|7|2011-05-13|fixed a bug with transferring certain types of tangents.|
|8|2011-05-14|fixed error baking things with transforms locked or hidden|
|9|2012-06-13|fixing duplicate name bug, adding more error checking.|
|10|2012-11-15|Converting UI to tabs, adding camera and explicit options.|
|11|2014-03-01|adding category|
|12|2015-05-14|Baking broken out and moved to ml_utilities|
|13|2018-02-17|Updating license to MIT.|
|14|2018-06-27|parenting options and marking menu|
|15|2018-07-18|marking menu|
