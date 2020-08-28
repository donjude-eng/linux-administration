 # Directory Permisiions revisited
 * permission on a directory can effect the files in the directory.
 * If the file permissions look correct, start checking directory permissions.
 * Work your way up to the root.

 # File Creation mask
 * File creation mask determines default permissions.
 * If no mask were used permssions would be ;
    1. 777 for directories.
    2. 666 for files.

# the umask Command
* umask [ -s] [ mode ]
* Sets the file creation mask to mode, if given
* Use -S for symbolic notation

# Umask mode to the default permisiion
![Linux Directories](Umask.PNG?raw=true "Title")

# Octal Subtraction Is an Estimation
![Linux Directories](octalsubtraction.PNG?raw=true "Title")

# Common umask mode
* 022
* 002
* 077
* 007

# Special Modes
* unmask 0022 is the same as unmask 022.
* chmod 0644 is the same as chmod 644
* The special modes are:
   1. setuid
   2. setgis
   3. sticky

# Umask testing
```
[adminuser@localhost ~]$ mkdir testumask
[adminuser@localhost ~]$
[adminuser@localhost ~]$
[adminuser@localhost ~]$ cd testumask/
[adminuser@localhost testumask]$
[adminuser@localhost testumask]$ umask
0002
[adminuser@localhost testumask]$
[adminuser@localhost testumask]$ umask -S
u=rwx,g=rwx,o=rx
[adminuser@localhost testumask]$ mkdir a-dir
[adminuser@localhost testumask]$ touch a-file
[adminuser@localhost testumask]$
[adminuser@localhost testumask]$ ls -l
total 0
drwxrwxr-x 2 adminuser adminuser 6 Aug 28 08:00 a-dir
-rw-rw-r-- 1 adminuser adminuser 0 Aug 28 08:01 a-file
[adminuser@localhost testumask]$
[adminuser@localhost testumask]$ rmdir a-dir
[adminuser@localhost testumask]$
[adminuser@localhost testumask]$ rm a-file
[adminuser@localhost testumask]$ unmask 007
bash: unmask: command not found...
[adminuser@localhost testumask]$ umask 007
[adminuser@localhost testumask]$
[adminuser@localhost testumask]$ umask -s
bash: umask: -s: invalid option
umask: usage: umask [-p] [-S] [mode]
[adminuser@localhost testumask]$ umask -S
u=rwx,g=rwx,o=
[adminuser@localhost testumask]$ ls -l
total 0
[adminuser@localhost testumask]$
```

# Summary
* Symbolic permissions
* nUmaric /Octal permissions
* File versus directory permissions
* Changing permissions
* Working with groups
* File creation mask