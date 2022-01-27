# Functions

I will expain functions in two ways one math related and one code related. Read both and use whatever works best for you.

Math: A fucntion in code like a function in math. It takes a input and produces a output after doing some operations on the data. In code you can not only do mathmatical operatations on the input data but also any other opreation you like.

Code: A function is a block of code that is can be run mutpbles times. Every time it is run it takes somthing called arumnets, these arumnets assign new values to varibales inside the function. Anythin that can be written outside a function can be written inside a function, so there is no limit to what you can do with them. Functions are one of the most usefull parts of any modern programing languges and save us from having to writ the same code in diffrent locatins.

## Calling a funciton

You have without knowing it already called functions in pyton `len()` is a built in function.

```python
length_of_list = len([1, 3, 4, 2])
```

When you call a function you put the input data in parathersis after the function name, in this case `[1, 3, 4, 2]` is the input. The functions then process this input data and outputs it like. This output can be assigned to a variale in this case `length_of_list` which is equal to `4`.

## Defining functions

We of course can also define out own funcitons in python.

```python
def add_numbers(input_1, input_2):
    return input_1 + input_2

a = add_numbers(1, 2)
#A has a value of 3
```

Breaking this down peice by peice

- `def` is a keyword used to decribe a function
- `add_numbers()` is the function name and is used later to call the function
- `(input_1, input_2)` are artibues: when we pass `add_numbers(1, 2)` is makes `input_1` = `1` and `input_2` = `2` inside the function
- `return` is another keyword: what ever the statement evaluates to that comes after it is retunred from the funcition
  - This means that `a = add_numbers(1, 2)` is realy equal to `a = input_1 + input_2` beacuse of the line `return input_1 + input_2`
- `a = add_numbers(1, 2)` is a function call. 1 and 2 are passed to the function and `a` is the return value

### More examples of functions

```pythonm
def get_data(url):
    respone_item = requests.get(url, params={'day': 'sunday}, auth=auth)
    json = reposne_item.json()
    json_data = json['data']
    return json_data
```

- You can call functions inside of other functions
- `json_data` is retunred

### Args

- Python function paramters are somwhat complex

```python
def example_func(pos_1, pos_2, args*, defaut = False):
    return (pos_1, pos_2, args, default)

example_func(1, 3) #Retuns (1, 3, [], False)
example_func(2) #Error
example_func(1, 1, 3, 2, 4)# returns (1, 1, [3, 2, 4], Flase)
example_func(1, 1, 1, 3, default = True)# returns (1, 1, [3, 2, 4], True)
```

- `(a, b, c)` these are positial arguments, the value they are assioated with is based on where the data is enterd into the call
- `(b = True)`: b is a default value, it will be `True` unless explicity changed in the call, not required
- `(args*)`: and posional argumnets that are more then those sprcifed is assisend to a list call args