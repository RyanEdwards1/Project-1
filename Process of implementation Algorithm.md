
#### Code For Drawing Player:
     context.beginPath();
     context.fillStyle = "#000000";
     context.fillRect(mouseX - 25, mouseY - 25, 25, 25); 
     context.fill();
        
The code above starts with context.beginPath which begings the drawing of retangles it draws too lines on the screen and the
next lines of code place it all togethere and make it into a rectangle.

Context.fillStyle is the colour that you want your rectangle to be using hex numbers which is made up of 6 differnet number and letter combinations.

Context.fillRect is to make the lines that was created earlier into a rectangle, Then in the brakets is numbers which is creating the size that you want your rectangle to be.


#### Code For Collision:
     function contains(targetA, targetB) {
	  return !(targetA.x > (targetB.x + targetB.width) || 
			   (targetA.x + targetA.width) < targetB.x || 
			   targetA.y > (targetB.y + targetA.height) ||
			   (targetA.y + targetA.height) < targetB.y);

Above you can see the Code That is used to create and detect the collision.

The way it works is my too rectangles are target A and B and when their x and y coordinates meet or overlap then the users rectangle will change colour showing there is a collision. As long as the too rectangles stay apart there will be no contact but as soon as the the rectangles meet it shows the collision. The user would then lose a life and continue to play enless they have lost 3 lives then it is game over 
