# **Quick Start**

## **Login**

You must have installed Pyplan in a server to access Pyplan.
Or you can request a trial account to access Pyplan cloud services [here](http://pyplan.com/contact/).

Once identified the server address and with valid user you can login Pyplan through a regular Login form:
![](http://img.pyplan.org/Quick_start_login1.png)

After login in, you will reach the app landpage that looks like the following picture:
![Pyplan Homepage](http://img.pyplan.org/Quick_start_home.png)
Here you will find sections for creating a new model, open recent models, recover any active session, or opening tutorials and examples. Click on create a new model, and then click on "Open Model"
## **Homepage Menu**
At the homepage 
![Open Model](http://img.pyplan.org/Quick_start_open_model.png)
Clicking on Open Model, you will access the sandbox for creating your model logic.
![Coding calculation logic](http://img.pyplan.org/Quick_start_model_code.png)

### Coding
There are five basic components for creating and organizing the calculation logic: Node, Module, Text, Button and Function.
A Node is the place where you code the app calculation logic. It can start with a node that read an external data source, followed by another node that makes some calculations and end with a node that produces a desired output.
![Code Components](http://img.pyplan.org/Quick_start_code_components1.png)
For now just drag and drop a "Node" into the canvas, provide a Title and lets inspect its attribute tabs.
![First Node](http://img.pyplan.org/Quick_start_first_node.png)

And then click on the Code tab.
![Coding and running](http://img.pyplan.org/Quick_start_evaluation.png)
On the left space you will write your Python code. On the right side will be displayed the console output.
If you double click the node or pressing <Ctrl + R>, it will show its result, which in this case is a 9.
Another alternative evaluation is the one launched pressing <Ctrl + E>, in this case, not only the console and result output will be displayed, but additional information (as data type) will be shown.

![Node Inspector](http://img.pyplan.org/Quick_start_inspector.png)

### User Interfaces

### File Manager

## **Modeling Business Rules**
### Reading External Datasources
### Nodes and Calculation

## **Evaluating Nodes**
### How does it evaluation works
### Types of data structures natively supported

## **Creating an App User Interface**
### Output Nodes
### Controls
### Input Nodes


Pyplan main object is called “node” and it´s codification, after importing any Python Library, can be easily done through its **_code_** windows.
Numpy Array could be codified as:

    >result = np.array([1,2,3])

Check that final line of Pyplan node should have the expression **_result=_** in order to indicate node which is going to be the final object of the code.
Numpy Array could be codified as:

![enter image description here](http://img.pyplan.org/Home_code_view.png)

By pressing **_Ctrl+R_** Pyplan will evaluate this object and show results in a table.

![enter image description here](http://img.pyplan.org/Home_result_view)

Graphical representation can be simple access through table menu:

![enter image description here](http://img.pyplan.org/Home_show_graph)

And result will be shown as a graph

![enter image description here](http://img.pyplan.org/Home_graph_view)
As simple as indicated Python based model can be structure.

Pyplan also provides user friendly interfaces for model management and API deployment. Check more about these topics on following chapters.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTI3MTM1MDY5NywtODY4MTY0NDY5LDEwND
UzNTg3ODgsLTE1MjI3ODU4MzEsLTY3MDI2Mzc2NCwxOTcxNTY2
Njk1LC0xODQ3OTM0MjMwLC0yMDQ2ODg2MTM0LC0xODA4MzQ0MD
A5LDExNzQ2NzIzODksLTE0NTQwMDQ5MzcsMTk4ODk1NDQwMSw0
NTEyNzI3MjQsLTgxMjcwNTA1MSwtMjUzNDc0NDg4LC0xMDY2MT
k3OTMxLC0xMTExMjg0NzUyLDgzNzExODM4NCw5NDkzODkxODld
fQ==
-->