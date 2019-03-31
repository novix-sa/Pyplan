# **Quick Start**

## **Login**

To access Pyplan, it must be installed in a server. Or you can request a trial account to access Pyplan cloud services  [here](http://pyplan.com/contact/).

Once the server address has been identified, you can log into Pyplan with valid user credentials using a regular login form:
![](http://img.pyplan.org/Quick_start_login1.png)

After login in, you will reach the app land page, which looks like the following picture:
![Pyplan Homepage](http://img.pyplan.org/Quick_start_home1.png)
Here you will find sections for creating a new model, opening recent models, recovering any active session, or opening tutorials and examples. Click on  “Create new” to create a new model.

## **Homepage Menu**
After the new model workspace has been created, click on "Open model"
![Open Model](http://img.pyplan.org/Quick_start_open_model.png)

Now you will access the sandbox for creating the logic of your model.
![Coding calculation logic](http://img.pyplan.org/Quick_start_model_code.png)

## **Modeling Business Rules**
The basic objects for creating and organizing the calculation logic are grouped in a toolbar titled "Code". You will find it on the right side of the modeling interface.

![enter image description here](http://img.pyplan.org/Quick_start_code_comp_right.png)


### **Node**
A  **node** is the place where you code, in pure Python, the calculation logic for the data analytics app. The app logic usually starts loading data from an external data source. Different types of analyses can be conducted in separate nodes or groups of nodes, which can either share or not steps in the calculation logic. At the end, some nodes will collect the results that will be shown as outputs of the app.

Let's create a simple analysis to understand how Pyplan works. As a first step, drag and drop a "Node" into the canvas, and enter a Title: "My first node". After accepting the title (or pressing the TAB key), an ID will be automatically provided

![First Node](http://img.pyplan.org/Quick_start_first_node.png)

Then, copy the following code and click on the Code tab:

    a = 4
    b = 5
    print('parameters: ' + str(a) + ',' + str(b))
    result = a+b
  
Paste your Python code on the left side of the “Code” tab. The console output will be displayed on the right side. After clicking the "run" button on the same tab, you should see something like this:

![Coding and running](http://img.pyplan.org/Quick_start_evaluation.png)

While the node is selected , if you press <Ctrl + R> or double click it, the result will be shown, which is 9 in this case. You can appreciate the difference between the console output and the node result. An alternative way to evaluate a node is by pressing <Ctrl + E>. In this case, not only the console and result output will be displayed, but also additional information (as data type) will be shown. It is also possible to inspect the calculation performance by clicking on **Show Profile** which allows you to fine-tune your code.

![Node Inspector](http://img.pyplan.org/Quick_start_inspector.png)

Create another node, draging and dropping a node called "CSV" that you will find in the "Data sources" section on the right menu. 
![enter image description here](http://img.pyplan.org/Quick_start_csv.png)
Then set its definition as:

    result = pd.read_csv('http://web.stanford.edu/class/archive/cs/cs109/cs109.1166/stuff/titanic.csv', sep=None)
You can inspect again the difference between the console output vs the node evaluation (Ctrl + R or double click). While the console output is pure text, Pyplan shows the result in a formatted table.
![Pandas Table](http://img.pyplan.org/Quick_start_first_table.png)

If you inspect the “Code” tab of the node, you will find new buttons next to the “Run” button . These buttons are displayed whenever a node evaluates a Dataframe/Pandas object type. The buttons provide a link to  [Pandas](https://pandas.pydata.org/) wizards to help Python beginners start learning how to use Pandas. Wizards allow you to select and filter data or create new calculation fields. The resulting code will be displayed on the left-hand code section for you to pick up from there.

![Pandas Wizards](http://img.pyplan.org/Quick_start_wizards.png)

### Index
The index object is how you define a dimension in Pyplan. Indexes are created using a Graphical Using Interface (GUI), by means of the drag and drop method, and they are created as Pandas Index.
![Index Definition](http://img.pyplan.org/Pyplan_library_index.png)

    pd.Index(["Item 1","Item 2","Item 3"])


For someone used to Xarray, the Index ID property is equivalent to the "Dim" property in Xarray, and the index values are the equivalent of "Coords." Unlike Xarray, Pyplan Index is defined by a unique set of values, and when used, all the elements are present in that dimension. Following the example above, any data cube indexed by "Items" will contain the elements "Item 1," "Item 2," and "Item 3".

The reasons that justify defining the Index behavior as previously described are: First, it helps to  **standardize the dimensions domain**. This is important to guarantee that when operating with DataArrays that share dimensions, these arrays share the same domain, so that the resulting domain is the same as that of the variables. If that is not the case, and you have a definition like this one:
![enter image description here](http://img.pyplan.org/Quick_start_node_domain.png)
You can see in the console output, that the sum of node1_ and node2_ is only computed for the intersection of Index domain  "MyTime" of the correspondent variables.

Second, we will later see that when creating apps, **controls for interacting with apps**, will be created using indexes.

### **Module**
Modules are meant to contain group of nodes in a way to organize large models.
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
![](http://img.pyplan.org/Quick_start_interface_design.png)

You can start splitting the screen horizontally or vertically for later indicating which node you want in each canvas. You can further divide the canvas any time.

### Output Nodes
There are several type of components that can be included in an interface: Tables, Charts, Diagrams, Text, Filters, Pivot Tables, and Maps. 
![](http://img.pyplan.org/Quick_start_interface_elements.png)

You can define what type of object you want in a specific division and then search for the node that contains the data to be shown
![](http://img.pyplan.org/Quick_start_ins_comp.png)

Or you can directly display the diagram in one division and then keeping pressed the **<Shift>** key and clicking a node, selecting it and dragging and dropping it at the desired division.
![](http://img.pyplan.org/Quick_start_create_interface.png)


### Input Nodes
They are meant to enter data needed for the application calculation logic.
They can be plain tables to enter numbers or tables for choosing among predefined options.


![enter image description here](http://img.pyplan.org/Quick_start_inputs2.png)


### Controls
Are the elements for interacting with the app. Can take the form of filters that automatically applies over all nodes that share the same dimension or selectors for choosing specific slices of data.
![enter image description here](http://img.pyplan.org/Quick_start_I-O.png)
There are other type of controls like buttons for launching specific tasks (scripts) or hyperlinks to create menus and navigate among interfaces.


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQyMTg1NjE4MiwtMTAwNjk1MTcwNywxND
AyODExNjI3LDEyMzg3MzE3MDMsLTY3NTAxMzQ4OCw4MjM3OTgx
MTgsMTA1ODgwNDg5Myw2Nzk4OTg1MjgsLTIwNjIyNTc4NzQsNT
Y3Nzg4ODU0LDIwNTE0OTM5MDgsLTUwOTQ3ODU4MCw4NzAzMDY3
MzMsLTEwMTUzNjYzNjEsLTEwODIyODE2MDYsLTEyOTUyNTA1ND
gsNDA0MDMwMzM2LC0xODQwNDE0MzMwLDEzMTcyNjk5ODUsLTE0
NzQzMDg4NTJdfQ==
-->