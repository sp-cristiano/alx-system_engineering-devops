0x00. Shell, basics describing what each scripts is doing\n
pwd Command prints the absolute path name of the current working directory.\n
ls Command displays the contents of your current directory.\n
cd ~ Command changes the working directory to the user's home directory.\n
ls -l  Command displays the current directory contents in a long format.\n
ls -al  Command to display current directory contents, including hidden files using the long format.\n
ls -lan Command to display current directory contents in long format showing hidden files and with user and group ids numerically\n
mkdiir /tmp/my_first_directory  Command will create a director named my_first_directory in the /tmp/ directory.\n
mv /tmp/betty /tmp/my_first_directory Command will move the file betty form /tmp/ to /tmp/my_first_directory.\n
rm /tmp/my_first_directory/betty Command will remove the file betty from  /tmp/my_first_directory.\n
rm -r /tmp/my_first_directory Command will delete the directory my_first_directory from the /tmp/ directory.\n
cd - Command will change the working directory to the previous one.\n
ls -al . .. /boot Command will list all files including hidden files in the current, parent of the current  and /boot directory in long format.\n
file /tmp/iamafile Command will print the type of the file named iamafile \n

ln -s /bin/ls __ls__ Command will create a symbolic link to /bin/ls with name __ls__
cp -un *.html ..   Command will copy all html files from current directory to the parent directory and also update files if the current file is more recent than the former
mv [[:upper:]]* /tmp/u Command will move all files begining with an uppercase letter to directory /tmp/u
