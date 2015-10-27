D R A F T

#sketch-text-tools

This plugin eases working with typography in Sketch. It enables displaying font metrics, aligning text-layers to text-layers or other layers relative to baseline, x-height and cap-height. Baseline grid reference layers can be extracted from text-layers or build with custom configurations. Text-layers can be split into several columns with specific gutter widths.


##Font Metrics

![Font Metric](./text-tools-font-metrics.gif)

###Cmd: Create Font Metrics From Text

Extracts font metrics from text layer fonts. Creates a reference layer displaying the fonts baseline, ascent, descent, x-height and cap-height as well as the default line-height relative to the font-size used ( *blue* ). Furthermore the x-height and cap-height center get displayed ( *red* ). Metrics get extracted for the first line of a text layer. width equals text-layer width.

##Text Align
![Align Artboard](./text-tools-artboard-align.gif)
*Text-Layer aligned to artboard*

![Align Text Layers](./text-tools-text-layer-align.gif)
*Multiple text-layers aligned*

![Align Text Layers Container](text-tools-text-layer-container-align.gif)
*Text-Layers aligned within container*

![Algin mixed selection](text-tools-mixed-align.gif)
*Mixed selection aligned*

![Align text](text-tools-alignment-panel.png)

###Cmd: Align Text

Aligns selected text-layers and non-text-layers. Alignment is based on a metric reference, e.g. centering all layers on a shared baseline or aligning all layers at the x-height top.

Option       | Description
------------ | -------------
Reference | The reference metric to be used. (Baseline,X-Height,Cap-Height)
Reference Alignment | Alignment to the reference. (e.g. to x-height center or top)
Layer Alignment | Alignment of text-layers and non-text-layers
Pixel Precision | Precision of resulting layer y position px


##Baseline Guides

![Baseline layer from text-layer](text-tools-baseline-layer-from-text.gif)

###Cmd: Create Baseline Layer From Text

Creates a baseline reference layer from a single or multiple text-layers.
The displayed spacing depends on the font metrics information and may not be as expected. The guides width equals the text-layer width, the number of lines corresponds to the layers height.

###Cmd: Create Baseline Layer From Text ½

Adds additional guides for half the line-height.


![Baseline layer 1/2 from text-layer](text-tools-baseline-layer.gif)

###Cmd: Create Baseline Layer

Creates a baseline reference layer from configuration.

##Columnize

![alt text](./text-tools-columnize.gif)

###Cmd: Columnize

Splits a text-layer into multiple columns. Number of columns, gutter width and column height can be specified.

***Sorry, no hyphenation at the moment.***
