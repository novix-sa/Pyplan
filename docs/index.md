# ** Pyplan **
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

## **Code organization**
The app code is structured through a hierarchical Influence Diagram ( a Workflow) that helps understand the calculation logic.
![Influence Diagram](http://img.pyplan.org/index_influence_diagram.png)

Python code is written inside nodes definition. Nodes have ID for calling its result from other nodes, working as global variables.
![enter image description here](http://img.pyplan.org/index_node_code.png)

## **Node evaluation**
Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That means that any node which result is an object of these types can be represented as a table or graph with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result.png)
When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change in a node that triggers recalculation downstream the logic.

## **Using Python Libraries**
Any library can be imported to be used within a node definition.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)





<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk3NDQ3MzU4NSwtMTk4MjgyNjI1NiwtMj
QxMzY5OTM5LC02MzYzNDY0NzgsOTc2ODg4NzYwLDk3MTI3NTMw
NiwxNjk4NjA1MjE0LDE4MjYzODc1MDUsMTE5MzgyOTY3MSwxMD
I3MzQyNzk2LC0xMjQ2NTI3MjMzLC0xMjU3MTk4Mjk5LDQ3NjY2
MzYwNSwtMTk5NjMzMjA3LC05NDI5NzQzOTEsLTE3MjM2Mzk0OT
YsLTY0MzcwNDAzNyw3MDEzMTYyMzQsMTI5NzcxNDYwOCwtMjEw
NDgyNzc5NV19
-->