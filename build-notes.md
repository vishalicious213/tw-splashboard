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

### Flex container

```html
<div class="flex items-center justify-between"></div>
```
- __flex__: display: flex
- __items-center__: align-items: center
- __justify-between__: justify-content: space-between

### Logo

```html
<div class="pt-2"></div>
```
- __pt-2__: padding-top: 2

### Menu

```html
<div class="hidden md:flex space-x-6">
```
- __hidden__: display: none
- __md__: medium, when combined with flex and hidden, the container is hidden by default (display: hidden), but shows up on medium size and larger (display: flex) in a mobile-first manner
- __flex__: display: flex
- __space-x-6__: margin-right: 1.5rem & margin-left: 1.5rem (the space between items)


### Menu items

```html
<a href="#" class="hover:text-darkGrayishBlue">Pricing</a>
```
- __hover__: add styling only for the hover state (other tags exist for focus, etc.)
- __text__: add text color (color name/details follow, above a custom color is used)

### Button

```html
<a href="" class="hidden md:block p-3 px-6 pt-2 text-white bg-brightRed rounded-full baseline hover:bg-brightRedLight">Get Started</a>
```
- __hidden__: display: none
- __md:block__: change from display:none to display:block on medium and greater screen widths
- __rounded-full__: border-radius: 9999px
- __baseleine__: should be align-baseline?

## Hero section

### Flex container

```html
<div class="container flex flex-col-reverse md:flex-row items-center px-6 mx-auto mt-10 space-y-0 md:space-y-0"></div>
```
- __container__: makes the element a container, setting max width and applying breakpoints
- __flex__: display: flex
- __flex-col-reverse__: flex-direction: column-reverse
- __md:flex-row__:  at medium width and higher: flex-direction: row
- __items-center__: align-items: center
- __px-6__: padding-left: 1.5rem & padding-right: 1.5rem
- __mx-auto__: margin-left: auto & margin-right: auto
- __mt-10__: margin-top: 2.5rem
- __space-y-0__: margin-top: 0 & margin-bottom: 0
- __md:space-y-0__: at medium width and higher: margin-top: 0 & margin-bottom: 0

### Left item in flex container

```html
<div class="flex flex-col mb-32 space-y-12 md:w-1/2">
```
- __flex__: display: flex
- __flex-col__: flex-direction: column
- __mb-32__: margin-bottom: 8rem
- __space-y-12__: margin-top & margin-bottom have some amount of rem unit spacing
- __md:w-1/2__: at medium width, make this container 1/2 the width of the parent element

### h1 in left item in flex container

```html
<h1 class="max-w-md text-4xl font-bold text-center md:text-5xl md:textleft">
```
- __max-w-md__: the width of the h1 caps out at whatever medium screen width is set to
- __text-4xl__: size of the text
- __font-bold__: bold
- __text-center__: center the text by default
- __md:text-5xl__: at medium width, change text size to 5xl
- __md:text-left__: at medium width, align the text left (override the center default, above)

### p in left item in flex container

```html
<p class="max-w-sm text-center text-darkGrayishBlue md:text-left">
```
- __max-w-sm__: the width of the p caps out at whatever small screen width is set to
- __text-center__: center the text by default
- __text-darkGrayishBlue__: set custom text color
- __md:text-left__: at medium width, align the text left (override the center default)