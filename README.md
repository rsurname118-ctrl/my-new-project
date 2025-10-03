# Chess Move Predictor AI

Final project for the Building AI course

## Summary

Chess Move Predictor is an AI tool that recommends the best next move based on the current chessboard. It uses historical professional game data to help players improve decision-making and strategy.

---

## Background

Many chess players, especially beginners and intermediates, struggle to consistently choose optimal moves. Learning purely by trial and error can be slow and frustrating. A move predictor AI provides guidance and accelerates learning.

This project addresses:

* Difficulty in selecting strong moves for amateur players
* Slow improvement due to lack of personalized guidance
* Need for interactive tools to practice strategy

---

## How is it used?

Users provide the current board state in standard chess notation (FEN) or interact with a visual board interface. The AI outputs the top recommended moves ranked by probability.

Typical use cases:

* While playing online or offline games for immediate move suggestions
* During practice sessions to analyze possible moves
* For learning strategies from professional patterns

Example of predicting a move in Python:

```
import chess
import chess.engine

board = chess.Board("r1bqkbnr/pppppppp/n7/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - 2 2")

predicted_move = predict_move(board)  # Your AI function
print("Recommended move:", predicted_move)
```

<img src="https://upload.wikimedia.org/wikipedia/commons/4/4f/Chess_board_opening_staunton.jpg" width="300">

---

## Data sources and AI methods

Data comes from open chess databases of professional games in PGN format. Example sources:

* [Lichess Database](https://database.lichess.org/)
* [Chess.com PGN archives](https://www.chess.com/games/archive)

AI Methods Used:

* Supervised learning with neural networks to predict moves from board positions
* Optional reinforcement learning for move optimization
* Evaluation using top-1 and top-3 move accuracy

| Syntax    | Description                         |
| --------- | ----------------------------------- |
| FEN input | Standard chess board representation |
| PGN files | Historical professional games       |
| Python AI | Trains and predicts optimal moves   |

---

## Challenges

* The model may struggle with uncommon positions not in the dataset
* AI suggestions are not guaranteed to always be optimal
* Ethical considerations: users should not rely solely on AI for competitive games
* Bias in training data may favor strategies from certain eras or styles

---

## What next?

* Integrate a full graphical interface for easier input
* Use reinforcement learning for stronger AI recommendations
* Expand dataset with more diverse games to improve predictions
* Collaborate with chess experts to fine-tune evaluation metrics

---

## Acknowledgments

* [Lichess PGN Database](https://database.lichess.org/)
* [Chess.com PGN Archive](https://www.chess.com/games/archive)
* Chess learning tutorials and AI guides from open sources
* [Chess board image by Wikipedia](https://upload.wikimedia.org/wikipedia/commons/4/4f/Chess_board_opening_staunton.jpg) / [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0)

