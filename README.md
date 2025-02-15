# CRASH-AI-CS-3030
Final Project

Michael Buslik

Jacob Quatkemeyer

Rob Standifer

Corse: CS 3030-001

Instructor: Damia Fuentes Escote

Due Date: December 15, 2019


Project Description:

This project explores artificial intelligence and reinforcement learning, 
using python. The primary goal is to build a python program to play a 
simple arcade-style game.

The target file is a game called Cave Runner, which is a side scrolling 
action game that involves a player that must continuously move through 
a cavern while avoiding various obstacles.

There are only two actions that can be controlled, jump and dash, which 
the runner activates to avoid pits, land on platforms, avoid/kill monsters, 
and avoid falling objects. 

The project objectives are to get python to play the game independently, 
while utilizing a set of simple AI strategies which will be compared for 
degrees of success.

Statistical analysis on each AI strategy will provide feedback on which 
strategies should be executed against the various levels of the game. 

With this analysis, the AI will be able to choose a specific strategy for 
each level that will provide optimum success. Since the game is procedurally 
generated from a finite set of programmed levels, the AI can be expanded as 
needed to address each challenge independently. 


Program Structure:

main.py is the main module that initiates the AI by setting up a dedicated 
thread to launch the game window and gets its coordinates. Then it begins 
tracking the objects generated by the game window.

These tasks are controlled with the following modules:

  open_game.py
  
  game_interaction.py
  
  find_objects.py

open_game.py allows the program to execute the Cave Runner file in a game
window, and moving the window to the upper-left corner of the screen.

game_interaction.py handles clicking the mouse to start the game and pressing 
and releasing a key to control the player actions.
 
find_objects.py is in charge of identifying objects in the game window. It draws 
a green rectangle around each object to provide visual feedback that the AI can 
identify necessary objects to react to.

The module proceeds to record snapshot images of the screen to display in a 
seperate window while simultaneously providing coordinates for each object that 
will be used by the AI.

Additional Functionality:

With the stated goal of implementing a simple AI, the proposed method is to 
design a set of automated responses that are designed to approach the game 
obstacles with three distinctly different strategies.

The Cave Runner game consists of a character that is always running from left
to right through a cave that contains obstacles and monsters. Obstacles include 
pits, walls, platforms, monsters, and spikes that fall from the ceiling of the 
cave (stalagtites). 

The actions required to avoid these obstacles are simple, and consist of 
jumping and dashing, and provide three basic options:

  1.) A jump is used to avoid obstacles in the player's path.
      * A jump may be performed whenever tha player is toucing the ground.
  
  2.) A dash is used to defeat a monster or teleport through an obstacle.
      * A dash has a ~1 second cooldown before it can be used again.
 
 
 
  
  
  To Do:
  
  AI starts its own timer to record success of the run
  
  write three distinct AI algorithms:
  
    AiAlpha.py
    
    AiBeta.py
    
    AiGamma.py
  
  Write python graphing program using matplotlib to graph AI Test Run Comparisons for:
  
    AiAlpha.txt
    
    AiDelta1000RandomTimes.txt
    
    AiGammaTimes.txt
  

 

