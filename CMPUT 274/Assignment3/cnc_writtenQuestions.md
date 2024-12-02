(a)

| Symbol | Meaning        |
| ------ | -------------- |
| \+     | Addition       |
| \-     | Subtraction    |
| \*     | Multiplication |
| \/     | Division       |
| \*\*   | Exponentiation |
Assuming that the nodes contain one of the previous symbols or any $n \in \mathbb{C}$ 

1st Equation
![[1st Equation.png]]
2nd Equation
![[2nd Equation.png]]


(b)

Start at the lowest level and for each pair of nodes go one node up and replace this node with the result of the operation stored in that node applied to node.left and node.right 
(in the order $left \rightarrow operation \rightarrow right$) 
then set the left and right pointers of the node to None,  if none are left in the current level go up to the next lowest level, do this until you are left with a single node. This is your answer.