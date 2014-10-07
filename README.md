# Things not supported in IE 8 and ways to tackle some of these problems

## Markup

* Semantic HTML5 elements like `article`, `aside`, `footer`, `header`, `nav`, `section`, etc (but you can use [HTML5 Shim](https://code.google.com/p/html5shim/) to solve this)
* Geolocation
* Video
* Audio

## Responsive Design

* Media queries (`@media`) (but you can use [Respond](https://github.com/scottjehl/Respond) to solve this)
* `Calc()`

## Units

* `rem`
* `vw`, `vh`
* `vmin`, `vmax`

## Typography

* .ttf, .otf, .woff (you must serve .eot – but the majority of web font providers have you covered already)

## Transparency

* `rgba()`
* `hsla()`
* `opacity` (but you can use something like `-ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=90)"`)

## Pseudo Selectors

* `:last-child`, `:nth-child()`, `:first-of-type`, `:last-of-type`
* `:checked`, `:valid`, `:invalid`, `:required`
* `:empty`
* `:not()`

## Graphics

* `canvas`
* SVG
* Multiple background images:
* ```
background-image: url('grass.png'), 
					url(sky.png'), 
					url('sun.png');
`````
* `background-position`
* `background-size`
* Therefore you can't make use of sprites

## Presentation

* `transform`s:
	* `rotate`
	* `translate`
	* `skew`
	* `scale`
	* `matrix`

* Apparently, we can use [CSS3 Pie](http://css3pie.com/) for these:
	* `box-shadow`
	* `border-radius`
	* gradients (or use something like `filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#063053', endColorstr='#395873');`)