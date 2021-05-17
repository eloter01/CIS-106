# Homework: 4  The Linux Filesystem

1. **Explain the difference between absolute path and relative path:**

Both the absolute bath and relative path give the address of a given directory. The absolute path, however, begins with the root directory, while the relative path begins with the current directory.

2. **Why Linux uses / instead of \ for its directory paths?**

Linux uses / because it was developed from Unix and that was the convention that was chosen.

3. **In Windows, these files are all the same: File FILE file and FiLE. But in Linux this is not the case, Why?**

This is because the Linux filesystem is case sensitive.

4. **What is the Filesystem Hierarchy Standard (FHS) and who maintains it?**

The FHS is a standard that defines and determines the directory structure of Linux distributions, and it is maintained by the Linux Foundation.

5. **Explain what type of files are stored in the following directories:**

| Directory | What is it used for? |
| --------- | -------------------- |
| /bin    | binary commands for use by system admins, users, and scripts |
| /dev    | device files, like audio drivers |
| /etc    | local and static configuration files, also unshareable |
| /home   | directories and personal files of all users on the system |
| /lib    | shared libraries that load on system start |    
| /opt    | static shareable add-on software packages |
| /tmp    | temporary files to be deleted by the system admin on startup |
| /var    | variable data files written by the system | 
| /proc   | provides information about the system hardware and processes running |
| /usr    | user binaries, documentations, header files for windowing system |

6. **How does a period at the beginning of a file name means (example .bashrc)?**

A period indicates that the files is a hidden file, and keeps it from showing in most common file managers and shell programs.

7. **Which command would you use to list all the files inside the /usr/share/ directory?**

sudo ls -l /usr/share/

8. **If you are working in the /usr/share/icons directory and want to move to your home directory, which command would you use?**

cd ~

9. **Explain what these commands do:**

* cd .config/.htop 

Takes you to the relative path through .config, a hidden folder, into .htop, another hidden folder.

* cd ../

Takes you up one directory. This is also a relative path.

* ls -lX

Long lists all files in current directory with the option of sorting alphabetically by entry extension.

10. **John has a lot of files in the directory /var/www/html/webapp. He wants to long list all the files, including hidden files, by modification time (newest first), and with human-readable file sizes. Which command should he use conjuring that his current working directory is:** 

'/home/john/.git/'

ls -athl /home/john/.git/ 