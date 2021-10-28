# Linux command line

---


## External connection and exchange file
| cmd            | job              |
| ------------- |:-------------:|
| ```ssh \<username>@<ipaddress_or_url>```     |Connect from my machine to another | 
| ```scp \<filename> <username>@<ipaddress_or_url>:~/``` or ```scp \<filename> <username>@<ipaddress_or_url>:home/```   | Send file      |  
| ```scp \<username>@<ipaddress_o_url> <filename>``` | Get file |
| ```cp <start_path> <end_path>``` | Copy file/one at time/no folder |

## Installation and exe file
| cmd            | job              |
| ------------- |:-------------:|
|```sudo apt update ```  | Download packages |
| ```sudo apt upgrade ``` | Install packages |
| ```chmod +x <filename>.sh ``` | Make file executable  |
| ```./<filename>.ch ``` | Execute file |
| ```sudo apt install <filename> ``` | Install package |
| ```sudo apt remove ``` | Remove package |
| ```sudo apt purge ``` | Remove dependences of removed package |

## Basics
| cmd            | job              |
| ------------- |:-------------:|
| ```.``` | Current position |
| ```wget <link> ``` | Download from link |
| ```mv <start_path> <end_path> ``` | Rename file |
| ``` cat <filename>``` | Print on screen content of file|
| ```crtl+c ``` | Kill process |
| ```mkdir <folder_name> ``` | Add new folder in current directory |
| ```echo <what_print> ``` | Print on screen |
| ```rmdir <foldername>``` | Remove empy and existing folder |
| ```rm <filename>``` | Remove file |
| ```rm -r <filename>``` | Remove full folder  |
| ```dir``` | Show file in current directory  |
| ```cd``` | Change directory  |
| ```cd /``` | Go in root  |
| ```cd ..``` | Go to upper level  |
| ```cd -``` | Go to previosly level  |

## Screen
| cmd            | job              |
| ------------- |:-------------:|
| ```screen -S <shell_name>```   | Create virtual shell |
| ```screen -r <shell_name> ``` | Restore opened shell |
| ```ctrl+a``` followed by ```ctrl+d``` | Exit from virtual shell/Ensure not to be in main shell |
| ```exit ``` | Exit from virtual shell or connection in ssh |
| ```nano ~/.screenrc``` in nano type ```# Enable mouse scrolling and scroll bar history scrolling termcapinfo xterm* ti@:te@```| Enable scroll for screen |


