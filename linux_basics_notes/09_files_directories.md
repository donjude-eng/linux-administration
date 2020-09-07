# Finding files and directories
### The find command
* find [ path...] [ expression]

* Recursively finds files in the path that match expression. if no arguments are supplied it find all files in the current directory.

# find Options
* -name pattern - Find files and directories that match pattern
* -iname pattern - Like -name, but ignores case.
* ls - performs an ls on each of the found items.
* mtime days - Finds files that are days old.
* size num - Finds file that are of size num.
* -newer file - Finds files that are newer than file.
* -exec command {} \;
* Run command against all the files that are found

## Important find command
```
find . -mtime +0 -mtime -13
find . -name s* -lsfind . -size +1M
find . -type d -newer mynotes.txtfind . -exec
file {} \; (Shows all the search results)
```

# A fast find - locate
* Locate us faster then the file command
 1. Lists files that match pattern
 2. Faster than the find command
 3. Quries and index
 4. Results are no in real time
 5. May not be enables on all systems

 # Summary
 * find command - Find search for files and directory in real time.I is very poerful
 * locate command - It is faster than find command but it is not real time.


