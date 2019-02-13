# **Pyplan**
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

## **Code organization**
The app code is structured through a hierarchical Influence Diagram of nodes ( a Workflow) that helps understand the calculation logic.
![Influence Diagram](http://img.pyplan.org/index_influence_diagram_drag.png)

Nodes are added by a drag and drop user interface and Python code is written inside their definition. Nodes have ID for calling its result from other nodes, working as global variables.
![enter image description here](http://img.pyplan.org/index_node_code.png)

## **Node evaluation**
Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That means that any node which result is an object of these types can be evaluated (by double clicking the node) and visualized as a table or graph with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result.png)
When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change in a node that triggers recalculation downstream the logic.

## **Using Python Libraries**
Any library from the extended Python developing community can be imported to be used to solve specific needs.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)
The example above imports Sklearn for machine learning and the Plottly for rendering the visualization. A Plotly 3D representation is appreciated in the figure below.
![enter image description here](http://img.pyplan.org/index_plotly_graph.png)

## Creating Apps
Apps interfaces are created dragging and dropping model nodes on an interface design tool.
![Interface Designer](http://img.pyplan.org/index_new_interface.png)
After creation, the app interface can be s
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg0NTMxNTM5MSwtMjA2ODM1MjAzNyw4MD
A1MjkyMDIsMTc3NTQwODQwLC0xNDgzNDc1NjEzLC0xODAwMzE0
ODIzLDE5NzQ0NzM1ODUsLTE5ODI4MjYyNTYsLTI0MTM2OTkzOS
wtNjM2MzQ2NDc4LDk3Njg4ODc2MCw5NzEyNzUzMDYsMTY5ODYw
NTIxNCwxODI2Mzg3NTA1LDExOTM4Mjk2NzEsMTAyNzM0Mjc5Ni
wtMTI0NjUyNzIzMywtMTI1NzE5ODI5OSw0NzY2NjM2MDUsLTE5
OTYzMzIwN119
-->