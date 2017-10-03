
#### Code For Drawing Player:
     context.beginPath();
     context.fillStyle = "#000000";
     context.fillRect(mouseX - 25, mouseY - 25, 25, 25); 
     context.fill();
        
The code above starts with context.beginPath which begings the drawing of retangles it draws too lines on the screen and the
next lines of code place it all togethere and make it into a rectangle.

Context.fillStyle is the colour that you want your rectangle to be using hex numbers.

Context.fillRect is to make the lines into a rectangle then in the brakets is the size that you want it to be.


#### Code For Collision:
     function contains(targetA, targetB) {
	  return !(targetA.x > (targetB.x + targetB.width) || 
			   (targetA.x + targetA.width) < targetB.x || 
			   targetA.y > (targetB.y + targetA.height) ||
			   (targetA.y + targetA.height) < targetB.y);
