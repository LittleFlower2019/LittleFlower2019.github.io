---
layout: post
title: How to decide input values of method in Python
lang: en
categories:
    - Python
tags:
    - Env
---

There are different way to define input parameters of method in Python. 

- Fixed Location Input
- Default Input
- Variance Input
- Keyword Input


##Fixed Location Input
  
  The input variables have to pass in as same as their location in which the method's definition.
 
 ```
def func(input_a, input_b)
    print(input_a, input_b)

one = 10
two = 20
show = func(10, 20)
print(show)
```

## Default Input
The input variable has been given a default value in case of missing pass a input variable.

```
def fixed_location(input_a='defaultValue' )
    print(input_a)
    
print(show)

Output
------------------
defualtValue
```

## Variance Input
*input, Passing a number of variables to method regarding to Dictionary.

Tuple
```
def func(*inputs)
    for i in inputs
        print(i)
    return inputs
    
input = func('Test', 'Ops')
print(input)

Output
------------------
Test
Ops

```
List
```
# Using elements of List as input parameters, which is same as Tuple
def func(*inputs)
    for i in inputs
        print(i)
    return inputs

inputs = ['Test', 'Ops'] 
input = func(*inputs)
print(input)

Output
------------------
Test
Ops
('Test' 'Ops')
```

## Keyword Input
**input, Passing a number of variables to method regarding to Dictionary.

```
# Dictionary
def func(name, **inputs)
    age = inputs.get('age') if inputs.get('age')
          else 'unknown'
    sex = inputs.get('sex') if inputs.get('sex')
          else 'unknown'
    
    return name, age, sex

inputs = {'sex':'boy', 'age':25}
input = func('Jim', **inputs)
print(input)

Output
------------------
Test
Ops
('Test' 'Ops')
```

## Note

In Python, passing variables have to follow the sequence in the definition of the method.








