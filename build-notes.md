## Navbar

```html
<nav class="relative container mx-auto p-6 bg-red-500">NAVBAR</nav>
```
- __relative__: position: relative
- __container__: makes the element a container, setting max width and applying breakpoints
- __mx-auto__: apply margin to left & right sides
    - mt: margin-top, mb: margin-bottom, ml: margin-left, mr: margin-right, mx: margin left & right, my: margin top & bottom
    - auto: applies auto as the margin value instead of a specific unit
- __p-6__: padding of 6 rem
- __bg-red-500__: background-color, color name, saturation

```html
<div class="flex items-center justify-between"></div>
```
- __flex__: display: flex
- __items-center__: align-items: center
- __justify-between__: justify-content: space-between

```html
<div class="pt-2"></div>
```
- __pt-2__: padding-top: 2

```html
<div class="hidden md:flex space-x-6">
```
- __hidden__: display: none
- __md__: medium, when combined with flex and hidden, the container is hidden by default (display: hidden), but shows up on medium size and larger (display: flex) in a mobile-first manner
- __flex__: display: flex
- __space-x-6__: margin-right: 1.5rem & margin-left: 1.5rem (the space between items)

```html
<a href="#" class="hover:text-darkGrayishBlue">Pricing</a>
```
- __hover__: add hover effect
- __text__: add text color (color name/details follow, above a custom color is used)