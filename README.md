# Things you can't do in IE 8

## HTML

* HTML5 elements *There are ways around this (HTML5 Shim)
* Geolocation
* Video
* Audio

## Responsive Design

* Media queries (`@media`) *There are ways around this (RespondJS)
* `Calc()`

## Units

* `rem`
* `vw`, `vh`
* `vmin`, `vmax`

## Typography

* .ttf, .otf, .woff (must serve .eot)

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

* SVG
* Multiple `background`s
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
* Apparently, we can use CSS3 Pie for these:
	* `box-shadow`
	* `border-radius`
	* gradients (or use something like `filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#063053', endColorstr='#395873');`)