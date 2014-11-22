+++
date = "2014-11-15T19:58:28-06:00"
draft = false
title = "array and slices in go"

+++

In **go** lang, an array looks like this -

`var x [5]int`

where x is an array which is composed of 5 ints.

Same as other c family languages, arrays are indexed starting from zero.

arrays length is fixed and go provides another type **slices** to work with this situation.

`var x []int`

x is a slice and has a length of 0.

We can also create a slice using builtin **make** function.

`x := make([]float64, 5, 10)`

Where 5 is the length and 10 is the capacity of the underlying array.

If you have programmed in python than there is a way to create slices that look entirely familiar.

`arr := []int{1, 2, 3, 4, 5}`

`x := arr[0:5]`

**x** is a slice of **arr** and holds all the values. You can change the values by changing the index in x.

`x := arr[1:2]`

We can also omit the **low:high** from slice.

`x[0:len(arr)]`

`x[0:]`

`x[:4]`

