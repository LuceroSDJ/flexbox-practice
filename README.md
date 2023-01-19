# flexbox-practice

## The flex layout allows responsive elements within a container to be automatically arranged depending on viewport size.


The Flexible Box Layout, usually referred to as flexbox, was designed as a one-dimensional layout model, and as a method that could offer space distribution between items in an interface and powerful alignment capabilities. 

When we describe flexbox as being one dimensional we are describing the fact that flexbox deals with layout in one dimension at a time — either as a row or as a column. This can be contrasted with the two-dimensional model of CSS Grid Layout, which controls columns and rows together.

Source: [Basic Concepts of Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox
) 

## What does flex: 1 mean?
flex-grow : 1;    ➜ The div will grow in same proportion as the window-size       
flex-shrink : 1;  ➜ The div will shrink in same proportion as the window-size 
flex-basis : 0;   ➜ The div does not have a starting value as such and will 
                     take up screen as per the screen size available for
                     e.g:- if 3 divs are in the wrapper then each div will take 33%.

Source: [What does flex:1 mean?](https://stackoverflow.com/questions/37386244/what-does-flex-1-mean) 

Notes: 
flex: 1 was useful for the flex chart. It enables our bar chart to shrink and grow based on the window-size, adding great responsiveness. In addition, it given us the green light to implement the following flex property to the individual bar chart item:
style="flex-basis: 10%

See example bellow:
```
 <div class="container">
    <div class="dish soup" style="flex-basis: 10%;">10%</div>
    <div class="dish fajita" style="flex-basis: 60%;">60%</div>
    <div class="dish rice" style="flex-basis: 30%;">30%</div>
 </div>
 ```