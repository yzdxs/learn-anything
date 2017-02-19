#[algorithms - graphs](https://my.mindnode.com/GafxJVenwGZPZbAgjCrCg3brxJJYAxmaTpFnJuRh)

![](http://i.imgur.com/1A0Zilg.png)

#mindmap index 🗄️

# resources


## [tree traversal](http://www.wikiwand.com/en/Tree_traversal)

### TODO: map all algos here


# graph algorithms


## [Dijkstra](https://wikiwand.com/en/Dijkstra%27s%20algorithm)

### desc

- Dijkstra's algorithm is an [algorithm](https://www.wikiwand.com/en/Algorithm) for finding the [shortest paths](https://www.wikiwand.com/en/Shortest_path_problem) between [nodes](https://www.wikiwand.com/en/Vertex_(graph_theory)) in a [graph](https://www.wikiwand.com/en/Graph_(abstract_data_type)), which may represent, for example, road networks

### algo

- step 0

	- step 1

		- step 2

			- step 3

### perf

- worst case: O(n²)

	- although not great, we must always consider what problem we're trying to solve, how big the desired input data is, and if we can make gains in other areas (e.g., caching)

### img

- makes sense

### [example](http://vasir.net/blog/game_development/dijkstras_algorithm_shortest_path)

- the blue circles represent "nodes" or "vertices" and the black lines are "edges" or "node paths"

	- Each edge has a cost associated with it. For -this- image, the number in each node in this image is simply a label for the node, not the individual node cost.

	- Our problem is to find the most cost efficient route from Node1 to Node4

	- The numbers on the node paths represent the "cost" of going between nodes.

	- The shortest path from Node1 to Node4 is to take Node1 to Node3 to Node4, as that is the path where the least cost is incurred

		- Specifically, the cost to go from Node1 to Node3 is (2), plus the cost of Node3 to Node4 (5) is 7 (2 + 5).

	- Now, we can see that the alternative (Node1 to Node2 to Node4) is much more costly (it costs 11, versus our 7). 

	- important note:

		- greedy algorithms aren't really effective here. A greedy algorithm would basically find the cheapest local costs as it traverses the graph with the hopes that it would be globally optimum when it's done. Meaning, a greedy algorithm would basically just take the first low value it sees. In this case, the lower value is 1 but the next value is 10. If we were to simply just apply a greedy algorithm, we end up taking the more costly from Node1 to Node4.

	- **applying the Dijkstra algorithm**

		- step 1

			- The following graph has changed a little from the one shown to the left. The nodes no longer have labels, apart from our starting point NodeA and our goal NodeB.

				- We assign a cost of 0 to Node A and infinity to everything else. We're done with this step now

			- legend

		- step 2

			- There are two temporary nodes adjacent to our current node, so calculate their cost values based on the current node's value + the cost of the adjacent node. Assign that value to the temporary node only if it's less than the value that's already there. So, to clarify

			- The top node is adjacent to the current node and has a cost of infinity. 0 (the current node's value) + 1 (the cost associated with the temporary node) = 1, which is a less than infinity, so we change it's value from infinity to 1. This value is not yet permanent. 

			- Now, do the same calculation for the next adjacent node. which is the bottom node. The value is 0 + 2 = 2, which is also less than infinity. To illustrate:

				- So we now have looked at each temporary node adjacent to the current node, so we're done with this step.

		- step 3

			- go back to step 1. From this point forward, I'll be using the term iteration to describe our progression through the graph via Dijkstra's algorithm. The steps we previously took I'll refer to as iteration 0, so now when we return to step 1 we'll be at iteration 1.

				- iteration 1

					- We’re back at the first step. It says look for the smallest temporary cost value and set it as permanent. We have two nodes to look at, the top node with cost 1 and the bottom node with cost 2.

					- The top node has a cost of 1, which is less than 2, so we set it as permanent and set it as our current node. We designate this by a yellow shadow in the image. Now, it is important to keep in mind that the bottom node still has a temporary cost assigned to it. This temporary cost is what allows the algorithm to find actual cheapest route

						- step 1

							- Find the cheapest node. Done, it’s set as permanent and our current node is this one. This node value will not change.

							- The yellow highlight indicates the node we are currently on, and the green text means the node cost is permanent. The nodes with white text for their costs are temporary nodes

						- step 2

							- Assign cost values. There is only one adjacent node to our current node. It's current value is infinity, which is less than 1 + 10, so we assign 11 to it's temporary cost value.

								- This is not the shortest path from NodeA to NodeB, but that's fine. The algorithm traverses all nodes in the graph, so you get the shortest path from a node to any other node. You can see that the shortest path from NodeA to the top node is the line between NodeA and the top node - well, of course, you say, because that's the only possible path from NodeA to the top node. And you are right to say that, because it's true. But let's say we have a node above the top node (we'll call it Top2). The shortest path to that would from NodeA to the top node to node Top2. Even though our goal is to go from A to B, as a side effect we also get the shortest route to every other node. If that's a bit unclear, it should clear up after we go through the next iteration. 

						- step 3

							- return to step 1

				- iteration 2

					- Ok, so now we look again at the temporary nodes to see which has the lowest value. Even though we calculated the temporary value of B to be 11, we are not done because that value might change (in this case, it will definitely change).

						- step 1

							- Pick the cheapest node and set it as our current node and make it permanent, and assign it its parent. We have two remaining temporary nodes with costs of 2 and 11. 2 is lower, so pick it and set it permanent and set it as our current node. Let’s take a look at the graph to elucidate a bit. So, out of 11 and 2, as we said, 2 is cheaper so pick it. We set this node’s value to be permanent and assign its parent is NodeA, demonstrated by the arrow.

						- step 2

							- Assign cost values to temporary nodes adjacent to the current node. Again, like in the previous iteration, there is only one node to do a cost calculation on, as there is only one temporary node adjacent to the current node. This adjacent node is NodeB. So, we check to see if 2 + 5 < Node B’s temporary cost of 11. It is, so we change Node B from 11 to 7.

						- step 3

							- return to step 1

				- iteration 3

					- step 1

						- Choose the cheapest temporary node value. There is only one temporary node remaining, so we pick it and set it as permanent, set it as our current node, and set it's parent.

					- step 2

						- Assign costs. There are no temporary nodes adjacent to Node B (there –are- permanent nodes, but we don’t check them)

					- step 3

						- return to step 1

				- iteration 4

					- step 1

						- Choose the cheapest temporary node. If none exists or c(x) = infinity, then stop. There are no more temporary nodes and no nodes have values of infinity, so we’re done. Algorithm has finished, and we have our shortest path from A to B, but also from that node to every other node in the graph. With such a small graph as this, it's not immediately obvious how powerful and useful this algorithm is. 

### notes

- Dijkstra's algorithm provides for us the shortest path from NodeA to NodeB

	- This high level concept (not this algorithm specifically) is essentially how Google maps provides you directions.

	- There are many thousands of vertices and edges, and when you ask for directions you typically want the shortest or least expensive route to and from your destinations. 

- very useful in game dev

	- a 2d grid or tile based map, there are many nodes (or tiles) and each tile can have a value associated with it (perhaps it is less expensive to walk across grass than it is to walk across broken bottles or lava).

	- You can set up your tiles so that each tile has a node path value associated with it, so if you put an non player character (NPC) in the map you can use Dijkstra's algorithm to compute the shortest path for the NPC to take to -ANY- tile in your map. 

### proof

### res

## Prim

## [Kruskal](http://www.wikiwand.com/en/Kruskal's_algorithm)

### desc

- Kruskal's algorithm is a [minimum-spanning-tree algorithm](http://www.wikiwand.com/en/Minimum_spanning_tree#Algorithms) which finds an edge of the least possible weight that connects any two trees in the forest

- It is a [greedy algorithm](http://www.wikiwand.com/en/Greedy_algorithm) in [graph theory](http://www.wikiwand.com/en/Graph_theory) as it finds a [minimum spanning tree](http://www.wikiwand.com/en/Minimum_spanning_tree) for a [connected weighted graph](http://www.wikiwand.com/en/Connectivity_(graph_theory)) adding increasing cost arcs at each step

- This means it finds a subset of the [edges](http://www.wikiwand.com/en/Edge_(graph_theory)) that forms a tree that includes every [vertex](http://www.wikiwand.com/en/Vertex_(graph_theory)), where the total weight of all the edges in the tree is minimised.

- If the graph is not connected, then it finds a minimum spanning forest (a minimum spanning tree for each [connected component)](http://www.wikiwand.com/en/Connected_component_(graph_theory))

## Bellman-Ford


