File Type:

dash	A regular file, which may be empty, or contain text or binary data

d	A directory file, which contains the names of other files and links to them

l	A symbolic link is a file name that refers (points) to another file.

b	A block file is one that relates to a block hardware device where data is read in blocks of data.

c	A character file is one that relates to a character hardware device where data is read one byte at a time.

p	A pipe file works similar to the pipe symbol, allowing for the output of one process to communicate to another process through the pipe file, where the output of the 
one process is used as input for the other process.

s	A socket file allows two processes to communicate, where both processes are allowed to either send or receive data.

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
