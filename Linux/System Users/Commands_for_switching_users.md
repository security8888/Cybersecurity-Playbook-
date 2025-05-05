|      Commands             |           What the Command Does                            |                            Flags                           |
|---------------------------|------------------------------------------------------------|------------------------------------------------------------|
|       su                  |        Allows you to switch users in shell                 |                          -                                 |
|                           |                                                            |                          -l                                |
|                           |                                                            |                          --login                           |
|       sudo                | Allows users to execute commands as another user           |                                                            |
|       who                 | Displays list of users who are currently logged in, where  |               -b (shows the last time system booted        |                    
|                           | they are logged in from and when they logged in            |-r (shows the time the system reached the current run level |
|       w                   | Shows a more detailed list on the users currently on the   |                                                            |
|                           | system                                                     |                                                            |
|       last                | Reads the entire login history from the /var/log/wtmp      |                                                            |
|      groupadd             |    Executed by the root user to create a new group         |               -g (specify group ID for new group)          |
|      groupmod             |    Make changes to groups                                  |               -n (change the name of group)                |
|                           |                                                            |               -g (change GID of group)                     |
|      groupdel             |    Delete a group                                          |                                                            |
|      useradd              | Before you begin creating users for your system you should |-D (allows you to view or change some of the default values)|
|                           | verify or establish practical values that are used by      |-g (allows you to use different primary group than default) |
|                           | default.                                                   |-b (allows you to use a different base directory group)     |
|                           |                                                            |-f (allows you to use a different INACTIVE value)           |
|                           |                                                            |-e (allows you to use a different EXPIRE value )            |
|                           |                                                            |-s (allows you to use a different login shell)              |
|                           |                                                            |-k (allows you to use a different SKEL directory)           |
|                           |                                                            |-u (allows you to specify the UID number)                   |
|                           |                                                            |-g (To specify a primary group w/ name or GID of the group) |
|      passwd               |  Change user password                                      |(user changes and admin changes giving user name as arguem.)|
|      change               |  Change password info in /etc/shadow file                  |(several options to change password aging information)      |
|      usermod              |  Offers many options for modifying an existing user        |(many can be changed when creating a new user account)      |
|      userdel              |  Delete users                                              |                                                            |
