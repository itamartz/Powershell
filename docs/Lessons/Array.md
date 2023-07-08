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
[ ][ ][ ]

## Example
Start an array with 0 cells.\
```powershell
$array = @()

```

Add data to the array: (In this example $item1 represent an object)\
```powershell
$array += $item1\
```
An we can get the data from this cell by running this command

```powershell
$array[0]
```


