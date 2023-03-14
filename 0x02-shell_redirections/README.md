#0x02. Shell, I/O Redirections and filters
##This README.md file describes what each script is doing.

echo "Hello, World" Command will print "Hello, World" followed by a new line to the standard output. /n

echo "\"(Ôo)'" Command will display a confused similey "(Ôo)'. /n

cat /etc/passwd Command will display the content of the /etc/passwd file. /n

cat /etc/passwd /etc/hosts Command will display the content of the /etc/passwd and /etc/hosts files. /n

tail /etc/passwd Command willl display the last 10 lines of /etc/passwd. /n

head /etc/passwd Command will display the first 10 lines of /etc/passwd. /n

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

grep -v "bin" /etc/passwd | wc -l Command displays all the lines in the file /etc/passwd
