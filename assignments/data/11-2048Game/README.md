Assignment 11 - 2048
===========================

Source
------

This is a nifty assignment from 2017 proposed by Kunal Mishra.
[Source](http://nifty.stanford.edu/2017/mishra-2048/)

Goals
-----
The purpose of this assignment is to learn to
1. Update and draw unique objects on a grid
2. Update object locations and handle interactions 
3. Set up a simple state machine

Programming
-----------
### Tasks

Create the game 2048 using the Bridges API. Being under the MIT license the game can be found in a variety of places online if the game is unfamiliar. The basics is each turn a new tile spawns on a 4x4 grid that contains the value 2 and rarely 4. The player can choose any cardinal direction to move all blocks  at one time. Once all blocks have reached either the edge or another block they stop and the player can choose another direction. If two blocks have the same value instead they merge and the values are added together. The ultimate goal of the game is to get the value 2048 on a tile. The player loses if they are unable to make a move.
 
#### Set up the board
There needs to be an object that represents a game tile. It holds a position and a value. Each tile takes up 1/4th of the grid in both directions.

#### Add functionality
When the player hits an arrow key the tiles should move until they either merge or they hit a wall/other tile that cannot be merged. While the tiles are moving the game should be a state that does not receive input. Once all tiles are moved or merged then the player can input the next move. After each turn the game should check if there is a game over (no moves to make) or the player has won (a tile has value 2048).
### Help
#### For C++
[NonBlockingGame documentation](http://bridgesuncc.github.io/doc/cxx-api/current/html/classbridges_1_1game_1_1_non_blocking_game.html)

#### For Python
[NonBlockingGame documentation](http://bridgesuncc.github.io/doc/python-api/current/html/classbridges_1_1non__blocking__game_1_1_non_blocking_game.html)
