# ractive-gauge

A simple UV-type meter for Ractive

## usage

```html
<div id="container"></div>

<script id='template' type='text/ractive'>
	<gauge value="{{value}}" label="coolness" /><br>
	<input min="0" max="100" type="range" value="{{value}}" style="width:255px;margin-left:2.5px"/>
</script>

<script src="https://cdn.ractivejs.org/latest/ractive.min.js"></script>
<script src="ractive.gauge.js"></script>
<script>
var ractive = new Ractive({
	el: 'container',
	template: '#template',
	data: {
		value: 0
	}
});
</script>
```