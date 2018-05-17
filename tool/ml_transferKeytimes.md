---
layout: page
permalink: tool/ml_transferKeytimes/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_transferKeytimes.png) Transfer Keytimes
Download [ml_transferKeytimes.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_transferKeytimes.py)

| Revision | 3 |
|---:|---|
| Last Update | 2018-05-13 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Copy keytimes from one node to another. Animation isn't fundamentally changed, but keys will be added or deleted. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_transferKeytimes.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_transferKeytimes
ml_transferKeytimes.main()
```

## Usage

 Select the source and destination nodes, keytimes will be transferred from first to second selection. Run the command. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_transferKeytimes.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_transferKeytimes ml_transferKeytimes.main() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2014-03-02|First publish.|
|2|2018-02-17|Updating license to MIT.|
|3|2018-05-13|shelf support|
