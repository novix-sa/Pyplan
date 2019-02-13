# Pyplan
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

The app code is structured through a hierarchical Influence Diagram ( a Workflow) that helps understand the calculation logic.
![Influence Diagram](http://img.pyplan.org/index_influence_diagram.png)

Python code is written inside nodes definition. Nodes have ID for calling its result from other nodes, working as global variables.
![enter image description here](http://img.pyplan.org/index_node_code.png)
When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps tracks of any change in a node that triggers recalculation downstream the logic.

Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That means that any node which result is an object of these types can be represented as a table or graph with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result.png)

Any library con be imported to be used within a node definition.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)





<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzMzgzODQ1MzMsLTE5ODI4MjYyNTYsLT
I0MTM2OTkzOSwtNjM2MzQ2NDc4LDk3Njg4ODc2MCw5NzEyNzUz
MDYsMTY5ODYwNTIxNCwxODI2Mzg3NTA1LDExOTM4Mjk2NzEsMT
AyNzM0Mjc5NiwtMTI0NjUyNzIzMywtMTI1NzE5ODI5OSw0NzY2
NjM2MDUsLTE5OTYzMzIwNywtOTQyOTc0MzkxLC0xNzIzNjM5ND
k2LC02NDM3MDQwMzcsNzAxMzE2MjM0LDEyOTc3MTQ2MDgsLTIx
MDQ4Mjc3OTVdfQ==
-->