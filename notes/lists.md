<<<<<<< HEAD
# Python Lists

A python list is a sequence of python variables. You can think of it like a line of people each item in the list being a person. A lot of actions can happen in the line of people someone can leave, switch with another person, or people can be added to the back of the line. (This is not all the operations you can do on a lists there are many more but you get the idea)

## Lists Creation

```py
my_list = [1, 3.23, "A string", True]
```

The syntax for creating a list is putting you elements in `[]`(square brackets) and separating them with a comma `,`. Note that this list has many variables with different datatype, this is allowed in python but not some packages or libraries.

## Indexing

```py
first_item = my_list[0]
third_item = my_list[2]
last_item = my_list[3]
last_item = my_list[-1]
```

We have a sequence of variables so we need a way to use and edit those variables. We do this by indexing the list with the number of the elements we want to aces, we can then use that as a variable normally in our code.

Note: The last examples used the index `-1` this means get the last element of the list. If you use `-2` you get the second to last in this case `"A string"`.

Note: The was we got the first item of the list was `my_list[0]`. Common thought would lead to using `1` to get the first element but Python uses **Zero indexed** lists. Which means the first element's index is `0` and the second's `1`.

We also use indexing to change a elements value.
```py
my_list[2] = 4
```

## Pop

Sometimes we want to get the last element in the list. When we call `my_list[-1]` it gives us access to the element but dose not remove it form the list but `pop()` dose.

```py
item = my_list.pop()
```

`my_lists` is now equal to `[1, 4, "A string"]`, and `item` is equal to `True`

## Append

We might also want to add to the end of a list. To do this we use the `.append()` method. 

```py
my_list.append('A NEW ELEMENT!!!!')
```

`my_lists` is now equal to `[1, 4, "A string", "A NEW ELEMENT!!!!"]`

## Slicing indices 

You can also take a portion of a list and group them.

```py
my_slice = my_list[1:-1]
```

my_slice is now a list containing the second to last element of my_list `['1, 4, "A String", "A NEW ELEMENT!!!!"]`

## Count and length

We can also see how many of a given element is in a list with `.count()` and the length of a list with `len()`

```py
count_list = [0, 0, 1, 0]
count = count_list.count(0)
length_of_count  = len(count_list)
```

`count` is equal to `3`, `length_of_count` is equal to `4`

## copy

When you use the equals sign between two lists it points the new list to the other list not making a new one. 

```
fruits = ['apple', 'pear']
foods = fruits

foods.append('egg')
```
`fruits` is now `['apple', 'pear', 'egg']`. Notice that when we were editing `foods` it was really `fruits`

This is solved with copy

```
fruits = ['apple', 'pear']
foods = fruits.copy()

foods.append('egg')
```

## Reverse self expiatory

It reverses the list.

```py
my_list = [1, 3, 2]
my_list.reverse()
```

## Sort

If there is a list which has data types then it can be sorted.

```py
my_list = [4, 2, 1]
my_list.sort()
```

`my_list` is now `[1, 2, 4]`

## remove

Removes a element by value

```py
my_list.remove(2)
```

## extend

You can add two lists together (in the same dim)

```py
my_list.extend([1, 3])
my_list = my_list + [1, 3]
```
Both have the same outcome `[1, 4, 1, 3]`


## insert

Inserts item at given location

```py
#my_list.insert(value, index)
my_list.insert(3, 2)
```

## clear

```py
my_list.clear()
```

`my_list` is now `[]`
=======
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


>>>>>>> 28efffda488ee8358cf433241eef2a5c3a90a1c6
