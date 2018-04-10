# CSS FLEX BOX
![IMAGE](https://raw.githubusercontent.com/selvesandev/flex-box/master/align-justify.png)

[Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
[Reference](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
### Terminology
Two main terminology used in flex box is
* flex-container 
* flex-items


### Flex Container
* (first step of creating a flex layout) 
* (contains flex items)
* (can be block on inline)



### Flex Items
* (every direct child of a flex container)
* (any number of flex items)



### Flexbox Axis
* Main Axis (horizontal) (default: left to right)
* Cross Axis (perpendicular) (default: top to bottom)
![IMAGE](https://raw.githubusercontent.com/selvesandev/flex-box/master/axis.png)


### Flex Direction
Flex items are by default arranged in left to right but you can change them by with `flex-direction` property

### Wrapping Flex Content.
With the `flex-wrap` property you can control.

### Change the Order of Flex Items
Order of any value by default is 0.


### Adjust the flex item width
`flex-grow:1`

When you add a `display:flex` property you turn the element into a parent or a flex container which
will contain some children which is called `flex items`. 
**Parent** `display:flex`  
**FlexItems** `children inside flex parent.`


#### Parent Flex Container Generally Have (properties)
* display
* justify-content
* align-center
* align-items 


#### Child Flex Items Generally Have (properties)
* order
* flex
* align-self


## Flex Container

```
display:flex; // contert the div into a flex box container which all it's children arranged inline which width
will be automatically arranged.
```

```
display: inline-flex;// the parent will be displayed as an inline element this means it won't take the full width. It will only take the width required
to display the content inside it. Also the flex items wont decrease it's width according to the parent.
```

```
flex-flow: row nowrap;/*this is a short had for using flex-direction and flex-wrap*/
        `row nowrap` is a default property.
        
flex-flow: row wrap; //will wrap the content meaning if the parent width is decreased the child will aumatically move to the next row (responsive behaviour)         


flex-flow: row wrap-reverse; //will wrap the content in reversed order meaning the content will jump to the upper level.         

flex-flow: row wrap; //will be arranged horizontally from left to right

flex-flow: row-reverse wrap; //will be arranged horizontally from right to left

```




#

The flex direction row will also consume the full height of that of it's parent. However we can change that.

#### align-items (refers to the alignment according to the cross axis)
```
align-items: center; 
align-items: flex-end; 
align-items: base-line; 
align-items: flex-start; 
```


#### justify-content (refers to the alignment according to the mail axis)
```
justify-content: center;
justify-content: space-around;
justify-content: flex-end;
justify-content: flex-start;
justify-content: space-between;
```



#### align-content (only works if you have more than one line)
```
align-content: space-between;
align-content: center;
```

## Flex Items

##### order
order takes a numeric value (0,1,3...) which will arrange the order of the content inside the flex container explicitly
```

```

##### align-self

##### flex
```
flex: 0 1 auto; // flex-grow, flex-shrink, flex-basis 
```