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
It follows and example importing Sklearn for machine learning and the Plottly for 3D representation.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)


![enter image description here](http://img.pyplan.org/index_plotly_graph.png)


<!--stackedit_data:
eyJoaXN0b3J5IjpbODIzMDU5MjYzLC0xODAwMzE0ODIzLDE5Nz
Q0NzM1ODUsLTE5ODI4MjYyNTYsLTI0MTM2OTkzOSwtNjM2MzQ2
NDc4LDk3Njg4ODc2MCw5NzEyNzUzMDYsMTY5ODYwNTIxNCwxOD
I2Mzg3NTA1LDExOTM4Mjk2NzEsMTAyNzM0Mjc5NiwtMTI0NjUy
NzIzMywtMTI1NzE5ODI5OSw0NzY2NjM2MDUsLTE5OTYzMzIwNy
wtOTQyOTc0MzkxLC0xNzIzNjM5NDk2LC02NDM3MDQwMzcsNzAx
MzE2MjM0XX0=
-->