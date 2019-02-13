# **Pyplan**
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

## **Code organization**
The app code is structured through a hierarchical Influence Diagram of nodes ( a Workflow) that helps understand the calculation logic. Nodes are added by dragg
![Influence Diagram](http://img.pyplan.org/index_influence_diagram_drag.png)

Python code is written inside nodes definition. Nodes have ID for calling its result from other nodes, working as global variables.
![enter image description here](http://img.pyplan.org/index_node_code.png)

## **Node evaluation**
Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That means that any node which result is an object of these types can be evaluated (by double clicking the node) and visualized as a table or graph with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result.png)
When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change in a node that triggers recalculation downstream the logic.

## **Using Python Libraries**
Any library from the extended Python developing community can be imported to be used to solve specific needs.
It follows and example importing Sklearn for machine learning and the Plottly for 3D representation.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)

![enter image description here](http://img.pyplan.org/index_plotly_graph.png)


<!--stackedit_data:
eyJoaXN0b3J5IjpbMjEyNjc1ODEwMiwxNzc1NDA4NDAsLTE0OD
M0NzU2MTMsLTE4MDAzMTQ4MjMsMTk3NDQ3MzU4NSwtMTk4Mjgy
NjI1NiwtMjQxMzY5OTM5LC02MzYzNDY0NzgsOTc2ODg4NzYwLD
k3MTI3NTMwNiwxNjk4NjA1MjE0LDE4MjYzODc1MDUsMTE5Mzgy
OTY3MSwxMDI3MzQyNzk2LC0xMjQ2NTI3MjMzLC0xMjU3MTk4Mj
k5LDQ3NjY2MzYwNSwtMTk5NjMzMjA3LC05NDI5NzQzOTEsLTE3
MjM2Mzk0OTZdfQ==
-->