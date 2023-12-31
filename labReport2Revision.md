**Lab Report 2 - Servers and SSH Keys** <br /> <br />

**Part 1** <br />
Code of StringServer.java <br />
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    int count = 1;
    String str = new String("");

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format("%s",str);
        } else {
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                    int len = parameters.length;
                    String message = new String("");
                    for (int i = 1; i < len; i++){
                        message = message + (parameters[i]);
                    }
                    String number = new String(Integer.toString(count));
                    str = str + number + ". " + message + "\n";
                    count++;
                    return String.format("%s",str);
                }
            }
            return "404 Not Found!";
        }
    }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```

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
- Additionally, when ```handleRequest``` is called, its argument is ```URI url``` and its value is ```http://ieng6-202.ucsd.edu:1989/add-message?s=Hello!```
<br />

**Values of relevant fields of the class change that are changed:** <br /> <br />
- String ```str``` is changed. A String version of the count value, a ". ", a String value from the query, and "\n" is added to ```str```. ```str``` now equals ```1. Hello\n```
- int ```count``` is changed. It increases by 1 after str is altered, making the new value of ```count``` 2.
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
- Additionally, when ```handleRequest``` is called, its argument is ```URI url``` and its value is ```http://ieng6-202.ucsd.edu:1989/add-message?s=How%20are%20you?```
<br />

**Values of relevant fields of the class change that are changed:**
<br /> <br />
- String ```str``` is changed. A String version of the count value, a ". ", a String value from the query, and "\n" is added to ```str```. ```str``` now equals ```1. Hello\n2. How are you?\n```
- int ```count``` is changed. It increases by 1 after str is altered, making the new value of ```count``` 3.
<br />

**Part 2** <br />
**Using the command line, show with ls and take screenshots of:** <br />
<br />
The path to the _private_ key for your SSH key for logging into ieng6 (on your computer or on the home directory of the lab computer): <br />
![Image](ssh-private.png) <br />
```/home/linux/ieng6/cs15lfa23/cs15lfa23kb/.ssh/id_rsa``` <br />
The path to the _public_ key for your SSH key for logging into ieng6 (within your account on ieng6): <br />
![Image](ssh-public.png) <br />
```/home/linux/ieng6/cs15lfa23/cs15lfa23kb/.ssh/id_rsa.pub``` <br />
Logging into ieng6 with course-specific account without being asked for a password: <br />
![Image](terminal-interaction.png)

**Part 3** <br />
From our labs, I learned how to ssh into a remote server. I also learned how to make a create a new server and run it, as shown in this week's lab. It's a lot more simple than I realized. Running a server requires two different java files. One of those files reads the url and determines what it shown on the server. The other file handles more complicated requests.
