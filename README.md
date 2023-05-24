# Zewail-city-navigation-AI-program

This is an application on Reinforcement Learning (RL) of type Active search using Q-value iteration.

* Phase 1: 

It  involves modeling the problem of finding the optimal way to travel from one place on the Zewail City (ZC) campus to another place as a search problem. The following are the tasks involved in this project:

Define the abstraction of the problem using the state space representation, successor function, set of actions.
To represent the state space, we can use a graph where each node represents a location on the ZC campus, and each edge represents a path between two locations. The set of actions would be the set of paths that can be taken from each node to its neighboring nodes.

Modeling assumptions
We assumed that there are no obstacles or roadblocks on the paths between the nodes, and that there are no traffic lights or other traffic control mechanisms. Additionally, we will assume that the distance between two nodes is proportional to the time it takes to travel between them.

Uninformed search algorithms
Using BFS, DFS, and IDS, we can find the best route between two nodes on the ZC campus. BFS is guaranteed to find the shortest path between two nodes, but it can be slow and memory-intensive. DFS is faster and uses less memory, but it may not find the shortest path. IDS is a compromise between BFS and DFS, and it guarantees to find the shortest path while using less memory than BFS.

Reflection on the results of the three algorithms
BFS is the best choice if we want to find the shortest path between twopoints on the ZC campus, but it may not be efficient for large or complex graphs. DFS is faster but may not find the shortest path, and IDS is a good compromise between the two. The choice of which algorithm to use depends on the size and complexity of the graph, as well as the time and memory constraints of the problem.

Heuristic functions
We defined two reasonable heuristic functions to use with the Greedy best-first and A* algorithms. One possible heuristic function is the straight-line distance between two nodes, which provides an estimate of the minimum distance between them. Another possible heuristic function is the Manhattan distance, which is the sum of the absolute differences between the x and y coordinates of two nodes.

Hill climbing and simulated annealing
We also used hill climbing or simulated annealing to find the best route between two nodes on the ZC campus. Hill climbing involves starting at a random point and searching for the highest point in the surrounding area, while simulated annealing is a probabilistic variant of hill climbing that allows for occasional moves that decrease the objective function.

* Phase 2:
This phase involves using reinforcement learning, specifically Q-learning, to design a route for an agent to pick up and deliver items from one location to another inside Zewail City (ZC) with the minimum number of steps. The agent starts at the main gate of ZC and needs to pick up items from the NB and HB locations and deliver them to the AB and One-stop-shop locations, respectively.

The project required designing an agent-based system that explores and learns in initially unknown environments. It involves using Q-learning, a type of reinforcement learning algorithm, to learn promising paths for the agent to take in order to complete its task efficiently.

The assumptions made in this phase include that each pickup location contains 4 items to be delivered, each delivery location can have at most 4 items, and the agent can only hold one item at a time.

The goal of the project was to design a route for the agent to send all items from pick-up locations to delivery locations with the shortest path using Q-learning. This involves defining a state space representation, successor function, and set of actions for the problem, as well as defining rewards and updating Q-values during the learning process.

After training the Q-learning algorithm, the agent used the learned policy to navigate the grid world and efficiently complete the task of picking up and delivering items.


