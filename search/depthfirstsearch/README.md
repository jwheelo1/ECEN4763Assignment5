# Depth first search

Depth-first search (DFS) is an algorithm used to determine whether there is a path between two nodes. It traverses iteratively through the graph, checking a node's children before it checks its siblings, therefore going deep in the graph before it can go wide, hence the name.

## Getting Started Steps

- running "make clean" will clean the project by removing all "pycache" folders and files
- running "make format will run autopep8 and docformatter to auto format the code
- running "make style" will run a lint checker on your code
- running "make test" or "make" will run all unit tests that have been created
- running "make coverage" will run all unit tests and give you a code coverage report

# Depth first search

## Requirements

- You must implement a class that handles the below interfaces for a DFS search.
- The class name must be called "DFSearch".
- You must implement at least 14 unit tests.
- Must get a 10/10 when running "make style"
- Your unit tests must reach 100% code coverage

## Interface

- The constructor __init__(self, graph_dict=None) should initialize the graph by calling the graph init function with graph_dict as the parameter. You may want to include more class variables to help in the depth first search. 
- The function dfs(self, node) traverses the graph using depth first search from node. It returns a list of the vertices visited in the order that they were first visited (i.e. a preordering). Visit the nodes in order of how they are stored in the graph. The example below may help.
- The function add_graph_dfs(self, graph) should replace the current graph to search on.
- You may add any extra helper functions that you deem necessary.
- The function get_space_complexity(), returns the space complexity of the search.
- The function get_time_complexity(), returns the time complexity of the search.

## Example
Given the following graph:
'''
GRAPH = {
    'a': ['b', 'c'],
    'b': ['d'],
    'c': ['d'],
    'd': []
}
'''
a depth first search starting at a would return the following: ['a', 'b', 'd', 'c'] as the nodes are traversed to in the order that they are stored in the graph. 

## Tests

- Space and time complexity of the sorting algorithm.
- Tests on a variety of types of graphs (complete, disjoint, containing cycles, etc)
- Tests starting from invalid vertices (should return [])
- Tests on empty graphs

## Library

You can only use basic python libraries (no special imports).
