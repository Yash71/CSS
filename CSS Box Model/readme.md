## Box Model
It ccontain*s different parts- margin, border, padding and content

### Parts of a box
* Content Box: 
    * The area where content is displayed
    * Size can be controlled using ```width``` and ```height``` properties
* Padding Box:
    * This sits around the content in the form of white space.
    * Size can be controlled by ```padding``` and related properties.
* Border Box:
    * It wraps the content and any padding around it.
    * Size can be controlled by ```border``` and related properties.
* Margin Box:
    * It wraps the content, padding and border in the form of white space.
    * Size can be controlled by ```margin``` and related properties.            

### The Standard CSS Box Model
If you give a box a ```width``` and ```height``` attribute, this defines the width and the height of the *contant* box.

### The Alternative CSS Box Model
If you give a box a ```width``` and ```height``` attribute, this defines the width and the height of the actual box. The size of *content* box will be the (actual size-padding-border)
To enable this box model use, ```box-sizing: border-box;```

>>Note: The margin is not counted towards the actual size of the box. The box's area stops at the border — it does not extend into the margin.

### Margin Collapsing
When two elements whose margin touch, then
* if both margins are positive, those margins will combine to form one margin, and its size will be the largest individual margin among the two of them.
* If one margin is negative, its value is subtracted from the total.
* If both are negative, the margins will collapse and the smallest value will be used.