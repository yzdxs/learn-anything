#[algorithms - searching](https://my.mindnode.com/87v7siq3h1pqwbPnW13ynTKWxAmwydrQ4HkdiAXi)

![](http://i.imgur.com/kHNE1Kg.png)

# searching


## [linear search](https://www.wikiwand.com/en/Linear_search)

### description

- linear search sequentially moves through your collection (or data structure)

### performance

### implementation

- in python

	- [my solution](https://github.com/nikitavoloboev/algorithms/blob/master/python/sorting/linear_search.py)

### images

- 

### res

- [good overview](https://github.com/stoimen/algorithms/wiki/Sequential-Search)

## [binary search](https://www.wikiwand.com/en/Binary%20search%20algorithm)

### description

- binary search is used to quickly find a value in a **sorted sequence**

- at each step, the algorithm compares the median value in the search space to the target value

- based on the comparison and because the sequence is sorted, it can then eliminate of the search space

- by doing it repeatedly, it will eventually be left with a search space consisting of a single element, the target value

### performance

### requirements

- **can only be used on sorted data**

### res

- [great description from topcoder](https://www.topcoder.com/community/data-science/data-science-tutorials/binary-search/)

- [great visualisation with animals](https://illustrated-algorithms-ommzftrylh.now.sh/)

### images

- 

## [DFS - depth first search](https://www.wikiwand.com/en/Depth-first%20search)

### desc

- in DFS, each vertex has three possible colours representing its state

	- 

	- for most algorithms boolean classification **unvisited / visited** is quite enough

### algo

- initially all vertices are white (unvisited), DFS starts in an arbitrary vertex and runs as follows

	- 1. mark vertex **u** as gray (visited)

	- 2. for each edge (**u, v**) where u is white, run DFS for **u** recursively

	- 3. mark vertex **u** as black and backtrack to the parent

### perf

### img

- example graph ran with DFS

	- 

		- 

			- 

				- 

					- 

						- 

							- 

								- 

									- 

										- 

											- 

												- 

													- 

														- 

															- 

																- 

																	- 

- 

	- In depth first, we would go in the order of 5–>2–>0–>1–>8–>3

### notes

- if a **graph** is **disconnected**, DFS won’t visit all of its vertices

- can easily be implemented using **recursion**

### res

- [BFS and DFS overview](https://www.ics.uci.edu/~eppstein/161/960215.html)

- [DFS for undirected graphs](http://www.algolist.net/Algorithms/Graph/Undirected/Depth-first_search)

	- has a great visual overview of the algorithm

## [BFS - breadth first search](https://www.wikiwand.com/en/Breadth-first%20search)

### desc

### algo

### img

- 5–>2–>8–>0–>1–>3

	- In breadth first, you want to travel down the node, layer by layer. In the image above, first layer has 5, second layer has 2 & 8, third layer has 0 & 1 & 3. So the order would be 5–>2–>8–>0–>1–>3. 

### res

- [amazing visualisation with animals](https://illustrated-algorithms-ommzftrylh.now.sh/bfs)

	- 


# resources


## [Which is the fastest string searching algorithm?](https://www.quora.com/Which-is-the-fastest-string-searching-algorithm)

### Boyer-Moore is the standard for regex matching, which runs in O(n)

- An O(m) algorithm is not possible since we must always process the string at least once

### There are several cool algorithms you can use that take advantage of suffix trees--building one can be done (surprisingly) in linear time


# notes

