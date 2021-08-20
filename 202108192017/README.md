# File Permissions on Linux

`ls -l` - To show file type and access permission

`chown <user>` Changing ownership of a file/dir
     
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`<user>` can be 
  * a-all
  * u-user
  * g-group
  * o-other

After user you add a + and The permissions you want to grant

## For example

`chmod a+rwx example.txt` This would give everyone that has access to this pc access to our example.txt file

`-` Removes permmisions from stated users 
`chmod o-x example.txt` Would remove the execute permission from other users not in the group or not you

### What about Directories??

Well for Directories the rwx has different meanings

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`r` Able to see contents

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`w` Able to Change contents

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`x` Able to Enter Into Directory



  
