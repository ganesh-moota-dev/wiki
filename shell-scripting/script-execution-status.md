# script execution status

Any script that was executed will either be successful or will get failed.

In order to know the success status of the most recently executed script we can use $0

| $? | meaning |
| -- | ------- |
| 0  | success |
| 1  | failed  |

```
#!/bin/bash

read -p "Enter your site url: " site

ping -c 1 $site

if [ $? -eq 0 ]
then 
    echo "connection to site $site was successful"
else
    echo "failed to establish a connnection with site $site"
fi

>> comment1
bash connectivity.sh
Enter your site url: www.google.com
PING www.google.com (172.217.166.36) 56(84) bytes of data.
64 bytes from bom07s18-in-f4.1e100.net (172.217.166.36): icmp_seq=1 ttl=118 time=3.25 ms

--- www.google.com ping statistics ---
1 packets transmitted, 1 received, 0% packet loss, time 0ms
rtt min/avg/max/mdev = 3.246/3.246/3.246/0.000 ms
connection to site www.google.com was successful
comment1

>> comment2
Enter your site url: www.localhost.com
ping: www.localhost.com: Name or service not known
failed to establish a connnection with site www.localhost.com
comment2
```
