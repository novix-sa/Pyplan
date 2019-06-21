
# UI Designer
Pyplan has a specific layer for **app deployment** once calculation on influence diagram layer has been concluded.
This layer can be accessed by clicking on the following icon. 

**User is able to generate apps and interfaces that can be easily shared.**

![enter image description here](http://img.pyplan.org/UI_interfaces.png)
## Layout
Interfaces manager shows those IO Interfaces created by the user and those that were  shared by some other. Shared interfaces can only be browsed unless they are copied to user own space.
Once it has been copied user has total control over that interface.
**Favs app** can also be set.
![enter image description here](http://img.pyplan.org/Ui_layout_new.png)

## Creating an Interface
Click on `New` and select interface. 
Define a name for it and double click on your new interface.
![enter image description here](http://img.pyplan.org/Ui_new_interface.png)

White Interface will open with one single widget.

New widgets can be added by pressing `+` and each of  them has the following characteristics.
![enter image description here](http://img.pyplan.org/Ui_blanck_interface.png)

Each widget can be used for presenting information from the diagram choosing among the different layouts explained on section  `Visualization` 

There are **two ways of selecting objects from diagram to represent them on an interface**.

1- Selecting type of data and searching object title or id:
![enter image description here](http://img.pyplan.org/UI_sele_obje_op1.png)

2- Use one widget to expose diagram and pressing <kbd>click+Shift</kbd> drag and drop the objet into a new widget:

![enter image description here](http://img.pyplan.org/UI_sele_obje_op2.png)

If you were the one that created the model this second option will appear useful for you.
## I/O 
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

Let’s suppose you have created an interface like the following where `region`, `item type` and `time`are explicitly exposed 
*Hint: check how text widget and background colours can help interfaces be more self explaining*

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
eyJoaXN0b3J5IjpbMTAwNjc0NDYwOCwtMTU3NzE3NjY3OSwtMT
kzMjA1NjE4MiwxNTI4NTEzMDk4LC0xODYwMjYyNjA1LDEyNjYx
MTY4OTksLTE2NjIzNDcxODEsLTEzNDI4NTg5MzMsNTc1MTIyNj
U2LDU5NDMwNjgxMyw3MzY2NjQxOTUsLTcwNzUwNDI3NywxNjM5
Nzg4NDU0LDExMjY1OTg3NTUsOTAzOTU2NDE1LDIzMTY2NDU3OC
wtNzk2MDE2OTksLTY0NjIzMDUyMiwxOTUxODU2MTMzLC0xMTA1
MTgzNDkyXX0=
-->