# Object_Oriented_Chess_Game_Design


A terminal-based Chess game implemented in C++, featuring all standard moves, turn-based gameplay, and core logic for piece movement and rules. This project demonstrates object-oriented design, logic implementation for board games, and the use of enums, classes, and other foundational C++ concepts.

Project Overview

This chess game was designed as an exercise in C++ programming, focusing on object-oriented design and logic-based programming for a board game. The implementation includes basic chess rules, a board display, and turn-based functionality for two players. Players can execute standard moves for each piece and are prompted for invalid moves, ensuring an interactive and correct chess experience.
Features

    Piece Movement: Implements movement logic for all chess pieces (King, Queen, Bishop, Knight, Rook, and Pawn).
    Validation of Moves: Checks for out-of-bound moves, invalid captures, and ensures players move their pieces.
    Turn Management: Alternates turns between White and Black, with win conditions when a King is captured.
    User-Friendly Console Output: The board is displayed in an easy-to-understand format with pieces represented by unique characters (e.g., K for White King, k for Black King).
    Replay Option: After game completion, players can start a new game or exit.

Installation
Prerequisites

    C++ Compiler: Ensure you have a C++ compiler like g++ installed.

Setup Instructions

    Clone this repository:

    bash

git clone https://github.com/username/chess-game.git

Navigate to the project directory:

bash

cd chess-game

Compile the code:

bash

g++ main.cpp chess.cpp -o chess_game

Run the compiled executable:

bash

    ./chess_game

Usage

Once the game starts, players will be prompted to enter their moves in a xyxy format, where x1, y1 are the coordinates of the piece to move, and x2, y2 are the destination coordinates. For example:

    Enter 0605 to move a piece from (6,0) to (5,0).
    Invalid moves will result in an error message, allowing the player to try again.

Controls

    Enter moves directly into the console.
    Use the format xyxy to specify piece movement, where coordinates range from 0-7 for an 8x8 board.

Sample Console Output

vbnet

   y: 0  1  2  3  4  5  6  7
x:
 0   R  H  B  Q  K  B  H  R
 1   P  P  P  P  P  P  P  P
 2   •  •  •  •  •  •  •  •
 ...
 7   r  h  b  q  k  b  h  r

White's turn
Type in your move as a single four character string. Use x-coordinates first in each pair.

Class Structure and Logic

The game is structured using two main classes: Square and Board.
Square Class

Represents each square on the chessboard, holding information about:

    The piece (Piece enum) occupying the square.
    The color (Color enum) of the piece.

Board Class

Represents the chessboard itself, containing an 8x8 array of Square objects. Key methods include:

    doMove(): Handles the input and validation of moves.
    setBoard(): Initializes the starting position of pieces on the board.
    movePiece() methods for each piece (e.g., movePawn, moveRook): Defines the movement logic and validation for each type of piece.

Future Enhancements

Potential features for extending this project include:

    Check and Checkmate Logic: Enhance the game rules to account for checks and checkmates.
    AI Opponent: Implement an AI that makes strategic moves against the player.
    Graphical Interface: Transition from the console to a GUI-based display using libraries like SFML.
    Save/Load Feature: Add functionality to save the game's state and resume later.
