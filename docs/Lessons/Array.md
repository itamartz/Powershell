---
title: Array
subtitle: Powershell Array
layout: page
hide_hero: false
show_sidebar: false
---

## Array
An array is a data structure that's designed to store a collection of items. The items can be the same type or different types.

I will try to explain by design

This is a array with 3 Cells, Array have an index that can point you to the value in a cell.\
Array start from the index 0, so if we want to get the value in the first cell we need to pass the index 0
Array start with index 0 for the first cell (from left), and if you need the last cell is -1.\

 &nbsp; &nbsp; &nbsp;  0  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  1  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;2\
[ $object ][ $object ][ $object ]\
&nbsp; &nbsp; &nbsp; -3  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; -2  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; -1

## Example
Start an array with 0 cells.
```powershell
$array = @()

```

Add data to the array: (In this example $item1 represent an object)\
```powershell
$array += $item1
```
An we can get the data from this cell by running this command

```powershell
$array[0]
```


