🎮 GridMind

ARC-style pattern puzzle game

GridMind is a minimalist puzzle game inspired by the Abstraction and Reasoning Corpus (ARC).
Your goal is to transform a grid of blocks into a target pattern using simple but non-trivial rules.

🧩 Gameplay

A Target Pattern is shown at the top

Move blocks on the grid using directional controls

Each block type behaves differently (movement and/or color change)

Complete the pattern before time runs out

🧱 Block Types
Type	Behavior
Classic	Normal movement
Reverse	Moves in the opposite direction
Static	Does not move, only changes color
Hybrid	Moves and changes color
Reverse Hybrid	Reverse movement + color change
🎲 Game Modes

Random Mode

Procedurally generated puzzles

Increasing difficulty

Endless gameplay

Campaign Mode

Predefined levels

Load levels from JSON packs

Stored locally in the browser

🛠️ Level Designer

Use gridmind_designer.html to create custom levels:

Place blocks and walls on a grid

Define target patterns

Set time limits and difficulty

Export levels as JSON

🚀 Running the Game

No setup required.
Just open index.html in a modern browser.

Optional local server:

python -m http.server

✨ Features

Responsive & mobile-friendly

Offline playable

Replay system

Progressive difficulty

Pure Vanilla JavaScript

🧠 Scoring
Score = (Pattern Width × Height × 20) + (Remaining Time × 2)

📄 License

MIT License.
