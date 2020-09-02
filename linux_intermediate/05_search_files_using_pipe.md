# The grep command
* grep - Displaying lines matching pattern
* grep pattern file

# grep options
* -i Performa search, ignoring case.
* -c Count the number of occurrences in a file.
* -n Precede output with line numbers.
* -v invert match. print lines that don't match

# fetching files using grep command
* grep user secret
* grep o secret
* grep -v o secret -- This will match the word that not contains the letter O.
* grep -i User secret -- To ignore the case will use this!
* grep -ci User secret -- Will match the oneline of user firstvol.
* grep -ni user secret  -- This option will display the line number

# cat -n secret (Will get the number of line )

# The file command
* file file_name Display the file type

# Pipes
* | Pipe symbol
* command-output | command-input

# grep pattern file
* cat file | grep pattern

# The cut command
* cut [ file] - Cut out selected portions of file. If file is omitted, use satndard output.

# cut Options
* -d delimiter : Use delimiter as the field separator
* -f N : Dispaly the Nth field

# searching pipe example
* Find all users named "bob" in etc/passwd.
* Print account name and real name.
* Print in alphabetical order by account name
* tr for translating character.

# piping Output to a pager
* more
* less

# Summary
* grep
* file
* cut
* tr
* column
* more
* less
* pipes



