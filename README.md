# Path Planning Algorithms
### Haoliang Shang hshang@ethz.ch
This repository contains two distinct path planning solutions for problems 1-3, implemented using the A-star algorithm and Q-learning. These algorithms are designed to navigate from a start point to an end point efficiently in a given environment.

<u>Please look at A-star.ipynb first as this one solves every subtasks required in the assignment while the Q-Learning one is more like a playground.</u> 

</br>
</br>

## 1. Algorithms

### A-star Algorithm

The A-star (`A_star.ipynb`) algorithm is a heuristic-based search algorithm that finds the least-cost path from a given start node to a target node. It uses a combination of `g(n)` (the cost from the start node to the current node) and `h(n)` (the heuristic estimated cost from the current node to the end node) to prioritize node exploration, making it efficient for pathfinding in a known environment.

### Q-learning

The Q-learning (`Q_learning.ipynb`) file implements a reinforcement learning algorithm that learns the value of actions in states without requiring a model of the environment. It updates the value (Q) of taking an action in a particular state based on the reward received and the future rewards expected. This approach is more adaptable to unknown environments.

</br>
</br>

## 2. Content

There are some optional steps which I found intuitive to do to either further improve my algorithms or to demonstrate my skills. Please ignore those if you find it unnecessary.

### A_star.ipynb
* (Optional) Read in the Grid with OpenCV
* Basic Path Planning Implementation
    * Task 1 & 2: Create a 5x5 grid with the obstacles, mark start and end points 
    * Task 3: Algorithm Implementation
    * Task 4: Visualization
* Integration of Waypoints
    * (Optional) Avoid passing through the finish point
* Varying Terrain
    * (Optional) New Elevation Map


### Q_learning.ipynb
* Basic Path Planning Implementation
* Integration of Waypoints
* Varying Terrain

</br>
</br>

## 3. Run

Simply follow the steps in each of the jupyter notebooks.

<u>To keep things smooth and simple, all the magic in these notebooks happens with the wand-waving of common libraries, so feel free to play through them in any of your beloved ML environments. But just for completeness, I've conjured up a requirements.txt file. Enjoy!</u>

</br>
</br>

## 4. Comparison Between A-star and Q-learning
Type: A-star is a deterministic search algorithm, while Q-learning is a reinforcement learning algorithm that is stochastic in nature.

Environment Requirement: A-star requires knowledge of the environment for its heuristic function, whereas Q-learning does not require a model of the environment and can learn optimal paths through interaction.

Efficiency: A-star is generally more efficient in deterministic environments. Q-learning is better suited for stochastic environments or where the environment model cannot be fully known in advance.

Adaptability: Q-learning can adapt to changes in the environment and is also suitable for dynamic environments. A-star's performance is fixed once the heuristic is defined and does not adapt to changes in the environment.