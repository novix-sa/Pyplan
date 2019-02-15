# **Pyplan**
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

## **Code Organization**
The app code is structured through a hierarchicaln Influence Diagram of nodes -a Workflow- that helps understand the calculation logic.
Nodes are added by a drag and drop user interface and Python code is written inside their Code attribute. 
![Node Code](http://img.pyplan.org/index_node_code.png)

Nodes have several properties: Title, ID, Units, Inputs, Outputs that are displayed when focus. 
The ID allows calling its result from other nodes, working as global variables.

![Node properties](http://img.pyplan.org/index_node_properties1.png)


## **Node alu**

Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That means that any node which result is an object of these types can be evaluated (by double clicking the node) and visualized with native Pyplan charts and tables with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result1.png)

When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change represented as a table or graph with no additional coding.


## **Using Python Libraries**
Any library from the extended Python developing community can be imported to be used to solve specific needs.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)
The example above imports Sklearn for machinnd Data Analytics potential.

Trough an innovative U/I consisting on influence diagrams, huge models can be learning and the Plottly for rendering the visualization. A Plotly 3D representation is appreciated in the figure below.
![enter image description here](http://img.pyplan.org/index_plotly_graph.png)

## **Creating Apps**
Apps interfaces are created dragging and dropping model nodes on an interface design tool.
![Interface Designer](http://img.pyplan.org/index_new_interface2.png)

After creation, the app can be shared with anybody internally or outside the enterprise environment.
![enter image description here](http://img.pyplan.org/index_share_app_ext.png)sily construct and audit by software experts as well as businessmen.




## User Interface
### File manager
### Modeler
### UI designer
### Task Manager
### Configuration








<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2NDQzNTYxNTcsMTc2ODk1MTQ3LDE5NT
c3MDA1NDQsLTQ3NDcyNDExMSwxMzcwNDczNTEzLDIwMzIyNzYx
MDEsMTEyNDgyMzQ2Niw0MTIwODEyMjAsLTExMzM5OTA1NzAsNj
I4MDYyMTk5LC0xNzA2NzQ1NDE3LC0xODY5Mjc5NDIsODc4OTk1
NDgsLTIwNjgzNTIwMzcsODAwNTI5MjAyLDE3NzU0MDg0MCwtMT
Q4MzQ3NTYxMywtMTgwMDMxNDgyMywxOTc0NDczNTg1LC0xOTgy
ODI2MjU2XX0=
-->