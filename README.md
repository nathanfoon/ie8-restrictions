# Things you can't do in IE 8

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