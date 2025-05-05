The su command allows you to run a shell as a different user. While switching to the root user is what the su command is used for most frequently, it can also switch to other users as well.
su [options] [username]

When switching users utilizing the login shell option is recommended, as the login shell fully configures the new shell with the settings of the new user, ensuring any commands executed run correctly. If this option is omitted, the new shell changes the UID but doesn't fully log in the user. 
The login shell option can be specified one of three ways:
su 
su -l
su --login

By default, if a username is not specified, the su command opens a new shell as the root user. The following two commands are equivalent ways to start a shell as the root user:
su - root
su -
