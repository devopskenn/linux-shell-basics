### Directory Navigation

`pwd` - Get the full path of the current working directory <br>
`cd`  - Navigate to the last directory you were working in <br>
`cd ~` or just `cd` - Navigate to the current user's home directory <br>
`cd ..` - Go to the parent directory of current directory (mind the space between cd and ..)


### Listing Files Inside A Directory

`ls -l` - List the ﬁles and directories in the current directory in long (table) format (It is recommended to use `-l` with ls for better readability) <br>
`ls -ld dir-name` - List information about the directory dir-name instead of its contents <br>
`ls -a` - List all the ﬁles including the hidden ones (File names starting with a . are hidden ﬁles in Linux) <br>
`ls -F` - Appends a symbol at the end of a ﬁle name to indicate its type (* means executable, / means directory, @ means symbolic link, = means socket, | means named pipe, > means door) <br>
`ls -lt` - List the ﬁles sorted by last modiﬁed time with most recently modiﬁed ﬁles showing at the top (remember -l option provides the long format which has better readability) <br>
`ls -lh` - List the ﬁle sizes in human readable format <br>
`ls -lR` - Shows all subdirectories recursively <br>
`tree` - Will generate a tree representation of the ﬁle system starting from the current directory 


### Copy, Paste, and Remove

Will copy the ﬁle from source to destination. -p stands for preservation. It preserves the original attributes of ﬁle while copying like ﬁle owner, timestamp, group, permissions etc <br>
```
cp -p source destination
```

`cp -R source_dir destination_dir` - Will copy source directory to speciﬁed destination recursively <br>
`mv file1 file2` - In Linux there is no rename command as such. Hence mv moves/renames the ﬁle1 to ﬁle2 <br>
`rm -i filename` - Asks you before every ﬁle removal for conﬁrmation. IF YOU ARE A NEW USER TO LINUX COMMAND LINE, YOU SHOULD ALWAYS USE rm -i. You can specify multiple ﬁles <br>
`rm -R dir-name` - Will remove the directory dir-name recursively <br>
`rm -rf dir-name` - Will remove the directory dir recursively, ignoring non-existent ﬁles and will never prompt for anything. BE CAREFUL USING THIS COMMAND! You can specify multiple directories <br>
`rmdir dir-name` - Will remove the directory dir-name, if it's empty. This command can only remove empty directories <br>
`mkdir dir-name` - Create a directory dir-name <br>
`mkdir -p dir-name/dir-name` - Create a directory hierarchy. Create parent directories as needed, if they don't exist. You can specify multiple directories <br>
`touch filename` - Create a ﬁle filename, if it doesn't exist, otherwise change the timestamp of the ﬁle to current time 


### Directory Permissions and Groups

`chmod <specification> filename` - Change the ﬁle permissions <br>
  Speciﬁcations = { <br>
  `u` - user <br>
  `g` - group <br>
  `o` - other <br>
  `+` - add permission <br>
  `-` - remove <br>
  `r` - read <br>
  `w` - write <br>
  `x` - execute. <br>
  } <br>
  
`chmod -R <specification> dirname` - Change the permissions of a directory recursively. To change permission of a directory and everything within that directory, use this command <br>
`chmod go=+r myfile` - Add read permission for the owner and the group <br>
`chmod a +rwx myfile` - Allow all users to read, write or execute myfile <br>
`chmod go -r myfile` - Remove read permission from the group and others <br>
`chown owner1 filename` - Change ownership of a ﬁle to user owner1 <br>
`chgrp grp_owner filename` - Change primary group ownership of ﬁle filename to group `grp_owner`. Change primary group ownership of directory `dir-name` to group `grp_owner` <br>
`chgrp -R grp_owner dir-name` - recursively. To change group ownership of a directory and everything within
that directory, use this command
