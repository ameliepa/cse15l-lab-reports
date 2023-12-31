- **Logging into ieng6** <br />
![Image](7-login.png)
No keys were used. I have an extension called Remote - SSH on VSCode that allows me to access my ieng6 account with one click.

- **Cloning the fork of the repository from my Github account (using the SSH URL)** <br />
![Image](7-cloning.png)
**Keys used:** g, i, t, `<space>`, c, l, o, n, e, `<space>`, `<command>` + V, `<enter>` <br /> <br />
Used the git clone command to clone my repository onto my remote account. `<command>` + V was used to paste the link to the repository I had copied.  <br />

- **Running the tests, demonstrating that they fail** <br />
![Image](7-runtests.png)
**Keys used:** c, d, `<space>`, l, a, b, 7, `<enter>`, b, a, s, h, `<space>`, t, `<tab>`, `<enter>` <br /> <br />
I used the cd command to change directory to lab7, allowing me to then type the command for the bash tests, using the `<tab>` shortcut. Then, I ran the command. <br />

- **Editing the code file to fix the failing test** <br />
Vim command:
![Image](7-vimcommand.png)
Using vim:
![Image](7-insidevim.png)
**Keys used:** <br /> v, i, m, `<space>`, L, `<tab>`, ., j, a, v, a, `<enter>` <br /> x, i, 2, `<esc>`, :, w, q, `<enter>` <br /> <br />
I used vim to edit the file from the command line. After `<enter>` was first pressed, the terminal was in vim. I clicked on 1 and then pressed x, resulting in 1 being removed. Normally, when in vim, you are unable to click on a character and you must use keys to get to your desired location within the file. However, I think due to the extension I used, I was able to click on the spot I wanted my cursor to be. Pressing i put me in insert mode where I was able to press 2, and use `<esc>` to exit insert mode. The command :wq allowed me to save my changes (the usage of the w) and quit vim (the usage of the q). <br />

- **Running the tests, demonstrating that they now succeed** <br />
![Image](7-runagain.png)
**Keys used:** `<up arrow>`,  `<up arrow>`, `<enter>` <br /> <br />
I used the `<up arrow>` shortcut to access and use a previous command, `bash test.sh`.<br />

- **Committing and pushing the resulting change to my Github account** <br />
![Image](7-committing.png)
**Keys used:** <br /> g, i, t, `<space>`, a, d, d, `<space>`, L, `<tab>`, ., j, a, v, a, `<enter>` <br /> g, i, t, `<space>`, c, o, m, m, i, t, `<space>`, -, m, `<space>`, ", c, h, a, n, g, e, d, `<space>`, i, n, d, e, x, 1, `<space>`, t, o, `<space>`, i, n, d, e, x, 2, ", `<enter>` <br /> g, i, t, `<space>`, p, u, s, h, `<enter>` <br /> <br />
I used git add to stage the file ListExamples.java, and used `<tab>` to . git commit creates a commit locally for the file I just staged. The -m option allows me to add a commit message: "changed index1 to index2". Then, git push copies the changes to the remote server, GitHub.
