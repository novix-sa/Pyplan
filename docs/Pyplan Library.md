
# **Pyplan Library**

Pyplan is a [Python](https://www.python.org/) library intended for supporting multidimensional dynamic simulation running on the Pyplan IDE web application. It is based on [Xarray](http://xarray.pydata.org/) DataArray object and take advantage of its N-dimensional labeled arrays functionalities.

## Main concepts
Pyplan library is based on two main objects:

### Index
The index object is the way to define a dimension in Pyplan. Indexes are created using a Graphical Using Interface (GUI), through drag and drop method.
![Index Definition](http://img.pyplan.org/Pyplan_library_index_definition.png)

    pp.index(["Item 1","Item 2","Item 3"])


For someone coming from X-Array, the index Id property is the equivalent of X-Array "Dim" and the index values are the equivalent of "Coords".
Diferent than X-Array, Pyplan index are defined with a unique set of values, and when used, all the elements are present in that dimension.
Following the example above, any data cube indexed by "Items" will contain "Item 1" , "Item 2" , "Item 3"


## Data Structure
Based on X-Array objects, with a different approach to index definition and manipulation

## Goals
Pyplanlib aims to become development package for data scientist and businessmen facing problems where a huge quantity of data needed be analyse and structure.

Complex problems and sophisticated mathematical operations involving multidimensional arrays should be solved using this library.

Pyplanlib combines and enhance Numpy, Pandas and Xarray concepts.
## Function List
## Selecting Data from Array
### PP.Sel

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
        """
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTEyNTU1MjE3NCwtMjEzNTcyMjY4OCwxMT
E4NzQ5MDY2LDQ5NDI4NTQ1OSwxMTYyODM4Mjk0LC0xMDA3NDky
Mzc4LC00MDY3MzUyMzgsMTY3MTE5NjUwNiwxMDAxOTQyODE0LC
00NDU3MDYwMzAsLTc2MTgyNjMzNSwtMTk2ODY2NTMzMiwxNjgw
MDAyOTYzLDkwODE5MDk3OCw0OTQ4MDc3MDNdfQ==
-->