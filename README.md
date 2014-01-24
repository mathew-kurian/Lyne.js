![lynejs logo](http://cdn.turredo.com/github/Lyne.js/logo.png)
=======
**Dynamic HTML5 Line Graph W/ Fluid Animation**
Live Examples
=======
http://bluejamesbond.github.io/Lyne.js/

Start Graphing
=======
Fast, no-hassle setup. Powerful, smooth, and animated. Uses pure Javascript and canvas without SVG.

```js

// Points to be plotted
var dataset = [ 500, 300, 100, 200, 800 ];
var canvas = ocument.getElementById( 'myCanvas1' );

// Initialize basic graph graph
var lyne = new Lyne.Graph( dataset, canvas );

// Customize with themes
var lyne = new Lyne.Graph( dataset, canvas, Lyne.Themes.Dark );
var lyne = new Lyne.Graph( dataset, canvas, Lyne.Themes.Light );

// Custom Themes: More information below
var lyne = new Lyne.Graph( dataset, canvas, customTheme );

```
Add | Remove | Generate | Repaint | isReady
=======
Everything is animated, so you will see your changes in a short period of time.

```js

// Append data
lyne.add(500, callback);

// Remove data by index
lyne.remove(10, callback);

// Append data while removing data at index 0
lyne.dataQueue(500, callback);

// Start auto-generation
lyne.startGenerate();

// Cancel auto-generation
lyne.cancelGenerate();

// Repaint
lyne.repaint();

// isReady
lyne.isReady();

```
Custom Theme
=======
Quickly make a new theme. I recommend you learn by experimenting.

```js

var Options = {
    xyAxisStrokeStyle : '#FFF',
    xyAxisLineWidth : 2,
    /*-------------------------------------*/
    yAxisLabelTextShadowStrokeStyle : "transparent",
    yAxisLabelTextShadowOffsetY : 1,
    yAxisLabelStrokeStyle : "#777",
    yAxisLabelFontSize : "12px",
    yAxisLabelFontWeight : "300",
    yAxisLabelFontFamily : "'Proxima Nova'",
    yAxisGridSpacingMin : 15,
    yAxisGridSpacingMax : 55,
    yAxisGridStrokeStyle : "rgba(255,255,255, 0.03)",
    yAxisGridLineWidth : 1,
    /*-------------------------------------*/
    xAxisLabelTextShadowStrokeStyle : "transparent",
    xAxisLabelTextShadowOffsetY : 1,
    xAxisGridStrokeStyle : "rgba(255,255,255, 0.03)",
    xAxisGridLineWidth : 1,
    xAxisLabelStrokeStyle : "#777",
    xAxisLabelFontSize : "12px",
    xAxisLabelFontWeight : "300",
    xAxisLabelFontFamily : "'Proxima Nova'",
    /*-------------------------------------*/
    plotPointStrokeStyle : '#222',
    plotPointFillStyle : '#FFF',
    plotPointLineWidth : 8,
    plotPointRadius : 3,
    /*-------------------------------------*/
    plotAreaFillGradientStyle : 1, // { 1 : vertical } { 0 : horizontal }
    plotAreaStrokeColorStart : '#FFF',
    plotAreaStrokeColorStop : '#FFF',
    plotAreaFillColorStart : '#111',
    plotAreaFillColorStop : '#333',
    plotAreaLineWidth : 3,
    /*-------------------------------------*/
    canvasPadding : 50,
    /*-------------------------------------*/
    debugVarTweener : true,
    debugVarTweenerLabelTextShadowStrokeStyle : "transparent",
    debugVarTweenerLabelTextShadowOffsetY : 1,
    debugVarTweenerLabelStrokeStyle : "#555",
    debugVarTweenerLabelFontSize : "10px",
    debugVarTweenerLabelFontWeight : "bold",
    debugVarTweenerLabelFontFamily : "'Proxima Nova'",
    /*-------------------------------------*/
    debugAboutLyne : true,
    debugAboutLyneLabelTextShadowStrokeStyle : "transparent",
    debugAboutLyneLabelTextShadowOffsetY : 1,
    debugAboutLyneLabelStrokeStyle : "#777",
    debugAboutLyneLabelFontSize : "10px",
    debugAboutLyneLabelFontWeight : "bold",
    debugAboutLyneLabelFontFamily : "'Proxima Nova'",
    /*-------------------------------------*/
    animationTime : 1800,
    animationYStartStretch : 0,
    animationXStartStretch : 2,
    animationClearQueue : true
};

```
=======
Contributors
=======

```js
bluejamesbond
```
