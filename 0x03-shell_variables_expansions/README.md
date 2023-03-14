#0x03. Shell, init files, variables and expansions
##README.md file that describe what each script is doing.

alias ls='rm *' Command will create an alias with name: ls and value: rm * \n

echo "hello $USER" Command will print hello user, where user is the current Linux user. \n

PATH=$PATH:/action Command adds /action to the PATH. \n

echo $PATH | tr ':' '\n' | wc -l Command will count the number of directories in the PATH. \n

printenv Command lists environment variables. \n


