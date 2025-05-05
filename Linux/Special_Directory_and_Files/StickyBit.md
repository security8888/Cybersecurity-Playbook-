Sticky Bit

The sticky bit permission is used to prevent other users from deleting files that they do not own in a shared directory.




 write permission on the directory 
so that users can still add and delete files in the directory, but files can only be deleted by the owner of the file or the root user.

A lowercase t means that both the sticky bit and execute permissions are set for others. 
An uppercase T means that only the sticky bit permission is set.

While the capital S indicated a problem with the setuid or setgid permissions, a capital T does not necessarily indicate a problem, 
as long as the group owner still has the execute permission.

To set the sticky bit permission symbolically, execute a command like the following:

chmod o+t <directory>

To set the sticky bit permission numerically, add 1000 to the directory's existing permissions 

chmod 1775 <file|directory>

To remove the sticky permission symbolically, run:

chmod o-t <directory>

‌⁠​​⁠​To remove the sticky bit permission numerically, subtract 1000 from the directory's existing permissions:

chmod 0775 <directory>


