# Project-1-BackLog
<html>
 
<head>

	<title>Canvas Follow Mouse</title>
	
		<style>
			canvas {
			border: #333 3px solid;
			}
			 
			body {
			padding: 5px;
			}
		</style>
</head>

 
<body>

	<canvas id="myCanvas" width="500px" height="500px"></canvas>
 
		<script>
			
			//Get mouse position
			
			var canvas = document.querySelector("#myCanvas");
			var context = canvas.getContext("2d");
						
			var canvasPos = getPosition(canvas);
			var mouseX = 0;
			var mouseY = 0;
			var sqSize = 50;
			var xPos = 0;
			var yPos = 0;
			var dX = 0;
			var dY = 0;
					 
			canvas.addEventListener("mousemove", setMousePosition, false);
			
			//Fix to track the mouse from the corner of the canvas and not the screen
					 
			function setMousePosition(e) {
			mouseX = e.clientX - canvasPos.x ;
			mouseY = e.clientY - canvasPos.y ;
			}       
			
			//Draw the player and NPC on screen and make it follow the mouse
			
			function update() {
				dX = mouseX - xPos;
				dY = mouseY - yPos;
 
				xPos += (dX / 20);
				yPos += (dY / 20)
			
			
			//Stops the characters from drawing everywhere the mouse goes
		
			context.clearRect(0, 0, canvas.width, canvas.height);
			
			// Generating NPC 
			context.fillStyle = "#ff0000";
			context.fillRect(xPos - sqSize / 2,
                   yPos - sqSize / 2,
                   sqSize,
                   sqSize);
				
			//Draw the player and follow the mouse
			
			context.beginPath();
			context.fillStyle = "#000000";
			context.fillRect(mouseX - 25, mouseY - 25, 25, 25);  
			context.fill();
			  
			requestAnimationFrame(update);
			}
			 
			//Starts the function
			
			update();
			
			//Something 
		
			function getPosition(el) {
			var xPosition = 0;
			var yPosition = 0;
			 
			while (el) {
			xPosition += (el.offsetLeft - el.scrollLeft + el.clientLeft);
			yPosition += (el.offsetTop - el.scrollTop + el.clientTop);
			el = el.offsetParent;
			}
			return {
			x: xPosition,
			y: yPosition
			};
			}  
			


		</script>
		<script>

		</script
</body>
 
</html>
