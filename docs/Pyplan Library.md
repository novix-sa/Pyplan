
# Pyplan Library
Pyplan natively interprets Pandas, Numpy and Xarray objects. That means that any of this type of objects can be evaluated and rendered as a table or graph with all customization natively offered by Pyplan.
Additionally, Pyplan encourage a the usage of Index for defining dimensions for Xarray datacubes. Let's understand how does it work.

## **Index**
The index object is how you define a dimension in Pyplan. Indexes are created using a Graphical Using Interface (GUI), by means of the drag and drop method, and they are created as Pandas Index.
![Index Definition](http://img.pyplan.org/Pyplan_library_index.png)

    pd.Index(["Item 1","Item 2","Item 3"])


For someone used to Xarray, the Index ID property is equivalent to the "Dim" property in Xarray, and the index values are the equivalent of "Coords." Unlike Xarray, Pyplan Index is defined by a unique set of values, and when used, all the elements are present in that dimension. Following the example above, any data cube indexed by "Items" will contain the elements "Item 1," "Item 2," and "Item 3".

The reasons that justify defining the Index behavior as previously described are: First, it helps to  **standardize the dimensions domain**. This is important to guarantee that when operating with DataArrays that share dimensions, these arrays share the same domain, so that the resulting domain is the same as that of the variables. If that is not the case, and you have a definition like this one:
![enter image description here](http://img.pyplan.org/Quick_start_node_domain.png)
You can see in the console output, that the sum of “node1_” and “node2_” is only computed for the intersection of Index domain "MyTime" of the corresponding variables.

Second, as we will later see, when creating apps,  **controls for interacting with those apps** will be created using indexes.



## Explicar la forma de trabajo de Pyplan con indices
## Dynamic
## Listado de funciones


Pyplan Library group a set of functions that helps operate with the concept of Index as defined in Pyplan.



![](http://img.pyplan.org/pyplan_library_list_of_functions.png)

## Operating with Indexes
### Set domain
### Subset
Returns a list of all the elements of the index for which dataArray is true. The function is used to create a new index that is a subset of an existing index.
        Ex. subset(sales>0)
 
### Change index
### Index from Pandas
### Index from Excel
### Concat Index

## Operating with dataArray along Indexes
### Aggregate
### Create dataArray
### Find
### Apply
### Subscript
### Lookup
### Get pos

## Create Indexed dataArrays
### Build Report
### Pandas from excel
### DataArray from Excel
### Split Text

## Other Functions
### Excel connection
### Kind to String

## Special Functions
### Choice
### Dynamic



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExMTc1NjcwMTcsLTE4NDM0OTgxNzZdfQ
==
-->