# Decoding ls -l Output
* Hidden files begin with a period
* Sometimes called "dot files".
* Hidden files are not diaplayed by default
* To show hidden files with ls, use ls -a

# ls - a ( This will show up if there is any hidden files , All files)
##### ls -l (Hidden files eill not be diplayed)
* Dot means this directory
* Dot Dot means parent directory

# Listing files by type
* Use ls -F to reveal file types
* / Directory
* @ Link
* * Executable

* ls -lF (Long listing file format)

# Listing files by time and in reverse
* ls -t : List files by time
* ls -r : Reverse order
* ls -latr : Long listing including all files reverse sorted by time

# Listing Files Recursively
* ls -R : Lists files recursively

# The tree Command
* Similar to ls - R, but creates visual output.
* tree -d : List directories only
* tree -c : Colorize output

# listing Files with color
* ls --color, colorize the output

# Listing directories
* ls Music
* ls -d Music
* ls -l Music
* ls -ld Music
* ls --color

# Working with spaces in names
* Just say no to spacs!
* Alternatives
  1. Hyphens(-)
  2. Underscores(_)
  3. CamelCase

# ls options
```
-a : List all files including hidden files
--color : List files with colorized output
-d : List directory names, not contents.
-l : Use the long lsiting format
-r : reverse the order
-R : List files recursively
-t : Sort by time most recent first

```





