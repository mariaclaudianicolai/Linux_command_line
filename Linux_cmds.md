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
| ```rsync -azP <source> <destination>``` | Sync local and remote directories |

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

## Python
| cmd            | meaning              |
| ------------- |:-------------:|
| ```python3 -m venv </path/to/new/virtual/environment>``` | Create venv |
| ```python3 -m venv venv --system-site-packages```   | Create venv importing existing packages |
| ```python3 install <name> --upgrade```   | Install last version of package |
| ```source venv/bin/activate``` | Activate venv |

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
| ```grep <pattern> <filename> ``` | Print lines that match patterns. Search for patterns in file.   |
| ```clear ``` | Clear console   |
| ```top``` | Show task manager   |
| ```htop``` | Show interactive task manager   |
| ```df -h``` | Check device space   |
| ```du -sh <folder_name>``` | Check folder dimension   |
| ```du -hd 1``` | Check folder size   |

## Modifying file 
| cmd            | meaning              |
| ------------- |:-------------:|
| ```nano <filename>.txt ``` | Create, open or modify text file   |
| ```sort <input_filename>.txt -o <output_filename>.txt``` | Sorting text file   |
| ```sort -r <filename>.txt ``` | Sorting in reverse order    |
| ```sort -n <filename>.txt ``` | Sorting a file numerically   |
| ```sort -nr <filename>.txt ``` | Sorting a file with numeric data in reverse order   |
| ```sort -k <filename>.txt ``` | Sorting a certain column. For example, use “-k 2” to sort on the second column.   |
| ```sort -u <filename>.txt ``` | To sort and remove duplicates. This will write a sorted list to standard output and remove duplicates.  |
| ```uniq -c <filename>.txt ``` | It tells how many times a line was repeated by displaying a number as a prefix with the line.  |
| ```awk '{print $1,$4}' <filename>.txt ``` | Splitting a line into fields: for each record i.e line, the awk command splits the record delimited by whitespace character by default and stores it in the $n variables.|
| ```awk '!seen[$0]++' <filename>``` | To remove duplicates lines in a file.|
| ```head <option> <filename> ``` | Without any option it displays only the first 10 lines of the file. ```-n <num>``` prints first num lines. ```-v``` data preceded by its file name. ```-c`<num>`` Prints the first ‘num’ bytes from the file. |


## Screen
| cmd            | meaning              |
| ------------- |:-------------:|
| ```screen -S <shell_name>```   | Create virtual shell |
| ```screen -L -S <screen_name>```   | Create virtual shell and a file with standard-out |
| ```screen -r <shell_name> ``` | Restore opened shell |
| ```ctrl+a``` followed by ```ctrl+d``` | Exit from virtual shell/Ensure not to be in main shell |
| ```exit ``` | Exit from virtual shell or connection in ssh |
| ```nano ~/.screenrc``` in nano type ```# Enable mouse scrolling and scroll bar history scrolling termcapinfo \\ xterm* ti@:te@```| Enable scroll for screen |
| ```screen -ls```   | To list all of the screen sessions for a user |
| ```screen -D <screen_name_to_detached>```   | To detach the attached screen session that you cannot access |

## Archive
| cmd            | meaning              |
| ------------- |:-------------:|
| ```tar -xzvf <filename.tar.gz> <path_where_to_extract>```   | Extract zip archive |
| ```tar -czvf <filename.tar.gz> <list_of_file_to_archive>```   | Create zip archive |
| ```tar -xjvf <filename.tar.bz2> <list_of_file_to_archive>```   | Extract bz2 archive |
| ```bzip2 -d <filename.bz2> <list_of_file_to_archive>```   | Extract bz2 archive |
| ```tar -cjvf <filename.tar.bz2> <list_of_file_to_archive>```   | Create bz2 archive |
