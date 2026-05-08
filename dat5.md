# DAT 5

## positioning

- position can be either static, relative, absolute, fixed or sticky
- **static**
	- default position setting
	- not affected by `top` etc.
- **relative**
	- positioned relative to its normal position in the document
	- `top` does affect it
- **absolute**
	- positioned relative to its nearest positioned parent
		- if there are no positioned parents, it uses the document body
- **fixed**
	- positioned relative to the viewport
		- -> stays in the same place at all times
- **sticky**
	- toggles between `relative` and `fixed` based on its visibility
		- -> when the element stops being visible due to scrolling, it switches from relative to fixed
		- before the switch, it behaves like a normal `relative` element

## text flow

- text flow is determined by the `text-wrap` property
- `text-wrap: wrap;` makes text wrap inside the element it is in
- `text-wrap: nowrap;` makes the text ignore the element and go out of bounds

## z-index

- the z-index determines how elements overlap
- higher value in `z-index:` property -> element is "higher", overlaps others
- only works on positioned elements
- is determined locally -> only in parent 
- if z-index is not specified, overlap is determined by order of definition in html 