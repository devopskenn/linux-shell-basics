# GNU/Linux Commands

## Commands and shortcuts within terminal

#### Start Terminal

`ctrl` + `alt` + `T` - Open a new Terminal Window



#### Close Terminal

`Ctrl` + `Shift` + `W` - Close terminal tab <br>
`Ctrl` + `Shift` + `Q` - To close entire terminal


  
#### Taking Charge of the Terminal

`ctrl` + `L` - Clears out all the texts in the Terminal Window <br>
`ctri` + `S` - Stops all console output without stopping the command from running. Useful for very long terminal/console output <br>
`ctrl` + `Q` - Resumes terminal/comsole output <br>
`ctrl` + `D` - Logs you out of all current sessions <br>
`ctrl` + `C` - Ends the current running process in terminal <br>
`ctrl` + `Z` -  Suspends (pause) currently running foreground process, which returns shell prompt. You can then use `bg` command allowing that process to run in the background. To again bring that process to foreground, use fg command. To view all background processes, use the `jobs` command. <br>
`Tab` - Auto-complete files and directory names <br>
`Tab` + `Tab` - DIsplays all possibilities when typed characters does not match file or directory names



#### Cursor Movement

`ctrl` + `A` - Jump to the beginning of the line you are typing on <br>
`ctrl` + `E` - Jump to the beginning of the line you are typing on <br>
`ctrl` + `F` - Move the cursor forward, one character at a time on the line you are typing on <br>
`ctrl` + `B` - Move the cursor backwards, one character at a time on the line you are typing on <br>
`alt` + `F`  - Move the cursor forward, one word at a time on the line you are typing on <br>
`alt` + `B`  - Move the cursor backwards, one word at a time on the line you are typing on <br>
`ctrl` + `X` + `X` - Highlight all the text on the current line you are typing on



#### Manipulating Texts

`Ctrl` + `U` - Cut the line from the current position to the beginning of the line, adding it to the clipboard. If you are at the end of the line, cut the entire line <br>
`Ctrl` + `K` - Cut the line from the current position to the end of the line, adding it to the clipboard. If you are at the beginning of the line, cut the entire line <br>
`Ctrl` + `W` - Delete the word before the cursor, adding it to the clipboard <br>
`Ctrl` + `Y` - Paste the last thing from the clipboard that you cut recently (undo the last delete at the current cursor position) <br>
`Alt` + `T`  - Swap the last two words before the cursor <br>
`Alt` + `L`  - Make lowercase from cursor to end of word <br>
`Alt` + `U`  - Make uppercase from cursor to end of word <br>
`Alt` + `C`  - Capitalize to end of word starting at cursor (whole word if cursor is at the beginning of word) <br>
`Alt` + `D`  - Delete to end of word starting at cursor (whole word if cursor is at the beginning of word) <br>
`Alt` + `.`  - Prints the last word written in previous command <br>
`Ctrl` + `T` - Swap the last two characters before the cursor



#### Accessing Historical Commands

`Ctrl` + `R` - Lets you search through previously used commands <br>
`Ctrl` + `G` - Leave history searching mode without running a command <br>
`Ctrl` + `J` - Lets you copy current matched command to command line without running it, allowing you to make modiﬁcations before running the command <br>
`Alt` + `R`  - Revert any changes to a command you’ve pulled from your history, if you’ve edited it <br>
`Ctrl` + `P` - Shows last executed command, i.e. walk back through the command history (Similar to up arrow) <br>
`Ctrl` + `N` - Shows next executed command, i.e. walk forward through the command history (Similar to down arrow)
