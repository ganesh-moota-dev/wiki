# Hello World program

1.  Create a script file and name it as hello\_world.sh

    ```bash
    touch hello_world.sh
    ```


2.  Open file using vi command.

    ```bash
    vi hello_world.sh
    ```


3. Click **"i"** to enter into insert mode.
4.  specify the shell interpreter using **"shebang"**

    ```bash
    #!/bin/bash
    ```


5.  add a line to print "hello world" to the output.

    ```bash
    echo "hello world"
    ```


6. Click "Esc" to exit from insert mode
7. Write ":wq" at the end of the file to save and exit.

## hello\_world.sh

```bash
#!/bin/bash

echo "hello world"
```

## How to run the script file?

* make sure script has execute permission "rwx".
*   run the script file using:

    ```
    ./script.sh

    bash script.sh
    ```


* Press "Ctrl + C" to terminate script
