# Artificial Intelligence Pacman Project Milestone 2

## Background

Multi-Agent Pacman:
- Pacman, now with ghosts.
- Minimax, Evaluation

## Objective

- P3-1 Reflex Agent (40%)
- P3-2 Minimax (25%)
- P3-3 Alpha-Beta Pruning (25%)
- P3-4 Better Evaluation (Bonus, 30%)

## Concepts

1. Adversarial Search - Minimax (P3-2)
2. Alpha-Beta Pruning (P3-3)
3. Evaluation Function (P3-1, P3-4)

## Requirements

### P3-1 Reflex Agent

> autograder.py -q q1 --no-graphics

Simple evaluation : eval(state, action) = ...

### P3-2 Minimax

> pacman.py -p MinimaxAgent -l minimaxClassic -a depth=4

> autograder.py -q q2 --no-graphics

Must use
- self.depth()
- self.evaluationFunction()
	- default: scoreEvaluationFunction()

### P3-3 Alpha-Beta Pruning

> pacman.py -p AlphaBetaAgent -l smallClassic -a depth=3

> autograder.py -q q3 --no-graphics

### P4-4 Better Evaluation

> pacman.py -p AlphaBetaAgent -l smallClassic -a depth=3, evalFn=better

> autograder.py -q q5 --no-graphics

Better evaluation : eval(state) = ...
Describe your featuers in the comments.

## Options

Options | Descriptions
------- | ------------
-z 0.5  | 0.5x window size
-n #    | Play # times
-q      | Quiet mode, no graphics
-g DirecitonalGhost | Using directional ghost
-k # | Number of ghosts = #
-f | Fixed random seed; line 533, pacman.py
--frameTime 0 | No frame time

## What to turn in?

1. multiAgents.py