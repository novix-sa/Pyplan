
# **Pyplan Library**

Pyplan is a [Python](https://www.python.org/) library intended for supporting multidimensional dynamic simulation running on the Pyplan IDE web application. It is based on [Xarray](http://xarray.pydata.org/) DataArray object and take advantage of its N-dimensional labeled arrays functionalities.

## Main concepts
Pyplan library is based on two main objects:

### Index
The index object is the way to define a dimension in Pyplan. Indexes are created using a Graphical Using Interface (GUI), through drag and drop method.
![Index Definition](http://img.pyplan.org/Pyplan_library_index_definition.png)

    pp.index(["Item 1","Item 2","Item 3"])

For someone coming from Xarray, the index Id property is the equivalent of Xarray "Dim" and the index values are the equivalent of "Coords".
Different than Xarray, Pyplan index are defined with a unique set of values, and when used, all the elements are present in that dimension.
Following the example above, any data cube indexed by "Items" will contain "Item 1" , "Item 2" , "Item 3"

### Cube
The Cube object is a labeled DataArray object defined as following:
![Cube Definition](http://img.pyplan.org/Pyplan_library_cube_definition.png)

    pp.cube( coords=[items], values=[10,20,30], dtype=None )
    # as well as
    pp.cube( [items], [10,20,30] )
As can be appreciated in the console output (at the right) the object type is a DataArray from Xarray, which means that it is possible to operate with Pyplan Cubes in the same way than with Xarray DataArray, inheriting not only all the properties but also the extensive functions list of this library.

Pyplanlib combines and enhance Numpy, Pandas and Xarray concepts.
## Functions List
Pyplan functions are group of functions for interacting with indexes of Pyplan data cubes. Pyplan library functions are called using the "pp." prefix. 
Function helper is launched pressing Ctrl+Space after writting the "pp." prefix. Use the arrows to scroll the list.
![enter image description here](http://img.pyplan.org/Pyplan_library_pp.png)
### Selecting Data from Array
#### pp.sel( dataArray, filterList, compareMode=1, defaultValue=None )

Filter dataArray using the fiterList filters

        Filter dataArray using the filterList filters. 
        dataArray: dataArray to be filtered
        filterList: the possible filters are:
                index==value
                index1==indice2 (in this case a changeindex will be made).
        compareMode: 1: by Value (default), 2: by pos (used only if changeindex is necessary)
        defaultValue: value to fill the elements that are not found (used only if changeindex is necessary) 
            Ex.
                pp.sel(dataArray1, index==value)  #as it is a single value no list is needed
                pp.sel(dataArray1, [index1==value1, index2==value2])
                pp.sel(dataArray1, [index1==value1, index2==index3])
        """

pp.lookup
pp.subset
pp.isel

Filter dataArray using the filterList filters. 
    

    pp.sel( dataArray, filterList, compareMode=1, defaultValue=None )
            
        dataArray: dataArray to be filtered
        filterList: the possible filters are:
                index==value
                index1==indice2 (in this case a changeindex will be made).
        compareMode: 1: by Value (default), 2: by pos (used only if changeindex is necessary)
        defaultValue: value to fill the elements that are not found (used only if changeindex is necessary) 
            Ex.
                pp.sel(dataArray1, index==value)  #as it is a single value no list is needed
                pp.sel(dataArray1, [index1==value1, index2==value2])
                pp.sel(dataArray1, [index1==value1, index2==index3])

### Pp.lookup
Returns the value of dataArray indexed by the index of dataMap.
  
      pp.lookup( dataArray, dataMap, sharedIndex, defaultValue=0 )
      dataArray must be indexed by sharedIndex and dataArray values must correspond to elements of sharedIndex.
        **For example**: Let's say you have a cube with an estimated inflation rate by Country ("inflation_rate" is the name of the cube; "country" is the name of the index) and you want to assign it to the corresponding Company depending on its location. On the other hand, there's a many-to-one map where each Company is allocated to a single Country ("country_to_company_allocation"). The sharedIndex, in this case, is Country ("country"). You can Add a default value for values not matching
        As a result, 
            pp.lookup( inflation_rate , country_to_company_allocation , country )
        will return the estimated inflation rate by Company.
  
## Basic Math and Missing Values

## Aggregation and Rolling window operations


  
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzQ3NjI4MTk2LC0xNTk0MjU0NDg5LDkwOD
c1MjI3MCwtNDM0OTY4MDI0LC0xMzE3MDYxNzMxLC0xODM0NzIy
Mjg4LDk3Mjk3MTk5NiwtMjEzNTcyMjY4OCwxMTE4NzQ5MDY2LD
Q5NDI4NTQ1OSwxMTYyODM4Mjk0LC0xMDA3NDkyMzc4LC00MDY3
MzUyMzgsMTY3MTE5NjUwNiwxMDAxOTQyODE0LC00NDU3MDYwMz
AsLTc2MTgyNjMzNSwtMTk2ODY2NTMzMiwxNjgwMDAyOTYzLDkw
ODE5MDk3OF19
-->