# Model

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
Nodes code **must end with the result definition**. The **"result"** variable contains the result of the node. That is the output to be displayed when the node is evaluated or when called from other node.
Intermediate local variables can be used and results printed in the console for tracing calculation, but at the end must come the result definition.
The right window displays the console output. Any `print()` statement will display outputs here.
When the code is modified, it shows a check and cancel box, and the Play button is turned orange to indicate the node needs to be run. 
 ![](http://img.pyplan.org/model-orange.png)

You can accept changes and run the node by pressing <kbd>Ctrl + Enter</></kbd> or clicking on the icons. 
After running the node the Play button is turned blue.
![enter image description here](http://img.pyplan.org/model-blue.png)


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
eyJoaXN0b3J5IjpbODkwNzI0NzU4LDE4MTQ5MTcwLDE5MTM4Mj
MxMiwtNjgyODA2NDAxLDQ0NTkzNDcyNyw2MTI0OTA1MSwtMzUy
NzI3ODI3LC03NDUyNjExNzksMzc0ODYzMDc5LDc1OTI5Mjc4OC
wxNTgxNjkxMDI3LC0yMDgwMzA0Nzk3LC00MTcwOTYzNywtMTgz
NjA1MzUxOSw1MTE4OTU1ODAsNjMwMjQxODQ0LC0xNDA2ODg1ND
IyLC00MDkyNjM2MjEsLTE0NDYzNzE4OTddfQ==
-->