# ❌⭘ Tic-Tac-Toe AI – Playable, Adjustable, Fun

Welcome to my small **Tic-Tac-Toe** project from an early learning phase (later polished for GitHub).  
You play as **X**, the computer plays as **O**. Difficulty ranges from “very easy” to “very hard,” powered by **Minimax with Alpha-Beta pruning**.

---

## 🎯 What’s Inside?

A clean, terminal-based Tic-Tac-Toe that:
- Lets you **choose difficulty**: very easy, easy, medium, hard, very hard
- Uses **Minimax + Alpha-Beta** for smart AI moves
- Shows a **live board** after every turn
- Tracks **wins, ties**, and even a small **blunders report** (when AI defeats you, it notes the move number)

This is a compact, beginner-friendly notebook meant for learning and quick play.

---

## 🎮 How It Works

![Workflow](tic%20tac%20flow.png)

**Game flow**
1. You enter your name.
2. Pick a difficulty.
3. The board prints after every move.
4. Type a number **1–9** to place your X.
5. AI responds with O, until someone wins—or it’s a tie.

**Under the hood**
- **Minimax with Alpha-Beta**: the AI searches future moves and prunes branches to play fast and smart.
- **Difficulty ↔ search depth**  
  - very easy → random  
  - easy → depth 2  
  - medium → depth 4  
  - hard → depth 6  
  - very hard → depth 8  
- **Checks** for win conditions, empty cells, and valid inputs.

---

## 🧪 Example Gameplay (Terminal)

```

Welcome to Tic-Tac-Toe!
You will play as 'X' and the AI will play as 'O'.
Enter your name: abc
Choose difficulty (very easy, easy, medium, hard, very hard): easy

\|   |
\---+---+---
\|   |
\---+---+---
\|   |

Choose your move (1-9): 1

X |   |
\---+---+---
\|   |
\---+---+---
\|   |

AI is making a move...

X | O |
\---+---+---
\|   |
\---+---+---
\|   |
...
AI wins!
Do you want to play again? (yes/no): no

Game Report:
AI: 1 | abc: 0 | Tie: 1
Blunders Report:
Blunder 1: Game 1, Move 4

````

---

## ⚙️ Quick Setup

**Requirements**
- Python 3.10+ (tested on 3.11)
- Jupyter Notebook (if running the `.ipynb`)

**Run (Notebook)**
1. Open the `.ipynb` in Jupyter
2. Run all cells
3. Follow the prompts in the terminal cell

**Run (Script)**
- Export core cells to a `.py` file with a `main()` entry (this notebook already has one).
- Run:
  ```bash
  python tictactoe.py
````

---

## 🧩 Controls & Rules

* **Input**: type a number **1–9** to pick a square (top-left is 1, bottom-right is 9).
* **Winning**: three in a row, column, or diagonal.
* **Invalid input**: the game asks you again if you enter something wrong or pick a filled spot.
* **Play again**: type `yes` to start a new game with a new difficulty.

---

## 🧠 Why I Built It

I wanted a short, hands-on way to understand:

* How **Minimax** decides optimal moves
* How **Alpha-Beta pruning** speeds things up
* How to map **difficulty → search depth** for a nicer player experience

This stays intentionally small and readable, perfect for a quick study and some fun play.

---

## 📉 Limitations

* Terminal UI only (no graphics)
* AI depth caps at “very hard” for speed and simplicity
* No save/resume feature

These choices keep the notebook compact and beginner-friendly.

---

## 🚀 Future Ideas

* Add a simple **web UI** with Flask/FastAPI
* Show **AI move reasoning** (scores per move)
* Add **score persistence** across sessions
* Add a **hint mode** for the player

---

## 🔧 Tech Notes

* Python, Jupyter Notebook
* Core pieces:

  * `minimax_alpha_beta(...)`
  * `optimal_move_alpha_beta(...)`
  * `check_winner(...)`, `player_move(...)`, `ai_move(...)`, `display_board(...)`
* Difficulty mapping lives in `DIFFICULTY_LEVELS`

---

## 🤝 Contributing

Feel free to explore, fork, and tweak the AI or UI.
If you make it smarter, faster, or prettier—awesome.

---

## 📝 License

Open source for learning and reuse. Have fun playing!


