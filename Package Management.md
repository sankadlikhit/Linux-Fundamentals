Chapter-1 Package Management.

1.1 Introduction -

  - A package delivers and maintains new software for Linux-based computers. 
  - Just as Windows-based computers rely on executable installers, the Linux ecosystem depends on packages that are administered through software repositories. 
  - These files govern the addition, maintenance, and removal of programs on the computer.

1.2 TYPES OF PACKAGE MANAGEMENT SYSTEMS -

  -  Debian and derivatives ->   apt-get / aptitude.
  -  CentOS ->   yum.
  -  openSUSE ->   zypper.
  -  Arch Linux ->  Pacman. 

1.3 COMMANDS FOR PACKAGE MANAGEMENT -

  - So we use 'yum' as we are having CentOS.

 
1.4 COMMANDS FOR PACKAGE MANAGEMENT. 

  - 'yum install httpd' -> here 'httpd' is package name and 'yum install' help to install      the package.
 
  - 'yum info httpd' -> This command basically provide information of package.

  - So here the is the output of command 'yum info httpd' 

		Installed Packages
 		Name        : httpd
 		Arch        : x86_64
 		Version     : 2.4.6
 		Release     : 97.el7.centos
 		Size        : 9.4 M
 		Repo        : installed
 		From repo   : updates
 		Summary     : Apache HTTP Server
 		URL         : http://httpd.apache.org/
 		License     : ASL 2.0
 		Description : The Apache HTTP Server is a powerful, efficient, and extensible web server.

  - 'yum history' -> This command help display the hisory of the recent activity.

  - 'yum repolists' -> This command helps to list down the repositories.

  - 'yum search keyword' ->  This command helps to searches package metadata for given keyword.

1.5 RPM.

 - RPM is package management tool for Red Hat-based distribution.

 - It can also perform package management operations like install,verify,earase,uninstall    but it cannot resolve dependency like the package management tool YUM. 

1.6 YUM REPOSITORY.

 - It is basically used for installing, querying, deleting and managing Red Hat Enterprise Linux RPM software packages from official Red Hat Software repositories as well as other    repositories.



 