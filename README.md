<h1>♔ Command Line Chess Game</h1>

<p>
  Welcome to <strong>Command Line Chess</strong>, where classic chess meets the terminal! This project is a fully functional, C++-based chess game designed with a minimalist interface, challenging AI, and an intuitive gameplay experience for the terminal.
</p>

<h2>🎮 Key Features</h2>

<ul>
  <li><strong>User-Friendly Interface</strong>: The board is displayed with clear, easy-to-read coordinates, making navigation seamless for players of all levels.</li>
  <li><strong>Smart Turn Management</strong>: Each player is prompted to enter moves in a straightforward four-character format (e.g., <code>0715</code>), simplifying interaction.</li>
  <li><strong>Fully Functional Pieces</strong>: All standard chess pieces are implemented with their unique movement rules—pawns, rooks, knights, bishops, queens, and kings.</li>
  <li><strong>Win Detection</strong>: Automatically detects checkmates, declaring the victor in style.</li>
</ul>

<h2>📦 Project Structure</h2>

<ul>
  <li><b>chess.h</b>: Houses the core classes, enums, and method definitions, encapsulating the chess board's structure and each piece’s behavior.</li>
  <li><b>Square and Board Classes</b>: Carefully crafted classes that manage board layout, piece positioning, and move validity for each player.</li>
  <li><b>main.cpp</b>: The entry point for launching the game, initializing the board, and providing an interactive session for players to make moves.</li>
</ul>

<h2>🛠️ Installation & Setup</h2>

<ol>
  <li><strong>Clone the repository:</strong>
    <pre><code>git clone https://github.com/your-username/command-line-chess.git
cd command-line-chess</code></pre>
  </li>
  <li><strong>Compile the code:</strong>
    <pre><code>g++ main.cpp -o chess</code></pre>
  </li>
  <li><strong>Run the game:</strong>
    <pre><code>./chess</code></pre>
  </li>
</ol>

<h2>👾 Gameplay Instructions</h2>

<ul>
  <li><strong>Move Input</strong>: Players enter moves as a single, four-character string, indicating the source and destination coordinates. For example, <code>0715</code> moves the piece from x=0, y=7 to x=1, y=5.</li>
  <li><strong>Win Condition</strong>: Capture the opponent's king to win the game! The board updates dynamically, showcasing each move in real-time.</li>
</ul>

<h2>🔥 Behind the Scenes</h2>

<ul>
  <li><strong>Efficient Data Structures</strong>: A compact 8x8 grid and an enum-based design allow for fast lookups and efficient memory usage.</li>
  <li><strong>Modular Code</strong>: Clean, modularized code structure for maintainable, scalable development.</li>
  <li><strong>Robust Move Validation</strong>: Comprehensive move-checking functions ensure that all piece moves adhere to the rules of chess, including blocking paths and valid moves.</li>
</ul>

<h2>🚀 Future Enhancements</h2>

<ul>
  <li><strong>AI Opponent</strong>: Implementing AI to allow single-player mode against the computer.</li>
  <li><strong>Advanced Chess Rules</strong>: Adding support for special moves like castling, en passant, and pawn promotion.</li>
  <li><strong>Move History & Undo Feature</strong>: Enable players to review move history and undo their last move.</li>
</ul>
