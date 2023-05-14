# Prep: Practice in the Terminal

## The Command Line:

- This basically explains the dfference between the command line terminal and a GUI (Graphic User Interface).
- This section is basically just an introduction to how to get to the terminal, how to check if you're running bash, and a quick tip about navigating recent history of commands entered previously.

## Basic Navigation:

- pwd = print working directory

- ls = list, this alone will list out the contents of the current directory. 
- -l = long list, this will contain the following:
> First character indicates whether it is a normal file ( - ) or directory ( d )

> Next 9 characters are permissions for the file or directory.

> The next field is the number of blocks (don't worry too much about this).

> The next field is the owner of the file or directory (ryan in this case).

> The next field is the group the file or directory belongs to (users in this case).

> Following this is the file size.

> Next up is the file modification time.

> Finally we have the actual name of the file or directory.

- /etc = this tells 'ls' to not list the current directory, rather it's contents.

- paths = there are two different types of paths, absolute and relative. Absolute paths begin with the root (the highest directory in the order) and continue by traveling into files or directories using the forward slash (/). 
    > Relative paths specify a location in relation to where we are in the system.

- ~ (tilde) = this just creates a shortcut to refer to the directory without having to type out the path.

- . (dot) = this is a reference to the current directory. 

- .. (dotDot) = this is a reference to the parent directory, it can be used to navigate out of the current directory by walking back on the path. 

- cd = change directory, if ran with no arguments it will take you back to the home directory. 

- tab completion = using the tab button invokes an auto complete action. If you type out the first few characters of a path and hit tab, it will fill the rest in for you. If tab is pressed again it will cycle through possiblities. 

## More About Files:

- Everything is a file, even directories.

- Linux is an extentionless system, it will figure out what kind of file type it is.

- file = obtain information about what type of file a file or directory is.

- Linux is case sensitive.

- Spaces create seperate items. However, if you use quotes it will regard it as a single item. A \ (backslash) will create a single item by nullifing the space.

- ls -a = this command will allow hidden files to be shown.

- . (dot, or full stop) = this makes it so that a file is hidden, by adding a . it will hide a file, to remove . from a file name will make a file un-hidden.

## Manual Pages:

> The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept.

- To exit out of the 'man' command/page press 'q' for quit. 

- man -k <search term> = this is a keyword search of the manual.

- /<term> = Within a manual page, perform a search for 'term'

- n = After performing a search within a manual page, select the next found item.

> If you want to search within a manual page this is also possible. To do this, whilst you are in the particular manual page you would like to search press forward slash '/' followed by the term you would like to search for and hit 'enter' If the term appears multiple times you may cycle through them by pressing the 'n' button for next.

- There are long hand and short hand commands, represented by - for short and -- for long.

## File Manipulation:

- mkdir = make directory

- mkdir -p = tells Linux to create parent directories as needed.

- mkdir -v = makes the 'mkdir' tell us what it is doing in regards to creating the directories and shows the paths. 

- rmdir = remove directory. ** There is NO undo! -p and -v work similiarly for rmdir. Also, a directory must be empty before removal.

- touch = creates a file, if there is a file referred to that does not exist, this will create it. 

- cp (source) (destination) = this copies a file. 
> Note that both the source and destination are paths. This means we may refer to them using both absolute and relative paths. 

> When we use cp the destination can be a path to either a file or directory. If it is to a file ... then it will create a copy of the source but name the copy the filename specified in destination. If we provide a directory as the destination then it will copy the file into that directory and the copy will have the same name as the source.

- -r = this is an option, which stands for recursive, that will copy directories, so if you are needing to copy many files within a directory this will include all. 

- mv (source)(destination) = move. 

- Within this command there is also an option to rename the file by providing an alternative title. 

- rm = remove, when used with the -r option it can be used to remove recersive files, or otherwise put, it can remove directories and anything contained therein. The -r option can also be used with i which stands for interactive **Pro-gamer move, because, again, there is NO un-do.

## Cheat Sheet:
[Here is a link to Ryan's Linux Tutorial Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)



