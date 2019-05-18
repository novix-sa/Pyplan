# Model

Pyplan structures code trough an influence digram of nodes. Nodes have properties that could be inspected and edited trough tabs <kbd>Properties</kbd><kbd>Code</></kbd><kbd>Docs</kbd>.

![enter image description here](http://img.pyplan.org/model-node-prop1.png)
The <kbd>Properties</kbd> tab contains:
 - **Title**: is the legend that will be displayed over the node
 - **ID**: the node identification. The way to call the node values when coding.
 - **Units**: A text value that will be displayed next to the title when evaluating a node.
 - **#**: the number format of the node.
 - **Inputs/Outputs**: list of nodes titles directly linked to the selected node. You can navigate to anyone through clicking on the node name.
 - **Code**: shortcut to the Code tab
The <kbd>Code</></kbd> tab:
![enter image description here](http://img.pyplan.org/model-code-tab.png)
The code tab presents two windows. The left one is the space to insert the code of the node.
Nodes definition must end with defining the variable result

On the right window you will find the console output. It shows 



The Python code is included asNodes are the su
The app code is structured using a hierarchical influence diagram of nodes -a Workflow- that helps understand the calculation logic. Nodes are added by means of a drag and drop user interface, and Python code is written inside their Code attribute tab. 
![Node Code](http://img.pyplan.org/index_node_code.png)

Nodes have several properties: Title, ID, Units, Inputs, and Outputs, which are displayed when a node is selected. The ID function allows to call the results from other nodes, and works as a global variable for programming.

![Node properties](http://img.pyplan.org/index_node_properties1.png)


## Model Creation
### Creating a new model
### Default imports
In order to avoid declaring the 'Import' sentence en each node, there is a node, called Default imports that collects the Library that will not require to declare import all across the model.

`import numpy, pandas, cubepy, xarray
#fill the following dict keys with the alias you need to import in each node
result = {
    "np":numpy,
    "pd":pandas,
    "cubepy":cubepy,
    "xr":xarray
}` in every model.


## Execution
## Pyplan approach to Xarray
## Dynamic simulation
## Using Python libraries


<img src="image.jpg" width="50%" height="50%" />
<i class="icon-file"></i>
<i class="fa fa-folder-open"></i>

mmm
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTA4MzExNjg0MywtMzUyNzI3ODI3LC03ND
UyNjExNzksMzc0ODYzMDc5LDc1OTI5Mjc4OCwxNTgxNjkxMDI3
LC0yMDgwMzA0Nzk3LC00MTcwOTYzNywtMTgzNjA1MzUxOSw1MT
E4OTU1ODAsNjMwMjQxODQ0LC0xNDA2ODg1NDIyLC00MDkyNjM2
MjEsLTE0NDYzNzE4OTddfQ==
-->