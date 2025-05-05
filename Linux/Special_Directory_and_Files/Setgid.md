Setgid

The setgid permission is similar to setuid, but it makes use of the group owner permissions.
There are two forms of setgid permissions: setgid on a file and setgid on a directory.
The behavior of setgid depends on whether it is set on a file or directory.

When set on a directory, the setgid permission causes files created in the directory to be owned by the group that owns the directory automatically.

In a long listing, the setgid permission is represented by an s in the group execute position. A lowercase s means that both setgid and group execute permissions are set.
An uppercase S means that only setgid and not group execute permission is set.
If you see an uppercase S in the group execute position of the permissions, then it indicates that although the setgid permission is set, it is not really in effect because
the group lacks the execute permission to use it.

Use the following syntax to add the setgid permission symbolically:

chmod g+s <file|directory>

To add the setgid permission numerically, add 2000 to the file's existing permissions:

chmod 2775 <file|directory>

To remove the setgid permission symbolically, run:

chmod g-s <file|directory>

To remove the setgid permission numerically, subtract 2000 from the file's existing permissions:

chmod 0775 <file|directory>
