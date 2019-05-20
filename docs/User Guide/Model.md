# Model
## Node Properties Tabs
Pyplan structures code trough an influence digram of nodes. Nodes have properties that could be inspected and edited, after selection, trough tabs <kbd>Properties</kbd><kbd>Code</></kbd><kbd>Docs</kbd>.

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

The <kbd>Docs</></kbd> tab:
This tab a complete HTML text editor to include rich text, links, images and videos that describes and explain the fundamentals of every calculation step. In this way, the app becomes an interactive knowledge repository.
![enter image description here](http://img.pyplan.org/model-docs.png)


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
eyJoaXN0b3J5IjpbLTEyODA1Nzg5MDUsMTIyNDM2OTE0NSw4OT
A3MjQ3NTgsMTgxNDkxNzAsMTkxMzgyMzEyLC02ODI4MDY0MDEs
NDQ1OTM0NzI3LDYxMjQ5MDUxLC0zNTI3Mjc4MjcsLTc0NTI2MT
E3OSwzNzQ4NjMwNzksNzU5MjkyNzg4LDE1ODE2OTEwMjcsLTIw
ODAzMDQ3OTcsLTQxNzA5NjM3LC0xODM2MDUzNTE5LDUxMTg5NT
U4MCw2MzAyNDE4NDQsLTE0MDY4ODU0MjIsLTQwOTI2MzYyMV19

-->