---
layout: page
permalink: tool/ml_resetBind/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_resetBind.png) Reset Bind
Download [ml_resetBind.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_resetBind.py)

| Revision | 2 |
|---:|---|
| Last Update | 2018-02-17 |
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

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_resetBind.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_resetBind ml_resetBind.main() 

## License

 Copyright 2018 Morgan Loomis Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2014-03-02|First publish.|
|2|2018-02-17|Updating license to MIT.|
