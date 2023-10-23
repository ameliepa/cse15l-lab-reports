**Lab Report 2 - Servers and SSH Keys** <br /> <br />

**Part 1** <br />
Code of StringServer.java
![Image](stringserver1.png) <br />

1) **Screenshot of using /add-message** <br />
![Image](add-message1.png) <br />
**Methods called in handleRequest upon using /add-messages?s=Hello:** <br />
- .getPath()
- .equals()
- .format()
- .contains()
- .getQuery
- .split()
- .toString()
- .length


- **What are the relevant arguments to those methods, and the values of any relevant fields of the class?**
Relevant arguments to the above methods:
the URI url <br />

- **How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why**
Values changed: count changes, str changes <br />

2) **Screenshot of using /add-message** <br />
![Image](add-message2.png) <br />
- Which methods in your code are called?

- What are the relevant arguments to those methods, and the values of any relevant fields of the class?

- How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why

**Part 2** <br />
Using the command line, show with ls and take screenshots of: 
The path to the _private_ key for your SSH key for logging into ieng6 (on your computer or on the home directory of the lab computer)
The **path to the _public_ key for your SSH key for logging into ieng6** (within your account on ieng6)

Logging into ieng6 with course-specific account without being asked for a password:
![Image](terminal-interaction.png)

**Part 3** <br />
In a couple of sentences, describe something you learned from lab in week 2 or 3 that you didn’t know before.
In lab, I learned about how to ssh into a remote server. I also learned how to make a new server and run it.
