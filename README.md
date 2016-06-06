# GraphSvg
A javascript/typescript library for converting graphs to SVG images.

Just include the `GraphSvg.js` in your page and pass the graph information:

``` javascript
var graph = {
	vertices: [{x:30, y:150}, {x:130, y:230}, {x:130, y:70}, {x:230, y: 150}],
	verticesLabel: ["A", "B", "C", "D"],
	edges: [[0, 1], [0, 2], [0, 3], [1, 2]],
	edgesWeight: [1, 1, 5, 1],
	verticesHoverLabel: ["Apple", "Book", "Cat", "Dog"]
};

var svgSettings: {
	width: 460,
	height: 260,
	edgeWidth: 1.5,
	vertexStrokeWidth: 1,
	vertexRadius: 19,
	vertexStrokeColor: "#BECFE9",
	edgeColor: "#CFE9BE",
	vertexFillColor: "#E9BECF"
};

document.getElementById("container").innerHtml = GraphSvg.toSvg("graphElementId", graph, settings);
```

to generate a svg:

![Svg Graph](http://reza1024.github.io/GraphSvg.svg)
