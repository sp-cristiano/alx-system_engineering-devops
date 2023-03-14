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

echo $(($POWER/$DIVIDE)) Command will print the result of environment variables POWER divided by DIVIDE. \n

echo $(($BREATH**$LOVE)) Command will display the result of BREATH to the power LOVE. \n

echo $((2#$BINARY)) Command will convert a number from base 2 to base 10 where the number in base 2 is stored in the environment variable BINARY

echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo" Command will print all possible compinations of two letters, except oo. \n

printf '%.2f\n' $NUM Command willprint a number with two decimal places. \n

printf '%x\n' $DECIMAL Command converts a number form base 10 to base 16. \n

tr 'A-Za-z' 'N-ZA-Mn-za-m' Command will encode and decode text using the rot13 encryption.

paste -d, - - | cut -d, -f1  Command will print every other line from the input, starting with the first line

printf "%o\n" $((5#$(echo $WATER | tr 'water' '01234') + 5#$(echo $STIR | tr 'stir.' '01234'))) | tr '01234567' 'bestchol' Command will add the two numbers stored in the environment variables WATER and STIR and print the result. \n




