
## Symbolic link: A symbolic link allows you to access large data or documents from another (new) directory without copying the data to the new directory.
This is important as it allows the use of minimum space for large data/documents. For example to create a symbolic link for "veps" located in "Data" directory,
so that it can be accessed from the directory "Tutorial", do the following:
- Move to directory Tutorial/
$ cd /home/tenghe/Tutorial
- Type the following:
$ ln -s /home/tenghe/Data/veps ./
- This creates a link of veps/ in Tutorial, i.e., /home/tenghe/Tutorial/veps@
From here on, all data in veps/ is accessible in Tutorial/, and all changes made in veps@ will appear in veps/
