# ♟ Chess AI: Minimax & Alpha-Beta Pruning

A simple Python project implementing a Chess AI using *Minimax* and *Alpha-Beta Pruning* algorithms with a visual interface and gameplay video generation. Designed for AI Game Playing assignments.

---

## 📁 Project Structure


chess-ai/
├── src/
│   ├── __init__.py
│   ├── chess_env.py         # Handles chess game logic using python-chess
│   ├── minimax.py           # Minimax agent
│   ├── alphabeta.py         # Alpha-Beta pruning agent
│   ├── evaluation.py        # Evaluation function for board state
│   └── visualizer.py        # Pygame-based visual board & video recorder
├── scripts/
│   ├── generate_video.py    # Main video generation script
│   └── simple_run.py        # Simplified interactive runner
├── videos/                  # Stores generated gameplay videos
├── requirements.txt         # Dependencies
└── README.md                # Project documentation


---

## 💠 Setup Instructions

### 1. Clone the repository
bash
git clone https://github.com/Aarya34/Ai_Assn_3.git
cd Ai_Assn_3


### 2. Create a virtual environment and install dependencies
bash
python -m venv venv
source venv/bin/activate       # On Windows: venv\Scripts\activate
pip install -r requirements.txt


---

## ✅ Dependencies

Contents of requirements.txt:

pygame
python-chess
opencv-python


Install manually if needed:
bash
pip install pygame python-chess opencv-python


---

## 🧠 Algorithms

- *Minimax*: Standard game tree search evaluating all possible future positions.
- *Alpha-Beta Pruning*: Optimized Minimax that skips unnecessary branches, increasing efficiency.

---

## 🎮 How to Run

### 🧪 Option 1: Simplified Interactive Run
bash
python scripts/simple_run.py

- Choose between Minimax or Alpha-Beta
- Set search depth (2–3 recommended)
- Choose whether to record a video

### 🎥 Option 2: Auto-Generate Video
bash
python scripts/generate_video.py --algorithm alphabeta --depth 3


*Options:*
- --algorithm: minimax or alphabeta (default: alphabeta)
- --depth: Search depth (default: 3)
- --max-moves: Max moves per game (default: 50)
- --no-display: Headless mode

---

## 🧮 Evaluation Function

The evaluation considers:
- Material balance (piece values)
- Positional weights (center control, piece development)
- King safety and pawn structure
- Mobility and board state

---

## 🖼 Visuals

- The board is rendered using *pygame*
- Moves are displayed step-by-step
- Videos are saved in videos/ as .mp4


---




## 📌 Notes

- If pygame throws errors on headless systems (like some Linux servers), use --no-display flag.
- Evaluation depth beyond 3 may get slow without additional optimizations.

---

## 🙇‍♂ Author

Aarya Chepuri(CS22B018)
Kowshik reddy Challa(CS22B015)  
AI Assignment 3: Game Playing  
April 2025