# Model

Pyplan structure code trough and influence digram of nodes. Nodes has pro

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
eyJoaXN0b3J5IjpbLTIwODAzMDQ3OTcsLTQxNzA5NjM3LC0xOD
M2MDUzNTE5LDUxMTg5NTU4MCw2MzAyNDE4NDQsLTE0MDY4ODU0
MjIsLTQwOTI2MzYyMSwtMTQ0NjM3MTg5N119
-->