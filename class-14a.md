# CSS Transforms, Transitions, and Animations

## 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS
@http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users

- I like this article, below are the 8 simple CSS3 transitions:

  - Fade in
  
  - Change color
  
  - Grow and Shrink
  
  - Rotate Elements
  
  - Square to circle
  
  - 3D Shadow
  
  - Swing
  
  - Inset border
 

## From `learn.shayhowe.com`

  - The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these 
  come with their own individual properties and values.
  
  - The actual syntax for the transform property is quite simple, including the transform property followed by the 
  value. The value specifies the transform type followed by a specific amount inside parentheses.
  
    - div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
          }

  - 2D Transforms
  
    - Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. 
    Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.
  
    - 2D Rotate
    
      - The transform property accepts a handful of different values. The rotate value provides the ability to 
      rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using 
      a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 
      50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.
  
        
    - 2D Scale
     
      - Using the scale value within the transform property allows you to change the appeared size of an element. The default scale 
      value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 
      makes an element appear larger.
      
    - 2D Translate
    
      - The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without 
      interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis 
      while using the translateY value will change the position of an element on the vertical axis.
      
      - As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, 
      followed by a comma, and then the y axis value.
      
      - The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages. 
      Positive values will push an element down and to the right of its default position while negative values will pull an element up and to 
      the left of its default position.

    - 2D Skew
    
      - The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax 
      is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the 
      skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value
      first, followed by a comma, and then the y axis value.%p

    - Combining Transforms
    
      - It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. 
      In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property
      one after the other without the use of commas.

      - Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would 
      be the same as if you were to set the height of an element numerous times.



 

[Back to Home](https://pdariuslee.github.io/reading-notes/)
