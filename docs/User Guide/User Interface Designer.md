
# UI Designer
Pyplan has a specific layer for **app deployment** .

This layer can be accessed by clicking on the icon `Interfaces` located on the left side of the screen. 



![enter image description here](http://img.pyplan.org/UI_interfaces.png)
## Layout
Interfaces manager shows those I/O Interfaces created by the user and those that were  shared by someone else. 
Shared interfaces can only be browsed unless they are copied to user own space.
For doing this **Right click** on the interface and select the option **Copy to My Interfaces**.
Once it has been copied user has total control over that interface.
 


![enter image description here](http://img.pyplan.org/Ui_layout_new.png)

**Favs app** for quick access can also be set once the user owns the interface.

## Creating an Interface
If you want to create and interface from scratch click on `New` and select `interface`. 

Define a name for it and double click on your new interface.
![enter image description here](http://img.pyplan.org/Ui_new_interface.png)

White Interface will open with one single widget.

New widgets can be added by pressing `+` and each of  them has the following characteristics.
![enter image description here](http://img.pyplan.org/Ui_blanck_interface.png)

Each widget can be used for presenting information from the influence diagram choosing among the different layouts explained on section  `Visualization`. 

There are **two ways of selecting objects from diagram to represent them on an interface**.

1- Selecting type of data from the wizards menu and searching object by title or id on the window that pops up:
![enter image description here](http://img.pyplan.org/UI_sele_obje_op1.png)

2- Use one widget to expose influence diagram and ,pressing <kbd>click+Shift</kbd>, drag and drop the object you want to be repsentred from the diagram into a new widget:

![enter image description here](http://img.pyplan.org/UI_sele_obje_op2.png)

**Hint:** If you were the one that created the model this second option will appear useful for you.
## I/O Interfaces
Interfaces can have inputs as well as outputs widgets.

If you need to create an **input widget you should choose a pivot grid.**

For instance, in this example `market growth` information can be modified to simulate different scenarios, you may want to do this on your interface.
![enter image description here](http://img.pyplan.org/UI_pivot_input.png)

By dragging dimension in the correct order and pressing <kbd>ok</kbd> you build your input interface.

There are other interesting inputs objects.

Most common are `indexes` (dimensions) and `selector`.

Indexes can be explicitly exposed on interfaces. This helps filtering  along these dimensions for final user.

If you need to set an index widget just drag it from de diagram or search for it using wizard object.
**Indexes widget has their specific options menu.**
![enter image description here](http://img.pyplan.org/UI_indexes.png)


**Selector object** can also being dragged and dropped from diagram to create input widget.

![enter image description here](http://img.pyplan.org/UI_choices.png)
## Synchronization
Once an Interface has been created shared dimensions are automatically synchronized.
That means that **every selection in any part of the interface will apply to every presented object** unless explicitly defined the opposite.

Let’s suppose you have created an interface like the following where `region`, `item type` and `time`are explicitly exposed.
 
*Hint: check how text widget and background colours can help interfaces be more self explaining*.

If you select a **single region, a couple of items and a range of time** these selections will apply to all interface.

![enter image description here](http://img.pyplan.org/UI_synchro.png)
**Remember you can always choose to des-synchronized indexes as explained in `visualization` section

## Deploying an App and Sharing
Once you have created various interfaces you may need to generate an application for sharing it with other users or even publicly.

**Creating an application.**

Creating an application is as simple as selecting `Application` from menu and defining a name for it.

![enter image description here](http://img.pyplan.org/UI_create_app.png)

By **dragging and dropping** previously created interfaces in the application deployment is done.
![enter image description here](http://img.pyplan.org/UI_drag_dro_inter.png)

**Sharing an application**

Select the application and press right bottom to access the following menu:
![enter image description here](http://img.pyplan.org/UI_share_app.png)

**Share the application externally and make it accessible for every person with the link.**

Congratulations your [python](https://www.python.org/) coded application has been deployed.


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgzNzgxNTI0NywtNTQ5NTI2MTI0LC0yNz
c2MzY5NTgsLTE5NzI4NjkwNjAsLTE1NzcxNzY2NzksLTE5MzIw
NTYxODIsMTUyODUxMzA5OCwtMTg2MDI2MjYwNSwxMjY2MTE2OD
k5LC0xNjYyMzQ3MTgxLC0xMzQyODU4OTMzLDU3NTEyMjY1Niw1
OTQzMDY4MTMsNzM2NjY0MTk1LC03MDc1MDQyNzcsMTYzOTc4OD
Q1NCwxMTI2NTk4NzU1LDkwMzk1NjQxNSwyMzE2NjQ1NzgsLTc5
NjAxNjk5XX0=
-->