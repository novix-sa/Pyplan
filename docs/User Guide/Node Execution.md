
# Executing Nodes
## Console Output
You can run any node, after editing its code, pressing <kbd>CTRL + Enter</kbd>.
It will show at the right side of the code window the console output resulting from running the node.
![enter image description here](http://img.pyplan.org/Node-execution-code-tab.png)
Any `Print()` statement written between code lines will display it result here.
It is intended for rapid evaluation of the node, to check it is properly defined.

## Result Explorer
Other way to run a node is by pressing <kbd>CTRL + E</kbd>.
This way of running displays more complete information about the node properties and its result.

![](http://img.pyplan.org/Node-execution-profile.png)
One of the most interesting feature accesible through this way of evaluation is the "Show Profile" feature that display the calculation path calculation time and memory usage by step (nodes)
![enter image description here](http://img.pyplan.org/Node-execution-console+.png)

## Evaluating a Node
<kbd>CTRL + R</kbd> to get its result

You can evaluate a node by double clicking on it or pressing <kbd>CTRL + R</kbd> after selecting it.
Differently with the previous run alternatives, the node is run and its result displayed in a new tab, called as the "Title" of the node, with a default table format.

![enter image description here](http://img.pyplan.org/Node-execution-default.png)
Pyplan natively interprets Numpy matrix, Pandas dataframe indexes and Xarray dimensions, that will be automatically displayed at the bottom of the table for pivoting and filtering.
Any default view can be changed using the Edit interface menu that can be launched clicking on the icon shown in the image below

![enter image description here](http://img.pyplan.org/Node-execution-edit-interface.png)

After clicking, the configuration menu is launched where it can be decided how the node will be rendered. After defining the node visualization configuration you must accept the changes to save them.
![enter image description here](http://img.pyplan.org/Node-execution-edit-inter3.png)

## Embedded tools
There are some embedded tools that appears when evaluating a node according to the type of result.
For example, any node that evaluates as a pandas data frame object will display the following tools:

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzODU1MDc5OTgsMjA1NzI5MzcyMSwyOD
U5NDYwNTAsLTQwNzE1NTY0NywtMTQ4NjIzOTc4OCw0NzczNTY4
NTIsMTI2OTExNTg2OCwtNDcyMjE4MjUwLC0zNzk5MTYwODAsLT
E4NTUzMjk5NzksMTQzNTUyNzI4MCwxMDgxMDc5NzQ1LDUwNTk1
MjI0MSw5NjAxMDg2LDExOTAzMjIxMDQsLTU0MjA1NzA0Ml19
-->