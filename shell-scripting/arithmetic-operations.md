# Arithmetic operations

## Wrong way of performing arithmetic operation:

```
#!/bin/bash

x=10
y=5

sum=$x*$y

echo "sum of $a and $b = $sum"
# sum of  and  = 10*5
```

## How to perform arithmetic operations correctly:

1. using \`let\` before the variable

```
#!/bin/bash

x=10
y=5

let sum=$x+$y

echo "sum of $x and $y = $sum"
# sum of 10 and 5 = 15
```

2. using ((expression)) syntax

```
#!/bin/bash

x=10
y=5

echo "sum of $x and $y = $(($x+$y))"
# sum of 10 and 5 = 15
```
