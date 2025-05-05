For every file created, there is a block of data on the file system that stores the metadata of the file. 
Metadata includes information about the file like the permissions, ownership, and timestamps.
Metadata does not include the file name or the contents of the file, but it does include just about all other information about the file.

This metadata is called the file's inode table.
The inode table also includes pointers to the other blocks on the file system called data blocks where the data is stored.
Every file on a partition has a unique identification number called an inode number.

