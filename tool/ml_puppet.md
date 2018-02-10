---
layout: page
permalink: tool/ml_puppet/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_puppet.png) Puppet
Download [ml_puppet.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_puppet.py)

| Revision | 23 |
|---:|---|
| Last Update | 2017-07-07 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 Support tools for puppets created by http://morganloomis.com/puppeteer

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_puppet.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_puppet
ml_puppet.main()
```

## Usage

 Launch the UI to see the options available. Press a button to make a selection or run a command. Right click buttons to create a hotkey for that option. All options are selection-sensitive, so for example if you have two puppets referenced into a scene, and select any part of one of them and run selectControls, it will select all the controls for that puppet only. With nothing selected it will select all controls in the scene. For Fk/Ik switching, select any part of the element you want to switch. So for an arm, you can select the ik hand control, the fk shoulder, the pole vector, and either way it will know to do the switch for that arm.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2013-03-10|First publish, fkIk switching only.|
|2|2014-02-24|Added selection scripts, UI, and updated for latest version of Puppeteer.|
|3|2014-03-01|adding category|
|4|2015-04-27|First major support for puppet marking menu.|
|5|2015-04-27|temp node clean up bug fixed.|
|6|2015-05-14|Space switch bake bug fixed.|
|7|2015-05-18|Minor bugfixes.|
|8|2015-06-23|puppet context menu fix for windows paths|
|9|2015-11-18|Updated fk ik switching code for latest puppeteer|
|10|2016-09-25|Minor KeyError bug fix.|
|11|2017-02-08|zero out pole twist when matching to ik|
|12|2017-02-21|fixing stepped tangents on ik switch attribute|
|13|2017-03-28|mirroring and visibility sets|
|14|2017-03-28|removing hide all sets, maya not allow|
|15|2017-04-06|Context menu bug fixes and additional features.|
|16|2017-04-23|Space Switch context menu bug fix|
|17|2017-04-25|FK IK switching keying update|
|18|2017-05-24|search higher for mirrored nodes when matching|
|19|2017-06-04|adding puppet settings attributes|
|20|2017-06-13|space switch matching bug fix|
|21|2017-06-29|full context menu for puppet node|
|22|2017-06-30|proper testing for puppet|
|23|2017-07-07|space switch and mirroring bugs|
