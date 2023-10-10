
**Running cd** <br /> <br />

1. **No arguments** <br />

![Image](cd-no-argument.png) <br />

**Working directory at the time of running the command:** /home <br />

The command cd is intended to change the directory of the terminal with a given path. Since no path was given as an argument, the path did not change. <br />

The output is an error because cd is meant to change the directory of the terminal, but no change occurred. <br />




2. **Path to directory as an argument** <br />

![Image](cd-path-directory.png) <br />

**Working directory at the time of running the command:** /home <br /> 

Using lecture1 as an arugument with the cd command resulted in the path of the directory changing. I ran pwd after running the lines of code above, and the working directory was no longer /home but instead /home/lecture1. This is also indicated in the command prompt changing from [user@sahara ~]$ to [user@sahara ~/lecture1]. <br /> 

The output is not an error, the code is running as intended. <br /> 




3. **Path to file as an argument** <br />

![Image](cd-path-file.png) <br />

**Working directory at the time of running the command:** /home <br />

Using the absolute path to the file en-us.txt as an argument resulted in an error and no changes made to the working directory. This is because the argument for cd is meant to be a path to a directory.
<br />

The output is an error because the path that was input did not lead to a directory, but instead a file, so cd did not work as intended.
<br /> <br />




**Running ls** <br /> <br />

1. **No arguments** <br />

![Image](ls-no-argument.png)<br />

**Working directory at the time of running the command:** /home <br />

Since no arguments were given in this command, the path defaulted to the current working directory, which was /home. Running this code printed the titles of the file lab1 and the folder lecture1 which are both located within /home. <br />

No error occurred. <br />


2. **Path to directory as an argument** <br />

![Image](ls-path-directory.png) <br />

**Working directory at the time of running the command:** /home <br />

Running ls with the directory lecture1 as a path printed out the titles of the files and folder within lecture1. <br />

No error occurred. <br />

3. **Path to file as an argument** <br />

![Image](ls-path-file.png)<br />

**Working directory at the time of running the command:** /home <br />

The purpose of ls is to list the files and folders of the path given. Since the path given led to a file instead of directory, no list could be printed. Instead, the path given was printed. <br />

This is an error because no list was printed. <br /> <br />

**Running cat** <br /> <br />

1. **No arguments** <br />

![Image](cat-no-argument.png)<br />

**Working directory at the time of running the command:** /home <br />

Running cat with no argument resulted in nothing being printed. The command prompt also disappeared, forcing me to create another terminal as I could not figure out how to fix this otherwise. <br />

The cat command is supposed to print the contents of a file. Since no file was given as an argument, an error occurred, removing the command prompt. <br />


2. **Path to directory as an arugment** <br />

![Image](cat-path-directory.png)<br />

**Working directory at the time of running the command:** /home <br />

Running cat with a directory as an argument did not print the contents of the directory, but instead a statement describing lecture1. <br />

This result is an error because no file contents were printed. <br />

3. **Path to file as an argument** <br />

![Image](cat-path-file.png)<br />

**Working directory at the time of running the command:** /home <br />

Running cat with a path to a file as an argument resulted in the contents of that file being printed successfully. <br />

No error occured.
