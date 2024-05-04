# if-else

## Performing condition statements using if-else

```
#!/bin/bash

read -p "Enter total marks: " marks

if [ $marks -gt 35 ]
then
    echo "You have passed"
else
    echo "You have failed"
fi
```

## Comparison operators:

| notation | meaning                  |
| -------- | ------------------------ |
| -eq      | equal to                 |
| -ne      | not equal to             |
| -gt      | greater than             |
| -ge      | greater than or equal to |
| -lt      | less than                |
| -le      | less than or equal to    |

## if-elif-else ladder:

```
#!/bin/bash

read -p "Enter total marks: " marks

if [ $marks -gt 80 ]
then
    echo "A grade"
elif [ $marks -gt 60 ]
then
    echo "B grade"   
else
    echo "C grade"
fi
```
