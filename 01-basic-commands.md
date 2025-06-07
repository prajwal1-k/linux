# Basic Commands of Linux

## 🧭 Navigation Commands
1.  **pwd (present working directory)**
  > This is for printing the currrent working directory

   ```bash
   prajwal@prajwal-Inspiron-15-3567:~$ pwd
   /home/prajwal
   ```
2. **cd (change directory)**
> This is for changing the directory from the current directory

  ```bash
  cd /home/user/Documents
 ````
3. **ls (lists)**

> 	Lists files and directories in the current directory. Use `ls -l` for detailed info, `ls -a` to include hidden files

```bash
prajwal@prajwal-Inspiron-15-3567:~$ ls
Desktop  Documents  Downloads 
```

```bash
prajwal@prajwal-Inspiron-15-3567:~$ ls -l
drwxr-xr-x   2 prajwal prajwal   4096 Mar 18 14:59 Desktop
drwxr-xr-x   2 prajwal prajwal   4096 May 28 00:04 Documents
drwxr-xr-x   9 prajwal prajwal   4096 Jun  1 13:05 Downloads
```

```bash
prajwal@prajwal-Inspiron-15-3567:~$ ls -a
```
---

## 📁 File and Directory Management


1. **mkidr**

> creates the new directory (i.e make directory)

```bash
prajwal@prajwal-Inspiron-15-3567:~$ mkdir new_folder
```

2. **touch**

> This is mainly for creating the new empty file

```bash
prajwal@prajwal-Inspiron-15-3567:~$ touch file1.txt
```

3. **cp**

> This command copies a files or directory

```bash
prajwal@prajwal-Inspiron-15-3567:~$ cp file1.txt file2.txt
```

4. **rm**

> This command is for removing or deleting the files or directory (use `rm -r` for deleting/ removing directory)

```bash
prajwal@prajwal-Inspiron-15-3567:~$ rm file1.txt
```

---

## ⚙️ System Info and Management

1. **uname**

> This will provide the name of the os your using

```bash
prajwal@prajwal-Inspiron-15-3567:~$ uname
Linux
```
  - uname -r 
  > This tells the version of the linux we are using

     ```bash
     prajwal@prajwal-Inspiron-15-3567:~$ uname -r
     6.11.0-8-generic
     ```
  - uname -a
  > Displays the information of the system

     ```bash
     prajwal@prajwal-Inspiron-15-3567:~$ uname -a
     Linux prajwal-Inspiron-15-3567 6.11.0-8-generic #8-Ubuntu SMP PREEMPT_DYNAMIC Mon Sep 16 13:41:20 UTC 2024 x86_64 x86_64 x86_64 GNU/Linux
     ```
2. **ps**
> This shows the currently running processes

```bash
prajwal@prajwal-Inspiron-15-3567:~$ ps
    PID TTY          TIME CMD
  13131 pts/1    00:00:00 bash
  25346 pts/1    00:00:00 ps
```
3. **free -h**
> This displays the free and used memory

```bash
prajwal@prajwal-Inspiron-15-3567:~$ free -h
               total        used        free      shared  buff/cache   available
Mem:            10Gi       4.2Gi       2.0Gi       743Mi       5.8Gi       6.7Gi
Swap:          4.0Gi       452Ki       4.0Gi
```
4. **df -h**
> Shows the disk usage in human-readable format

```bash
prajwal@prajwal-Inspiron-15-3567:~$ df -h
Filesystem      Size  Used Avail Use% Mounted on
tmpfs           1.1G  2.4M  1.1G   1% /run
/dev/sda2       469G   31G  415G   7% /
tmpfs           5.5G  153M  5.4G   3% /dev/shm
tmpfs           5.0M  8.0K  5.0M   1% /run/lock
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-journald.service
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-udev-load-credentials.service
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-tmpfiles-setup-dev-early.service
tmpfs           5.5G   30M  5.5G   1% /tmp
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-sysctl.service
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-tmpfiles-setup-dev.service
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-tmpfiles-setup.service
tmpfs           1.0M     0  1.0M   0% /run/credentials/systemd-resolved.service
tmpfs           1.1G  144K  1.1G   1% /run/user/1000
```
5. **uptime**
> shows the system uptime

```bash
prajwal@prajwal-Inspiron-15-3567:~$ uptime
 00:23:35 up 15:36,  2 users,  load average: 1.30, 0.86, 0.79
```

6. **whoami**
> Shows the current user

```bash
prajwal@prajwal-Inspiron-15-3567:~$ whoami
prajwal
```
---

## 📦 Package Management (Debian-based systems like Ubuntu)

1. **sudo apt update**
> This is for updating the package list

```bash
prajwal@prajwal-Inspiron-15-3567:~$ sudo apt update
```

2. **sudo apt install <pkg_name>**
> This for downloading the new package

```bash
prajwal@prajwal-Inspiron-15-3567:~$ sudo apt install pkg_name
[sudo] password for prajwal:
```

3. **sudo apt upgrade**
>

```bash
prajwal@prajwal-Inspiron-15-3567:~$ sudo apt upgrade
```
---

## 🌐 Networking

```bash
ping <host>                # Ping a host
ifconfig / ip a            # Show network interfaces
curl <url>                 # Fetch data from URL
wget <url>                 # Download file from URL
```

## 🚧 More Coming Soon...
This is just the beginning! Many more Linux concepts, commands, and advanced topics (like scripting, package management, services, networking, and user management) will be covered in upcoming updates. Stay tuned and feel free to contribute!

## 📝 Contributing
Feel free to fork, clone, and contribute by submitting a pull request! Any improvements or additions are welcome.

---
## 📚 Resources
Here are some recommended resources to learn more about Linux:

[Youtube Channel] (https://www.youtube.com/user/TheLinuxFoundation)
<br>
[geeksforgeeks] (https://www.geeksforgeeks.org/basic-linux-commands)




   

   
