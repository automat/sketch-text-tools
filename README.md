#sketch-text-tools

This plugin eases working with typography in Sketch. It enables displaying font metrics, aligning text-layers to text-layers or other layers relative to baseline, x-height and cap-height. Baseline grid reference layers can be extracted from text-layers or build with custom configurations. Text-layers can be split into several columns with specific gutter widths.

###Commands

[**1. Create Font Metrics**](#1)  
[**2. Align Text**](#2)   
[**3. Create Baseline Layer**](#3)   
[**4. Count Characters Per Line**](#4)   
[**5. Columnize**](#5)   

---

<a name="1"/>
##1. Create Font Metrics

![Font Metric](./text-tools-font-metrics.gif)

Extracts font metrics from text layer fonts. Creates a reference layer displaying the fonts baseline, ascent, descent, x-height and cap-height as well as the default line-height relative to the font-size used ( *blue* ). Furthermore the x-height and cap-height center get displayed ( *red* ). Metrics get extracted for the first line of a text layer. width equals text-layer width.

<a name="2"/>
##2. Align Text

![Align text](text-tools-align.gif)
![Align text](text-tools-alignment-panel.png)

Aligns selected text-layers and non-text-layers. Alignment is based on a metric reference, e.g. centering all layers on a shared baseline or aligning all layers at the x-height top.

Option              | Description
------------------- | ---------------------------------------------------------------
Reference           | The reference metric to be used. (Baseline,X-Height,Cap-Height)
Reference Alignment | Alignment to the reference. (e.g. to x-height center or top)
Layer Alignment     | Alignment of text-layers and non-text-layers
Pixel Precision     | Precision of resulting layer y position px

<a name="3"/>
##3. Create Baseline Layer

![Baseline Layer](text-tools-baseline-layer.gif)
![Baseline Layer](text-tools-baseline.png)
![Baseline Layer](text-tools-baseline-panel.png)

Creates a baseline reference layer either from text-layers or from configuration.

Option       | Description
------------ | --------------------------------------------------------------------------------------
Layer Width  | The width of the baseline layer ('auto' on text-layers sets width to text-layer width)
Line Height  | The line height  ('auto' on text-layers sets line-height to text-layer line-height )
Num Lines    | The number of lines to display ('auto' on text-layers sets number of lines relative to text-layer height)
½ Step       | If enabled an additional guide displaying half the line-height will be added
Shared Style | Choose a custom styling via shared styles

<a name="4"/>
##4. Count Characters Per Line

Counts characters of all lines within a text layer. Shows the minimum and maximum amount of characters, the line indices for both values as well as the total amount of characters. 

<a name="5"/>
##5. Columnize

![Columnize](text-tools-columnize.gif)

Splits a text-layer into multiple columns. Number of columns, gutter width and column height can be specified.

***Sorry, no hyphenation at the moment.***
