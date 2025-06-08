# Bash Prompt

> In the Bash shell, the prompt is what you see when the shell is ready to accept a command.
It's typically something like:
`username@hostname:~$`

> `[~]$` Here ~ = **Present working directory (pwd)** and the $ = **User prompt symbol**

```bash
prajwal@prajwal:~$ echo $PS1
[\W]$
```
- \W = Present working directory
- $ = prompt symbol

### Customize the Prompt

```bash
prajwal@prajwal:~$ PS1 = "ubuntu-server:"
```
```bash
prajwal@prajwal:~$ echo $PS1
ubuntu-server:
```
---
Breakdown of common escape sequences in PS1:
```bash
Code	Meaning
\u	    Username
\h	    Hostname (up to first .)
\H	    Full hostname
\w	    Current working directory (with ~)
\W	    Last part of the working directory
\d	    Date
\t	    Current time (HH:MM:SS)
\T	    Time (12-hour format)
\@	    Time (12-hour format with AM/PM)
\n	    New line
\$	    # if root, $ otherwise
\!	    History number
\#	    Command number of this command
``` 

> 🔧 Bonus: Secondary Prompts
```bash
Variable	Used for
PS1	       Main prompt
PS2	       Shown when a command spans multiple lines (default is >)
PS3	       Used in select loops in scripts
PS4	       Used when debugging with set -x (default is +)
```



