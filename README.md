# CSS FLEX BOX
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

flex-flow: column wrap; //will be arranged horizontally from left to right

flex-flow: column-reverse wrap; //will be arranged horizontally from right to left

```
