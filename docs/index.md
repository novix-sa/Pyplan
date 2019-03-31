# **Pyplan**
Pyplan is an assisted  **Graphical Integrated Development Environment** designed for easily creating and sharing **Data Analytics Apps** based on  **Python** programming language.

## **Code Organization**
The app code is structured using a hierarchical influence diagram of nodes -a Workflow- that helps understand the calculation logic. Nodes are added by means of a drag and drop user interface, and Python code is written inside their Code attribute tab. 
![Node Code](http://img.pyplan.org/index_node_code.png)

Nodes have several properties: Title, ID, Units, Inputs, and Outputs, which are displayed by hovering the cursor over them[L1] . The ID function allows to call the results from other nodes, and works as a global variable for programming.

----------

[L1]El término “focus” es un poco confuso en este contexto. ¿Es la idea que las características aparecen cuando se posa el cursor sobre ellas? La modificación que hicimos expresa eso.

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
eyJoaXN0b3J5IjpbMTMyNjM5ODA2LC0zNjM0NTYyMzEsNjYxOT
I5NjIwLC0xMTQyNjM2NTg3LC01MTM4MjUxMDMsLTE5OTc0MzUw
ODMsLTIwMzUzMzk5NDIsLTYwNzExMTI5NywtMTkwMzc5OTA3OS
wtMTE1MTAwNDk4MiwtMTY0NDM1NjE1NywxNzY4OTUxNDcsMTk1
NzcwMDU0NCwtNDc0NzI0MTExLDEzNzA0NzM1MTMsMjAzMjI3Nj
EwMSwxMTI0ODIzNDY2LDQxMjA4MTIyMCwtMTEzMzk5MDU3MCw2
MjgwNjIxOTldfQ==
-->