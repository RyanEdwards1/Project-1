# Project-1 Trace Ball

## Introduction
#### The aim of this project was to create a web based game. There are two characters: the player, and the enemy npc. The aim of the game is to keep your character away from the enemy, until a timer concludes. The player has three lives, if the enemy NPC hits the player they lose a life. When the player runs out of lives, the game ends

## Description
#### A non-playing character NPC (that is a character controlled by the computer) targets the users mouse position as the player moves across the screen, the game is over once the NPC touches the players mouse position 3 times

## User Stories
#### As a player I would like to know when I have come in contact with the NPC 
#### As a player I would want my character to follow my mouse 
#### As a player I would want to know when I have lost all 3 lives 
#### As a user I would like to play it in a browser 
#### As a player I'd want the NPC to follow my character 
#### As a user I would like to see both characters 


## Flow Chart
![flowchart](https://user-images.githubusercontent.com/31927415/33268043-9047a1a6-d373-11e7-9032-3bedf0c82ee0.JPG)


## Time Line
![cfpture](https://user-images.githubusercontent.com/31927415/33266395-5fdb6db4-d36d-11e7-8043-b6b6ff564e4a.JPG)


### The IDE i used Was NotePad++

#### Notepad ++ was a good option to use as it shows the syntax highlights with colours instead of normal notpad just showing the text so this helped me out alot as i was able to see when i was correcting indenting things and making other syntaxs correctly aswell Notepad++ also aloud us to preview it in many differnt browsers so we could check in real time to see if are code was working or not.

#### I also used a little bit of "Repl.it" as i got closer to the end of my code as this helped with displaying errors and helping me locate them it also saved time as it split the screen into two so i could see what i was changing live instead of tabing in and out of notpad and a web browser. 

## Example Code

#### Code For Drawing Player:
     context.beginPath();
     context.fillStyle = "#000000";
     context.fillRect(mouseX - 25, mouseY - 25, 25, 25); 
     context.fill();
        
#### The code above starts with context.beginPath which begings the drawing of retangles it draws too lines on the screen and the next lines of code place it all togethere and make it into a rectangle.

#### Context.fillStyle is the colour that you want your rectangle to be using hex numbers which is made up of 6 differnet number and letter combinations.

#### Context.fillRect is to make the lines that was created earlier into a rectangle, Then in the brakets is numbers which is creating the size that you want your rectangle to be.

## Debugging Process
#### When we first started coding using notepad++, we did not have an easy way of debugging problems with our code, we would have to scroll through the code and make changes and keep running the code to see the changes. Once we switched to 'repl.it' our debugging improved as we were able to see a live preview as well as get valid debugging messages to tell us where we made mistakes.

## Coding Standards
#### During the coding process, I made sure to constantly indent my code often so that I was able to identify the breaks in commands or even functions. it also means you don’t have to press space a lot to get the same affect.

## Evaluation
#### Overall I feel that as this was my first game that i have coded it went pretty good as i meet all the requirements that we needed to. I learnt have to diagnose simple coding errors/mistakes as well as pick up simple terminology whilst being able to implement it into my code. although i did not comment on my code as much as was recommended I felt that I was able to understand everything and understand what each line of code did as well as its importance.
