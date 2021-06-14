# Othello
Task 5: Game Playing
ProblemStatement:​Code a Bot to play the game of Othello in an optimal way,in order to win the game.
Description:​In this assignment,you will code a bot to win the game of Othello.Given a board configuration and a turn,your bot will return a valid move.The game ends when neither of the players can make a valid move. The player with the maximum number of coins is the winner.
Programming Language: C++System 
specifications: 64-bit Linux distribution
Instructions
Setting up the framework. We will be providing you with a framework(Desdemona.zip)that lets two bots compete against each other.
1. Extract the contents of Desdemona.zip into a suitable directory.
2. Set up the framework by issuing a make command in the root of this directory.

# Submission:
Apply a minimax algorithm to code a bot(minmax_bot.so)and alpha-beta pruning to code the other(AB_bot.so). Test the two bots against each other and record the observations.

# Heuristic functions considered:-
A good heuristic function for othello/reversi needs to capture more aspects of the positions, including:

• Coin parity : returns the lead of the player with respect to their opponent.

• Mobility (No. of possible moves) : If we have more choices, it is likely to be the case that our best choice is better. This heuristic tries to improve our freedom to make a variety of moves with respect to our opponent.

• Corner captivity (corners are stable/cannot be turned and have special importance) : The number of corners occupied improves the chances of winning drastically. This heuristic returns the difference in the corners occupied.

Reference taken for these aspects and provided implementation of a good heuristic function here:
http://kartikkukreja.wordpress.com/2013/03/30/heuristic-function-for-reversiothello/
