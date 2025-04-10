The typical format for a command is as follows:
command [options] [arguments]

Scripting: The ability to place commands in a file and then interpret (effectively use Bash to execute the contents of) the file, resulting in all of the commands being executed. This feature also has some programming features, such as conditional statements and the ability to create functions (AKA subroutines).
Aliases: The ability to create short nicknames for longer commands.
Variables: Used to store information for the Bash shell and for the user. These variables can be used to modify how commands and features work as well as provide vital system information.

There are three types of quotes that have special significance to the Bash shell: double quotes ", single quotes ', and back quotes `. Each set of quotes alerts the shell not to treat the text within the quotes in the normal way.
Double quotes stop the shell from interpreting some metacharacters (special characters), including glob characters. 
Single quotes prevent the shell from doing any interpreting of special characters, including globs, variables, command substitution and other metacharacters that have not been discussed yet.
Backquotes, or backticks, are used to specify a command within a command, a process called command substitution.

The semicolon ; character can be used to run multiple commands, one after the other

The double ampersand && acts as a logical "and"; if the first command is successful, then the second command will also run. If the first command fails, then the second command will not run.

The double pipe || is a logical "or". Depending on the result of the first command, the second command will either run or be skipped.


