Download Link: https://assignmentchef.com/product/solved-cs312-lab-5-game-playing
<br>
<span class="kksr-muted">Rate this product</span>




Problem Statement: ​Code a Bot to play the game of Othello in an optimal way, in order to win the game.

Description: ​In this assignment, you will code a bot to win the game of Othello. Given a board configuration and a turn, your bot will return a valid move. The game ends when neither of the players can make a valid move. The player with the maximum number of coins is the winner.

Programming Language: C


System specifications: 64-bit Linux distribution

Instructions

Setting up the framework

We will be providing you with a framework (Desdemona.zip) that lets two bots compete against each other.

1. Extract the contents of Desdemona.zip into a suitable directory.2. Set up the framework by issuing a make command in the root of this directory.

Programming the bot

● You will modify “MyBot.cpp” to return a valid move whenever the function “play is called. The file is located in “bots/MyBot”.

<ul>

 <li>●  The makefile is also provided at this location. Use it to generate a “.so” file.</li>

 <li>●  All other source files are to be left untouched.</li>

 <li>●  You can test your bot against another bot by issuing the command “./bin/Desdemona to bot1.so &gt;./&lt;path to bot2.so &gt;”</li>

 <li>●  By convention, the first bot is BLACK and the second RED.</li>

 <li>●  A random bot (bots/Random Bot) has been provided for testing.</li>

</ul>

./&lt;path

<ul>

 <li>●  At the end of the game, a “game.log” file is created that contains the sequence of moves made.</li>

 <li>●  There should be NO print statements in the code submitted.</li>

 <li>●  If a bot returns an invalid move, it will be disqualified.Helper functionsThe following functions have already been written to assist you:</li>

</ul>

<ul>

 <li>●  bool OthelloBoard::validateMove( Turn turn, int x, int y )True if the move (x,y) is valid for the turn, False otherwise</li>

 <li>●  bool OthelloBoard::validateMove( Turn turn, Move move )True if the move is valid for the turn, False otherwise</li>

 <li>●  void OthelloBoard::makeMove( Turn turn, int x, int y )Updates the board configuration by making the move (x,y); throws an exception if the move is not valid</li>

 <li>●  void OthelloBoard::makeMove( Turn turn, Move move )Updates the board configuration by making the specified move; throws an exception if the moveis not valid</li>

 <li>●  list&lt;Move&gt;OthelloBoard::getValidMoves( Turn turn )Returns a list of valid moves that can be made given the turn</li>

 <li>●  int OthelloBoard::getBlackCount()Returns the number of black coins on the board</li>

 <li>●  int OthelloBoard::getRedCount()Returns the number of red coins on the board</li>

 <li>●  void OthelloBoard::print( Turn turn )Prints the turn, the board configuration, and the number of black and red coins. ’X’ is BLACK, ’O’ is RED, and unfilled locations are blank</li>

</ul>

Time Constraints