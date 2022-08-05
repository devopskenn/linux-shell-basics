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

Copy the ﬁle from source to destination. -p stands for preservation. It preserves the original attributes of ﬁle while copying like ﬁle owner, timestamp, group, permissions etc.
``` sh
cp -p source_dir destination_dir
```

Copy source directory to speciﬁed destination recursively
``` sh
cp -R source_dir destination_dir
````

In Linux there is no rename command as such. Hence mv moves/renames the ﬁle_1 to ﬁle_2
```sh
mv file1 file2
```

To remove/delete a file. It asks you before every ﬁle removal for conﬁrmation. IF YOU ARE A NEW USER TO LINUX COMMAND LINE, YOU SHOULD ALWAYS USE rm -i. You can specify multiple ﬁles
```sh
rm -i filename
```

To remove the directory dir-name recursively <br>
```sh
rm -R dir-name
```

To remove the directory dir recursively, ignoring non-existent ﬁles and will never prompt for anything. BE CAREFUL USING THIS COMMAND! You can specify multiple directories
```sh
rm -rf dir-name
```

To remove the directory dir-name, if it's empty. This command can only remove empty directories
```sh
rmdir dir-name
```

Create a directory dir-name
```sh
mkdir dir-name
```

Create a directory hierarchy. Create parent directories as needed, if they don't exist. You can specify multiple directories
```sh
mkdir -p dir-name/dir-name
```

Create a ﬁle filename, if it doesn't exist, otherwise change the timestamp of the ﬁle to current time 
```sh
touch filename
```


### Directory Permissions and Groups

Change the ﬁle permissions
```sh
chmod <specification> filename
```
  Speciﬁcations = { <br>
  `u` - user <br>
  `g` - group <br>
  `o` - other <br>
  `+` - add permission <br>
  `-` - remove <br>
  `r` - read <br>
  `w` - write <br>
  `x` - execute. <br>
  }


#### Change the permissions of a directory recursively. 

To change permission of a directory and everything within that directory, use this command
```sh
chmod -R <specification> dirname
```

Add read permission for the owner and the group
```sh
chmod go=+r myfile
```

Allow all users to read, write or execute myfile
```sh
chmod a +rwx myfile
```

Remove read permission from the group and others
```sh
chmod go -r myfile
```

Change ownership of a ﬁle to user owner1
```sh
chown owner1 filename
```

Change primary group ownership of ﬁle filename to group `grp_owner`. Change primary group ownership of directory `dir-name` to group `grp_owner`
```sh
chgrp grp_owner filename
```

To change group ownership of a directory and everything within that directory, use this command
```sh
chgrp -R grp_owner dir-name
```
