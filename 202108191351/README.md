# Copy, Move ,Remove,Rename in The Linux Filesystem


## Copy ##
`
cp` Copies Files 
* `cp <a.txt> <b.txt>` creates a new file with the name contents as the first argument
* `cp a.txt ~/Desktop` Or it can be used to copy to a directory
* `cp <a.txt> <b.txt> <directory>` to copy multiple files to a directory (last argument has to be a directory)
* `cp *.txt <dir>` Copies all files of said type to a directory
* `cp -Rv` Recursivly copies whole directories
* `-f` Force
* `-i` Confirm overwrite

### Remove ###

`rm <filename>` Deletes a file
*  `rmdir` Removes a dir

#### Move and Rename ####
`mv file "new file path"` Moves the files to the new location
* `mv filename new_file_name` Renames the file to a new filename
