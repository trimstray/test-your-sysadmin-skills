<p align="center">
    <img src="https://github.com/trimstray/sysadmin-interview-questions/blob/master/doc/img/sysadmin_interview_questions_preview.png"
        alt="Master">
</p>

<br>

<h4 align="center">Sysadmin Interview Questions 2018 Edition.</h4>

<br>

<p align="center">
  <a href="https://github.com/trimstray/sysadmin-interview-questions/tree/master">
    <img src="https://img.shields.io/badge/Branch-master-green.svg?longCache=true"
        alt="Branch">
  </a>
  <a href="http://www.gnu.org/licenses/">
    <img src="https://img.shields.io/badge/License-GNU-blue.svg?longCache=true"
        alt="License">
  </a>
</p>

<div align="center">
  <sub>Created by
  <a href="https://twitter.com/trimstray">trimstray</a> and
  <a href="https://github.com/trimstray/sysadmin-interview-questions/graphs/contributors">
    contributors
  </a>
</div>

<br>

***

## Table of Contents

- **[General Knowledge](#general-knowledge)**
  * [Introduction](#introduction) - 0 Questions, 0 Answers
  * [Junior Sysadmin](#junior-sysadmin) - 21 Questions, 21 Answers
  * [Regular Sysadmin](#regular-sysadmin) - 27 Questions, 11 Answers
  * [Senior Sysadmin](#senior-sysadmin) - 19 Questions, 0 Answers
- **[Secret Knowledge](#secret-knowledge)**
  * [Guru Sysadmin](#guru-sysadmin) - 0 Questions, 0 Answers

## <a name="general-knowledge">General Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="introduction">Introduction</a>

### :diamond_shape_with_a_dot_inside: <a name="junior-sysadmin">Junior Sysadmin</a>

###### System Questions

**What are the Linux Distribution (Operating System) names?**

- Redhat Enterprise Linux  
- Fedora Linux  
- Debian Linux  
- Suse Enterprise Linux  
- Ubuntu Linux  
- CentOS Linux  
- Slackware Linux  

**What do you understand by CLI?**

CLI is an acronym for Command Line Interface. We have to provide the information to the computer so that it can perform the function accordingly. In Linux, CLI is the interface that provides the user an interface so that user can type the commands and it complete the tasks. CLI is very easy to use, but it should be typed very precisely.

**What is your favourite shell and why?**

BASH as my favorite. It’s really a preferential kind of thing, where I love the syntax and it just "clicks" for me. The input/output redirection syntax (>>, << 2>&1, 2>, 1>, etc) is similar to C++ which makes it click even easier in my mind. Again, what shell you choose really depends on your preference- just don’t use crosh (chrome shell).

I also like ZSH shell because is much much more customizable than BASH. It has great Oh-MY-Zsh framework, powerful context based tab completion, pattern matching/globbing on alien steroids, loadable modules and more.

**What is the swap space?**

Swap space is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space. While swap space can help machines with a small amount of RAM, it should not be considered a replacement for more RAM. Swap space is located on hard drives, which have a slower access time than physical memory.

**How to check memory stats and CPU stats?**

Using `free` and `vmstat` command we can display the physical and virtual memory statistics respectively. With the help of 'sar' command we see the CPU utilization & other stats.

**Where is password file located in Linux?**

Linux passwords are stored in the **/etc/shadow** file. They are salted and the algorithm being used depends on the particular distribution and is configurable.

**How to create partition and filesystem?**

1) fdisk, gparted - create a new partition
2) mkfs - create a new filesystem

**Why should you avoid telnet to administer a system remotely?**

Telnet uses most insecure method for communication. It sends data across the network in plain text format and anybody can easily find out the password using the network tool. In the case of Telnet, these include the passing of login credentials in plain text, which means anyone running a sniffer on your network can find the information he needs to take control of a device in a few seconds by eavesdropping on a Telnet login session.

**What is the difference between Linux and UNIX?**

UNIX - Only big companies are allowed to use the UNIX copyright and name. IBM AIX, Sun Solaris, and HP-UX all are UNIX operating systems. Most UNIX operating systems are commercial in nature.

- UNIX operating systems are considered as a complete OS as everything come from a single vendor.
- Most UNIX like operating systems are not free.
- UNIX operating systems comes with its own firewall products.
- UNIX supports file systems like jfs, gpfs (AIX), jfs, gpfs (HP-UX), jfs, gpfs (Solaris).

Linux is a Unix clone. But if you consider Portable Operating System Interface (POSIX) standards then Linux can be considered as UNIX.

- Linux is Free. You can download it from the Internet or redistribute it under GNU licenses. 
- All Linux distributions include GUI system, GNU utilities, installation & management tools, GNU c/c++ Compilers, Editors (vi), and various applications like OpenOffice, Firefox.
- Linux comes with open source Netfilter and IPTables based firewall tool to protect your server and desktop from the crackers and hackers.
- By default, Linux supports and use ext3 or ext4 file systems.

**What are some common things between Linux & UNIX?**

- GUI, file, and windows managers (KDE, Gnome)
- Shells (ksh, csh, bash)
- Various office applications such as OpenOffice.org
- Development tools like perl, php, python, GNU c/c++ compilers
- Posix interface

**How do you change directory and subdirectory with file permissions in Linux/UNIX?**

To change all the directories eg. to 755 (drwxr-xr-x):

```bash
find /opt/lampp/htdocs -type d -exec chmod 755 {} \;
```
To change all the files eg. to 644 (-rw-r--r--):

```bash
find /opt/lampp/htdocs -type f -exec chmod 644 {} \;
```

**What are the kinds of permissions under Unix-like?**

- **Read**: users can read the files or list the directory
- **Write**: users may write to the file or add new files to the directory
- **Execute**: users may run the file or lookup a specific file within a directory

**How do you terminate an ongoing process?**

Explain how every process in the system is identified by a unique process id or pid.

Using the `kill` command followed by pid terminates that process. You can add a line on how to terminate all processes at once, by using `kill 0`.

**Describe the root account in Unix-like systems.**

The root account is like a systems administrator account, and allows you full control of the system. Root always has a UID of zero.

**What is the difference between "m" and "m –r"?**

`rm` removes files and `-rf` are to options:

- `-r` remove directories and their contents recursively
- `-f` ignore nonexistent files, never prompt

**Explain file content commands along with the description.**

- **head**: to check the starting of a file.
- **tail**: to check the ending of the file. It is the reverse of head command.
- **cat**: used to view, create, concatenate the files.
- **more**: used to display the text in the terminal window in pager form.
- **less**: used to view the text in the backward direction and also provides single line movement.

**What is grep command?**

`grep` searches file patterns. If you are looking for a specific pattern in the output of another command, grep highlights the relevant lines. Use this grep command for searching log files, specific processes, and more.

**How do you list contents of tar.gz and extract only one file?**

```bash
tar tf archive.tgz
tar xf archive.tgz filename
```

**How do you find who is logged in?**

Use this command to find who logged in: `w`.

###### Network Questions

**What are the default ports used for SMTP, FTP, DNS, DHCP and SSH protocols?**

| SERVICE | PORT |
|---|---|
| SMTP | 25 |
| FTP | 20 for data transfer and 21 for connection established |
| DNS | 53 |
| DHCP | 67/UDP for DHCP server, 68/UDPfor DHCP client |
| SSH | 22 |

**How to check default route and routing table?**

Using the commands `netstat -nr`, `route -n` or `ip route show` we can see the default route and routing tables.

### :diamond_shape_with_a_dot_inside: <a name="regular-sysadmin">Regular Sysadmin</a>

###### System Questions

**What is Linux and also explain the basic components of Linux?**

Linux operating system is consist of 3 components which are as below:

- **Kernel**: Linux is a monolithic kernel that is free and open source software that is responsible for managing hardware resources for the users.
- **System Library**: System Library plays a vital role because application programs access Kernels feature using system library.
- **System Utility**: System Utility performs specific and individual level tasks.

**How to increase the size of LVM partition?**

Use the `lvextend` command for resize LVM partition:

```bash
# extending the size by 500MB
lvextend -L +500M /dev/<vgroup>/<lvolume>
# extending all available free space
lvextend -l +100%FREE /dev/<vgroup>/<lvolume>
```

and `resize2fs` or `xfs_growfs` to resize filesystem:

```bash
# for ext
resize2fs /dev/<vgroup>/<lvolume>
# for xfs
xfs_growfs <mountpoint_for_/dev/<vgroup>/<lvolume>
```

**Which algorithms are supported in passwd file?**

The algorithms supported are MD5, Blowfish, SHA256 and SHA512.

**How to change the default run level in Linux?**

To change the run level we have to edit the file **/etc/inittab** and change initdefault entry (id:5:initdefault:). Using `init` command we change the run level temporary like `init 3`, this command will move the system in runlevl 3.

**What is umask? How to set it permanently for a user?**

umask stands for 'User file creation mask', which determines the settings of a mask that controls which file permissions are set for files and directories when they are created.

Permanently change (set eg. `umask 02`):

- **~/.profile**
- **~/.bashrc**
- **~/.zshrc**
- **~/.cshrc**

**What is load average?**

Is the average system load calculated over a given period of time of 1, 5 and 15 minutes. Lower numbers are better. Higher numbers represent a problem or an overloaded machine.

**Why when load is 1.00 on one-core machine is not ideal?**

The problem with a load of 1.00 is that you have no headroom. In practice, many sysadmins will draw a line at 0.70:

The "Need to Look into it" Rule of Thumb: 0.70 If your load average is staying above > 0.70, it's time to investigate before things get worse.

The "Fix this now" Rule of Thumb: 1.00. If your load average stays above 1.00, find the problem and fix it now. Otherwise, you're going to get woken up in the middle of the night, and it's not going to be fun.

Rule of Thumb: 5.0. If your load average is above 5.00, you could be in serious trouble, your box is either hanging or slowing way down, and this will (inexplicably) happen in the worst possible time like in the middle of the night or when you're presenting at a conference. Don't let it get there.

**What is the name and path of the main system log?**

By default, the main system log is **/var/log/messages**. This file contains all the messages and the script written by the user. By default all scripts are saved in this file. This is the standard system log file, which contains messages from all system software, non-kernel boot issues, and messages that go to `dmesg` (is a system file that is written upon system boot).

What is the difference between ext2 and ext3 file systems?

**Explain /proc filesystem?**

**/proc** is a virtual file system that provides detailed information about kernel, hardware and running processes. Files under **/proc** directory named as Virtual files.

Since **/proc** contains virtual files, it is called virtual file system. These virtual files have unique qualities. Most of them are listed as zero bytes in size.

Virtual files such as **/proc/interrupts**, **/proc/meminfo**, **/proc/mounts** and **/proc/partitions** provide an up-to-the-moment glimpse of the system’s hardware. Others: **/proc/filesystems** file and the **/proc/sys/** directory provide system configuration information and interfaces.

**What is a zombie/defunct process?**

Is a process that has completed execution (via the **exit** system call) but still has an entry in the process table: it is a process in the "Terminated state".

List out the differences between Softlink and Hardlink?

What are symbolic links?

What is redirection?

What is key-based authentication? Explain.

What is the advantage of executing the running processes in the background? How can you do that?

Explain Linux Boot Sequence.

Which command would you use if you want to remove the password assigned to a group?

What is an Inode?

Which command is used to review boot messages?

Which utility is used to make automate rotation of a log?

What is env command in Linux?

What is lsof command in Linux?

How do you limit memory usage for commands?

**Describe a process to create partition, lvm and filesystem.**

1. Create partition

```bash
fdisk /dev/sdb
```

2. Create LVM

```bash
pvcreate /dev/sdb1
vgcreate vg0 /dev/sdb1
lvcreate --name datastore --size 50G vg0
```

3. Create filesystem

```bash
mkfs -t xfs /dev/mapper/vg0-datastore
```

###### Network Questions

How to check which ports are listening in my Linux Server?

###### Protocols Questions

How to check which ports are listening in my Linux Server? What does curl command do in Linux?

### :diamond_shape_with_a_dot_inside: <a name="senior-sysadmin">Senior Sysadmin</a>

###### System Questions

What does Sar provides and at which location Sar logs are stored?

How to scan newly assigned luns on linux box without rebooting?

How to add & change the Kernel parameters?

What is LD_LIBRARY_PATH?

What is the difference between Cron and Anacron?

How shadow passwords are given by in Linux?

Explain all the fields in the /etc/passwd file?

What shell does a Linux Administrator assign to a POP3 mail-only account?

What are the different modes when using vi editor?

Explain the logical steps to increase the size of LVM partition?

Explain system calls used for process management?

What are the different types of Kernels? Explain.

Explain Interrupts in Linux and also explain Interrupt handlers.

How can we edit a file without opening in Linux?

What is the Pluggable Authentication Modules? Explain.

What is strace/ptrace command in Linux?

How do you kill program using one port in Linux?

How do you run command every time a file is modified?

How do you run a command for a limited time?

###### Network Questions

## <a name="secret-knowledge">Secret Knowledge</a>

### :diamond_shape_with_a_dot_inside: Guru Sysadmin
