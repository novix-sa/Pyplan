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
Any library from the extended Python developing community can be imported to be used to solve specific needs.
It follows and example importing
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)





<!--stackedit_data:
eyJoaXN0b3J5IjpbMjM1ODQxODQ4LDE5NzQ0NzM1ODUsLTE5OD
I4MjYyNTYsLTI0MTM2OTkzOSwtNjM2MzQ2NDc4LDk3Njg4ODc2
MCw5NzEyNzUzMDYsMTY5ODYwNTIxNCwxODI2Mzg3NTA1LDExOT
M4Mjk2NzEsMTAyNzM0Mjc5NiwtMTI0NjUyNzIzMywtMTI1NzE5
ODI5OSw0NzY2NjM2MDUsLTE5OTYzMzIwNywtOTQyOTc0MzkxLC
0xNzIzNjM5NDk2LC02NDM3MDQwMzcsNzAxMzE2MjM0LDEyOTc3
MTQ2MDhdfQ==
-->