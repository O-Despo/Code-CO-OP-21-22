# Python List

Lists are a way of representing things in a order in the real world. They do the same thing in Python.

A list stores items in a array, you can imagine items on a shopping list. You can do things to these items change their position, cross them off, add more, etc.

## List Syntax

A list stores a sequence of variables.

```py
my_list = ['a string', 3, 12.23, True]
```

As you can see a Python List can store any datatype all in the same list. The items in this list are `'a string'`, `3`, `12.23`, `True`. We can access these items and use them as variables using **indices**

### Indices

```py
a_item = my_list[0]
```

`a_item` is now equal to `'a string'` and there has been no change to the list. 

Note that 0 gave us the first element of the list. This is called **zero indexing**, it means that the first item will have the index zero instead of 1.

| Normal Counting | List Index | Value of item |
|-----------------|------------|---------------|
| 1               | 0          | 'a string'    |
| 2               | 1          | 3             |
| 3               | 2          | 12.23         |
| 4               | 3          | True          |


```py
a_item = my_list[0:2]
```


