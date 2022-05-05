# Lab 0: Terminal and Git Usage

## Objectives

<ol>
  <li>Learn basic terminal commands and how to work with a text editor</li>
  <li>Learn to run a Python program from the command-line</li>
</li>

## Terminal

On your computer, you probably navigate your hard drive by double clicking on icons. While convenient for simple tasks, this approach is limited. For example, imagine that you want to delete all of the music files over 5 MB that you haven’t listened to in over a year. This task is very hard to do with the standard double-click interface but is relatively simple using the terminal.

On the your iMacs, click the Spotlight button (at the top bar, on the right) and type “terminal” in the input box. Click the “terminal” icon to open the terminal window.

A terminal window will open and you will see text of the form:
```
username@computer: ~ %
```
where `username` has been replaced by your AU username and `computer` is the name of the computer you happen to be using. This string is called the prompt. When you start typing, the characters you type will appear to the right of the `%`.

The program that runs within a terminal window and processes the commands the you type is called a <i>shell</i>. We use `zsh` as you can see on the top of your terminal window. This is the current default shell on the latest macOS.

## Navigating the File System

Files in macOS are stored in directories/folders, just like in Linux/Windows. Directories can hold files or other subdirectories and there are special directories for your personal files, your Desktop, etc.:
| Name | Mac | Linux | Windows |
| --- | --- | --- | --- |
| Root directory | / | / | C:\ |
| Home directory | /Users/username | /home/username| C:\Documents and Settings\username |

![filesystem username](https://user-images.githubusercontent.com/52186621/166872720-fea6c655-0059-48bd-954f-7cbec43596f6.svg)
The figure above illustrates how Linux organizes the file system. Your own computer might have a slightly different organization (e.g., you might replace / with C:), but the idea is the same.

For the above and from this point forward, consider that the text “username” is replaced with your own actual username, which is just your AU username.

## Show Files

The terminal will start in your home directory, `/Users/username/`, which is a special directory assigned to your user account. Two very useful commands are `pwd` and `ls`:

|   |   |
| --- | --- |
|`pwd`| Prints your current working directory - tells you where you are in your directory tree. |
|`ls`| Lists all of the files in the current directory. |

The following is an example using these two commands in a terminal window:
```
username@computer: ~ % pwd
/Users/username
username@computer: ~ % ls
Desktop  Documents  Downloads  Music  Pictures  Public  Library  Movies
username@computer: ~ %
```
Try these commands yourself to verify that everything looks similar.

Notice that the directory path and list of files that you see if you open your home folder graphically are identical to those provided by `pwd` and `ls`, respectively. The only difference is how you get the information, how the information is displayed, and how easy it is to write a script that, say, processes all the Python files in a directory.
