# Visualization
When a node is run (double clicking it) its result can be rendered as a table, a pivot table, different type of graphs, or a map.
The visualization type is selected clicking on the configuration wheel that appears when you enter in the visualization edit mode. After clicking the configuration wheel the following menu is displayed to navigate and set the options.
![enter image description here](http://img.pyplan.org/viz-edit2.png)

The first choice to be made is about the type of chart (Table, Graph or Map). The menu is accessed clicking on the first option called "Chart and filters".
![enter image description here](http://img.pyplan.org/viz-viz-type1.png)


# Tables
There are two types of tables intended for different purposes. 
Regular tables and pivot tables.
The image below show some different configuration features from these tables:


## Regular Table
Is the default view of any node. The user can pivot dimensions and filter any dimension by clicking the `(all)` legend next to each dimension.
It is possible to generate custom configurations by rows or cols. Heatmaps and Background colors based on customized ranges are also possible.
 ![enter image description here](http://img.pyplan.org/viz-table-standard.png)
 
Number format menu and advanced options may help you generating the view you need for each variable.

![enter image description here](http://img.pyplan.org/Vizua_tables_format.png)

### Conditional Format
Regular table has the option of defining conditional format rules to coloured, highlight with different font or even add a shape on displayed information.

Pyplan also has and advance option for linking different interfaces trough these formats.

These configurations enhance visualization analysis options.
![enter image description here](http://img.pyplan.org/Vizua_cond_format.png)
## Pivot Tables
Different than the standard table It allows multiple dimensions in rows or cols as well as filtering.
It has fewer customization options compared to regular tables.
![enter image description here](http://img.pyplan.org/viz-tables-dif1.png)
But one main differentiation is that can work as an input table, allowing the user to manually change table values.
![enter image description here](http://img.pyplan.org/viz-edit-table.png)
# Graphs
Pyplan includes several type of standard chart graphs.
Take advantage of graph generation shortcut to create a graph in one click.

![enter image description here](http://img.pyplan.org/Visua_table_n_graph.png)

Graphs customization options are availbale on rigth menu. 
Types of graphs, labels, legends, axis configurations and other can be defined on this menu.
 ![enter image description here](http://img.pyplan.org/Visua_graph_cust.png)
# Advanced Options and Index Sync

Regular tables as well as graphs shared a couple of advanced options that can be very helpful. Click on  `Hide empty data`,  `View index detail` and  `Enable drilldown` to see how these options impact on tables and graphs.

`Index Sync` is a powerful toll when working with tables and graphs of the same interface.
Pyplan **synchronizes** **shared dimensions** among objects presented in an interface.
For instance, on the following example ***total cost Information*** is presented as a table and as a graph and as all of it dimensions are synchronised.

![enter image description here](http://img.pyplan.org/Visua_index_sync.png)

This means that **any dimension filtered on table will apply of graph and vice versa.**

On the other hand, it may be useful to **des-synchronised** dimensions between objects.
For instance, you may need to filter some item type on table while all item type is shown on graph.
De synchronizing index `Item type` on the menu shown above will allow you to do this kind of selective filtering.

![enter image description here](http://img.pyplan.org/Visua_index_des_sync.png)

This characteristic will also be very **useful when designing a user interface** colleting  information from different parts of your app which shares dimensions.

# Maps
(todo)
# Other visualization libraries
(todo)




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMyNDU4NjQwNCwtMTQyODUwMzcwNCwtMj
c3Nzc3ODE5LDEwNTEzMjI4NjMsLTE4ODQyMzA4NzMsODExNTI2
Njc0LDExNTQzMjM5ODYsMzA3NzExOTI1LDQ1MzkxOTMwNiwxMz
kyMzY4NTM4LC02NDU3NjExMjMsMTAxMTY5NjM3MiwtNzE2MTEw
NzM4LC0xMTIyODkwNjk1LC03NDQ5MjA4MjEsLTExMjI4OTA2OT
UsLTc0NDkyMDgyMSwtNzc5MDE4NjM5LC0yMTE4OTc2MTEyLDE5
NDg5NzU5ODFdfQ==
-->