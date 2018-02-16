---
layout: page
permalink: tool/ml_frameGraphEditor/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_frameGraphEditor.png) Frame Graph Editor
Download [ml_frameGraphEditor.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_frameGraphEditor.py)

| Revision | 5 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Frame the graph editor nicely based on the time slider range or the selected keys. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_frameGraphEditor.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_frameGraphEditor
ml_frameGraphEditor.main()
```

## Usage

 Alternately, if you want the result to be centered on the current time, use the command:  ml_frameGraphEditor.main(centerCurrentTime=True) For best results, assign this command to a hotkey. The main() function is a replacement for fitPanel -selected, so it can be used to replace the standard "f" hotkey. It frames the graph editor if the graph editor is in focus, otherwise it falls back to the default MEL framing command. If you want a command that just frames the graph editor and nothing else, use the frameGraphEditor() function. 

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_utilities.py 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_frameGraphEditor.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_frameGraphEditor ml_frameGraphEditor.main() 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-05-07|First publish.|
|2|2016-05-08|Frame values correctly for given frame range, option to center on current time.|
|3|2016-05-09|Updated to support graph editor visibility, now requires ml_utilities.|
|4|2016-05-10|Wrapping fitPanel, updating header info.|
|5|2018-02-17|Updating license to MIT.|
