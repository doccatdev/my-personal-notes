# Kali Linux – Basic Command

## List of Kali Linux Command

### Navigating the File System

- `pwd`: preworking directory

```bash
┌──(kali㉿kali)-[~]
└─$ pwd
/home/kali
```

---

- `cd`: change directory

```bash
┌──(kali㉿kali)-[~]
└─$ cd workout
                                                                     
┌──(kali㉿kali)-[~/workout]
└─$ pwd
/home/kali/workout
```

!!! note "for `cd` command"

- `cd ..` to move up one level from `/etc` or `/` (root)
- `cd .. / ..` to move up two level from `/etc` or `/` (root)
- `cd .. / ..  / .. ` to move up three level and so on from `/etc` or `/` (root)

---

- `ls`: list of directory content

```bash
┌──(kali㉿kali)-[/]
└─$ ls
bin   home            lib32       mnt   run   sys  vmlinuz
boot  initrd.img      lib64       opt   sbin  tmp  vmlinuz.old
dev   initrd.img.old  lost+found  proc  srv   usr
etc   lib             media       root  swap  var
```

---

`mkdir` : make directories

```bash
┌──(kali㉿kali)-[~]
└─$ mkdir Exercise
                                                                             
┌──(kali㉿kali)-[~]
└─$ ls
Desktop    Downloads  Music     Public     Videos
Documents  Exercise   Pictures  Templates  workout
                                                             
```

---

- `rm` : remove files or directories

```bash
┌──(kali㉿kali)-[~]
└─$ rm -r Exercise
                                                                             
┌──(kali㉿kali)-[~]
└─$ ls
Desktop    Downloads  Pictures  Templates  workout
Documents  Music      Public    Videos

```

---

- `rmdir` : remove empty directories

```bash
┌──(kali㉿kali)-[~]
└─$ rmdir Cat 
                                                                             
┌──(kali㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos
```

!!! info "`cat` Command"

- if your file have space, you can do this `cat < "this is file name"`
- if your file have dashed, you can do this `cat < -`
- if your file have space and dashed, you can do this `cat < --"this is file name"--`



---

- `cp` : copy files and directories

```bash
┌──(kali㉿kali)-[~]
└─$ cp text.txt Documents
                                                                             
┌──(kali㉿kali)-[~]
└─$ cd Documents         
                                                                             
┌──(kali㉿kali)-[~/Documents]
└─$ ls
text.txt

```

---

- `mv` : move and/or (rename) files

```bash
┌──(kali㉿kali)-[~]
└─$ mv text.txt Downloads
                                                                             
┌──(kali㉿kali)-[~]
└─$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos

┌──(kali㉿kali)-[~]
└─$ cd Documents   
                                                                
┌──(kali㉿kali)-[~/Documents]
└─$ ls
text.txt

```

---

- `locate` : find files by name, quickly

!!! info "Informatin for `locate` command"

- Use `updatedb` to update a database for `locate`

---

`find` : search for files in a directory hierarchy

```bash
┌──(kali㉿kali)-[~/Downloads]
└─$ find text.txt
text.txt

```

---

- `passwd` : change user password

!!! note "For Command Help"

- use [`command name` `--help`] to get information about quick overview of usage and syntax for specific command
- use [`man` `command name`] to get manual page for specific command

### Users and Privilages

- `chmod` : change file mode bits (change file permission)

```bash
┌──(kali㉿kali)-[~]
└─$ ls -la

-rw-rw-r--  1 kali kali     6 Dec  2 01:00 hello.txt

┌──(kali㉿kali)-[~]
└─$ chmod +rwx hello.txt
                                                                             
┌──(kali㉿kali)-[~]
└─$ ls -la

-rwxrwxr-x  1 kali kali     6 Dec  2 01:00 hello.txt

```

!!! info "Linux File Permission 101"

---

- `adduser` : add or manipulate users
(add new users)

```bash
┌──(kali㉿kali)-[~]
└─$ sudo su      

[sudo] password for kali: 
┌──(root㉿kali)-[/home/kali]
└─# adduser zero

```

!!! info "Linux/Kali Linux File System"

---

- `su` : run a command with substitute user and group ID (switch to another user)

```bash
┌──(root㉿kali)-[/home/kali]
└─# su zero     

┌──(zero㉿kali)-[/home/kali]
└─$ man su

```

---

`sudo` : execute a command as another user
(allows a permitted user to execute a command as the superuser (root) or another user)

```bash
┌──(kali㉿kali)-[~]
└─$ sudo su    

[sudo] password for kali: 
┌──(root㉿kali)-[/home/kali]
└─# 
```

### Common Network Commands

`ifconfig` : configure a network interface

```bash
┌──(kali㉿kali)-[~]
└─$ ifconfig

---

```

`ip a` : show / manipulate routing, network device, interface, tunnels. It replaces the earlier and now deprecated `ifconfig` program

```bash
┌──(kali㉿kali)-[~]
└─$ ip a
```


`iwconfig` : configure wireless network interface

```bash
┌──(kali㉿kali)-[~]
└─$ ifconfig
```

`iw a` : show / manipulate wireless device and their configuration.

```bash
┌──(kali㉿kali)-[~]
└─$ iw a
```

---

`ping` : send ICMP ECHO_REQUEST to network hosts

```bash
┌──(kali㉿kali)-[~]
└─$ ping
```

---

`netstat` : Print network connections, routing tables, interface statistics, masquerade connections, and multicast memberships

```bash
┌──(kali㉿kali)-[~]
└─$ netstat
```

### Viewing, Creating, and Editing Files

- `echo` : display a line of text

```bash
┌──(kali㉿kali)-[~]
└─$ echo "Hello World" > hello.txt
                                                                             
┌──(kali㉿kali)-[~]
└─$ cat hello.txt              
Hello World

┌──(kali㉿kali)-[~]
└─$ echo "Hello Hello World" >> hello.txt
                                                                             
┌──(kali㉿kali)-[~]
└─$ cat hello.txt
Hello World
Hello Hello World
```

!!! info "`echo` Command"

`>>` use that symbol to append output in existing file, if use `>` the file will be overwriten if already exist

- `touch` : change file timestamps and create new empty file

```bash
┌──(kali㉿kali)-[~]
└─$ touch newfile.txt
                                                                             
┌──(kali㉿kali)-[~]
└─$ ls    
Desktop    Downloads  Music        Pictures  Templates
Documents  hello.txt  newfile.txt  Public    Videos
```

---

- `cat` : concatenate files and print on the standard output (view, create and combine file content directly from the terminal)

```bash
┌──(kali㉿kali)-[~]
└─$ cat newfile.txt
Hello world, this is example of using touch and nano command in Kali Linux

```

---

- `du` : estimate file space usage

```bash
┌──(kali㉿kali)-[~]
└─$ du Downloads
8       Downloads
                     
```

- `find` : search for files in a directory hierarchy

```bash
┌──(kali㉿kali)-[~]
└─$ find ~ -name "hello.txt" 
/home/kali/hello.txt
```

!!! info "`find` Command"

`find [options] [path] [expression]`

---

- `file` : 

```bash
┌──(kali㉿kali)-[~]
└─$ file Downloads          
Downloads: directory
```

### Starting and Stopping Services

- `service` : run a System V init script

```bash
┌──(kali㉿kali)-[~]
└─$ sudo service apache2 start
```

- `systemctl` : Control the systemd system and service manager

```bash
┌──(kali㉿kali)-[~]
└─$ sudo systemctl disable  apache2
Synchronizing state of apache2.service with SysV service script with /usr/lib/systemd/systemd-sysv-install.
Executing: /usr/lib/systemd/systemd-sysv-install disable apache2
Removed '/etc/systemd/system/multi-user.target.wants/apache2.service'.
                                                                             
┌──(kali㉿kali)-[~]
└─$ sudo systemctl status apache2
○ apache2.service - The Apache HTTP Server
     Loaded: loaded (/usr/lib/systemd/system/apache2.service; disabled; pres>
     Active: inactive (dead)
       Docs: https://httpd.apache.org/docs/2.4/

Dec 06 01:12:08 kali systemd[1]: Starting apache2.service - The Apache HTTP >
Dec 06 01:12:08 kali apachectl[5840]: AH00558: apache2: Could not reliably d>
Dec 06 01:12:08 kali systemd[1]: Started apache2.service - The Apache HTTP S>
Dec 06 01:14:09 kali systemd[1]: Stopping apache2.service - The Apache HTTP >
Dec 06 01:14:09 kali apachectl[7218]: AH00558: apache2: Could not reliably d>
Dec 06 01:14:09 kali systemd[1]: apache2.service: Killing process 5852 (apac>
Dec 06 01:14:09 kali systemd[1]: apache2.service: Killing process 5853 (apac>
Dec 06 01:14:09 kali systemd[1]: apache2.service: Deactivated successfully.
Dec 06 01:14:09 kali systemd[1]: Stopped apache2.service - The Apache HTTP S>
lines 1-14/14 (END)

```

### Install and Updating Tools

- update and upgrade kali linux machine

```bash
┌──(root㉿kali)-[/home/kali]
└─# apt update && apt  upgrade
```

---

- installing software / package

```bash
┌──(root㉿kali)-[/home/kali]
└─# apt install postgresql-18    
```

---

- Installing tools / clone repository from Github

```bash
┌──(root㉿kali)-[/home/kali]
└─# git [repository link]



```

### Scripting with Bash

## Resource

- <https://github.com/shreyaschavhan/linux-commands-cheatsheet>
- <https://www.youtube.com/watch?v=lZAoFs75_cs>
- Kali Linux User Command Manual Page
