Permission Groups
The next nine characters demonstrate the permissions of the file.

-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
The permissions set on these files determine the level of access that a user has on the file. When a user runs a program and the program accesses a file, then the permissions are checked to determine whether the user has the correct access rights to the file.

The permissions are grouped into three different roles, representing the different users that may try to access the file.

If you aren't the owner and you're not a member of the file/directory group, then your permissions would be others.

User Owner

-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
Characters 2-4 indicate the permissions for the user that owns the file. If you are the owner of the file, then only the user owner permissions are used to determine access to that file.

Group Owner

-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
Characters 5-7 indicate the permissions for the group that owns the file. If you are not the owner but are a member of the group that owns the file, then only group owner permissions are used to determine access to that file.

Other Permissions

-rw-r--r-- 1 root root 4135 May 27 21:08 /etc/passwd
Characters 8-10 indicate the permissions for others or what is sometimes referred to as the world's permissions. This group includes all users who are not the file owner or a member of the file's group.

The permissions themselves are deceptively simple and have a different meaning depending on whether they are applied to a file or a directory.

Read

The first character of each group represents the read permission. There is an r character if the group has the read permission, or a - character if the group does not.

On a file, this allows processes to read the contents of the file, meaning the contents can be viewed and copied.
On a directory, file names in the directory can be listed, but other details are not available.

Write

The second character of each group represents the write permission. There is a w character if the group has the write permission, or a - character if the group does not.

A file can be written to by the process, so changes to a file can be saved. Note that w permission really requires r permission on the file to work correctly.
On a directory, files can be added to or removed from the directory. Note that w permission requires x permission on the directory to work correctly.

Execute

The third character of each group represents the execute permission. There is an x character if the group has the execute permission, or a - character if the group does not.

A file can be executed or run as a process.
On a directory, the user can use the cd command to "get into" the directory and use the directory in a pathname to access files and, potentially, subdirectories under this directory.
