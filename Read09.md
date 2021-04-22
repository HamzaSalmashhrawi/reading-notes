# Choosing A Text Editor
#### A text editor is a piece of software that you download and install on your computer, or you access online through your web browser, that allows you to write and manage text, especially the text that you write to build a web site. The text editor has to be one of the most important tools you can use as an aspiring web developer.
#### the most important features are: 
1. code completion;
2. syntax highlighting; 
3. a nice variety of themes (to reduce eye strain and
fatigue); 
4. the ability to choose from a healthy selection of extensions available when you need them

## Visual studio code: 
![VScodeimg](https://www.tmssoftware.com/images/visualstudiocodelogo.png)
#### Visual Studio Code is a free text editor made by the folks at Microsoft. It is available for Windows computers, Mac computers and Linux computers. VS Code has the Emmet shorthand for HTML and CSS already built-in with no additional work from you at all. VS Code has everything: syntax highlighting, themes, extensions and code completion. It seems like VS Code has a very healthy following in the web developing community.

### The Difference Between Text Editors and IDEs
##### A text editor kind of gives away what it does in the title—it edits text. It also manages text, and manages files. I love that name “text wrangler” because in a way that’s what really a text editor does. It wrangles your text together into something meaningful.
##### An IDE (Integrated Development Environment) is really a suite of different software all coming together. An IDE is a text editor, a file manager, a compiler, and a debugger all in one software package.

# The Command Line
#### A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text. 
#### The command line typically presents you with a prompt. As you type, it will be displayed after the prompt. Most of the time you will be issuing commands. Here is an example:

1. user@bash: ls -l /home/ryan
2. total 3
3. drwxr-xr-x  2 ryan users 4096 Mar 23 13:34 bin
4. drwxr-xr-x 18 ryan users 4096 Feb 17 09:12 Documents
5. drwxr-xr-x  2 ryan users 4096 May 05 17:25 public_html
6. user@bash:
* Line 1 presents us with a prompt ( user@bash ). After that we entered a command ( ls ). Typically a command is always the first thing you type. After that we have what are referred to as command line arguments ( -l /home/ryan ). Important to note, these are separated by spaces (there must be a space between the command and the first command line argument also). The first command line argument ( -l ) is also referred to as an option. Options are typically used to modify the behaviour of the command. Options are usually listed before other arguments and typically start with a dash ( - ).
* Lines 2 - 5 are output from running the command. Most commands produce output and it will be listed straight under the issuing of the command. Other commands just perform their task and don't display any information unless there was an error.
* Line 6 presents us with a prompt again. After the command has run and the terminal is ready for you to enter another command the prompt will be displayed. If no prompt is displayed then the command may still be running (you will learn later how to deal with this).
* Your terminal probably won't have line numbers on it. I have just included them here to make it easier to refer to different parts of the material.

## Opening a terminal:
* If you're on a Mac then you'll find the program Terminal under Applications -> Utilities. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.
* If on Linux then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.
* If you are on Windows and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty (free) .

# Basic Navigation

#### pwd which stands for Print Working Directory. (You'll find that a lot of commands in linux are named as an abbreviation of a word or words describing them. This makes it easier to remember them.) The command does just that. It tells you what your current or present working directory is
#### The command for this task is ( ls ) . It's short for list.


* Line 1 - We ran ls in it's most basic form. It listed the contents of our current directory.
* Line 4 - We ran ls with a single command line option ( -l ) which indicates we are going to do a long listing. A long listing has the following:
First character indicates whether it is a normal file ( - ) or directory ( d )
Next 9 characters are permissions for the file or directory (we'll learn more about them in section 6).
The next field is the number of blocks (don't worry too much about this).
The next field is the owner of the file or directory (ryan in this case).
The next field is the group the file or directory belongs to (users in this case).
Following this is the file size.
Next up is the file modification time.
Finally we have the actual name of the file or directory.
Line 10 - We ran ls with a command line argument ( /etc ). When we do this it tells ls not to list our current directory but instead to list that directories contents.
* Line 13 - We ran ls with both a command line option and argument. As such it did a long listing of the directory /etc.
* Lines 12 and 18 just indicate that I have cut out some of the commands normal output for brevities sake. When you run the commands you will see a longer listing of files and directories.
### for more info about navigation back to this link:
[navigation](https://ryanstutorials.net/linuxtutorial/navigation.php)


# About Files
#### everything is actually a file. A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc. To begin with, this won't affect what we do too much but keep it in mind as it helps with understanding the behaviour of Linux as we manage files and directories.
### Quotes
##### The first approach involves using quotes around the entire item. You may use either single or double quotes (later on we will see that there is a subtle difference between the two but for now that difference is not a problem). Anything inside quotes is considered a single item.
1. user@bash: cd 'Holiday Photos'
2. user@bash: pwd
3. /home/ryan/Documents/Holiday Photos

### Escape Characters
##### Another method is to use what is called an escape character, which is a backslash ( \ ). 
##### What the backslash does is escape (or nullify) the special meaning of the next character.
1. user@bash: cd Holiday\ Photos
2. user@bash: pwd
3. /home/ryan/Documents/Holiday Photos

### For more info about files :
[about files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php)