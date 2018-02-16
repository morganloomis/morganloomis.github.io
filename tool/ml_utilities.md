---
layout: page
permalink: tool/ml_utilities/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_utilities.png) Utilities
Download [ml_utilities.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py)

| Revision | 32 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 A collection of support functions that are required by several of the tools in this library. The individual tools will tell you if this script is required. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_utilities.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_utilities
ml_utilities.main()
```

## Usage

 ml_utilities isn't a stand alone tool, and so it isn't meant to be used directly. However, you can certainly call these functions if they seem useful in your own scripts. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_utilities.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_utilities ml_utilities._showHelpCommand() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## UI Options


| |Right-click for more options||
|---|---|---|
| |Right-click for more options||
| |Right-click for more options||

## Revision History

| Revision | Date | Note|
|---|---|---|
|1||First publish|
|2|2011-05-04|Fixed error in frameRange.|
|3|2012-05-31|Adding Menu and Icon update to UI, adding KeyframeSelection object, and a few random utility functions.|
|4|2012-06-01|Fixing bug with UI icons|
|5|2012-07-23|Expanding and bug fixing Keyselection, added SkipUndo, minor bug fixes.|
|6|2012-07-23|KeySelection bug fix|
|7|2012-08-07|Minor bug with Keyselection, adding functions.|
|8|2012-11-06|Backwards incompatable update to KeySelection, and several new functions.|
|9|2013-10-29|Update to support more options for goToKeyframe, update to preserve isolateSelect.|
|10|2014-03-01|adding category, updating contact.|
|11|2014-03-08|Fixed keySelection bug with keyed channels.|
|12|2015-04-27|updated for ml_puppet support|
|13|2015-05-13|UI function updates|
|14|2015-05-16|minor update to setAnimValue|
|15|2015-05-18|Small bugfix in matchBake|
|16|2016-02-29|Support for animCurveEditor and fixing some old hotkey bugs.|
|17|2016-03-23|keySelection bug fix.|
|18|2016-05-05|Update matchBake to support tangent weights.|
|19|2016-06-02|temp patching hotkey issue with > 2015|
|20|2016-07-31|Update to MlUi to support subclassing.|
|21|2016-07-31|MlUi bug fixes.|
|21|2016-08-11|windows support for icons|
|22|2016-10-01|changing frameRange to return consistent results when returning timeline or selection.|
|23|2016-10-12|Tangent bug fixes for 2016.5|
|24|2016-10-31|Adding selection field to mlUI|
|25|2016-11-21|silly icon path bug|
|26|2016-12-05|Adding getSkinCluster|
|27|2016-12-10|Adding Vector class to remove euclid dependency|
|28|2017-03-20|bug fix and support for ml_puppet|
|29|2017-04-25|matchBake support input frames|
|30|2017-06-13|unify version test, isolate view update|
|31|2017-06-30|getCamera support for stereo camera|
|32|2018-02-17|Updating license to MIT.|