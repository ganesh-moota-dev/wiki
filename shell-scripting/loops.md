# loops

## for loop:

for loop can iterate on any thing that can be iterated like an array or sequence

```
FILE = "/root/scripts/servers.txt"

for server in $(cat $FILE)
do 
    echo $server
done
```

## while loop:

```
count=0
num=10

while [$count -le $num]
do
    echo "Count = $count"
    (($count++))
done
```
