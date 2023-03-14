#0x03. Shell, init files, variables and expansions
##README.md file that describe what each script is doing.

alias ls='rm *' Command will create an alias with name: ls and value: rm * \n

echo "hello $USER" Command will print hello user, where user is the current Linux user. \n

PATH=$PATH:/action Command adds /action to the PATH. \n

echo $PATH | tr ':' '\n' | wc -l Command will count the number of directories in the PATH. \n

printenv Command lists environment variables. \n

set Command list local and environment variables and functions. \n

BEST="School" Command will create a new local variable with name: BEST and value: School. \n

export BEST="School" Command will create a new glocal variable with name: BEST and value: School . \n

echo $((128 + $TRUEKNOWLEDGE)) Command will print the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE. \n

echo $(($POWER/$DIVIDE)) Command will print the result of environment variables POWER divided by DIVIDE

