# The Vi Editor
* vi [ file] : Edit file
* vim [ file] : same as vi, but more features
* view [ file] : starts vim in read-only mode

# VI Command Mode and Navigation
* k : up one line
* j :Down one line
* h :left one character
* l : Right one character
* w : Right one word
* b :left one word
* ^ : Go to the begining of the line
* $ Go to the end of the line

# Vi-Repeating Commands
* Repeat a command by preceding it with a number.
  1. 5k = Move up a line 5 time.
  2. 80i<Text><ESC> = insert<Text>80times
  3. 80i_<Esc> = Insert80"_"characters

# vi - Deleting Text
* x : Delete a character.
* dw : Delete a word.
* dd : Delete a line
* D : Delete from the current position

# Vi - Changing Text
* r : Replace the current character
* cw : Change the current word
* cc : Change the current line.
* c$ : Change the text from the current position
* C : Same as c$
* ~ : reverses the case of a character

# Vi - Undo / Redo
* u - Undo
* ctrl-R - Redo