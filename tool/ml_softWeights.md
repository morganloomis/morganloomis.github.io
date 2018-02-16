---
layout: page
permalink: tool/ml_softWeights/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_softWeights.png) Soft Weights
Download [ml_softWeights.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_softWeights.py)

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

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_softWeights.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_softWeights ml_softWeights.ui() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-12-31|Initial publish|
|2|2018-02-17|Updating license to MIT.|
