# Basic Ubuntu Commands

## Sudo
sudo (Superuser DO) This is the same as Run as administor

``sudo``

## apt-get
This command is used to install, update, upgrade, and remove any package. Examples below will show how to use in different ways:

* **sudo apt-get update**
    
    superuser privileges. This command updates your system along with the packages that are installed.

    ``sudo apt-get update``

* **sudo apt-get upgrade**

    You will run this command after you ran
    
     ``sudo apt-get upgrade``

    This will upgrade the packages that have available updates. You can also upgrade just one package by adding a space along with the package name after upgrade.

    ``sudo apt-get upgrade node.js``

* **sudo apt-get install _package-name you wish to install_  
  You would replace the package-name with the name of the program you wish to install.

    ``sudo apt-get install curl``

## ls

ls (list) command will list out the files in the current working directory you are in.

``ls``

You can also look at different files in other directories by adding a space then the direct path to the other directory you wish to look into following the ls.

``ls /home/User/Dev``

We can also see hidden files by using the -a

``ls -a``

This command will list all the files in that directory including hidden files.

## cd

(change director) used to change the current working directory. You use it by typing cd space then the folder name within the your current directory or full paths to the folder if in a different directory. Examples of different ways below:

``cd/`` - Takes you to the root directory.

``cd ..`` - Takes you up on directory level.

``cd -`` - Takes you to the previous directory.

Examples:

``cd /home/User/Dev`` - This will take me to the Folder Dev in the directory.

``cd /home/User/Dev/JS\ Practice\ Folder`` - This will take me to the JS Practice Folder. **Note I used backslah+space. This does the same as** 

``cd /home/User/Dev/"JS Practice Folder"`` - I used "" instead of the backslah+space.

## pwd

(print working directory) This will display the full pathname of the working directory.

Using the last example above - 

``pwd``  

Returns:

``/home/User/Dev"JS Practice Folder"``

## cp

(copy) - After typing cp you type the file you want to copy + space + location you want to place the copied file.

``cp "JS Practice Folder" /home/User/Dev/JS``

## mv

(move) A lot like cp (copy) but instead of copying the file you will move it from one folder to another folder in the directory. Just like cp (copy) after typing mv + space + the file you want to move + location to move it too.

``mv pyproject.py /home/User/Dev/Python_Project`` - This will move the pyproject.py file in my current directory to the Python_Project folder in the directory.

## rm

(remove) This command will remove the specified file but not the directory. This will delete if from the directory.

``rm js_practice``

Here are some other uses of using rm:

* **rmdir**
    
    (remove directory) - Removes an empty directory

    ``rmdir /home/User/Dev/My_Empty_Folder``

* **rm -r**

    (remove recursively) - Removes a dirctroy along with its content.

    `` rm -r /home/User/Dev/No_Longer_Needed_Practice_Folder``

* **rm -f**

    (remove force)
    This will forcefully remove files. To forcefully remove dirctorie use ``rm -rf <fileName>``

* **rm -i**

    This is use to be prompt before every removal.

    ``rm -i <fileName>``

## mkdir

(make directory) This command will allow you to create a new directory. You can also specify where you want to create this directory's location by putting a space followed by the location behind mkdir. Example:

``mkdir Basic_Terminal /home/User/Learn``

Or if I wish to make a new directory in the current directory I would do:

``mkdir Learn_Terminal_Basic``

## locate

Helps you to find files and their location by their name. If you are not sure if the file name is upper case or lower case us -i to ignore the case.
If you wish to locate two or more words at a time you can seprate each word with (*). Examples:

``locate -i *hello*his``

If you just want to have a count of the times the word is in the directory you can use -c. Example:

``locate -i -c Python``

This would return a number of how many time the word Python in being used in the directory.

## echo

This command helps us move data into text files. Example:

``echo I'm learning how to use the terminal in Ubuntu.>>basic_terminal.txt``

We did not have to use backslashs or wrap the sentence in "" because we used two >>(greater than) symbols before we put in the file to echo the sentence into.

## history

This command will display all of your previous commands **up to the history memory limit.**

``history``

This will return your previous commands.

## df

(display filesystem) This will display information about your disk space usage of your filesystem.

``df``

## free

This command displays the amount of free space available on the system.

``free``

## top

This will display the processes using the most resources. You can exit out by typing q

``top``

## cat

Displays the contents of a file.

``cat /home/User/Dev/Practice_Python/Basic.py``

or to cat in your current directory

``cat Basic.py``