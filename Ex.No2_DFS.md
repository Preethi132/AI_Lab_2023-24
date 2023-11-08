# Ex.No: 2  Implementation of Depth First Search
### DATE:                                                                            
### REGISTER NUMBER : 212221040132
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:
```
graph = {
 '5' : ['3','7'],
 '3' : ['2', '4'],
 '7' : ['8'],
 '2' : [],
 '4' : ['8'],
 '8' : []}
visited = [] # List for visited nodes.
queue = [] #Initialize a queue
def bfs(visited, graph, node): #function for BFS
 visited.append(node)
 queue.append(node)
 while queue: 
     m = queue.pop(0)
     print (m, end = " ")
     for neighbour in graph[m]:
         if neighbour not in visited:
             visited.append(neighbour)
             queue.append(neighbour)
print("Following is the Breadth-First Search")
bfs(visited, graph, '5')
```
### Output:

![image](https://github.com/Preethi132/AI_Lab_2023-24/assets/136288465/3b31419a-b0d7-4519-a013-669a297bf153)


### Result:
Thus the depth first search order was found sucessfully.
