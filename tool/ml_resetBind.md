---
layout: page
permalink: tool/ml_resetBind/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_resetBind.png) Reset Bind
Download [ml_resetBind.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_resetBind.py)

| Revision | 1 |
|---:|---|
| Last Update | 2014-03-02 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Quickly remove and recreate a skinCluster while maintaining history. Essentially this allows you to "reset" the skin cluster after you've moved some joints. It also deletes the original bindPose node.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_resetBind.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_resetBind
ml_resetBind.main()
```

## Usage

 Select the skinned meshes you'd like to reset, and run the command.

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2014-03-02|First publish.|
