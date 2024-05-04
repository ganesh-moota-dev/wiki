# Variables

## Syntax

```
#!/bin/bash

# defining variables
name="Ganesh"
age=23

echo "My name is $name and my age is $age"
```

## Eval $( )

In order to store output of commands executed in variable we can use eval function as below

```bash
#!/bin/bash

DIRECTORY=$(pwd)
USER=$(whoami)
```

## Constant Variables

```bash
#!/bin/bash

readonly userId="123"
```

## Accept user inputs and save them in variables

```
#!/bin/bash

read -p "Enter your name: " name

echo "Your name is $name"
```
