📌 Project Overview
A fully-featured Snake Game built using Python's turtle module. This is not just a basic game — it includes a proper start screen, in-game HUD, game over state, and a persistent high score that saves between sessions so you never lose your best run.

✨ Features

🎮 Smooth snake movement — no stuttering, no weird jumps
🖥️ Dark-themed game window (600×600 pixels)
🟢 Distinctive snake head color (white/light green) with orange body segments
🍎 Random food — shape and color change every time
📊 Real-time score + high score display (Candara font, 24pt bold)
💾 High score persists between sessions via highscore.txt
🚀 Speed gradually increases as you eat food
🔄 Start screen, gameplay state, and game over screen
⌨️ Supports both WASD and Arrow keys
🧱 Visible play area border
✍️ On-screen signature: Coder: Uddeshya


🎮 Controls
ActionKeyAlternativeMove UpW↑ Up ArrowMove DownS↓ Down ArrowMove LeftA← Left ArrowMove RightD→ Right ArrowStart / RestartSPACE—QuitQClose window

🕹️ Game States
StateDescriptionStart ScreenDisplays title, instructions ("Press SPACE to Start"), and the saved high scoreGameplaySnake, food, and live score — clean and distraction-freeGame OverShows final score with option to press SPACE to restart or Q to quit

📈 Difficulty Progression
Score RangeFrame DelayFeel0 – 500.100 → 0.095Pretty chill60 – 1500.094 → 0.085Getting quicker160 – 3000.084 → 0.070Now it's a challenge300+Floors at 0.050Good luck!

🛠️ Tech Stack
TechnologyPurposePython 3.8+Core languageturtleGraphics and window managementtimeGame loop speed controlrandomFood position and appearance randomizationPlain text (highscore.txt)Persistent high score storage

⚡ No external libraries required — everything is from Python's standard library!


📂 Project Structure
Snake-Game/
│
├── main.py          # Entry point — starts the game and runs the loop
├── snake.py         # Snake class — movement, growth, and reset
├── food.py          # Food class — random spawning and appearance
├── scoreboard.py    # Scoreboard — score display, high score read/write
├── game.py          # Game class — collision detection, state management
├── config.py        # All constants (colors, sizes, speeds, fonts)
├── highscore.txt    # Saved high score (auto-generated on first run)
└── README.md        # This file

🚀 Installation & Setup
bash# 1. Clone the repository
git clone https://github.com/uddeshya-kumar-1621/Snake-Game.git

# 2. Navigate to the project folder
cd Snake-Game

# 3. Run the game (no pip install needed!)
python main.py

Requires Python 3.8+. The turtle module comes pre-installed with Python.


🎯 Gameplay Rules

Snake hits a wall or runs into itself → Game Over + full reset
Play area boundary: -290 to +290 on both axes
Snake cannot reverse direction (180° turn is blocked)
Food will never spawn on the snake's body
Every food eaten → +10 points


💾 High Score Persistence
The high score is saved to highscore.txt automatically:

Close the game — score is saved ✅
Reopen the game — previous high score loads ✅
File missing or corrupted — gracefully defaults to 0 ✅


🐛 Error Handling
ErrorHandlingturtle.TerminatorWindow closed mid-game → clean exit, no tracebackFileNotFoundErrorhighscore.txt missing on first run → starts at 0ValueErrorCorrupted file content → defaults to 0Delay underflowSpeed is floored at 0.050 — always stays playable

📸 Screenshots

(Coming Soon — add gameplay screenshots here)


🔮 Future Ideas

🌀 Wall wrapping mode (go off one side, appear on the other)
🧱 Obstacles that appear as score increases
⚡ Special power-up food items (slow motion, double points)
👥 Two-player mode on the same keyboard
🏆 Top 10 leaderboard with player initials
🎨 Multiple visual themes (neon, retro, minimalist)


👨‍💻 Author
Uddeshya Kumar

GitHub: @uddeshya-kumar-1621

