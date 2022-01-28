## Static positioning

Default position for every element

## relative positioning

* very similar to static positioning
* once the positioned element has taken palce in normal flow, you can modify its final position.
* positioning takes place from the position in normal flow.
* ```top```, ```bottom```, ```left``` and ```right``` properties can be implemented here.
* allows to define the z-index for an element.

## z-index
* when multiple elements are relatively positioned, they stack up on eachother, to change the order of the elements in the stack, we can use z-index
* B.D. every element has a ```z-index:0```, which is effectively 0.
* element with positive values will move above in the stack.
* element with negative vlaues will move below in the stack.

## Abosulte Positioning
* different from relative positioning.
* positioning takes place with respect to the previous ancestor.
* elements are removed from the document flow.

## Fixed Positioning
* this fixes the element to its normal flow position.
* element won't be considered under the document flow and other elements move to occupy its space.

## Sticky Positioning
* mixture of both fixed and relative positioning.
* it allows a positioned element to act like it's relatively positioned until it's scrolled to a certain limit, after which it becomes fixed.
