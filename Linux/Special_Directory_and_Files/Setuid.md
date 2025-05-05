Setuid

When the setuid permission is set on an executable binary file (a program) the binary file is run as the owner of the file, not as the user who executed it.
This permission is set on a handful of system utilities so that they can be run by normal users, but executed with the permissions of root, providing access 
to system files that the normal user doesn't normally have access to.

Special permissions can be set with the chmod command, using either the symbolic and octal methods.

To add the setuid permission symbolically, run:

chmod u+s file

To add the setuid permission numerically, add 4000 to the file's existing permissions (assume the file originally had 775 for its permission in the following example):

chmod 4775 file

To remove the setuid permission symbolically, run:

chmod u-s file

To remove the setuid permission numerically, subtract 4000 from the file's existing permissions:

chmod 0775 file
