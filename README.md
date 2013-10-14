jquery-blureffect
=================

Blureffect - Lightweight jQuery blur effect plugin with canvas



Requirements
==========

jQuery 1.1 and above
The img tag should have an ID attribute
HTML5 doctype ```html <!DOCTYPE html> ``` (for IE)



Usage
==========

Use jquery.blureffect.js for development (with comments), jquery.blureffect.min.js in production (only 7kb)

```html
<img id="an-id" src="your_image.jpg" alt="" />
```

```javascript
$('#an-id').blureffect({
	radius: 50,//radius of blur effect
	alpha: false,//whether to apply some transparency to the blur effect
	regions: [
		{startX: 10, startY: 10, width: 200, height: 200},
		{startX: 500, startY: 500, width: 100, height: 100}
	],//array of blur region coordinates, one item is [startX, startY, width, height]
	top: '20px',//image and canvas will be absolutely positioned and need top and left in pixels
	left: '20px'//left in pixels
});
```


Demo
==========

For now please check [index.html](index.html) for basic usage and delayed image load examples