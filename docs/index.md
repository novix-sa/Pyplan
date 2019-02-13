# Pyplan
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

## Code organization
The app code is structured through a hierarchical Influence Diagram ( a Workflow) that helps understand the calculation logic.
![Influence Diagram](http://img.pyplan.org/index_influence_diagram.png)

Python code is written inside nodes definition. Nodes have ID for calling its result from other nodes, working as global variables.
![enter image description here](http://img.pyplan.org/index_node_code.png)

## Node evaluation
Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That means that any node which result is an object of these types can be represented as a table or graph with no additional coding.
When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change in a node that triggers recalculation downstream the logic.

![enter image description here](http://img.pyplan.org/index_node_result.png)

## Python Libraries Use
Any library can be imported to be used within a node definition.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)





<!--stackedit_data:
eyJoaXN0b3J5IjpbOTQ0NzAwNjY4LC0xOTgyODI2MjU2LC0yND
EzNjk5MzksLTYzNjM0NjQ3OCw5NzY4ODg3NjAsOTcxMjc1MzA2
LDE2OTg2MDUyMTQsMTgyNjM4NzUwNSwxMTkzODI5NjcxLDEwMj
czNDI3OTYsLTEyNDY1MjcyMzMsLTEyNTcxOTgyOTksNDc2NjYz
NjA1LC0xOTk2MzMyMDcsLTk0Mjk3NDM5MSwtMTcyMzYzOTQ5Ni
wtNjQzNzA0MDM3LDcwMTMxNjIzNCwxMjk3NzE0NjA4LC0yMTA0
ODI3Nzk1XX0=
-->