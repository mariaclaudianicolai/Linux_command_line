# Linux command line

---


## External connection and exchange file
| cmd            | meaning              |
| ------------- |:-------------:|
| ```ssh \<username>@<ipaddress_or_url>```     |Connect from my machine to another | 
| ```scp \<filename> <username>@<ipaddress_or_url>:~/``` or ```scp \<filename> <username>@<ipaddress_or_url>:home/```   | Send file      |  
| ```scp \<username>@<ipaddress_o_url> <filename>``` | Get file |
| ```cp <start_path> <end_path>``` | Copy file/one at time/no folder |
| ```who``` | Show users connected |

## Installation and exe file
| cmd            | meaning              |
| ------------- |:-------------:|
|```sudo apt update ```  | Download packages |
| ```sudo apt upgrade ``` | Install packages |
| ```chmod +x <filename>.sh ``` | Make file executable  |
| ```./<filename>.ch ``` | Execute file |
| ```sudo apt install <filename> ``` | Install package |
| ```sudo apt remove ``` | Remove package |
| ```sudo apt purge ``` | Remove dependences of removed package |
| ```nano <name>.sh``` | Create bash file/ create file and type on the top ```#!/bin/sh```/ make executable

## Basics
| cmd            | meaning              |
| ------------- |:-------------:|
| ```.``` | Current position |
| ```..``` | Parent/in path is that upper |
| ```/``` | Root |
| ```wget <link> ``` | Download from link |
| ```mv <start_path> <end_path> ``` | Rename file |
| ``` cat <filename>``` | Print on screen content of file|
| ```crtl+c ``` | Kill process |
| ```mkdir <folder_name> ``` | Add new folder in current directory |
| ```echo <name> ``` | Print on screen name |
| ```echo $<NAME> ``` | Print on screen environment variable |
| ```rmdir <foldername>``` | Remove empy and existing folder |
| ```rm <filename>``` | Remove file |
| ```rm -r <filename>``` | Remove full folder  |
| ```dir``` | Show file in current directory  |
| ```cd``` | Change directory  |
| ```cd /``` | Go in root  |
| ```cd ..``` | Go to upper level  |
| ```cd -``` | Go to previous level  |
| ```cd /home/claudia/desktop``` | Follow this path  |
| ```ls``` | List local contents |
| ```ls -l``` | List local contents in list format  |
| ```ls -h -a``` | List local contents in human format  |
| ```ls -l -a ``` | List local hidden contents  |
| ```pwd ``` | Print working directory  |
| ```nano <filename> ``` | Open or modify text file   |
| ```grep <name> ``` | Search name   |
| ```clear ``` | Clear console   |
| ```top``` | Show task manager   |
| ```htop``` | Show interactive task manager   |

## Screen
| cmd            | meaning              |
| ------------- |:-------------:|
| ```screen -S <shell_name>```   | Create virtual shell |
| ```screen -r <shell_name> ``` | Restore opened shell |
| ```ctrl+a``` followed by ```ctrl+d``` | Exit from virtual shell/Ensure not to be in main shell |
| ```exit ``` | Exit from virtual shell or connection in ssh |
| ```nano ~/.screenrc``` in nano type ```# Enable mouse scrolling and scroll bar history scrolling termcapinfo xterm* ti@:te@```| Enable scroll for screen |

## Archive
| cmd            | meaning              |
| ------------- |:-------------:|
| ```tar -xzvf <filename.tar.gz> <list_of_file_to_archive>```   | Extract zip archive |
| ```tar -czvf <filename.tar.gz> <list_of_file_to_archive>```   | Create zip archive |
| ```tar -xjvf <filename.tar.bz2> <list_of_file_to_archive>```   | Extract bz2 archive |
| ```tar -cjvf <filename.tar.bz2> <list_of_file_to_archive>```   | Create bz2 archive |
