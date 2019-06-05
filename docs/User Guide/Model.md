# Model
## Node Properties Tabs
Pyplan structures code trough an influence digram of nodes. When a node is selected (on edit mode) it is open a properties window. Nodes attributes can be inspected and edited trough tabs that are labeled as <kbd>Properties</kbd><kbd>Code</></kbd><kbd>Docs</kbd>.

![enter image description here](http://img.pyplan.org/model-node-prop1.png)
The <kbd>Properties</kbd> tab contains:

 - **Title**: is the legend that will be displayed over the node
 - **ID**: the node identification. The way to call the node values when coding.
 - **Units**: A text value that will be displayed next to the title when evaluating a node.
 - **#**: the number format of the node.
 - **Inputs/Outputs**: list of nodes titles directly linked to the selected node. You can navigate to anyone through clicking on the node name.
 - **Code**: shortcut to the Code tab

The <kbd>Code</></kbd> tab:
![enter image description here](http://img.pyplan.org/model-code-tab1.png)
The code tab presents two windows. The left one is the space to insert the code of the node.
Nodes code **must end with the result definition**. The **"result"** variable contains the output of the node. That is the values to be displayed when the node is evaluated or when called from other node.
Intermediate local variables can be used within the node code. These local variables can be printed in the console for tracing calculation, but at the end must come the result definition.
The right window displays the console output. Any `print()` statement will display outputs here.
When the code is modified, it shows a check and cancel box, and the Play button is turned orange to indicate the node needs to be run. 
 ![](http://img.pyplan.org/model-orange.png)

You can accept changes and run the node by pressing <kbd>Ctrl + Enter</></kbd> or clicking on the icons. 
After running the node the Play button is turned blue to indicate it has already been calculated.
![enter image description here](http://img.pyplan.org/model-blue.png)

The <kbd>Docs</kbd> tab:
This tab a complete HTML text editor to include rich text, links, images and videos that describes and explain the fundamentals of every calculation step. In this way, the app becomes an interactive knowledge repository.
![enter image description here](http://img.pyplan.org/model-docs.png)
## Type of Nodes
The main elements for creating the app calculation logic are the following:

<img src="http://img.pyplan.org/model-nodes-type.png"
	style="float: right; margin-left: 10px;"
	ALIGN=”top”
	height="300" /> 

### Node
Is the main element for creating the calculation logic. It is like a global variable for programming and its definition ends defining the output value of the variable as:

    localvar = 5
    result = 'this is the ouput:' + str(localvar*2)

### Function
This element is used for creating user defined functions.
Functions in python are defined 


### Decision
### Index
### Button
### Module
### Text

## Model Preferences

### Default imports
In order to avoid declaring the 'Import' sentence en each node, there is a node, called Default imports that collects the Library that will not require to declare import all across the model.

    import numpy, pandas, cubepy, xarray
    #fill the following dict keys with the alias you need to import in each node
    result = {
    "np":numpy,
    "pd":pandas,
    "cubepy":cubepy,
    "xr":xarray}

## Pyplan approach to Xarray

## Dynamic simulation
## Using Python libraries

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc0MDk3MTMwNSwtMTIzODkxODYyMCwtND
cwMDE0Njg2LDI2MTAxMTQ1OSwtMTU4NDcxNzI5LC0xODY4ODg1
MDE5LDEyNDQ5NDk4MjcsMzE5OTgzNDg5LC03MjI5NzgzOTksLT
E1NTMyOTY0MzksMjE0MTY0MzE0NSwtMTc3OTEwNzgyOSw3OTIw
ODk2NjgsLTY3MzQ0NTI1OSwxMzI4NDI1Mjg3LDE5Mjc5MjUxOT
AsOTcwOTcyMywtMTI4MDU3ODkwNSwxMjI0MzY5MTQ1LDg5MDcy
NDc1OF19
-->