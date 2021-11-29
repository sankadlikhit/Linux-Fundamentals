Chapter-2 Linux Partition. 

2.1 Introduction.
 
 - There are mainly two types chips UEFI and BIOS.

 - Both UEFI and BIOS are low-level software that starts when you boot your PC before booting your operating system, but UEFI is a more modern solution, supporting larger hard drives,          faster boot times, more security features, and—conveniently—graphics and mouse cursors.

 - In BIOS, MBR(master boot record) method is used which as MSDOS. 

 - In UEFI, GPT(GUID partition table) method is used.

 
2.2 How to create a partition.

 step-1 =>  First get list of all partition present on system.
            'command parted -l' command is used to list all partitions.

 step-2 => In this step we have to label the partiton.
           - For this step we have to in '/dev/vdb' to enable the GNU interface, then run command mklabel msdos.

 step-3 => Now make the partition.
           - To make a partition use '/dev/vdb' and it enables GNU.
           - After you enable GNU, run command 'mkpart' this helps to make partition and ask you to select type.
           - Now we have to select the size of partititon, usually every linux user select starting point from 2048s and total size can be decided by giving size or by mentioning                         percentage.
           - Use 'quit' command to exit.

 step-4 =>  Now let partition be settle.
           - We use command 'udevadm settle' to settle partititon and it may take sometime. 

 step-5 => Attach the file system to the partition and change file system to XFS file system.
           - To show metadata use command 'mkfs.xfs /dev/vdb1'
           
 step-6 => Mount the partition to a directory.
           - To mmount the partition use command 'mkdir /archive'.

 step-7 => Add entry in fstab.
          - If we didn't add entry in fstab the partition will be deleted after reboot of system.
          - Use command 'Lsblk --fs /dev/vdb'.

 step-8 => Now we have to restart the deamon service 
          - By using command 'systemctl deamon-reload' we can restart the deamon service.

 step-9 => Now check whether partition is mounted to directory or not.
          - use command 'df -h'. 
 
                                             
   
