# AI Players for Crazy 8 Card Game

This project introduces the development of artificial intelligence (AI) players for the Crazy 8 card game. The objective is to design and implement intelligent virtual players capable of strategic decision-making and adaptive gameplay in the dynamic and unpredictable environment of Crazy 8.

## Abstract
In this project, four different AI players were designed and tested in a competitive environment. The players include two variants of Alpha-Beta algorithms with different evaluation functions, a Monte Carlo Tree Search (MCTS) player, and a Reinforcement Learning (RL) player. The game was played in a two-player setup, and the performance of the AI players was evaluated based on total wins and points obtained after 200 games.

## Problem Formulation
Challenges for the AI agent
Creating an AI player for Crazy 8 poses challenges due to diverse states and inherent randomness. The game involves incomplete information, making it a suitable testbed for AI algorithms applicable to sequential security games, medical recommendations, etc.

## Rules of the game
The game is played with two players, and the goal is to discard all cards by playing a card that matches the rank or suit of the top card. Eights are wildcards, allowing the player to change the suit.

## AI Agent and Task Environment
The AI agent's goal is to maximize performance measured by total points or victories against opponents. The task environment includes cards of both players, the deck, and the top card. The agent suggests optimal moves based on its decision-making process.

## Proposed Solution: AI Agents
### 1. Alpha-Beta Algorithm
Two Alpha-Beta players were created:

Alpha-beta player 1: Uses a heuristic evaluation function based on the total points of the player in the terminal state.
Alpha-beta player 2: Utilizes a simpler utility function assigning points for wins, negative points for losses, and zero for ties.

### 2. Reinforcement Learning Algorithm
Q-state Reinforcement Learning algorithm uses an epsilon-greedy strategy and approximates the Q-function using features such as the number of cards in hand, number of eights, and current suit.

### 3. Monte Carlo Tree Search Algorithm
Generates moves by simulating possible outcomes and evaluates moves based on the proportion of wins in random simulations.

## Numerical Experiments
The AI players were tested in a competition where each player played against others for 200 games. Results indicate that Alpha-Beta algorithms performed better in terms of points and wins.

