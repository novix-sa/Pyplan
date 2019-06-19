
# UI Designer
Pyplan has a specific layer for **App deployment** once calculation on influence diagram layer has been concluded.
This layer can be accessed by clicking on the following icon and final user is able to generate Apps and Interfaces that can be easily shared.

![enter image description here](http://img.pyplan.org/UI_interfaces.png)
## Layout
Interfaces manager shows those IO Interfaces created by user and those that were  shared by some other user. In this case user can only browse interfaces unless he copied them to his own space.
Once it has been copied user has total control over that interface.
Favs App can also be set.

![enter image description here](http://img.pyplan.org/Ui_layout.png)

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

2- Use one widget to expose diagram and using <kbd>click+Shift</kbd> drag and drop the objet into a new widget:
![enter image description here](http://img.pyplan.org/UI_sele_obje_op2.png)

If you were the one that created the model this second option will appear useful for you
## I/O 
Interfaces can have inputs as well as outputs widgets.

If you need to create an **inputs widget you should choose a pivot grid.**

For instance, in this example `market growth` information can be modified to simulate different scenarios, you may want to do this on your interface.
![enter image description here](http://img.pyplan.org/UI_pivot_input.png)

By dragging dimension in the correct order and pressing <kbd>ok</kbd> you build you input interface.

There other interesting inputs objects.

More popular are `indexes` or dimensions and `selector`.

Indexes can be explicitly expose in interfaces so that filtered along these dimensions is simple to access by final user.

If you need to set an index widget just drag it from de diagram or search for it using wizard object.
Indexes widget hast their specific options menu.
![enter image description here](http://img.pyplan.org/UI_indexes.png)


**Selector object** can be also drag ad drop from diagram to create input widget

![enter image description here](http://img.pyplan.org/UI_choices.png)
## Synchronization
Once an Interface has been created shared dimensions are automatically synchronized.
That means that every selection in any part of the interface will apply to on every presented object unless explicitly define not to be synchronized.

Let’s suppose you have crated an interface like the following where `region`, `item type` and `time`explicitly exposed (*check how text widget and background colours can help interfaces be more self explaining*)

If you select a single region, a couple of items and a range of time these selections will apply to all interface making analysis very powerful.

![enter image description here](http://img.pyplan.org/UI_synchro.png)
**Remember you can always choose to desynchronized indexes as explained in `visualization` section

## Deploying an App and Sharing

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNDI4NTg5MzMsNTc1MTIyNjU2LDU5ND
MwNjgxMyw3MzY2NjQxOTUsLTcwNzUwNDI3NywxNjM5Nzg4NDU0
LDExMjY1OTg3NTUsOTAzOTU2NDE1LDIzMTY2NDU3OCwtNzk2MD
E2OTksLTY0NjIzMDUyMiwxOTUxODU2MTMzLC0xMTA1MTgzNDky
LC0xOTUwNDI1MjU5LDE0NjI2ODQ1NTYsLTE4NzczMTI4MzEsNT
U1OTIzMjQ2LDE1Njk5OTgzNzEsLTE4NzczMTI4MzEsLTE3Mjg2
ODE0Ml19
-->