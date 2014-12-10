jquery.areaSelect.js
====================

areaSelect is a jQuery plugin that gives you the ability to Select multiple area from an image.


```html
<script src="jquery.js"></script>
<script src="jquery.areaSelect.js"></script>
<script>
  $('img').load(function () {
			var options = {
				initAreas: [{"x": 280, "y": 93, "width": 50, "height": 50}]
			};
			$(this).areaSelect(options);
			$('#get').click(function () {
				alert(JSON.stringify($('img').areaSelect('get')));
			});
		});
</script>
```
