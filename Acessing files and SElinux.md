Chapter-4 Accessing files

4.1 Introduction 
 * By using 'ls -l' command we can get all the files and subdirectories present in current directory.

 * After using the above-mentioned command the outcome looks like this, 
           dr-xr-x---.  4 root root 4096 Jul 25  2019 .
           dr-xr-xr-x. 18 root root 4096 Jul 25  2019 ..
           -rw-r--r--.  1 root root   18 Dec 29  2013 .bash_logout
           -rw-r--r--.  1 root root  176 Dec 29  2013 .bash_profile
           -rw-r--r--.  1 root root  176 Dec 29  2013 .bashrc
           -rw-r--r--.  1 root root  100 Dec 29  2013 .cshrc
           -rw-r--r--.  1 root root    0 Nov 19  2017 .hushlogin
           -rw-------.  1 root root 2150 Nov 19  2017 original-ks.cfg
           drwxr-----.  3 root root 4096 Jul 25  2019 .pki
           drwxr-xr-x.  2 root root 4096 Nov 19  2017 .ssh
           -rw-r--r--.  1 root root  129 Dec 29  2013 .tcshrc

 * Now, lets divide the info in parts and let me explain about them,
    ' dr-xr-x---.  4 root root 4096 Jul 25  2019 .'
    
   - here 'd' is first character which tells us that its a directory.
  
   - 'r-x/r-x/---' we have divided this into three parts,
        first compartment:- Users permissions.
        secound compartment:- group permissons.
        Last compartment:- Others permissions.

   - Here are permissions 
          * read(r)= 4,

          * write(w)= 2,

          * Execute(x)= 1.

   - In above example User have reand execute permission as others have no permissions.
 
   - The first 'root' represent the user and secound 'root' represents the group.
 
   - There is date which represents the actual date of file creation.

4.2 Basic Commands
 
 * chmod - To modify the permissions of a file.
           (syntax:- chmod 771 Hello.txt) 
           - The number are sum of permissions and file name is one to which these permissions are gonna apply.

 * chown - Command is used to change the user of a file.
           (syntax:- sudo chown user :: admin Hello.txt )
           - Here user is one who is going to be new owner of a file and at end it file name.





Chapter-5 SELinux.

5.1 Introduction. 

 * Security-Enhanced Linux (SELinux) is a security architecture for Linux systems. 

 * This allows administrators to have more control over who can access the system.



5.2 Modes in SELinux.

 * This has basically two modes,
  
    -Disabled - In this SElinux is completely disabled.
  
    -Enable:- This is further divided into two,
            * Permissive - You get warning about the threats, but no action will be taken. 
              
            * Active - The security enforce in enabled in this case. 

5.3 Basic commands.
 
 * sestatus - Helps to get know current status about SElinux.

 * getinforce - Helps to enforce the policy.


5.4 How to change the modes of SELinux.

 * vi /etc/se

 * vi /etc/selinux/config     After this it will enable you to change the mode of SELinux.