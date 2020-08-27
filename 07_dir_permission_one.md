# Permissions - files vs Directories
* Read(r) : Allow file names in the directory to be read
* Write(w) : Allows entries to be modidfies within the directory
* Execute(x) : AAllow access to contents and metadata for entries

# Permission Categories
* u - User
* g - Group
* o - other
* a - All

# Groups
1. Every user belongs to one group
2. Users can be belong to many group
3. You can also us id -Gn.

# Secret Decoder Ring
![Linux Directories](/secretdecoder.PNG?raw=true "Title")

# Changing permissions
1. chmod : Change mode command
2. ugoa : User catogory user, froup, other, all
3. +-= : Add,subtract, or set permssions
4. rwx : read, Write, Execute.

# Order has meaning
* Symboloic [U - rwx] [G :r-x] [O - r--]
* Binary [ 111 ] [ 101 ] [ 100 ]
* Decimal [ 7 ]  [ 5 ] [ 4]

# Commanly used permsiion
```
Symbolic        Octal
-rwx-------     700
-rwxr-xr-x      755
-rw-rw-r--      664
-rw-rw----      660
-rw-r--r--      644

```


