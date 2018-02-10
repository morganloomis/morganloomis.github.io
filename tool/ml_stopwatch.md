---
layout: page
permalink: tool/ml_stopwatch/
---

# ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_stopwatch.png) Stopwatch
Download [ml_stopwatch.py](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_stopwatch.py)

| Revision | 3 |
|---:|---|
| Last Update | 2016-05-01 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This is a tool for helping to plan out the timing of a shot. It's a simple timer that records the timing of button clicks, and then reports them in a UI that allows you to record notes for individual beats and navigate through them in the timeslider.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_stopwatch.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_stopwatch
ml_stopwatch.ui()
```

## Usage

 Run the UI, and then click the big button to start recording time. Once recording has begun, continue clicking the big button to record the timing of beats. When you're done recording, click the stop button to stop recording and open up the results UI. From there you can change the start frame if you want a different reference point for your timing. Click the individual frame buttons or the previous and next buttons to navigate between the beats. Use the text fields to write notes about specific beats.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<input type="checkbox" checked="yes"> Round to nearest frame|Only whole number frames||
|---|---|---|
|<button type="button">Stop</button>|Stop the recording.||
|<button type="button"><< Previous</button>|Go to the previous frame in the list.||
|<button type="button">Next >></button>|Go to the next frame in the list.||

## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2012-06-04|First publish.|
|2|2014-03-01|adding category|
|3|2016-05-01|Fixing go to frame buttons import error.|
