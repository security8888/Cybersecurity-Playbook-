Hello World:

#!/bin/bash

echo "Hello, World!"

Explanation: A basic script that prints “Hello, World!” to the terminal.

Directory Listing

#!/bin/bash

ls -l

Explanation: Lists files and directories in the current directory with details.

System Info

#!/bin/bash

uname -a

Explanation: Prints system information, including the kernel version

File Permissions

#!/bin/bash

file="file.txt"

chmod +x "$file"

Explanation: Grants execute permission to a file.

User Info

#!/bin/bash

username=$(whoami)

echo "Current user: $username"

Explanation: Prints the username of the current user.

Process Kill

#!/bin/bash

process_id=12345

kill -9 "$process_id"

Explanation: Kills a process by its process ID.

Check Internet Connection

#!/bin/bash

ping -c 5 google.com

Explanation: Checks internet connectivity by pinging Google.

System Shutdown

#!/bin/bash

shutdown -h now

Explanation: Shuts down the system immediately.

System Reboot

#!/bin/bash

reboot

Explanation: Reboots the system.

