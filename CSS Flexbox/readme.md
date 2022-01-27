## flex: shorthand vs longhand
```flex``` property can be used to assign three different values:
* ```flex-grow``` property: unitless proportion.
* ```flex-shrink``` property: used when the flex items are overflowing their container.
* ```flex-basis``` property: minimum size value.

## Horizontal and Vertical alignment
```align-items``` controls where the flex items sit on the cross axis.
*  the value is stretch, which stretches all flex items to fill the parent in the direction of the cross axis. If the parent doesn't have a fixed width in the cross axis direction, then all flex items will become as long as the longest flex item.
* ```center``` value causes the items to maintain their intrinsic dimensions, but be centered along the cross axis.
* one can also use values like ```flex-start``` and ```flex-end```, which will align all items at the start and end of the cross axis respectively

>To override the ```align-items``` behavior for individual flex items, applly the ```align-self``` property to them.

```justify-content``` controls where the flex items sit on the main axis.
* default value is ```flex-start```.
* ```center``` value can be used to make the flex items sit in the center of the main axis.
* ```space-around``` distributes all items evenly along the main axis with a bit of space left at either side.
* ```space-between``` does the same thing as the above value but doesn't leave any space at either end.

## Ordering flex items
flexbox also has a feature for changing the layout order of the flex items without changing the source order.
* By default, every flex item has the order value as 0.
* Flex items with higher order values will appear later in the display order than items having lower order values.
* Flex items with same order value will appear as they appear in source order.
* negative order values make the item appear than items whose value is 0.