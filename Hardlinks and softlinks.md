Chapter-2 Hardlinks and softlinks.

 
2.1 Basic commands

  * ln - command shows links of file.
  
  * ln -li - command shows the inode number.
   
  * df -h - command shows the display information about total space and available space on a file system in a readable format such as Mb,Kb. 


2.2 Hardlinks

  * A hard link is a mirror copy of the original file.
  
  * If you delete the original file, the hard link will still has the data of the original file. Because hard link acts as a mirror copy of the original file.

2.3 Softlinks
  
  * A symbolic or soft link is an actual link to the original file.

  * If you delete the original file, the soft link has no value, because it points to a non-existent file.
