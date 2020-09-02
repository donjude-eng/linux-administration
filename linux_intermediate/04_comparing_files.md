# diff commands (Comparing the contents of the files)
* diff file1 file 2 (Compare two files)
* sdiff file1 file2 (Side-by-side comparison)
* vimdiff file1 file2 (Highlight differences in vim)

# vimdiff
* ctrl-w w = Go to next window
* :q (close current window)
* qa (Quit all (close both files)
* qa! (Force quit all)

# Example
```
[adminuser@localhost files]$ ls
firsttest.txt  firstvol  secondtest.txt  secondvol
[adminuser@localhost files]$ cat firstvol
1 tags: credentials
2 site: facebook.com
3 user: jason
4 pass: Abee!
5 tags: credentails
[adminuser@localhost files]$ cat secondvol
1 tags: credentials
2 site: facebook.com
3 user: jason
4 pass: bee!
5 tags: credentials

[adminuser@localhost files]$
[adminuser@localhost files]$ diff firstvol secondvol
4,5c4,6
< 4 pass: Abee!
< 5 tags: credentails
---
> 4 pass: bee!
> 5 tags: credentials
>
[adminuser@localhost files]$ sdiff firstvol secondvol
1 tags: credentials						1 tags: credentials
2 site: facebook.com						2 site: facebook.com
3 user: jason							3 user: jason
4 pass: Abee!						      |	4 pass: bee!
5 tags: credentails					      |	5 tags: credentials >
```
* vimdiff firstvol secondvol




