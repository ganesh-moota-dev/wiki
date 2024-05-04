# switch-case

when there are multiple conditions instead of if-else ladder it is better to use a switch case for conditional logic.

```
#!/bin/bash

echo "Please choose an option"
echo "a = To print current datetime and hostname"
echo "b = To print current working directory"
echo "c = To list all the finles in current directory"

read choice

case $choice in
    a) 
        date
        hostname
        ;;
    b) pwd;;
    c) ls;;
    *) echo "You have provided invalid input"
esac
```
