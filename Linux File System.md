Chapter-1

1.1 Linux File System.

 
 * Linux file system is generally a built-in layer of a Linux operating system used to handle the data management of the storage.  

 * It helps to arrange the file on the disk storage. It manages the file name, file size, creation date, and much more information about a file.

1.2 Basic commands.

   * ls - command basically used to list all the files and folders present in Directory.
  
   * pwd - command used to know users current working Directory.

   * cd - command used to change Directory.

   * mv - command used to move files and also used to rename them.

   * cp - command used to cpoy files.
         (-r is used to copy files recursively)

   * cat - command used to dislpay content of a file.
          (syntax:- cat filename)

   * touch - command to create a new file.
           (synatax:- touch filename.extension)

   * echo - command used to display text on terminal.
           (syntax:- echo "Hello world")
           (echo "Hello world" >> file.txt :- used to insert the text in a particular file)

   * mkdir - command used to create a new directory.

   * rmdir - command used to remove or delete a directory(empty).

   * rm - command to remove a file.
         (-r:- to remove a non-empty directory)

   * whoami - command used to identify the current user.
 
   * ping - command used to check whether the network is reachable.
  
   * vi - command to enter into a text editor on a terminal.
         (syntax:- vi filename.txt)

   * head - command used to view top most file  instead of all files from a directory.
    
   * tail - command used to view bottom most file instead of all files from a directory.
           // head and tail command can be used to with '- number of lines you need to view eg:- head -5'//

   * uname - command helps to get name of linux currently running. 


1.3 Directories and types.

   Now, here are some pre-existed directories:-
  
   * ./boot - This directory basically contain boot files which are required for starting device.
   * ./temp - This directory stores temp files.
   * ./var -  This directory stores files which change regularly.
   * ./lib -  This directory has all the libraries and provide libraries for commands
   * ./etc -  This directory stores storage system configuration files, executables required to boot the system, and some log files.
   * ./root - This directory is starting point where all branches originate from and also known as administrator's home.
   * ./dev -  This directory  is the location of special or device files.
   * ./media - This directory basically contain subdirectories where removable media devices connected to device are mounted.



