## ExpNo 2 : 
Implement Depth First Search Traversal of a Graph 
## Name:
PRAGATHI KUMAR 
## Register Number:
212224230200     
## Aim:
To Implement Depth First Search Traversal of a Graph using Python 3.
## Theory:
Depth First Traversal(or DFS) for a graph is like Depth First Traversal of a tree. The only catch here is that, unlike trees, graphs may contain cycles (a node may be visited twice). Use a Boolean visited array to avoid processing a node more than once. A graph can have more than one DFS traversal. 
Depth-first search is an algorithm for traversing or searching trees or graph data structures. The algorithm starts at the root node (selecting some arbitrary node as the root node in the case of a graph) and explores as far as possible along each branch before backtracking.
## Step 1: 
Initially, stack and visited arrays are empty.

 ![alt text](<Screenshot 2025-04-30 133710.png>)


Queue and visited arrays are empty initially.
Stack and visited arrays are empty initially.
## Step 2:
 Visit 0 and put its adjacent nodes which are not visited yet into the stack.
![alt text](image.png)

 Visit node 0 and put its adjacent nodes (1, 2, 3) into the stack
 Visit node 0 and put its adjacent nodes (1, 2, 3) into the stack

## Step 3:
 Now, Node 1 at the top of the stack, so visit node 1 and pop it from the stack and put all of its adjacent nodes which are not visited in the stack.
 ![alt text](image-1.png)
Visit node 1
 Visit node 1

## Step 4:
 Now, Node 2 at the top of the stack, so visit node 2 and pop it from the stack and put all of its adjacent nodes which are not visited (i.e, 3, 4) in the stack.
 ![alt text](image-2.png)

 Visit node 2 and put its unvisited adjacent nodes (3, 4) into the stack
 Visit node 2 and put its unvisited adjacent nodes (3, 4) into the stack

## Step 5:
 Now, Node 4 at the top of the stack, so visit node 4 and pop it from the stack and put all of its adjacent nodes which are not visited in the stack.
 ![alt text](image-3.png)

 Visit node 4
 Visit node 4

## Step 6:
 Now, Node 3 at the top of the stack, so visit node 3 and pop it from the stack and put all of its adjacent nodes which are not visited in the stack.
 ![alt text](image-4.png)
Visit node 3
Visit node 3

Now, the Stack becomes empty, which means we have visited all the nodes, and our DFS traversal ends.

## Algorithm:
```
 1.Construct a Graph with Nodes and Edges
 2.Depth First Search Uses Stack and Recursion
 3.Insert a START node to the STACK
 4.Find its Successors Or neighbors and Check whether the node is visited or not
 5.If Not Visited, add it to the STACK. Else Call The Function Again Until No more nodes needs to be visited.
```

## Sample Input:
```
8 9 
A B 
A C 
B E 
C D 
B D 
C G 
D F 
G F 
F H 
```
## Sample Output:
```
['A', 'B', 'E', 'D', 'C', 'G', 'F', 'H']
```


## Sample Input:
```
5 5 
0 1 
0 2 
0 3 
2 3 
2 4 
```

## Sample Output
```
['0', '1', '2', '3', '4']
```
## Result:
Thus,a Graph was constructed and implementation of Depth First Search for the same graph was done successfully.

