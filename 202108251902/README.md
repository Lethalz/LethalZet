# Linux Commands basics


-Reference

● cal - to show calendar
● date - to display current time and date
● pwd - location of where we are currently located
● man ___(command) - shows the manual page of command
● cd - to go somewhere else, change directory
● exit - to end a terminal session
● Using up and down keys to navigate the command history
● Using left and right arrow keys to navigate within the current command
● mkdir - to create directory
● mkdir -v - shows message for each created directory
● mkdir _ _ - can also create multiple directory
● mkdir __/__ - to create directory elsewhere (if parent dir doesn’t exist, it will fail)
● mkdir -p __/__ - creates parent dir as needed
● mkdir {2008..2017}-{01..12} - creates folders performing brace expansion

● ls - displays the content of current dir
● less (path) - to open any text file
● To exit less press Q
● less -N - to display with line numbers (when working with codes)
● Less is capable to show any language
● less (path)/* - to show several text files
● ls (path) - to show contents of non-current dir
● ls .. - refers to the parent of current dir
● ls -l (path) - to see the symbolic link of file (long listing)
● file - to see the symbolic link of file
● ls -a, -all - lists dir with hidden files
● ls -l - shows additional information for each file
● ls -lh - prints size of files in human readable format
● ls *.h - displays all files whose filenames end in .h (or any other string)
● rm - to delete files
● rm -i - prompts before every removal
● rm -v - explains what is being done
● rm -r - removes file with their content
● . - refers to the current dir
● .. - refers to the parent dir
● cd (without path) - change to the home dir
● mv _ _ - to move(rename) files
● mv -v _ _ - explains what is being done
● mv __ __ __ _ - to move multiple files
● cd ~USERNAME - refers to the home dir of the user
● cd ~ - refers to own home dir
● ln - creates symbolic links between files
● ln target linkname - linkname links to target
● ln target - creates symbolic link to that file with the same name in the current dir
● cp source dest - to copy file to another destination
● cp dir dest - to copy dir to another destination
● cp -r dir dest - to copy dir with contents, if dest doesn’t exist it will be created
● echo - displays simple message
● echo -e - enables using backslash-escaped characters
● echo * - displays the listing of files of current dir
● echo ~USERNAME - shows the abs path of home dir of user
● echo $(( 5 + 5 )) - performs arithmetic expressions OUTPUT: 10
● echo abc{A,B,C}mm - performs brace expansion OUTPUT: abcAmm abcBmm
abcCmm
● echo num_{1..3} - OUTPUT: num_1 num_2 num_3 (also works for letters)
● echo $( ls _ ) - firs, the command inside $( ) will be executed, then echo
● echo \(character) - \ is used to escape character conflicts
● grep _ [file] - print lines matching a pattern [searches in file]
● grep -i - to ignore case sensitiveness
● grep -v - selects non-matching lines
● grep -c - prints a count of matching lines
● head [file]- prints the first 10 lines
● tail [file]- prints the last 10 lines
● head/tail -n -specifies the lines of prints
