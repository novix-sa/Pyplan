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
There are five basic components for creating and organizing the calculation logic. They are grouped in a toolbar titled "Code" you can find in the right side of the modeling app.

![Code building blocks](http://img.pyplan.org/Quick_start_code_components.png)



### **Node**
A **Node** is the place where you code, in pure Python, the data analytic app calculation logic. 
The app logic, usually starts loading data from an external datasource. Different type of analysis can be conducted in separate nodes or group of nodes, sharing or not steps in the calculation logic.
At the end some nodes will collect results to be shown as outputs of the app.

Let's create a simple analysis to understand how Pyplan works.
As a first step, drag and drop a "Node" into the canvas, provide a Title:"My first node". After accepting the title (or pressing the TAB key) an ID will be automatically provided.
![First Node](http://img.pyplan.org/Quick_start_first_node.png)

Then copy the following code and click on the Code tab:

    a = 4
    b = 5
    print('parameters: ' + str(a) + ',' + str(b))
    result = a+b
  
On the left space of the Code Tab, you will paste your Python code. On the right side will be displayed the console output.
After clicking the "run" button on the same tab, you should see something like this:
![Coding and running](http://img.pyplan.org/Quick_start_evaluation.png)

If you double click the node or press <Ctrl + R>, it will show its result, which in this case is a 9. You can appreciate the difference between the console output and the node result.
Another alternative way to evaluate a node is by pressing <Ctrl + E>, in this case, not only the console and result output will be displayed, but additional information (as data type) will be shown. It is possible also to inspect calculation performance clicking on **Show Profile** for tunning your code.

![Node Inspector](http://img.pyplan.org/Quick_start_inspector.png)

Create another node (drag and drop a node block) called "Read External Datasource" and set its definition as:

    result = pd.read_csv('http://web.stanford.edu/class/archive/cs/cs109/cs109.1166/stuff/titanic.csv', sep=None)
You can again inspect the difference on the console output vs evaluating (Ctrl R or double click) the node. While console output is pure text, Pyplan result is a formatted table.

![Pandas Table](http://img.pyplan.org/Quick_start_first_table.png)

Inspecting the node Code Tab you will find new buttons next to the Run button. These buttons are displayed whenever a node evaluates to a Dataframe/Pandas object type. The buttons links to [Pandas](https://pandas.pydata.org) wizards for helping Python newbies start learning Pandas.
Through the wizards you will be able to select and filter data or create new calculated fields. The resulting code will be displayed on the code section at the left for you to pick up from there.
![Pandas Wizards](http://img.pyplan.org/Quick_start_wizards.png)

### **Index**
An index is used for defining dimensions of DayaArrays and Dataframes. Draging an Index element creates a Pandas index of the form:

    result = pd.Index(["Itemm 1","Item 2","Item 3"])

Indexes are important to be explicitly defined for two reasons:

First, it helps **homogenize Dimensions domain**. That is important to guarantee that when you operate with DataArrays that share dimensions, they share the same domain, so that the result domain is the same of the variables.
If that is not the case and you have a definition like this
![enter image description here](http://img.pyplan.org/Quick_start_node_domain.png)
You can see in the console output, that the sum of node1_ and node2_ is only computed for the intersection of Index domain  "MyTime" of the correspondent variables.

Second, we will later see that when creating apps, **controls for interacting with the app**, are created using indexes.

### **Module**
Modules are ment to contain group of nodes in a way to organize large models.
For example if your model is an integrated planning tool of a manufacturing company, the influence diagram could look like this:
![enter image description here](http://img.pyplan.org/Quick_start_IBP_diagram.png)

Where each module contains the underlying logic of each area of a company. In this example, the Supply & Operation Planning Module looks like this:

![S&OP](http://img.pyplan.org/Quick_start_sop.png)


## **Evaluating and Visualizing Data**
In order to explore the evaluation and visualization alternatives, let's copy to your own workspace the app called "My First App.ppl" that you will find in the Public folder. After selecting it, click on the "Copy in" section as shown in the figure below:
![My First App file](http://img.pyplan.org/Quick_start_file_app_1.png)

![enter image description here](http://img.pyplan.org/Quick_start_own_ws_ad.png)

Now open the copied file and then go to the model (Click Open Model, or the Model icon at the left). You should see the following diagram:
![enter image description here](http://img.pyplan.org/Quick_start_mfa_model_.png)
Now you can inspect any node values by selecting and evaluating it.
There are three alternatives for evaluating a node:
The first one is by clicking on the **"Run"** button that you will finde in the Code Tab  after selecting a node. The same result can be obtained by pressing **<Ctrl + Return>** when editing the code. This will show/update the console output resulting of evaluating the node.
![enter image description here](http://img.pyplan.org/Quick_start_eval1.png)
Try adding `Print('Hello World')`in the first line before the result definition. Run the node and check the console output.
You will find this Printing functionality useful for inspecting intermediate values in your calculations.

The second alternative is, after selecting the node, pressing **<Ctrl + E>**. In this case a more complete window is open showing 
![enter image description here](http://img.pyplan.org/Quick_start_ctrl+E.png)
Performance profiling information can be displayed clicking on **"Show Profile"**

![enter image description here](http://img.pyplan.org/Quick_start_ctrl+E+ShowProfile.png)

The third way of running a node is by **double clicking** it or pressing **<Ctrl + R>**. Any node is initially evaluated as a table, until the user customize it visualization.
There is a group of customization that can be rapidly set clicking on the configuration icon next to the title of the node:
![enter image description here](http://img.pyplan.org/Quick_start_configuration_wheel.png)

![enter image description here](http://img.pyplan.org/Quick_start_evaluate.png)
One interesting feature is the ability to show the node result as table and graph simutaneously.
All customization are lost when closing the node, unless you explicitly indicates that you want to set the current view as the default view for opening this specific node. To do that you must click on the icon with a pencil ![enter image description here](http://img.pyplan.org/Quick_start_pencil20.png) , at the top left corner. This will open the visualization editor with all the customization features. Click on the check mark to accept changes and setting the default view of the node.


### Types of data structures natively supported
Pyplan supports programming in pure Python, and natively interprets Numpy, Xarray and Pandas objects that are rendered as pivotable multidimensional tables or graphs for result inspection. It allows to import and use any other specific library you may need to attend your specific goals.
Pyplan can also render a node that evaluates generating an HTML file. This functionality is particularly useful for using visualization libraries, which result need to be rendered by the app.

### Understanding how does it evaluation works
When you ask for a node to be run, Pyplan trace all predecesor variables and run them in sequence in order to have computed every input that this node needs. The results of intermediate nodes are preserved in memory for future inspection. When the definition of a node change, all downstream nodes are marked to be recalculated so that the user does not need to be aware about the updated value of any predecesor when running a node.

## **Creating an App User Interface**
One of the most important characteristic of Pyplan is its ability for rapidly creating and sharing apps.
Apps are constructed using one or more user interfaces. To start creating an app, you need first to enter into the interface designer:
![](http://img.pyplan.org/Quick_start_interface_.png)

Click on the New green button, and then select Interface
![](http://img.pyplan.org/Quick_start_new_interface.png)

Provide the name **"First I/O dashboard"** to the new interface
![](http://img.pyplan.org/Quick_start_new_interface2.png)

Now double click the new interface to start designing it:
![](http://img.pyplan.org/Quick_start_new_interface_design.png)



### Output Nodes
### Controls
### Input Nodes


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTUzNjI3MTgwOCwtODQ5OTMzNTY2LDc0NT
kxMzMxMiwxODM4Mzc2MTM0LC02ODkzMTExNzUsMTIzNTU0MjEw
MywxNTAxMDk4OTMwLDYyMjI4NzcyMSwtMTUyNjYyMTMwMiwtNT
Y2ODU1MDksMTU3MTc3OTUyNywtMjAxMjg2NTg3MywtMTk2ODkw
MjI3NywtMTM2MTAyMDc0MiwxNjgzNjI3MTEwLC0xNDE3MjQ5OT
U1LC0yNjExNjk4NTMsLTUyNjk3NDcwNCw4NjQ0NTcwNTMsMTI1
ODg5NDM4M119
-->