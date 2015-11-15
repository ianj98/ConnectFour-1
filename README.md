## Description

Play [Connect Four](https://en.wikipedia.org/wiki/Connect_Four) against the computer. Right click on the mouse to drop a piece in the highlighted column. After watching your piece fall the computer will make its move.

Adjust the difficulty setting to play on either easy, medium, or hard settings.

## Download

* Download: [zip](https://github.com/jostmey/ConnectFour/zipball/master)
* Git: `git clone https://github.com/jostmey/ConnectFour`

## Compile and Run

sudo apt-get install openjdk-7-jdk

javac *.java -d bin/ 

appletviewer Connect4.html

## How It Works

The program searches every possible move several turns into the future looking for "traps". A trap is a condition in the game such that no matter what you do the computer can still win. The progam will pick the move that offers the greatest possibility of laying a trap to catch you while it tries to avoid any traps you set for it. As the program searches for its best move, the algorithm used to score each move assumes that you will pick the optimal move. In this respect, the underlying algorithm resembles the [minimax alrogithm](https://en.wikipedia.org/wiki/Minimax).
