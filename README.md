# Path Planning Algorithms

This repository contains two distinct path planning solutions for problems 1-3, implemented using the A-star algorithm and Q-learning. These algorithms are designed to navigate from a start point to an end point efficiently in a given environment.

## Algorithms

### A-star Algorithm

The A-star (`A_star.py`) algorithm is a heuristic-based search algorithm that finds the least-cost path from a given start node to a target node. It uses a combination of `g(n)` (the cost from the start node to the current node) and `h(n)` (the heuristic estimated cost from the current node to the end node) to prioritize node exploration, making it efficient for pathfinding in a grid-based environment.

### Q-learning

The Q-learning (`Q_learning.py`) file implements a model-free reinforcement learning algorithm that learns the value of actions in states without requiring a model of the environment. It updates the value (Q) of taking an action in a particular state based on the reward received and the future rewards expected. This approach is more adaptable to environments with stochastic transitions or where the model of the environment is not fully known.

## Run

Simply follow the steps in each of the jupyter notebooks.

### To keep things smooth and breezy, all the magic in these notebooks happens with the wand-waving of common libraries, so feel free to dance through them in any of your beloved ML environments. But just for that extra sprinkle of completeness, I've conjured up a requirements file. Enjoy!

## Comparison Between A-star and Q-learning
Algorithm Type: A-star is a search algorithm, while Q-learning is a reinforcement learning algorithm.
Environment Knowledge: A-star requires knowledge of the environment for its heuristic function, whereas Q-learning does not require a model of the environment and can learn optimal paths through interaction.
Efficiency: A-star is generally more efficient in deterministic environments where the model is known and can be heuristic-driven. Q-learning is better suited for stochastic environments or where the environment model cannot be fully known in advance.
Adaptability: Q-learning can adapt to changes in the environment over time, which makes it suitable for dynamic environments. A-star's performance is fixed once the heuristic is defined and does not adapt to changes in the environment.