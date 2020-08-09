# From the MDN web docs

## Basic usage of canvas

- The `<canvas>` element

  - Canvas element has only two attributes, width and height
  
  - When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high.

  - The <canvas> element differs from an <img> tag in that, like for <video>, <audio>, or <picture> elements, it is easy 
  to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer
  earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

- The Grid

  - Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous
  page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. 
  Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at
  coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes
  x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin
  to a different position, rotate the grid and even scale it, but for now we'll stick to the default.


- The colors

  - 2 important properties:
  
    - fillStyle
      
      - Sets the style used when filling shapes.
    
    - strokeStyle
    
      - Sets the style for shapes' outlines.
    
- Drawing Text

   - fillText
    
      - Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

   - strokeText
   
      - Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.


  

  
  
  
  



 




 

[Back to Home](https://pdariuslee.github.io/reading-notes/)
