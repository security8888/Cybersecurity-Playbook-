The numeric method (also called the octal method) is useful when changing many permissions on a file. It is based on the octal numbering system in which each permission type is assigned a numeric value:

4	Read

2	Write

1	Execute

By using a combination of numbers from 0 to 7, any possible combination of read, write and execute permissions can be specified for a single permission group set. For example:

7	rwx

6	rw-

5	r-x

4	r--

3	-wx

2	-w-

1	--x
0	---
