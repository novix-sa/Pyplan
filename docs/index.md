# **Pyplan**
Pyplan is an assisted  **Graphical Integrated Development Environment** designed for easily creating and sharing **Data Analytics Apps** based on  **Python** programming language.

## **Code Organization**
The app code is structured through a hierarchical influence diagram of nodes -a Workflow- that helps understand the calculation logic.
Nodes are added by a drag and drop user interface and Python code is written inside their Code attribute. 
![Node Code](http://img.pyplan.org/index_node_code.png)

Nodes have several properties: Title, ID, Units, Inputs, Outputs that are displayed when focus. 
The ID allows calling its result from other nodes, working as global variables for programming.

![Node properties](http://img.pyplan.org/index_node_properties1.png)


## **Node Evaluation**
Pyplan natively interprets Pandas, Numpy and XArray data objects. Any node which result is an object of these types can be evaluated (by double clicking the node) and visualized with native Pyplan charts and tables with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result1.png)

When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change in a node that triggers recalculation downstream the calculation logic path.

## **Using Python Libraries**
Any library from the extended Python developing community can be imported to be used to solve specific needs.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)
The example above imports Sklearn for machine learning and the Plottly visualization library for rendering the graph. 
A Plotly 3D representation is appreciated in the figure below.
![enter image description here](http://img.pyplan.org/index_plotly_graph.png)

## **Creating Apps**
Apps interfaces are created dragging and dropping nodes on an interface design tool.
![enter image description here](http://img.pyplan.org/index_interface_design.png)

![Interface Designer](http://img.pyplan.org/index_interface_design1.png)

After creation, the app can be shared with anybody internally or outside the enterprise environment.

![enter image description here](http://img.pyplan.org/index_share_app_ext.png)





<!--stackedit_data:
eyJoaXN0b3J5IjpbMjAyNjI0MzM3NSwtMzYzNDU2MjMxLDY2MT
kyOTYyMCwtMTE0MjYzNjU4NywtNTEzODI1MTAzLC0xOTk3NDM1
MDgzLC0yMDM1MzM5OTQyLC02MDcxMTEyOTcsLTE5MDM3OTkwNz
ksLTExNTEwMDQ5ODIsLTE2NDQzNTYxNTcsMTc2ODk1MTQ3LDE5
NTc3MDA1NDQsLTQ3NDcyNDExMSwxMzcwNDczNTEzLDIwMzIyNz
YxMDEsMTEyNDgyMzQ2Niw0MTIwODEyMjAsLTExMzM5OTA1NzAs
NjI4MDYyMTk5XX0=
-->