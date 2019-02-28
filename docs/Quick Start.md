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
The Index element creates a Pandas index. An index is used for defining dimensions of DayaArrays and Dataframes. 
They are important to be explicitly defined as this for two reasons:
First, it help homogenize Dimension domains. 

Its importance comes from

### **Module**
Modules are ment to contain group of nodes in a way to organize large models.
For example if your model is an integrated planning tool of a manufacturing company, the influence diagram could look like this:
![enter image description here](http://img.pyplan.org/Quick_start_IBP_diagram.png)

Where each module contains the underlying logic of each area of a company. In this example, the Supply & Operation Planning Module looks like this:

![S&OP](http://img.pyplan.org/Quick_start_sop.png)


## **Evaluating and Visualizing Data**
In order to explore the evaluation and visualization alternatives, let's copy to your own workspace the app called "My First App.ppl" that you will find in the Public folder. After selecting it, click on the "Copy in" section as shown in the figure below:
![My First App file](http://img.pyplan.org/Quick_start_file_app_1.png)

![enter image description here](http://img.pyplan.org/Quick_start_own_ws.png)

Now open the copied file and then go to the model (Click Open Model, or the Model icon at the left). You should see the following diagram:
![enter image description here](http://img.pyplan.org/Quick_start_mfa_model_.png)
Now you can inspect any node values by selecting and evaluating it.
There are three alternatives for evaluating a node:
The first one is by clicking on the **"Run"** button that you will finde in the Code Tab  after selecting a node. The same result can be obtained by pressing **<Ctrl + Return>** when editing the code. This will show/update the console output resulting of evaluating the node.
![enter image description here](http://img.pyplan.org/Quick_start_eval1.png)
Try adding `Print('Hello World')`in the first line before the result definition. Run the node and check the console output.
You will find this functionality useful for inspecting intermediate values in your calculations.

The second alternative is, after selecting the node, pressing **<Ctrl + E>**. In this case a more complete window is open showing 
![enter image description here](http://img.pyplan.org/Quick_start_ctrl+E.png)
Performance profiling information can be displayed clicking on **"Show Profile"**

![enter image description here](http://img.pyplan.org/Quick_start_ctrl+E+ShowProfile.png)
In order to understand how the Pyplan evaluation works

### How does it evaluation works
dependency solved, memory persistency
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
eyJoaXN0b3J5IjpbMTY5NzUyMDkxMCwtMjAxMjE1NjAsLTk5OD
c0NDA0OCwtMTE1NDA2ODk2LDE1OTc1NjM5NDAsMTA4NzEwODM3
NywtMTUwMzUwNjkyOSwtNjAwNjI4MzYwLDIxODM2MDU0OCwxNz
gxNDExNTM4LDM1Nzc3MzIyNiwtMjcyMzk1MDgxLC0xNzk3NDUx
NDM4LC0zMDkzMjU2ODMsMzE4MDAwOTkyLC0xMzMzMjEzNTc1LC
0xMTQwNjM2ODA3LDc5NTA5NzEsLTUwMzM5NTYzMCwtMjAxMTcw
MTM0Nl19
-->