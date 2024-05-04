---
description: >-
  arrays in bash can have elements of different data types and are space
  separated.
---

# Arrays

## Array declaration

```
#!/bin/bash

arr = (1 2 "John" 25.6)
```

## Reading an Array

Arrays are \`0\` indexed and can be read as shown below:

```
echo ${arr[0]}

echo ${arr[1]}
```

## Print all elements in the Array

```
echo ${arr[*]} 

# here '*' indicates all elements
```

## Length of array

```
echo ${#arr[*]}
```

## Range in array

```
# this will print from 'startIndex' till last element
echo ${arr[*]:startIndex} 

# this will print from 'startIndex' till 'endIndex'

echo ${arr[*]:startIndex:endIndex}
```

## Creating a dictionary (key-value pair) from array

```
array = $(["name"]="Ganesh" ["age"]=23)

echo ${array["name"]}
echo ${array["age"]}
```
