#0x02. Shell, I/O Redirections and filters
##This README.md file describes what each script is doing.

echo "Hello, World" Command will print "Hello, World" followed by a new line to the standard output. /n

echo "\"(Ôo)'" Command will display a confused similey "(Ôo)'. /n

cat /etc/passwd Command will display the content of the /etc/passwd file. /n

cat /etc/passwd /etc/hosts Command will display the content of the /etc/passwd and /etc/hosts files. /n

tail /etc/passwd Command willl display the last 10 lines of /etc/passwd. /n

head /etc/passwd Command will display the first 10 lines of /etc/passwd. /n

echo "Best School" > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*:\) Command creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School. \n

head -n 3 ./iacta | tail -n 1 Command will display the third line of the file iacta. /n

ls -la > ls_cwd_content Command writes into the file ls_cwd_content the result of the command ls -al. \n

tail -n 1 iacta >> iacta Command will duplicate the last line of the file iacta. \n

find . -type f -name "*.js" -delete Command will delete all the regular files with a .js extension.\n

find . mindepth 1 -type d | wc -l Command will count the number of directories and sub-directories in the current directory. \n 

ls -t | head Command display the 10 newest files in the current directory.\n

sort | uniqu -u Command takesa list of words as input and prints only words that appear exactly once. \n

grep "root" /etc/passwd Command will Display lines containing the pattern “root” from the file /etc/passw. \en

grep "bin" /etc/passwd | wc -l Command will displah the number of lines that contain the pattern "bin" in the file /etc/passwd. \n

grep -A 3 "root" /etc/passwd Command display lines containing the pattern "root" and 3 lines after them in the file /etc/passwd. \n 

grep -v "bin" /etc/passwd Command displays all the lines in the file /etc/passwd . \n

grep '^[[:alpha:]]' etc/ssh/sshd_config Command will display all lines of the file /etc/ssh/sshd_config starting with a letter. \n

tr Ac Ze Command will replace all characters A and c from input to Z and e respectively. \n

tr -d 'cC' Command will removes all letter c and C from input. \n

rev  Command will reverse its input. \n

cut -d":" --fields=1,6 etc/passwd | sort  Command will display all users and their home directories, sorted by users. \n

find . -empty | rev | cut -d '/' -f 1 | rev Command will find all empty files and directories in the current directory and sub-directories. \n

find -type f -name "*.gif" | rev | cut -d "/" -f 1 | cut -d '.' -f 2- | rev | LC_ALL=C sort -f
 Command will list all the files with a .gif extension in the current directory and all its sub-directories

cut -c 1 | paste -s -d '' Command decoded acrostics that use the first letter of each line. \n

tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev |cut -d ' ' -f -1 | rev
  Command will parse web server logs in TSV format as input and displays the 11 hosts or IP addresses which did the most request. \n
