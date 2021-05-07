Chapter-3 Users and groups.

3.1 Introduction.

 * The users are individual users.
 * These users are can read, write and execute the files if they have permissions.

3.1.1 su(switch user).
 
 * su command is used to use system as root user, because you need administrator access to install some or update package and some other stuff too.

3.1.2 sudo.
  
 * Disadvantages of using 'su' command is that admin cannot trace the one who modified or changed the permission recently.
 * so, sudo command give users administrator access or to run some command which requires administrative access.
 
3.2 Groups.

 * group are basically of two types.
   1) Primary groups:-
      -This is default group to which user belongs.

   2) Secoundry groups:- 
      - Once the user is created with primary group it can be added to the other groups.

3.3 Basic commands.

 * su -	To switch user.

 * groupadd - Command is basically used to a user to a group.

 * passwd - Command to assign or to change password of a user.

 * useradd - Command to add a new user.
 
 * groupdel - Command to delete group.

 * iduser - Command to get info about user and there group.
