# List of algorithms (CAP 5636)

* Depth First Search
    - Depth first search is a tree-based graph traversal algorithm that is used to search a graph. 
    - Unlike BFS, a DFS algorithm traverses a tree or graph from the parent vertex down to its children and grandchildren vertices in a single path until it reaches a dead end.
	- When there are no more vertices to visit in a path, the DFS algorithm will backtrack to a point where it can choose another path to take. It will repeat the process over and over until all vertices have been visited
    
* Breadth First Search
	- Breadth First Search (BFS) algorithm traverses a graph in a breadthward motion and uses a queue to remember to get the next vertex to start a search, when a dead end occurs in any iteration.
	- We traverse through one entire level of children nodes first, before moving on to traverse through the grandchildren nodes. And we traverse through an entire level of grandchildren nodes before going on to traverse through great-grandchildren nodes.

* Uniform Cost Search 

	- Uniform cost search is a tree search algorithm related to breadth-first search. Whereas breadth-first search determines a path to the goal state that has the least number of edges, uniform cost search determines a path to the goal state that has the lowest weight.
	- It's worth observing that uniform cost search assumes that no edges have negative weight. If any edges have negative weight, then it is possible that a path p begins with a vertex whose edge to its parent has a high positive weight, which will exclude it from consideration by the search.

* Dijkstra's Algorithm
	- Dijkstra’s algorithm is very similar to Prim’s algorithm for minimum spanning tree. Like Prim’s MST, we generate a SPT (shortest path tree) with given source as root. 
	- We maintain two sets, one set contains vertices included in shortest path tree, other set includes vertices not yet included in shortest path tree. 
	- At every step of the algorithm, we find a vertex which is in the other set (set of not yet included) and has a minimum distance from the source.

* Minimum-Spanning-Tree
	- A minimum spanning tree (MST) or minimum weight spanning tree is a subset of the edges of a connected, edge-weighted undirected graph that connects all the vertices together, without any cycles and with the minimum possible total edge weight.
	1. Kruskal's Algorithm
		- Kruskal's algorithm is a minimum-spanning-tree algorithm which finds an edge of the least possible weight that connects any two trees in the forest. It is a greedy algorithm in graph theory as it finds a minimum spanning tree for a connected weighted graph adding increasing cost arcs at each step.
	2. Prim's Algorithm	
		- Prim's algorithm is a greedy algorithm that finds a minimum spanning tree for a weighted undirected graph. This means it finds a subset of the edges that forms a tree that includes every vertex, where the total weight of all the edges in the tree is minimized. 

* Priority Queues
	- Priority Queue is similar to queue where we insert an element from the back and remove an element from front, but with a one difference that the logical order of elements in the priority queue depends on the priority of the elements. 
	- The element with highest priority will be moved to the front of the queue and one with lowest priority will move to the back of the queue. 
* A* Search
	- A* is a computer algorithm that is widely used in pathfinding and graph traversal. The algorithm efficiently plots a walkable path between multiple nodes, or points, on the graph.
	- On a map with many obstacles, pathfinding from points A to B can be difficult. A robot, for instance, without getting much other direction, will continue until it encounters an obstacle, as in the path-finding example to the left below.
	- However, the A* algorithm introduces a heuristic into a regular graph-searching algorithm, essentially planning ahead at each step so a more optimal decision is made.
* Minimax
	- Minimax is a decision-making algorithm, typically used in a turn-based, two player games. The goal of the algorithm is to find the optimal next move.
	- In the algorithm, one player is called the maximizer, and the other player is a minimizer. If we assign an evaluation score to the game board, one player tries to choose a game state with the maximum score, while the other chooses a state with the minimum score.
	- In other words, the maximizer works to get the highest score, while the minimizer tries get the lowest score by trying to counter moves.
* Alpha-Beta Pruning
	- Alpha-Beta pruning is not actually a new algorithm, rather an optimization technique for minimax algorithm.
	- It reduces the computation time by a huge factor. This allows us to search much faster and even go into deeper levels in the game tree. It cuts off branches in the game tree which need not be searched because there already exists a better move available. 
	- It is called Alpha-Beta pruning because it passes 2 extra parameters in the minimax function, namely alpha and beta.
* Expectimax Search
	- The expectiminimax algorithm is a variation of the minimax algorithm, for use in artificial intelligence systems that play two-player zero-sum games, such as backgammon, in which the outcome depends on a combination of the player's skill and chance elements such as dice rolls. 
	- In addition to "min" and "max" nodes of the traditional minimax tree, this variant has "chance" nodes, which take the expected value of a random event occurring. In game theory terms, an expectiminimax tree is the game tree of an extensive-form game of perfect, but incomplete information.
* Q-Learning
	- Q-learning is a reinforcement learning technique used in machine learning. The goal of Q-learning is to learn a policy, which tells an agent what action to take under what circumstances. 
	- It does not require a model of the environment and can handle problems with stochastic transitions and rewards, without requiring adaptations.
* State Space Graphs
	- State space search is a process used in the field of computer science, including artificial intelligence, in which successive configurations or states of an instance are considered, with the intention of finding a goal state with a desired property.
	- Problems are often modelled as a state space, a set of states that a problem can be in. The set of states forms a graph where two states are connected if there is an operation that can be performed to transform the first state into the second.
* Iterative Deepening
	- Iterative deepening depth first search is a hybrid of BFS and DFS. In IDDFS, we perform DFS up to a certain “limited depth,” and keep increasing this “limited depth” after every iteration.
	- It is a state space/graph search strategy in which a depth-limited version of depth-first search is run repeatedly with increasing depth limits until the goal is found. 
	- IDDFS is equivalent to breadth-first search, but uses much less memory; at each iteration, it visits the nodes in the search tree in the same order as depth-first search, but the cumulative order in which nodes are first visited is effectively breadth-first.
* Greedy Search
	- A greedy algorithm is an algorithmic paradigm that follows the problem solving heuristic of making the locally optimal choice at each stage with the intent of finding a global optimum. 
	- In many problems, a greedy strategy does not usually produce an optimal solution, but nonetheless a greedy heuristic may yield locally optimal solutions that approximate a globally optimal solution in a reasonable amount of time.
* Markov Decision Processes
	- MDPs are meant to be a straightforward framing of the problem of learning from interaction to achieve a goal. The agent and the environment interact continually, the agent selecting actions and the environment responding to these actions and presenting new situations to the agent.
	- Formally, an MDP is used to describe an environment for reinforcement learning, where the environment is fully observable. Almost all RL problems can be formalized as MDPs.
* Reinforcement Learning
	- Reinforcement learning is an area of machine learning concerned with how software agents ought to take actions in an environment so as to maximize some notion of cumulative reward. 
	- The problem, due to its generality, is studied in many other disciplines, such as game theory, control theory, operations research, information theory, simulation-based optimization, multi-agent systems, swarm intelligence, statistics and genetic algorithms.