**Lab Report 2 - Servers and SSH Keys** <br /> <br />

**Part 1** <br />
Code of StringServer.java <br />
![Image](stringserver1.2.png) <br />
![Image](stringserver2.png) <br />

1) **Screenshot of using /add-message?s=Hello!** <br />
![Image](add-message1.png) <br />

**Methods called in handleRequest upon using /add-messages?s=Hello:** 
<br /> <br />
- .getPath()
- .equals()
- .format()
- .contains()
- .getQuery()
- .split()
- .toString()
- .length
<br />

**Relevant arguments to those methods and the values of any relevant fields of the class:** <br /> <br />

- .equals("/") and .equals("s")
- .format("%s",str)
- .contains("/add-message")
- .split("=")
- Integer.toString(count)
- int count = 1
- String str = ""
- Additionally, when handleRequest is called, its argument is URI url and its value is http://ieng6-202.ucsd.edu:1989/add-message?s=Hello!
<br />

**Values of relevant fields of the class change that are changed:** <br /> <br />
- String str is changed. A String version of the count value, a ". ", a String value from the query, and "\n" is added to str.
- int count is changed. It increases by 1 after str is altered.
<br />

2) **Screenshot of using /add-message?s=How%20are%20you?** <br />
![Image](add-message2.png) <br />

**Methods called in handleRequest upon using /add-message?s=How%20are%20you?** <br /> <br />
- .getPath()
- .equals()
- .format()
- .contains()
- .getQuery()
- .split()
- .toString()
- .length
<br />

**Relevant arguments to those methods and the values of any relevant fields of the class:**
<br /> <br />
- .equals("/") and .equals("s")
- .format("%s",str)
- .contains("/add-message")
- .split("=")
- Integer.toString(count)
- int count = 2
- String str = "1. Hello!\n"
- Additionally, when handleRequest is called, its argument is URI url and its value is http://ieng6-202.ucsd.edu:1989/add-message?s=How%20are%20you?
<br />

**Values of relevant fields of the class change that are changed:**
<br /> <br />
- String str is changed. A String version of the count value, a ". ", a String value from the query, and "\n" is added to str.
- int count is changed. It increases by 1 after str is altered.
<br />

**Part 2** <br />
**Using the command line, show with ls and take screenshots of:** <br />
<br />
The path to the _private_ key for your SSH key for logging into ieng6 (on your computer or on the home directory of the lab computer): <br />
![Image](ssh-private.png) <br />
The path to the _public_ key for your SSH key for logging into ieng6 (within your account on ieng6): <br />
![Image](ssh-public.png) <br />
Logging into ieng6 with course-specific account without being asked for a password: <br />
![Image](terminal-interaction.png)

**Part 3** <br />
From our labs, I learned how to ssh into a remote server. I also learned how to make a create a new server and run it, as shown in this week's lab. 
