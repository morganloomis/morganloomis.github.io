---
layout: page
permalink: tool/ml_toolbox/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_toolbox.png) Toolbox
Download [ml_toolbox.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_toolbox.py)

| Revision | 6 |
|---:|---|
| Last Update | 2018-02-17 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Create custom menus in Maya's main menu bar for organizing scripts, just by putting them into directories. Insert tools into the existing maya menus, or add entirely new menus. 

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_toolbox.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_toolbox
ml_toolbox.main()
```

## Usage

 Make sure the ml_toolbox_menu folder is in your scripts directory or some other python path. Run the command mentioned above, or for best results, add the command to your scripts/userSetup.mel file, like so:  python('import ml_toolbox;ml_toolbox.main()'); To add a script to the menu, create folders and sub-folders in the ml_toolbox_menu directory. If you add a folder that is named the same as a maya menu, the tools in that folder will be added to the maya menu, rather than a new menu. For MEL scripts to work, the main global proc needs to be the same name as the file. For python scripts, the main function needs to be "main" or "ui" 

## Installation

 Copy this file into your maya scripts directory, for example: C:/Documents and Settings/user/My Documents/maya/scripts/ml_toolbox.py Run the tool in a python shell or shelf button by importing the module, and then calling the primary function: import ml_toolbox ml_toolbox.main() 

## Advanced

 If you have large menus and you don't like all the printing (if it's slowing startup), you can remove the verbose flag from Toolbox call in the main() function to suppress it. For python scripts, there's a few extra things you can do to get the most out of this tool. If you want any additional functions to be searched for besides main() etc, add them to the functionList variable below. They are sorted in search order. You can add an optional insertAfter variable to a script to have its menu item inserted after an existing menuItem in a maya menu. See the bundled scripts for examples of this. If you'd like to automatically set up a hotkey for a tool, add a hotkey variable to script file with the value set to the modifier+hotkey button. (See the bundled create/snapLocator for an example of this.) 

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2016-01-31|First publish.|
|2|2016-02-01|Fixing Windows compatibility|
|3|2016-03-07|more windows path support|
|4|2016-03-23|Fixing slash bug in some windows cases.|
|5|2016-12-10|Fixing print, and auto creation of __init__ files on windows.|
|6|2018-02-17|Updating license to MIT.|
