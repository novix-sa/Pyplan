
# Pyplan Library

Pyplan is an open source library providing easy-to-use labelled data structures and data analysis functions for [Python](https://www.python.org/) programming language.

Pyplanlib is based on Xarray DataArray object and take advantage of its N-dimensional arrays.

Pyplanlib pp.cube and pp.index are mirrors of Xarray Dataarray and Coords but managed in a more structured manner so that businessmen and data scientist can easily create models with a bunch of python tools.

Pyplanlib has an extensive number of functions that help modelers developing.

## Main concept

## Data Structure
Based on X-Array objects, with a different approach to index definition and manipulation

## Goals
Pyplanlib aims to become development package for data scientist and businessmen phasing problems where a huge quantity of data needed be analyse and structure.

Complex problems and sophisticated mathematical operations involving multidimensional arrays should be solved using this library.

Pyplanlib combines and enhance Numpy, Pandas and Xarray concepts.
## Function List
## Selecting Data from Array
### PP.Sel
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

### Pp.lookup
Returns the value of dataArray indexed by the index of dataMap.
  
      dataArray must be indexed by sharedIndex and dataArray values must correspond to elements of sharedIndex.
        **For example**: Let's say you have a cube with an estimated inflation rate by Country ("inflation_rate" is the name of the cube; "country" is the name of the index) and you want to assign it to the corresponding Company depending on its location. On the other hand, there's a many-to-one map where each Company is allocated to a single Country ("country_to_company_allocation"). The sharedIndex, in this case, is Country ("country"). You can Add a default value for values not matching
        As a result, 
            pp.lookup( inflation_rate , country_to_company_allocation , country )
        will return the estimated inflation rate by Company.
        """
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc2MTgyNjMzNSwtMTk2ODY2NTMzMiwxNj
gwMDAyOTYzLDkwODE5MDk3OCw0OTQ4MDc3MDNdfQ==
-->