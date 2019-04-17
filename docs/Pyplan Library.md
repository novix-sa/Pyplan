
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

## Function List
Pyplan Library group a set of functions that helps operate with the concept of Index as defined in Pyplan.
For more transparency, these functions are contained in a module that is automatically imported when creating or opening a model. You can inspect its code, searching the functions by name in the Search Box
You can search for any of the following functions at the digram
![](http://img.pyplan.org/pyplan_library_list_of_functions.png)

## Operating with Indexes
### Set domain
### Subset
Returns a list of all the elements of the index for which dataArray is true. The function is used to create a new index that is a subset of an existing index.
        Ex. subset(sales>0)
### Index from Pandas
### Index from Excel
### Concat Index
### Copy Index
### Change index

## Operating with Time Index
### Create Time
### Add Periods

## Operating with dataArray along Indexes
### Aggregate
### Create dataArray
### Find
### Apply
### Slice
### Subscript
### Lookup
### Get pos
### Linear Depreciation
### IRR
### NPV

## Create Indexed dataArrays
### Build Report
### Pandas from excel
### DataArray from Excel
### Create dataArray
### Copy as values
### to Dataarray

## Other Functions
### Excel connection
### Kind to String
### Split Text
### Goal Seek
### Intall Library

## Special Functions
### Choice
### Dynamic



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTM3MDgwNDMzLC00NjcwNDA5MTAsLTE5NT
c5NDczMzcsLTEyMTkwODI5NDMsLTExMzgyMzcyNzcsMTUwNDA4
MTEyOSwtMTExNzU2NzAxNywtMTg0MzQ5ODE3Nl19
-->