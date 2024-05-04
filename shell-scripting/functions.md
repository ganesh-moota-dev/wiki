# functions

## functions declaration:

```
#!/bin/bash

function func1(){
  echo "function func was called."
}

func1
function func was called.
```

## arguments passing in function:

```
#!/bin/bash

function func2(){
  echo "sum of the two numbers is $(($1 + $2))"
}

func2 10 5
# sum of the two numbers is 15
```

## Command line arguments passed while executing script:

```
#!/bin/bash

# accessing command line arguments
echo "the first argument passed was $1"
echo "the second argument passed was $2"

echo "the total number of arguments passed are $#"
echo "all the arguments that were passed are = $@"

```

Add logic to check if atleast one arguments is passed while executing the script

```
#!/bin/bash

if [ $# -eq 0 ]
then 
    echo "Please provide atleast one argument"
    exit 1
fi

echo "all the arguments that were passed are = $@"
```
