jquery.areaSelect.js
====================

AreaSelect is a jQuery plugin that gives you the ability to Select multiple areas from an image.

view demo: http://blog.gongshw.com/jquery.areaSelect.js/demo/demo.html

Init
====
```javascript
var options = { // all the option fields are optional
	initAreas: [{"x": 280, "y": 93, "width": 50, "height": 50}], // the initial areas when the plugin load
	deleteMethod: 'click', //or 'doubleClick'
	area: {strokeStyle: 'red', lineWidth: 2}, // style to draw selected areas
	point: {size: 3, fillStyle: 'black'}, // style to draw point
};
$img.areaSelect(options);
```

Get Selected Areas
=================
```javascript
var selectAreas = $img.areaSelect('get');
// [{"x":280,"y":93,"width":50,"height":50}]
```

Event
=====
```javascript
$img.areaSelect('bindChangeEvent', function (event, data) {
	//invoke when selected areas changed
	alert(data.areas);
});
```
