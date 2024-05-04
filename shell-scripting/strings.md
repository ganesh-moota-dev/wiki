# Strings

## String operations

```
#!/bin/bash

str="Hi John, how are you?"

echo "length of the string = ${#str}"
# length of the string = 21

echo "uppercase will be = ${str^^}"
# uppercase will be = HI JOHN, HOW ARE YOU?

echo "lowercase will be = ${str,,}"
# lowercase will be = hi john, how are you?

echo "replace name to Ganesh = ${str/'John'/'Ganesh'}"
# replace name to Ganesh = Hi Ganesh, how are you?

echo "slice first 10 characters = %{str:0:10}
# slice first 10 characters = Hi John, h
```
