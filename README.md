###Linux Commands

1. `ls` - lists Down everything present in the current directory/folder.
   - **-a** is used to list all the hidden files.
   - **-l** shows details about the folder like permissions, etc.
   - **-r** shows all the folder and files inside the folder (recursive).
2. `cd` - helps in changing the directory.
   - **cd ..** helps in moving one folder out.
   - **cd** moves you to the root folder.
   - **cd `folder_name`** moves to that folder (`folder_name` can be relative or absolute)
3. `mkdir` - helps creating a new folder.
   - **-p** can be used to create folders inside child folder.
4. `where` - helps in locating the location of the command
5. `open` - helps to open the folder in the explorer.
6. `echo` - help in printing on terminal.
7. `Environment variables` - are used to store location of the file associated with a key. It can be accessed using _$PATH_.
8. `.bashrc` - it is a file which is run automatically when the terminal starts.
9. `cat` - it displays the content of the file on the terminal.
10. `>` - will create a file if doesn't exist with the name provides and will wait to write content inside the file.
    Ex. `cat > abc` will create a file id doesn't exist abc and will wait till `^C` and write everything written inside the terminal (only one line) into the file. - **space** we can combine 2 or more files by separating them with ` ` and `>` to put the content of the combined files into.
11. `vim` - is used to edit files.
    - **:q** quit the vim.
    - **:q!** quit the vim without saving.
    - **:wq** write and quit the vim.
12. `pwd` - shows the current directory.
13. `man` - help to know about any command.
14. `tr` - helps to translate text.
15. `|` - is used to separate 2 commands such that output of first command acts as input for te second command.
16. `\` - helps in writing new command instead of running it.
17. `touch` - is used to create file.
18. `cp` - is used to create copy of the file.
    - **-R** copies all the subdirectories and files even after error is occurred.
19. `mv` - is used to move file from one location to another.
20. `rm` - is used to delete the file permanently.
    - **-rf** is used to delete forcefully.
    - **-R** is used to delete folders and subfolder.
21. `sudo` - is used to run administrative commands.
22. `df` - is used to check the systems disk usage in KB.
    - **-m** is used to display in MB.
    - **-g** is used to display in GB.
    - **-h** is used to display in human readable format.
23. `du` - is used to check the file and folder size of the current directory in KB.
    - **-m** is used to display in MB.
    - **-g** is used to display in GB.
    - **-h** is used to display in human readable format.
24. `head` - is used to display first 10 lines of any file.
    - **-n** is used o customize the number of lines displayed.
25. `tail` - is used to display last 10 lines of any file.
    - **-n** is used o customize the number of lines displayed.
26. `diff` - compares the 2 files line by line and output the lines which doesn't match.
27. `locate` - is used to locate any file that matches the regex passed.
28. `find` - is used to find everything inside the location passed.
    - **-type** is used to sort whether to display file of folder or type of the files.
    - **-name** is used to search for the name of file or folder(case sensitive).
    - **-iname** is used to search for the name of file or folder(case insensitive).
    - **-mmin +/-`i`** is used to find files that are modifies i minutes ago. If `+` modified later than i minutes and `-` modified before i minutes.
    - **-mtime +/-`i`** is used to find files that are modifies i days ago. If `+` modified later than i days and `-` modified before i days.
    - **-maxdepth** only search up to passed depth
    - **-size +/- `i`** is used to find files or folder with size grater than or less than i.
    - **-empty** is used to find files or folders that are empty.
    - **-perm** find the files with the passed permissions.
29. `chmod` - is used to change the permissions of a file.
    - **-rwe-rwe-rwe** is used the assign read, write and execute permission to root, user and others.
    - **777** is used the assign permission using octal numbers.
30. `whomi` - is used the check the user logged in.
31. `chown` - is used to change the owner of a file.
32. `-exec` - is used to execute a command after some other command.
    Ex. `find . -type f -name "*.txt" -exec rm -rf [] +`
    this command will first find all the files and then execute the command `rm -rf` on each file. `[]` is a placeholder for the output that will be generated by the `find` command.
33. `grap` - is used to search for the keyword inside the files (case sensitive).
    - **-w** is used to search for the complete word.
    - **-i** is case insensitive.
    - **-n** displays the line number of the occurrence.
    - **-B `i`** it shows the i number of lines before the match.
    - **-l** shows the location of the file match occurred.
    - **-c** counts the match of the word in the file.
34. `history` - is used to list the history of the commands used.
    **Note-** use can use `|` with history like this. `history | grap "ls"`.
35. `!` - is used to run command from history.
36. `clear` - is used to clear the screen.
37. `;` - is used to run multiple commands separated by `;`.
38. `sort` - sorts the content.
    - **-r** is used to sort in reverse order.
39. `job` - is used to display the ongoing jobs.
40. `ping` - is used to check the networking status of you system.
41. `wget` - is used to download files from internet.
42. `obs` - is used to check the processes running.
43. `kill` - is used to kill a process with the ID passed.
44. `zip` - is used to zip files.
45. `unzip` - is used to unzip files.
46. `hostname` - is used to get the hostname.
    - **-i** returns the IP address of the system.
47. `useradd` - is used to add a new user.
48. `passwd` - is used to set the password for that user.
49. `userdel` - is used to delete a user.
50. `uname` - is used to get the information about the Kernel.
    - **-o** type of the kernel
    - **-a** architecture of the kernel
    - **-r** version of the kernel
51. `lscpu` - give all the CPU details.
52. `free` - check the free memory.
53. `vmstat` - displays stats about virtual memory.
54. `id` - get the ID of the current user.
    - **-g** get the group ID
55. `getent` - get information about user, group, etc.
56. `lsof` - list all the open files.
57. `nslookup` - displays the information about the URL or the IP passed.
58. `netstat` - displays information about ports of the system active.
59. `sed` - is used to deal with logs.
60. `ipconfig` - displays the systems IP address.
61. `cut` - select a portion of a line.
62. `ssh` - used to login into remote machines.
63. `htop` - used to display the process that are consuming the resources.
64. `ps aux` - display information about the processes.
65. `&` - creates a child process which runs in the background.
66. `&&` - runs the second command only after completion of the first.
67. `||` - runs the second command only after failure of the first.
68. `!` - used to do tasks over all the files except the files passed in the `!`.
69. `>>` - used to append the content and `>` is used to replace the content.
70. `{}` - used to group commands.
