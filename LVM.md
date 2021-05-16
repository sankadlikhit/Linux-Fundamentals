Chapter-3 LVM(Logical Volume Management)

3.1 Introduction.
    - LVM stands for Logical Volume Management. 
    - It is a system of managing logical volumes, or filesystems, that is much more advanced and flexible than the traditional method of partitioning a disk into one or more segments and          formatting that partition with a filesystem.

3.2 Storage structure.
    - 3.2.1 => Linux partition.
  
    - 3.2.2 => Physical volume.
               -  Physical volumes are regular storage devices. LVM writes a header to the device to allocate it for management.
 
    - 3.2.3 => Volume group.
               -   LVM combines physical volumes into storage pools known as volume groups. 
               -   Volume groups abstract the characteristics of the underlying devices and function as a unified logical device with combined storage capacity of the component physical                    volumes. 
 
    - 3.2.4 => Logical volume. 
               -  A volume group can be sliced up into any number of logical volumes. 
               -  Logical volumes are functionally equivalent to partitions on a physical disk, but with much more flexibility. 
               -  Logical volumes are the primary component that users and applications will interact with.


3.3 Basic Command used in LVM.
    - lvcreate -n name -L[size] name => To create a logical volume.
    - lvdisplay => To display the logical volume.
    - vgdisplay => To display volume group.
    - vgcreate vgname[pv] => To create logical group.
    - pvcreate => To create a physical volume.
    - pvdisplay => To display physical volume.

3.4 To create a LVM.
    Step-1 => First set the flag for LVM by following the given steps.
              - flag set 1
                Flag to invert? lvm
                New state [on]/[off]? on
     
    step-2 => Now rum command 'yum install lvm2'.

    step-3 => First we have to Create a physical volume before continuing further.
              - Command to create a physical volume 'pvcreate /dev/vdb1 /dev/vdc1'.

    step-4 => Now suppose you have random number of physical volume, we have to create the volume group with name "serverg" then use following command 'vgcreate serverg /dev/vdb1/dev/vdc1'

    step-5 => Now create Logical Volume for the volume group with LV name serverlv then following command is used,
              - 'lvcreate -n serverlv -L 10G serverg'.

    step-6 => Here -n option is used to indicate a name for the LV, whereas -L assigns a fixed size.

           =>To display the created logical volume we use lvdisplay command.

  

