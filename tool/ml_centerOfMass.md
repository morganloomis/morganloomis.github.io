---
layout: page
permalink: tool/ml_centerOfMass/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_centerOfMass.png) Center Of Mass
Download [ml_centerOfMass.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/scripts/ml_centerOfMass.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Create a locator that approximates the Center of Mass for the character. This locator can be live and simply used as reference, or you can transfer the root animation of your character to the center of mass, and then back again after you've adjusted any motion. This workflow is helpful for debugging action animation when a characters body needs to move in a believable way. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_centerOfMass.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_centerOfMass
ml_centerOfMass.ui()
```

## Usage

 Run the tool to launch the UI. Select the root control of your puppet. The tool may not error if you select something other than the root, but it may behave strangely, so it's up to you to choose the correct control. Then choose to either create a live COM node, or transfer your root animation to the center of mass. After transferring from Root to COM, you can then transfer back after editing. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_centerOfMass.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_centerOfMass ml_centerOfMass.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-12-05|First publish.|
|2|2018-02-17|Updating license to MIT.|
