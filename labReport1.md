
## **Running cd** <br /> <br />

1. **No arguments** <br />

![Image](cd-no-argument.png) <br />

Working directory at the time of running the command: /home <br />

The command cd is intended to change the directory of the terminal with a given path. Since no path was given as an argument, the path did not change. <br />

The output is an error because cd is meant to change the directory of the terminal, but no change occurred. <br />




2. **Path to directory as an argument** <br />

![Image](cd-path-directory.png) <br />

Working directory at the time of running the command: /home <br /> 

Using lecture1 as an arugument with the cd command resulted in the path of the directory changing. I ran pwd after running the lines of code above, and the working directory was no longer /home but instead /home/lecture1. This is also indicated in the command prompt changing from [user@sahara ~]$ to [user@sahara ~/lecture1]. <br /> 

The output is not an error, the code is running as intended. <br /> 




3. **Path to file as an argument** <br />

![Image](cd-path-file.png) <br />

Working directory at the time of running the command: /home <br />

Using the absolute path to the file en-us.txt as an argument resulted in an error and no changes made to the working directory. This is because the argument for cd is meant to be a path to a directory.
<br />

The output is an error because the path that was input did not lead to a directory, but instead a file, so cd did not work as intended.
<br /> <br />




## **Running ls** <br /> <br />

1. **No arguments** <br />

![Image](ls-no-argument)<br />

Working directory at the time of running the command: /home <br />

Since no arguments were given in this command, the path defaulted to the current working directory, which was /home. Running this code printed the titles of the file lab1 and the folder lecture1 which are both located within /home. <br />

No error occurred. <br />


2. **Path to directory as an argument** <br />

![Image](ls-path-directory) <br />

4.

## **Running cat** <br /> <br />

1. **No arguments**
2. **Path to directory as an arugment**
3. **Path to file as an argument**
