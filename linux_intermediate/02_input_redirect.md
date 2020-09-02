# file Redirection

* ls -l (listing the files)
* ls -l > files.txt (To redirect the files.txt)
* cat files.txt ( This will result the contents of files.txt)

# Input the files and redirect the output file using the commands
* input command - ls -l > files.txt
* redirect the files - sort < files.txt > sorted_files.txt

# Standard output
* ls files.txt not-here 1> out 2 > out err

# Standard error
* cat out.err

# Combaining standard output and the error
* ls files.txt not-here > out.both2>&1
* cat out.both
  *  Example :
  ```
    [adminuser@localhost ~]$ ls files.txt not-here > out.both 2>&1
    [adminuser@localhost ~]$ cat out.both
    ls: cannot access 'not-here': No such file or directory
    files.txt
    ```
# Null device
* ls files.txt not-here >/dev/null 2>&1




