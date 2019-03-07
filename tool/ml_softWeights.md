---
layout: page
permalink: tool/ml_softWeights/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_softWeights.png) Soft Weights
Download [ml_softWeights.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/scripts/ml_softWeights.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Set cluster or skinCluster weights based on the current vertex soft selection. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_softWeights.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_softWeights
ml_softWeights.ui()
```

## Usage

 For clusters, just select vertices and adjust the desired soft selection, then press the button. For skinClusters, do the same, but additionally select the desired joint as well, then press the skinCluster button. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_softWeights.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_softWeights ml_softWeights.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-12-31|Initial publish|
|2|2018-02-17|Updating license to MIT.|
