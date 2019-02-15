# **Pyplan**
Pyplan is an assisted **Graphical Integrated Development Environment** designed for easy creation and sharing of **Data Analytics Apps** based on **Python** programming language.

## **Code Organization**
The app code is structured through a hierarchicaln Influence Diagram of nodes -a Workflow- that helps understand the calculation logic.
Nodes are added by a drag and drop user interface and Python code is written inside their Code attribute. 
![Node Code](http://img.pyplan.org/index_node_code.png)

Nodes have several properties: Title, ID, Units, Inputs, Outputs that are displayed when focus. 
The ID allows calling its result from other nodes, working as global variables.

![Node properties](http://img.pyplan.org/index_node_properties1.png)


## **Node Evaluation**
Pyplan natively interprets Pandas, Numpy and XArray dataobjects. That allows any node which result is an object of these types can be evaluated (by double clicking the node) and visualized with native Pyplan charts and tables with no additional coding.
![enter image description here](http://img.pyplan.org/index_node_result1.png)

When asking to run a node, all precedent nodes are calculated too, and its results are kept in memory, available for inspection and reuse. Pyplan engine keeps track of any change in a node that triggers recalculation downstream the calc logic path.

## **Using Python Libraries**
Any library from the extended Python developing community can be imported to be used to solve specific needs.
![Importing libraries for use within Pyplan](http://img.pyplan.org/index_import_lib.png)
The example above imports Sklearn for machine learning and the Plottly visualization library for rendering the graph. 
A Plotly 3D representation is appreciated in the figure below.
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
eyJoaXN0b3J5IjpbMTE4NjY2NzkwMywtMTkwMzc5OTA3OSwtMT
E1MTAwNDk4MiwtMTY0NDM1NjE1NywxNzY4OTUxNDcsMTk1Nzcw
MDU0NCwtNDc0NzI0MTExLDEzNzA0NzM1MTMsMjAzMjI3NjEwMS
wxMTI0ODIzNDY2LDQxMjA4MTIyMCwtMTEzMzk5MDU3MCw2Mjgw
NjIxOTksLTE3MDY3NDU0MTcsLTE4NjkyNzk0Miw4Nzg5OTU0OC
wtMjA2ODM1MjAzNyw4MDA1MjkyMDIsMTc3NTQwODQwLC0xNDgz
NDc1NjEzXX0=
-->