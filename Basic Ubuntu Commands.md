# Basic Ubuntu Commands

This is a list of the most basic but extremely useful commands. Learning these will help you have a strong foundation to add more sophisticated commands upon.

## Sudo

(Superuser DO) This is the same as "Run as administor"

```
sudo
```

## apt-get

This command is used to install, update, upgrade, and remove any package. Examples below will show how to use in different ways:

- **sudo apt-get update**

  superuser privileges. This command updates your system along with the packages that are installed.

  ```
  sudo apt-get update
  ```

- **sudo apt-get upgrade**

  You will run this command after you ran

  ```
  sudo apt-get upgrade
  ```

  This will upgrade the packages that have available updates. You can also upgrade just one package by adding a space along with the package name after upgrade.

  ```
  sudo apt-get upgrade node.js
  ```

- **sudo apt-get install _package name you wish to install_**
  You would replace the package-name with the name of the program you wish to install.

  ```
  sudo apt-get install curl
  ```

## ls

(list) command will list out the files in the current working directory you are in.

```
ls
```

You can also look at different files in other directories by adding a space then the direct path to the other directory you wish to look into.

```
ls /home/User/Dev
```

We can also see hidden files by using the -a

```
ls -a
```

This command will list all the files in that directory including hidden files.

## cd

(change directory) used to change the current working directory. You use it by typing cd space then the file name within your current directory or full path to another directory and/or file if in a different directory. Examples of different ways below:

```
cd
```

- Takes you to the root directory.

```
cd ..
```

- Takes you up on directory level.

```
cd -
```

- Takes you to the previous directory.

Examples:

```
cd /home/User/Dev
```

- This will take me to the directory Dev.

```
cd /home/User/Dev/JS\ Practice
```

- This will take me to the JS Practice. **Note I used backslash+space. This does the same as**

```
cd /home/User/Dev/"JS Practice"
```

- I used "" instead of the backslash+space.

## pwd

(print working directory) This will display the full pathname of the working directory.

Using the last example above -

```
pwd
```

Returns:

```
/home/User/Dev"JS Practice"
```

## cp

(copy) - After typing cp you type the file you want to copy + space + location you want to place the copied file.

```
cp "app.js" /home/User/Dev/JS
```

## mv

(move) A lot like cp (copy) but instead of copying the file you will move it from one directory to another directory. Just like cp (copy) after typing mv + space + the file you want to move + location to move it too. Example below:

```
mv pyproject.py /home/User/Dev/Python_Project
```

- This will move the pyproject.py file in my current directory to the Python_Project directory. You can also move directories using this command.

## rm

(remove) This command will remove the specified file but not the directory.

```
rm myApp.js
```

Here are some other uses of the rm command:

- **rmdir**

  (remove directory) - Removes an empty directory

  ```
  rmdir /home/User/Dev/My_Empty_Dir
  ```

- **rm -r**

  (remove recursively) - Removes a directory along with its content. This will remove a non-empty directory

  ```
  rm -r /home/User/Dev/No_Longer_Needed_Practice_File
  ```

- **rm -f**

(remove force)
This will forcefully remove files.  
But to forcefully remove non-empty dirctories use:

```
rm -rf <fileName>
```

- **rm -i**

Using this will make rm prompt you before every removal.

```
rm -i <fileName>
```

## mkdir

(make directory) This command will allow you to create a new directory. You can also specify where you want to create this directory's location by putting a space followed by the location behind mkdir. Example:

```
mkdir Basic_Terminal /home/User/Learn
```

Or if I wish to make a new directory in the current directory I would do:

```
mkdir Learn_Terminal_Basic
```

## locate

Use this command to find files and their location by their name. If you are not sure if the file name is upper case or lower case use -i to ignore the case.
If you wish to locate two or more words at a time you can seprate each word with (\*). Example below:

```
locate -i *hello*Practice
```

If you just want to have a count of the times the word is in the directories you can use -c. Example:

```
locate -c Python
```

This would return a number of how many times the word Python is in the directories.

or you could do this:

```
locate -ic Python
```

This will ignore the case and return a count for how many times Python and/or python is in the directories.

## echo

This command helps us move data into text files. Example:

```
echo I'm learning how to use the terminal in Ubuntu.>>basic_terminal.txt
```

We did not have to use backslashs or wrap the sentence in "" because we used two >>(greater than) symbols before the file name.

## history

This command will display all of your previous commands **up to the history memory limit.**

```
history
```

## df

(display filesystem) This will display information about your disk space usage of your filesystem.

```
df
```

## free

This command displays the amount of free space available on the system.

```
free
```

## top

This will display the processes using the most resources. You can exit out by typing q

```
top
```

## cat

Displays the contents of a file.

```
cat /home/User/Dev/Practice_Python/basic.py
```

or to cat in your current directory

```
cat basic.py
```

## man

(manual) This command will give you a description of any command that come after the command man. Example:

```
man install
```

## info

(information) This command is a lot like man but the different is that info goes into more information about the command. Example:

```
info apt-get
```

## rename file or directory

Ubuntu 18.04 does not have the command rename installed but can be installed using:

```
sudo install rename
```

But the Ubuntu community recommands using mv command. Let's say I have a file in my Dev directory I want to rename.

```
mv /home/jason/Dev/Basic_Terminal_Commands/basic_commands.md /home/jason/Dev/Basic_Terminal_Commands/ubuntu_terminal_commands.md
```

Here is another way that was suggested but it is more complicated:

```
for file in <the file or dir you want to rename>; do mv $file ${file//<name of the file or dir you want to rename>/<the new name you want>}; done
```
