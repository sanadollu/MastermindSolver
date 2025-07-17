# MastermindSolver
This project presents a comparative analysis of heuristic algorithms to solve the Mastermind Game, a code-breaking game in a limited trial.  All algorithms were implemented in Python and evaluated across 1000 randomly generated game scenarios.

## Project Overview
The Mastermind game challenges players to guess a secret color code. After each guess, feedback is provided in the form of black and white pegs representing correct positions and colors. Despite its simple appearance, the game is NP-complete and ideal for testing heuristic algorithms.

This study evaluates the algorithms based on:
- Average Number of Guesses (ANG)
- Success Rate (within 10 tries)
- Average Runtime for 1000 games

## Implemented Algorithms

### Genetic Algorithm
- Evolves a population of guesses using crossover & mutation

- Fitness based on feedback consistency

### Constraint Propagation
- Narrows the solution space by eliminating inconsistent guesses

- Fastest method, 100% success rate in tests

### Minimax Strategy (Knuth's algorithm)
- Minimizes the worst-case remaining possibilities

- Guarantees optimal solution in ≤ 6 guesses

### Simulated Annealing
- Probabilistic search, accepts worse guesses early on

- Slightly less reliable (99.6% success)

The system supports both user-defined and randomly generated secret codes.

## Insights & Takeaways
Best for speed: Constraint Propagation

Best for minimal moves: Minimax

Best overall trade-off: Genetic Algorithm

Most flexible/stochastic: Simulated Annealing

| Algorithm              | Success Rate | Avg. Guesses | Runtime (1000 games) |
| ---------------------- | ------------ | ------------ | -------------------- |
| Constraint Propagation | 100%         | \~4.9        | 6.84 seconds         |
| Minimax                | 100%         | \~4.5        | 1483.52 seconds      |
| Genetic Algorithm      | 100%         | \~4.72       | 410.03 seconds       |
| Simulated Annealing    | 99.6%        | \~5.33       | Varies               |

## Developers
Sena Ezgi Anadollu

## About the Project
This project was developed as part of an Artificial Intelligence course. The development was completed in April 2025.

