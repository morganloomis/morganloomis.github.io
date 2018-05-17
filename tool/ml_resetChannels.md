---
layout: page
permalink: tool/ml_resetChannels/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_resetChannels.png) Reset Channels
Download [ml_resetChannels.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_resetChannels.py)

| Revision | 11 |
|---:|---|
| Last Update | 2018-05-13 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Set the selected channels in the channel box to their default values. If no channels are selected, resets all keyable channels. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_resetChannels.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_resetChannels
ml_resetChannels.main()
```

## Usage

 Select channels in the channel box, and run the command directly, as a hotkey or shelf button. Run command line to use the transformsOnly flag, in order to only reset transform attributes. The excludeChannels argument takes a list of channel names to exclude. The resetPuppetControl() command is a wrapper for resetting puppeteer controls by skipping certain settings attributes. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_resetChannels.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_resetChannels ml_resetChannels.main() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|5|2012-05-27|Added revision notes, updated to use ml_utilities, changed primary function to main() for consistency|
|6|2013-04-23|added transformsOnly and selected flags to support cgMonks|
|7|2014-03-01|adding category|
|8|2015-05-14|Added excludeChannels argument.|
|9|2015-05-16|argument update in order to be supported in puppet context menu.|
|10|2018-02-17|Updating license to MIT.|
|11|2018-05-13|shelf support|
