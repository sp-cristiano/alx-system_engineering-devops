0x01. Shell, permissions
Description of what each script is doing

su betty Command switches the current user to the user betty.\n
whoami Command prints the effective username of the current user.\n
groups Command prints all the groups the current user is part of. \n
sudo chown betty hello Command changes the owner of the file hello to betty. \n
touch hello Command will create an empty file callled hello. \n
chmod u+x hello Command will add execute permission to the owner of the file hello. \n
chmod +114 hello Command will add execute permission the the owner, and permission to other users to the file
chmod +111 hello Command add execute permission to everybody. \n
chmod 007 hello Command wil set permission for only other ussers to have all permissions. \n
chmod 753 hello Command will set permission of hello to -rwxr-x-wx. \n
chmod --reference olleh hello Command will set the mode of the file hello the same as olleh's mode. \n
chmod -R +111 */  Command will add execute permission to all subdirectories of the current directoryto all user, groups and owner. \n
mkdir -m 751 my_dir Command creates directory called my_dir with permissions 751. \n
chgrp school hello Command will change the group owner to school for the file hello. \n
chown vincent:staff * Command will change the owner to vincent and the group owner to staff. \n
own -h vincent:staff _hello Command changes the owner adn the group owner of _hello to vincent and staff respectively. \n
chown --from=guillaume bettty hello Command changes the owner of the file hello to betty only if it is owned by the user guillaume. \n

