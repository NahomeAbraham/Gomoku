# Gomoku
Gomoku game created using MIPS assembly language 
We created a board game called Gomoku. The game board is a 19x19 board with the goal of getting 5 in a row to win. 
In order for the player and computer to choose a position on the board, input is taken in the form of 
a letter (A-S) followed by a number (1-19), such as B4. Since the board is 19x19, there are a total of 361 spaces. 
To hold the space needed for the board we allocated 1444 bytes in memory (361x4=1444). 
We struggled in coding the section that checks diagonally in regard to the winning state.
When jumping to subroutines, there was an issue with storage. Consequently, after the game would check for a diagonal win 
there was no way of getting back to the game. To resolve this issue, we used a stack to store the addresses of previous subroutines in memory.
