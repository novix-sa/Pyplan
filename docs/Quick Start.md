# **Quick Start**

## **Login**

You must have installed Pyplan in a server to access Pyplan.
Or you can request a trial account to access Pyplan cloud services [here](http://pyplan.com/contact/).

Once identified the server address and with valid user you can login Pyplan through a regular Login form:
![](http://img.pyplan.org/Quick_start_login1.png)

After login in, you will reach the app landpage that looks like the following picture:
![Pyplan Homepage](http://img.pyplan.org/Quick_start_home.png)
Here you will find sections for creating a new model, open recent models, recover any active session, or opening tutorials and examples. 
Click on create a new model.
## **Homepage Menu**
After the new model workspace is created, click on "Open Model" 
![Open Model](http://img.pyplan.org/Quick_start_open_model.png)

Now you will access the sandbox for creating your model logic.
![Coding calculation logic](http://img.pyplan.org/Quick_start_model_code.png)

## **Modeling Business Rules**
There are five basic components for creating and organizing the calculation logic diplayed at the right side of the modeling app.

![Code building blocks](http://img.pyplan.org/Quick_start_code_components2.png)

### **Node**
A **Node** is the place where you code, in pure Python, the data analytic app calculation logic. 
It usually start loading data from and external datasource to start analyzing.
Different type of analysis can be conducted in separate nodes or group of nodes, sharing or not steps in the calculation logic. At the end some nodes will collect results to be shown as outputs of the app.
Let's create a simple analysis to understand how Pyplan works.
For now just drag and drop a "Node" into the canvas, provide a Title and lets inspect its attribute tabs.
![First Node](http://img.pyplan.org/Quick_start_first_node.png)

And then click on the Code tab.
![Coding and running](http://img.pyplan.org/Quick_start_evaluation.png)
On the left space you will write your Python code. On the right side will be displayed the console output.
If you double click the node or press <Ctrl + R>, it will show its result, which in this case is a 9.
Another alternative way to evaluate a node is by pressing <Ctrl + E>, in this case, not only the console and result output will be displayed, but additional information (as data type) will be shown. It is possible also to inspect calculation performance clicking on **Show Profile** for tunning your code.

![Node Inspector](http://img.pyplan.org/Quick_start_inspector.png)

Create another node (drag and drop a node block) called "Read External Datasource" and set its definition as:

    result = pd.read_csv('http://web.stanford.edu/class/archive/cs/cs109/cs109.1166/stuff/titanic.csv', sep=None)
You can inspect the difference on the console output vs evaluating (Ctrl R or double click) the node.

![Pandas Table](http://img.pyplan.org/Quick_start_first_table.png)

Inspecting the node code tab you will find that some new buttons next to the Run button. These are [Pandas](https://pandas.pydata.org) wizards for helping Python newbies start learning Pandas.
Through the wizards you will be able to make selections and filtering or create new calculated fields. The resulting code will be displayed on the code section at the left.
![Pandas Wizards](http://img.pyplan.org/Quick_start_wizards.png)

### Module
Modules are ment to contain group of nodes. For example if your model is an integrated planning tool of a manufacturing company, the influence diagram could look like this:
![S&OP](http://img.pyplan.org/Quick_start_sop.png)

Where each module contains the underlying logic of each area of a company. In this example, the Supply & Operation Planning Module looks like this:




### Text

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
eyJoaXN0b3J5IjpbMTgzNDIzNDE1LC0yMDExNzAxMzQ2LDE0OT
Y1NzIxOTAsMTgxNjQ1MDg2NCwtMTQzNDEzNzU1OCwtMTczODcy
OTQ4MywxNDYzMzYxNjk5LC0zMzgxODExMDIsLTE3Mzk1MjU5Mj
gsLTE4NzQwMDUxOTMsLTg2ODE2NDQ2OSwxMDQ1MzU4Nzg4LC0x
NTIyNzg1ODMxLC02NzAyNjM3NjQsMTk3MTU2NjY5NSwtMTg0Nz
kzNDIzMCwtMjA0Njg4NjEzNCwtMTgwODM0NDAwOSwxMTc0Njcy
Mzg5LC0xNDU0MDA0OTM3XX0=
-->