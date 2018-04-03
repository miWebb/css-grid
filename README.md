# CSS Flexbox Grid

The CSS Grid library using Flexbox.
Use 'row' class to initiate the row div and 'col* ' to initate the column divs.
There are multiple row extentions to alter the grids behaviour:
* row--same-size
* row--reverse
* row--top
* row--middle
* row--bottom
* row--left
* row--center
* row--right
* row--around
* row--between
* row--evenly
* row--no-gutter

There are multiple columns classes: use col-1 through col-12 for a standard layout in sizes in steps of 12 and use col for a auto single row spacing. Use desktop (1440px) tablet (1024px) or mobile (640px) indicators to specify a certain breakpoint: col-mobile-4. Use offset to give the column a offset in steps of 12: col-offset-2 or col-mobile-offset-0.


## Example

```html
<link rel="stylesheet" type="text/css" href="grid.css">
```

### Simple Grid
```html
<div class="row">
	<div style="background-color: red;" class="col-12">foo</div>
	<div style="background-color: green;" class="col-4">bar<br />foo</div>
	<div style="background-color: blue;" class="col-4">bar</div>
	<div style="background-color: yellow;" class="col-4">foo</div>
	<div style="background-color: orange;" class="col-4 col-offset-1">bar</div>
	<div style="background-color: pink;" class="col-4 col-offset-2">foo</div>
</div>
```

### Simple Grid with different Mobile sizing
```html
<div class="row">
	<div style="background-color: red;" class="col-12 col-mobile-12">foo</div>
	<div style="background-color: green;" class="col-4 col-mobile-12">bar<br />foo</div>
	<div style="background-color: blue;" class="col-4 col-mobile-12">bar</div>
	<div style="background-color: yellow;" class="col-4 col-mobile-12">foo</div>
	<div style="background-color: orange;" class="col-4 col-offset-1 col-mobile-12 col-mobile-offset-0">bar</div>
	<div style="background-color: pink;" class="col-4 col-offset-2 col-mobile-12 col-mobile-offset-0">foo</div>
</div>
```

### Simple Grid with no column Padding
```html
<div class="row row--no-gutter">
	<div style="background-color: red;" class="col-12">foo</div>
	<div style="background-color: green;" class="col-4">bar<br />foo</div>
	<div style="background-color: blue;" class="col-4">bar</div>
	<div style="background-color: yellow;" class="col-4">foo</div>
	<div style="background-color: orange;" class="col-4 col-offset-1">bar</div>
	<div style="background-color: pink;" class="col-4 col-offset-2">foo</div>
</div>
```

### Simple Grid with Same Height Columns
```html
<div class="row row--same-size">
	<div style="background-color: red;" class="col-12">foo</div>
	<div style="background-color: green;" class="col-4">bar<br />foo</div>
	<div style="background-color: blue;" class="col-4">bar</div>
	<div style="background-color: yellow;" class="col-4">foo</div>
	<div style="background-color: orange;" class="col-4 col-offset-1">bar</div>
	<div style="background-color: pink;" class="col-4 col-offset-2">foo</div>
</div>
```

### Auto Fill Remaining Space
```html
<div class="row">
	<div style="background-color: red;" class="col-6">foo</div>
	<div style="background-color: blue;" class="col">bar</div>
	<div style="background-color: blue;" class="col">foo</div>
</div>
```

### Vertical Align Columns
```html
<div class="row row--bottom">
	<div style="background-color: red;" class="col">foo</div>
	<div style="background-color: green;" class="col">foo<br />bar</div>
	<div style="background-color: blue;" class="col">foo</div>
	<div style="background-color: yellow;" class="col">bar</div>
	<div style="background-color: orange;" class="col">foo</div>
	<div style="background-color: pink;" class="col">bar</div>
</div>
```

### Horizontal Align Columns
```html
<div class="row row--center">
	<div style="background-color: red;" class="col-6">foo</div>
	<div style="background-color: blue;" class="col-2">bar</div>
</div>
```

### Auto Horizontal Spacing
```html
<div class="row row--evenly">
	<div style="background-color: red;" class="col-6">foo</div>
	<div style="background-color: blue;" class="col-2">bar</div>
</div>
```