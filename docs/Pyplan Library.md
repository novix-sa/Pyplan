
# **Pyplan Library**

Pyplan is a [Python](https://www.python.org/) library intended for supporting multidimensional dynamic simulation based on the Pyplan IDE web applica. 
It is based on [Xarray](http://xarray.pydata.org/) DataArray object and take advantage of its N-dimensional labeled arrays functionalities.


## Main concept
Pyplanlib is based on two main objects:
pp.index is the way to define a dimension in Pyplan

    pp.index(["Item 1","Item 2","Item 3"])

pp.Index
pp.Cube
pp.cube and pp.index are mirrors of Xarray Dataarray and Coords but managed in a more structured manner so that data scientist can easily create models using the extensive set of tool developed for Python.

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
eyJoaXN0b3J5IjpbLTE3OTE4MDg0NzAsLTEwMDc0OTIzNzgsLT
QwNjczNTIzOCwxNjcxMTk2NTA2LDEwMDE5NDI4MTQsLTQ0NTcw
NjAzMCwtNzYxODI2MzM1LC0xOTY4NjY1MzMyLDE2ODAwMDI5Nj
MsOTA4MTkwOTc4LDQ5NDgwNzcwM119
-->