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

## Execution

### Console Output
You can run any node, after editing its code, pressing <kbd>CTRL + Enter</kbd>.
It will show at the right side of the code window the console output resulting from running the node.
Any `Print()` statement written between code lines will display it result here.
It is intended for rapid evaluation of the node, to check it is properly defined.

### Result Explorer
Other way to run a node is by pressing <kbd>CTRL + E</kbd>.
This way of running displays not only


### Evaluating a Node
<kbd>CTRL + R</kbd> to get its result


## Pyplan approach to Xarray
## Dynamic simulation
## Using Python libraries


<img src="model-orange.png" width="50%" height="50%" />
<i class="icon-file"></i>
<i class="fa fa-folder-open"></i>
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzkyMDg5NjY4LC02NzM0NDUyNTksMTMyOD
QyNTI4NywxOTI3OTI1MTkwLDk3MDk3MjMsLTEyODA1Nzg5MDUs
MTIyNDM2OTE0NSw4OTA3MjQ3NTgsMTgxNDkxNzAsMTkxMzgyMz
EyLC02ODI4MDY0MDEsNDQ1OTM0NzI3LDYxMjQ5MDUxLC0zNTI3
Mjc4MjcsLTc0NTI2MTE3OSwzNzQ4NjMwNzksNzU5MjkyNzg4LD
E1ODE2OTEwMjcsLTIwODAzMDQ3OTcsLTQxNzA5NjM3XX0=
-->