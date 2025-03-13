GRAPH BASED- SOCIAL NETWORK ANALYSIS 

Creating a Graph-Based Social Network Analysis in C requires implementing a graph structure where:Nodes represent users.

Edges represent friendships between users.

Key Features

1. Graph Representation using an adjacency list.

2. Shortest Path Calculation using Breadth-First Search (BFS).

3. Friend Recommendations using common friends.

4. Handling Cycles using visited arrays during traversal.

HOW IT WORKS 

1. Graph Representation
Users are stored in an adjacency list.
Each user has a linked list of their friends.

2. Finding the Shortest Path
Uses BFS to traverse the graph.
Stores the previous node to reconstruct the path.

3. Friend Recommendations
Counts mutual friends of a user’s friends.
Suggests friends who are not directly connected.

4. Handling Cycles
BFS ensures each user is visited only once.

A visited array prevents infinite loops.

Example Output:

Social Network Graph:
User 0 -> 2 1 
User 1 -> 4 3 0 
User 2 -> 4 0 
User 3 -> 5 1 
User 4 -> 5 2 1 
User 5 -> 4 3 

Shortest Path from User 0 to User 5:
0 1 4 5 

Friend Recommendations for User 0:
User 3 (Mutual Friends: 1)
User 5 (Mutual Friends: 1)
