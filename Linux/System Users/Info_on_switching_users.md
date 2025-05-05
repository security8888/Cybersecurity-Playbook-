The su command allows you to run a shell as a different user. 
While switching to the root user is what the su command is used for most frequently, it can also switch to other users as well.
su [options] [username]
When switching users utilizing the login shell option is recommended, as the login shell fully configures the new shell with the settings of the new user, ensuring any commands executed run correctly. If this option is omitted, the new shell changes the UID but doesn't fully log in the user. The login shell option can be specified one of three ways:
su -
su -l
su --login
By default, if a username is not specified, the su command opens a new shell as the root user. The following two commands are equivalent ways to start a shell as the root user:
su - root
su -

The sudo command allows users to execute commands as another user. Similar to the su command, the root user is assumed by default.
sudo [options] command
prints user and group information for a specified user.

The who command displays a list of users who are currently logged into the system, where they are logged in from, and when they logged in
The who command has several options for displaying system status information. For example, the -b option shows the last time the system started (booted), and the -r option shows the time the system reached the current run level.
The w command provides a more detailed list about the users currently on the system 
The last command reads the entire login history from the /var/log/wtmp
The who command reads from the /var/log/utmp file which logs current users, while the last command reads from the /var/log/wtmp file, which keeps a history of all user logins.
The groupadd command can be executed by the root user to create a new group. The command requires only the name of the group to be created. The -g option can be used to specify a group id for the new group:
The groupmod command can be used to either change the name of a group with the -n option or change the GID for the group with the -g option.
If you decide to delete a group with the groupdel command
Before you begin creating users for your system, you should verify or establish practical values that are used by default with the useradd command
The -D option to the useradd command allows you to view or change some of the default values used by the useradd command. 
The -g option to the useradd command allows you to use a different primary group than the default when creating a new user account.
The -b option to the useradd command allows you to use a different base directory group than the default when creating a new user account.
The -f option to the useradd command allows you to use a different INACTIVE value than the default when creating a new user account.
The -e option to the useradd command allows you to use a different EXPIRE value than the default when creating a new user account.
The -s option to the useradd command allows you to use a different login shell than the default when creating a new user account.
The -k option to the useradd command allows you to use a different SKEL directory than the default when creating a new user account
Adding the -u option to the useradd command allows you to specify the UID number.
To specify a primary group with the useradd command, use the -g option with either the name or GID of the group
There are several ways for a user password to be changed. The user can execute the passwd command, the administrator can execute the passwd command providing the username as an argument, or graphical tools are also available.
The chage command provides many options for managing the password aging information found in the /etc/shadow file.
Here's a summary of the chage options:
Short Option	Long Option	Description
-l	--list	List the account aging information
-d LAST_DAY	--lastday LAST_DAY	Set the date of the last password change to LAST_DAY
-E EXPIRE_DATE	--expiredate EXPIRE_DATE	Set account to expire on EXPIRE_DATE
-h	--help	Show the help for the chage command
-I INACTIVE	--inactive INACTIVE	Set account to permit login for INACTIVE days after password expires
-m MIN_DAYS	--mindays MIN_DAYS	Set the minimum number of days before the password can be changed to MIN_DAYS
-M MAX_DAYS	--maxdays MAX_DAYS	Set the maximum number of days before a password should be changed to MAX_DAYS
-W WARN_DAYS	--warndays WARN_DAYS	Set the number of days before a password expires to start displaying a warning to WARN_DAYS

The usermod command offers many options for modifying an existing user account. Many of these options are also available with the useradd command at the time the account is created. The following chart provides a summary of the usermod options:
Short Option	Long Option	Description
-c	COMMENT	Sets the value of the GECOS or comment field to COMMENT.
-d HOME_DIR	--home HOME_DIR	Sets HOME_DIR as a new home directory for the user.
-e EXPIRE_DATE	--expiredate EXPIRE_DATE	Set account expiration date to EXPIRE_DATE.
-f INACTIVE	--inactive INACTIVE	Set account to permit login for INACTIVE days after password expires.
-g GROUP	--gid GROUP	Set GROUP as the primary group.
-G GROUPS	--groups GROUPS	Set supplementary groups to a list specified in GROUPS.
-a	--append	Append the user's supplemental groups with those specified by the -G option.
-h	--help	Show the help for the usermod command.
-l NEW_LOGIN	--login NEW_LOGIN	Change the user's login name.
-L	--lock	Lock the user account.
-s SHELL	--shell SHELL	Specify the login shell for the account.
-u NEW_UID	--uid NEW_UID	Specify the user's UID to be NEW_UID.
-U	--unlock	Unlock the user account.
The userdel command is used to delete users
