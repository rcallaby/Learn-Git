# Git - Basic Navigation

- Opening the BASH Terminal
- Navigating through Directories
- Listing Directory Contents
- Creating and Moving Directories
- Creating and Removing Files
- Conclusion

# Introduction:
The BASH terminal is a powerful command-line interface that allows users to navigate through their computer's file system, perform various tasks, and interact with version control systems like Git. Git is a widely-used distributed version control system that provides efficient collaboration and tracking of changes to code repositories. In this article, we will explore how to navigate and utilize basic commands in the BASH terminal to work with Git effectively.

## Opening the BASH Terminal:
To begin, open your preferred terminal application. On most Unix-based systems, you can find the terminal in the "Applications" or "Utilities" folder. Once launched, a command prompt will appear, ready to accept your commands.

## Navigating through Directories:

The pwd stands for Print Working Directory, and prints the path of the working directory.
```commandline
pwd
```
This command does not have any arguments or options.

The cd command (short for "change directory") is fundamental for navigating through the file system. Here are some common cd usage examples:

To move into a directory, use cd <directory> (replace <directory> with the desired directory name). Such as:
```
cd Documents
```
To go back one directory level, type cd .. such as:
```
cd ..
```
To go to your home directory, use cd or cd ~ Such as:
```
cd ~
```
To move to the previous directory, use cd - Such as:
```
cd -
```

## Listing Directory Contents:
The ls command is used to list the contents of a directory. By default, it displays the files and directories in the current directory. Some useful flags to enhance ls functionality:

ls -l displays the contents in a detailed list format.
```
ls -l
```
ls -a shows hidden files and directories.
```
ls -a
```
ls -h provides human-readable file sizes.
```
ls -h
```
ls -R lists directories and their contents recursively.
```
ls -R
```

## Creating and Removing Directories:
You can create directories using the mkdir command followed by the desired directory name:
To create a directory in the current location, use mkdir <directory>. Such as:
```
mkdir thisdirectory
```
To create nested directories, utilize mkdir -p <parent_directory>/<child_directory>.
```
mkdir -p thisdirectory/subdirectory
```
To remove directories, employ the rmdir command:
rmdir <directory> deletes an empty directory.
```
rmdir thisdirectory
```
Moving and Renaming Files and Directories:
The mv command allows you to move and rename files and directories:
To move a file or directory, use mv <source> <destination>. Such as:
```
mv thisdirectory newdirectoryname
```

To rename a file or directory, employ mv <old_name> <new_name>.
```
mv olddirectory newdirectory
```

## Creating and Removing Files:
You can create a new file using touch command.
```commandline
touch new_file_name
```
Or in a directory, like:
```commandline
touch directory/new_file_name
```
Now let's remove a file using rm command.
```commandline
rm file_name
```
To remove directories and their contents recursively
```commandline
rm -r file_name
```
To ignore nonexistent files and arguments, never prompt.
```commandline
rm -f file_name
```
To check what is being done
```commandline
rm -v file_name
```
To remove everything inside a directory.
```commandline
rm *
```
# Conclusion:
The BASH terminal, coupled with Git, offers a robust environment for efficient version control and file management. By familiarizing yourself with basic commands such as mkdir, rmdir, rm, mv, cd, ls, pwd, and Git-specific commands like git init, git add, git commit, git push, and git pull, you can navigate through directories, create and remove directories, move and rename files, delete files, and effectively manage your Git repositories. Practice and exploration will help you become more proficient in using these commands, enabling you to streamline your development workflow.