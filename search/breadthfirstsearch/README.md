# Breadth first search

Breadth-first search (BFS) is an algorithm used to traverse graphs. It traverses the graph by looking at siblings of a node before the node's children, which is done by adding nodes to a queue and selecting the least recently added node to traverse next.

## Getting Started Steps

- running "make clean" will clean the project by removing all "pycache" folders and files
- running "make format will run autopep8 and docformatter to auto format the code
- running "make style" will run a lint checker on your code
- running "make test" or "make" will run all unit tests that have been created
- running "make coverage" will run all unit tests and give you a code coverage report

# Breadth first search

## Requirements

- You must implement a class that handles the below interfaces for a BFS search.
- The class name must be called "BFSearch".
- You must implement at least 14 unit tests.
- Must get a 10/10 when running "make style"
- Your unit tests must reach 100% code coverage

## Interface

- The constructor __init__(self, graph_dict=None) should initialize the graph by calling the graph init function with graph_dict as the parameter. You may want to include more class variables to help in the breadth first search.
- The function bfs(self, node) traverses the graph using Breadth First Search. It should return an array containing the vertices visited in the order that they were first visited. See the example below.
- The function add_graph(self, graph) should replace the current graph to search on.
- The function get_space_complexity(), returns the space complexity of the search.
- The function get_time_complexity(), returns the time complexity of the search.
- You may add any extra helper functions that you deem necessary.

## Example
Given the following graph:
```
GRAPH = {
    'a': ['b', 'c'],
    'b': ['d'],
    'c': ['d'],
    'd': []
}
```
a breadth first search starting at a would return the following: ['a', 'b', 'c', 'd'] as the nodes are traversed to in the order that they are stored in the graph.

## Tests

- Space and time complexity of the algorithm.
- Tests on a variety of types of graphs (complete, disjoint, containing cycles, etc)
- Tests starting from invalid vertices (should return [])
- Tests on empty graphs

## Library

You can only use basic python libraries (no special imports).
