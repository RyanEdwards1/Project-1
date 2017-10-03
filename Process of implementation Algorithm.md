### Drawing Player

The code that is used to draw the users player onto the screen is:

  ##### context.beginPath();
  ##### context.fillStyle = "#000000";
  ##### context.fillRect(mouseX - 25, mouseY - 25, 25, 25); 
  ##### context.fill();
        
The code above starts with context.beginPath which begings the drawing of retangles it draws too lines on the screen and the
next lines of code place it all togethere and make it into a rectangle.

Context.fillStyle is the colour that you want your rectangle to be using hex numbers.

Context.fillRect is to make the lines into a rectangle then in the brakets is the size that you want it to be.
