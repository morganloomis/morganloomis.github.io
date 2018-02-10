---
layout: page
title: Arc Tracer
permalink: tool/ml_arcTracer/
---

Download ![icon](https://raw.githubusercontent.com/morganloomis/ml_tools/master/icons//ml_arcTracer.png) [ml_arcTracer](https://raw.githubusercontent.com/morganloomis/ml_tools/master/ml_arcTracer.py).py

| Revision | 6 |
|---:|---|
| Last Update | 2017-06-30 |
| License | [MIT](https://opensource.org/licenses/MIT) |

## Description

 This tool is a substitute for tracing arcs on your screen by hand with a marker. It creates a thick line to represent the path of an object, either as an overlay on your camera view, or in world space. It's a bake process; like a marker it doesn't update interactively. Lines are colored randomly, to distinguish between multiple traces. Frames are marked along the arc as black dots, with keyframes colored red, and the current frame is highlighted.

## Installation

Copy this file into your maya scripts directory, for example:

`C:/Documents and Settings/user/My Documents/maya/scripts/ml_arcTracer.py`

Run the tool in a python shell or shelf button by importing the module, 
and then calling the primary function:

```python
import ml_arcTracer
ml_arcTracer.ui()
```

## Usage

 Run the UI, and press the buttons to choose the action.

## Requirements

 This script requires the ml_utilities module, which can be downloaded here: http://morganloomis.com/wiki/tools.html#ml_utilities

## UI Options


|<button type="button">Trace Camera</button>|Trace an arc as an overlay over the current camera.|Right-click to create a shelf or hotkey|
|---|---|---|
|<button type="button">Trace World</button>|Trace an arc in world space.|Right-click to create a shelf or hotkey|
|<button type="button">Retrace Previous</button>|Retrace the previously traced arc.|Right-click to create a shelf or hotkey|
|<button type="button">Clear Arcs</button>|Clear all arcs.|Right-click to create a shelf or hotkey|

## Video Tutorial
[![youtube](http://img.youtube.com/vi/xLA1aglvPYM/0.jpg)](http://www.youtube.com/watch?v=xLA1aglvPYM)
## Revision History

| Revision | Date | Note|
|---|---|---|
|1|2011-05-01|First publish|
|2|2011-05-14|minor bug fix involving error with duplicate names|
|3|2011-05-14|Revision notes update.|
|4|2014-03-01|adding category|
|5|2016-12-10|removing euclid dependency|
|6|2017-06-30|Fixing bug with moving cameras, adding line width|

<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="heading">
<tr bgcolor="#7799ee">
<td valign=bottom>&nbsp;<br>
<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong><a href="ml_arcTracer.html"><font color="#ffffff">ml_arcTracer</font></a>.py</strong></big></big></font></td
><td align=right valign=bottom
><font color="#ffffff" face="helvetica, arial"><a href=".">index</a><br><a href="/Users/morganloomis/Google Drive/morganloomis.github.io/tool/ml_arcTracer.py">/Users/morganloomis/Google Drive/morganloomis.github.io/tool/ml_arcTracer.py</a></font></td></tr></table>
    <p><tt>#&nbsp;&nbsp;&nbsp;-=&nbsp;ml_arcTracer.py&nbsp;=-<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;__&nbsp;&nbsp;&nbsp;by&nbsp;Morgan&nbsp;Loomis<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;____&nbsp;___&nbsp;&nbsp;/&nbsp;/&nbsp;&nbsp;<a href="http://morganloomis.com">http://morganloomis.com</a><br>
#&nbsp;&nbsp;&nbsp;&nbsp;/&nbsp;__&nbsp;`__&nbsp;\/&nbsp;/&nbsp;&nbsp;Licensed&nbsp;under&nbsp;Creative&nbsp;Commons&nbsp;BY-SA<br>
#&nbsp;&nbsp;&nbsp;/&nbsp;/&nbsp;/&nbsp;/&nbsp;/&nbsp;/&nbsp;/&nbsp;&nbsp;<a href="http://creativecommons.org/licenses/by-sa/3.0/">http://creativecommons.org/licenses/by-sa/3.0/</a><br>
#&nbsp;&nbsp;/_/&nbsp;/_/&nbsp;/_/_/&nbsp;&nbsp;_________&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;/_________/&nbsp;&nbsp;Revision&nbsp;6,&nbsp;2017-06-30<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_______________________________<br>
#&nbsp;-&nbsp;-/__&nbsp;Installing&nbsp;Python&nbsp;Scripts&nbsp;__/-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;<br>
#&nbsp;<br>
#&nbsp;Copy&nbsp;this&nbsp;file&nbsp;into&nbsp;your&nbsp;maya&nbsp;scripts&nbsp;directory,&nbsp;for&nbsp;example:<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;C:/Documents&nbsp;and&nbsp;Settings/user/My&nbsp;Documents/maya/scripts/ml_arcTracer.py<br>
#&nbsp;<br>
#&nbsp;Run&nbsp;the&nbsp;tool&nbsp;by&nbsp;importing&nbsp;the&nbsp;module,&nbsp;and&nbsp;then&nbsp;calling&nbsp;the&nbsp;primary&nbsp;function.<br>
#&nbsp;From&nbsp;python,&nbsp;this&nbsp;looks&nbsp;like:<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;import&nbsp;ml_arcTracer<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ml_arcTracer.<a href="#-ui">ui</a>()<br>
#&nbsp;From&nbsp;MEL,&nbsp;this&nbsp;looks&nbsp;like:<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;python("import&nbsp;ml_arcTracer;ml_arcTracer.<a href="#-ui">ui</a>()");<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_________________<br>
#&nbsp;-&nbsp;-/__&nbsp;Description&nbsp;__/-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;<br>
#&nbsp;<br>
#&nbsp;This&nbsp;tool&nbsp;is&nbsp;a&nbsp;substitute&nbsp;for&nbsp;tracing&nbsp;arcs&nbsp;on&nbsp;your&nbsp;screen&nbsp;by&nbsp;hand&nbsp;with&nbsp;a&nbsp;marker.<br>
#&nbsp;It&nbsp;creates&nbsp;a&nbsp;thick&nbsp;line&nbsp;to&nbsp;represent&nbsp;the&nbsp;path&nbsp;of&nbsp;an&nbsp;object,&nbsp;either&nbsp;as&nbsp;an&nbsp;overlay&nbsp;on&nbsp;your&nbsp;camera&nbsp;view,<br>
#&nbsp;or&nbsp;in&nbsp;world&nbsp;space.&nbsp;It's&nbsp;a&nbsp;bake&nbsp;process;&nbsp;like&nbsp;a&nbsp;marker&nbsp;it&nbsp;doesn't&nbsp;update&nbsp;interactively.<br>
#&nbsp;Lines&nbsp;are&nbsp;colored&nbsp;randomly,&nbsp;to&nbsp;distinguish&nbsp;between&nbsp;multiple&nbsp;traces.<br>
#&nbsp;Frames&nbsp;are&nbsp;marked&nbsp;along&nbsp;the&nbsp;arc&nbsp;as&nbsp;black&nbsp;dots,&nbsp;with&nbsp;keyframes&nbsp;colored&nbsp;red,&nbsp;and<br>
#&nbsp;the&nbsp;current&nbsp;frame&nbsp;is&nbsp;highlighted.<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;___________<br>
#&nbsp;-&nbsp;-/__&nbsp;Usage&nbsp;__/-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;<br>
#&nbsp;<br>
#&nbsp;Run&nbsp;the&nbsp;UI,&nbsp;and&nbsp;press&nbsp;the&nbsp;buttons&nbsp;to&nbsp;choose&nbsp;the&nbsp;action.<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;____________________<br>
#&nbsp;-&nbsp;-/__&nbsp;Video&nbsp;Tutorial&nbsp;__/-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;<br>
#&nbsp;<br>
#&nbsp;<a href="http://www.youtube.com/watch?v=xLA1aglvPYM">http://www.youtube.com/watch?v=xLA1aglvPYM</a><br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;________________<br>
#&nbsp;-&nbsp;-/__&nbsp;UI&nbsp;Options&nbsp;__/-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;<br>
#&nbsp;<br>
#&nbsp;[Trace&nbsp;Camera]&nbsp;:&nbsp;Trace&nbsp;an&nbsp;arc&nbsp;as&nbsp;an&nbsp;overlay&nbsp;over&nbsp;the&nbsp;current&nbsp;camera.<br>
#&nbsp;[Trace&nbsp;World]&nbsp;:&nbsp;Trace&nbsp;an&nbsp;arc&nbsp;in&nbsp;world&nbsp;space.<br>
#&nbsp;[Retrace&nbsp;Previous]&nbsp;:&nbsp;Retrace&nbsp;the&nbsp;previously&nbsp;traced&nbsp;arc.<br>
#&nbsp;[Clear&nbsp;Arcs]&nbsp;:&nbsp;Clear&nbsp;all&nbsp;arcs.<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;__________________<br>
#&nbsp;-&nbsp;-/__&nbsp;Requirements&nbsp;__/-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;<br>
#&nbsp;<br>
#&nbsp;This&nbsp;script&nbsp;requires&nbsp;the&nbsp;ml_utilities&nbsp;module,&nbsp;which&nbsp;can&nbsp;be&nbsp;downloaded&nbsp;here:<br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="http://morganloomis.com/wiki/tools.html#ml_utilities">http://morganloomis.com/wiki/tools.html#ml_utilities</a><br>
#&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;__________<br>
#&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;-&nbsp;/_&nbsp;Enjoy!&nbsp;_/-&nbsp;-&nbsp;-</tt></p>
<p>
<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
<tr bgcolor="#aa55cc">
<td colspan=3 valign=bottom>&nbsp;<br>
<font color="#ffffff" face="helvetica, arial"><big><strong>Modules</strong></big></font></td></tr>
    
<tr><td bgcolor="#aa55cc"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
<td width="100%"><table width="100%" summary="list"><tr><td width="25%" valign=top><a href="maya.OpenMaya.html">maya.OpenMaya</a><br>
<a href="math.html">math</a><br>
</td><td width="25%" valign=top><a href="maya.cmds.html">maya.cmds</a><br>
<a href="maya.mel.html">maya.mel</a><br>
</td><td width="25%" valign=top><a href="random.html">random</a><br>
<a href="ml_utilities.html">ml_utilities</a><br>
</td><td width="25%" valign=top></td></tr></table></td></tr></table><p>
<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
<tr bgcolor="#eeaa77">
<td colspan=3 valign=bottom>&nbsp;<br>
<font color="#ffffff" face="helvetica, arial"><big><strong>Functions</strong></big></font></td></tr>
    
<tr><td bgcolor="#eeaa77"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
<td width="100%"><dl><dt><a name="-applyBrush"><strong>applyBrush</strong></a>(curve, parent)</dt><dd><tt>Simply&nbsp;applies&nbsp;the&nbsp;paint&nbsp;effects&nbsp;brush&nbsp;to&nbsp;the&nbsp;curve&nbsp;with&nbsp;the&nbsp;settings&nbsp;we&nbsp;want.</tt></dd></dl>
 <dl><dt><a name="-clearArcs"><strong>clearArcs</strong></a>(*args)</dt><dd><tt>Simply&nbsp;deletes&nbsp;the&nbsp;arc&nbsp;group&nbsp;by&nbsp;name.</tt></dd></dl>
 <dl><dt><a name="-getWorldValueAtFrame"><strong>getWorldValueAtFrame</strong></a>(attr, frame)</dt></dl>
 <dl><dt><a name="-retraceArc"><strong>retraceArc</strong></a>(*args)</dt><dd><tt>Reads&nbsp;the&nbsp;global&nbsp;variables&nbsp;to&nbsp;trace&nbsp;the&nbsp;previous&nbsp;selection&nbsp;and&nbsp;settings.</tt></dd></dl>
 <dl><dt><a name="-setLineWidthCallback"><strong>setLineWidthCallback</strong></a>(slider, *args)</dt></dl>
 <dl><dt><a name="-traceArc"><strong>traceArc</strong></a>(space<font color="#909090">='camera'</font>)</dt><dd><tt>The&nbsp;main&nbsp;function&nbsp;for&nbsp;creating&nbsp;the&nbsp;arc.</tt></dd></dl>
 <dl><dt><a name="-traceCamera"><strong>traceCamera</strong></a>(*args)</dt><dd><tt>Wrapper&nbsp;for&nbsp;tracing&nbsp;in&nbsp;camera&nbsp;space</tt></dd></dl>
 <dl><dt><a name="-traceWorld"><strong>traceWorld</strong></a>(*args)</dt><dd><tt>Wrapper&nbsp;for&nbsp;tracing&nbsp;in&nbsp;world&nbsp;space</tt></dd></dl>
 <dl><dt><a name="-ui"><strong>ui</strong></a>()</dt><dd><tt>User&nbsp;interface&nbsp;for&nbsp;arc&nbsp;tracer</tt></dd></dl>
</td></tr></table><p>
<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
<tr bgcolor="#55aa55">
<td colspan=3 valign=bottom>&nbsp;<br>
<font color="#ffffff" face="helvetica, arial"><big><strong>Data</strong></big></font></td></tr>
    
<tr><td bgcolor="#55aa55"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
<td width="100%"><strong>__author__</strong> = 'Morgan Loomis'<br>
<strong>__category__</strong> = 'animationScripts'<br>
<strong>__license__</strong> = 'Creative Commons Attribution-ShareAlike'<br>
<strong>__revision__</strong> = 6</td></tr></table><p>
<table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
<tr bgcolor="#7799ee">
<td colspan=3 valign=bottom>&nbsp;<br>
<font color="#ffffff" face="helvetica, arial"><big><strong>Author</strong></big></font></td></tr>
    
<tr><td bgcolor="#7799ee"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
<td width="100%">Morgan&nbsp;Loomis</td></tr></table>