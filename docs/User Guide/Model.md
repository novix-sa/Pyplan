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
The main elements for creating the app calculation logic are the following
![enter image description here](http://img.pyplan.org/model-nodes-type.png)
<i class="icon-compass"></i>
<img src="http://img.pyplan.org/model-nodes-type.png"
	alt="Markdown Monster icon"
	style="float: left; margin-right: 10px;"
	size="100px" />

### Node
### Function
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
eyJoaXN0b3J5IjpbLTcyMjk3ODM5OSwtMTU1MzI5NjQzOSwyMT
QxNjQzMTQ1LC0xNzc5MTA3ODI5LDc5MjA4OTY2OCwtNjczNDQ1
MjU5LDEzMjg0MjUyODcsMTkyNzkyNTE5MCw5NzA5NzIzLC0xMj
gwNTc4OTA1LDEyMjQzNjkxNDUsODkwNzI0NzU4LDE4MTQ5MTcw
LDE5MTM4MjMxMiwtNjgyODA2NDAxLDQ0NTkzNDcyNyw2MTI0OT
A1MSwtMzUyNzI3ODI3LC03NDUyNjExNzksMzc0ODYzMDc5XX0=

-->