The widely accepted method of making changes to a network interface is to take the interface down using a command such as ifdown eth0, 
make the desired changes to the configuration file, and then bring the interface back up and into service with a command such as ifup eth0.

/etc/hosts	This file contains a table of hostnames to IP addresses. It can be used to supplement a DNS server.
sysadmin@localhost:~$ cat /etc/hosts  
127.0.0.1       localhost

/etc/resolv.conf	This file contains the IP addresses of the name servers the system should consult in any attempt to resolve names to IP addresses. These servers are often DNS servers. It also can contain additional keywords and values that can affect the resolution process.
sysadmin@localhost:~$ cat /etc/resolv.conf  
nameserver 127.0.0.11

/etc/nsswitch.conf	This file can be used to modify where hostname lookups occur. It contains a particular entry that describes in what 
order name resolution sources are consulted.
sysadmin@localhost:~$ cat /etc/nsswitch.conf 

/etc/hosts	This file contains a table of hostnames to IP addresses. It can be used to supplement a DNS server.
sysadmin@localhost:~$ cat /etc/hosts  
127.0.0.1       localhost

/etc/resolv.conf	This file contains the IP addresses of the name servers the system should consult in any attempt to resolve names to 
IP addresses. These servers are often DNS servers. It also can contain additional keywords and values that can affect the resolution process.
sysadmin@localhost:~$ cat /etc/resolv.conf  
nameserver 127.0.0.11

/etc/nsswitch.conf	This file can be used to modify where hostname lookups occur. It contains a particular entry that describes in what 
order name resolution sources are consulted.
sysadmin@localhost:~$ cat /etc/nsswitch.conf 

The ss command is designed to show socket statistics and supports all the major packet and socket types

Netid:	The socket type and transport protocol

State:	Connected or Unconnected, depending on protocol

Recv-Q:	Amount of data queued up for being processed having been received

Send-Q:	Amount of data queued up for being sent to another host

Local Address:	The address and port of the local host’s portion of the connection

Peer Address:	The address and port of the remote host’s portion of the connection


