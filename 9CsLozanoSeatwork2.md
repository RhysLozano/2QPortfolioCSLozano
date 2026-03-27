<!DOCTYPE html>
<html>
<div class="notice">Notice!</div>

<head>
  <meta name="author" content="<Kuch Lozano>" />
  <meta name="revised" content="<March 27 2026>" />
  <style>
    body { font-family: Arial, sans-serif; }
    .header, .footer {
      background: lightblue;
      padding: 10px;
    }
    .footer {
       opacity: 0.5;
       position: fixed; bottom: 0; width: 100%;
    }
    .sidebar {
      background: lightgreen;
      width: 150px;
      height: 200px;
      position: relative; top: 20px; left: 20px;
    }
    .content {
      background: lightyellow;
      width: 300px;
      height: 200px;
      position: absolute; top: 66px; left: 200px;
      z-index: 1;
    } 
    .notice {
        position : absolute;
        top : 65px;
        left: 436px;
        background: orange;
        padding: 10px;
        z-index: 2;
    }  
    
  </style>
</head>
<body>
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="content">Main Content</div>
  <div class="footer">Footer</div>
</body>
</html>



###
Challenge:

- What changes that you have to do on the code that will position .notice box on the top right corner of the .content box? Please write the code on paper as well (both html and css on the part of .notice and .content).
 .notice {
        position : absolute;
        top : 65px;
        left: 436px;
        background: orange;
        padding: 10px;
        z-index: 2;
    }  
    
Try to change the position of .content to relative then to fixed. What do you observed each time?
- It changes the positions of the boxes according to what position value you set it to, in this case relative and fixed where relative is positioned relative to its normal position while fixed is relative to the viewport 
What do you observe on about the effect of z-index on .notice and .content boxes?
- It affects how its displayed as it can be displayed behind if it the z is set to 1 and displayed at the front if z is set to 2 and vice versa depending on how many  "layers" you need

### 
a. Could you summarize the differences between the CSS position values (static, relative, absolute, fixed)?
Static - The default positioning 
Relative - Positioned relative to normal position 
Absolute - Positioned relative to nearest positioned ancestor without affecting the layout of other elements
Fixed -  Positioned relative to viewport & it does not move when it is being hovered on 


b. How does absolute positioning depend on its parent element?
- It depends on its parent ancestor that has a position : static, relative, absolute, fixed,etc. to act as its default point, as without it it will be positioned to its initial containing block 

c. How do you differentiate sticky from fixed (you can research on sticky)?
- Sticky allows an element to remain in a fixed position regardlesss if  the user is scrolling, while relative keeps the element in normal flow but can be moved to its original position. WHile 

d. If you were designing a webpage for a school event, how might you use positioning to highlight important information? Please give concrete examples.
- Would use positioning to highlight important information such as by putting display boxes of steps or information I'd like to share for whoever is viewing it and adding smaller oxes layered on top saying "Notice !"or "Information" to help the viewer notice that specific set of important information to help guide them. 