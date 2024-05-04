# file path concepts

## 1. different path values can be extracted using below pre-defined variables:

| variable | what it returns                                               | example                                               |
| -------- | ------------------------------------------------------------- | ----------------------------------------------------- |
| basename | strip directory info and return only current file/folder name | <p>basename $(pwd)<br># bash-scripts</p>              |
| dirname  | strip the file name and give directory path                   | <p>dirname $(pwd)<br># /home/ganesh</p>               |
| realpath | gives you full path of file                                   | <p>realpath $(pwd)<br># /home/ganesh/bash-scripts</p> |

## 2. check if file/dir exists?

| condition               | meaning                    |
| ----------------------- | -------------------------- |
| if \[ -f file\_name ]   | if file exists             |
| if \[ ! -f file\_name ] | if file does not exist     |
| if \[ -d dir\_name ]    | if directory exists        |
| if \[ ! -d dir\_name ]  | if directory doesn't exist |

### example:

```
#!/bin/bash

readonly file_name "/root/scipts/connectivity.sh"

if [ ! -f file_name ]
then 
    echo "File with path $file_name doesn't exist"
    exit 1
fi

```
