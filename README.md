# linux-administration
Testing and learning Linux administration.

# Cat command in Linux with examples

* $cat filename : It will show content of given filename
* $cat file1 file2 : This will show the content of file1 and file2.
* $cat -n filename : It will show content with line number.
* $ cat >newfile : Will create and a file named newfile
* $cat [filename-whose-contents-is-to-be-copied] > [destination-filename] : The content will be copied in destination file
* $cat -s notes.txt : Will suppress repeated empty lines in output
* $cat file1 >> file2 : Will append the contents of one file to the end of another file
* $tac filename : Will display content in reverse order 
* $cat -E "filename" : Will highlight the end of line
* $cat -- "-dashfile" : Will display the content of -dashfile


sort

sort file       //Sort text in file
sort -r         //Sort in reverse order
sort -u         //Sort unique (remove duplicate line)
sort -k F       //Sort by key. F is the field number
Creating collectoin of files

tar c|x|t f tarfile         // create a list of contents
tar options

c           Create a tar archive
x           Extract files from the archive
t           Display the tabke of contents list
v           Be verbose
z           Use compression
f file      Use this file
Disk Usage

du          Estimate file usage
du -k       Displays size in Kilobytes
du -h       Display sizes in human readable format



