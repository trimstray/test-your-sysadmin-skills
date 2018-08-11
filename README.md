<p align="center">
    <img src="https://github.com/trimstray/sysadmin-interview-questions/blob/master/doc/img/sysadmin_interview_questions_preview.png"
        alt="Master">
</p>

<br>

<h4 align="center">Sysadmin Interview Questions 2018 Edition (work in progress).</h4>

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

****

## Table of Contents

- <b>[General Knowledge](#general-knowledge)</b>
  * [Introduction](#introduction)
  * [Junior Sysadmin](#junior-sysadmin)
  * [Regular Sysadmin](#regular-sysadmin)
  * [Senior Sysadmin](#senior-sysadmin)
- <b>[Secret Knowledge](#secret-knowledge)</b>
  * [Guru Sysadmin](#guru-sysadmin)

## <a name="general-knowledge">General Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="introduction">Introduction</a>

0 Questions

### :diamond_shape_with_a_dot_inside: <a name="junior-sysadmin">Junior Sysadmin</a>

25 Questions.

###### System Questions

<details>
<summary><b>What are the Linux Distribution names?</b></summary><br>

- Redhat Enterprise Linux<br>
- Fedora Linux<br>
- CentOS Linux<br>
- Debian Linux<br>
- Ubuntu Linux<br>
- Suse Enterprise Linux<br>
- Slackware Linux

</details>

<details>
<summary><b>What is the difference between Linux and UNIX?</b></summary><br>

UNIX - Only big companies are allowed to use the UNIX copyright and name. IBM AIX, Sun Solaris, and HP-UX all are UNIX operating systems. Most UNIX operating systems are commercial in nature.<br>

- UNIX operating systems are considered as a complete OS as everything come from a single vendor.<br>
- Most UNIX like operating systems are not free.<br>
- UNIX operating systems comes with its own firewall products.<br>
- UNIX supports file systems like jfs, gpfs (AIX), jfs, gpfs (HP-UX), jfs, gpfs (Solaris).<br>

Linux is a Unix clone. But if you consider Portable Operating System Interface (POSIX) standards then Linux can be considered as UNIX.<br>

- Linux is Free. You can download it from the Internet or redistribute it under GNU licenses.<br>
- All Linux distributions include GUI system, GNU utilities, installation & management tools, GNU c/c++ Compilers, Editors (vi), and various applications like OpenOffice, Firefox.<br>
- Linux comes with open source Netfilter and IPTables based firewall tool to protect your server and desktop from the crackers and hackers.<br>
- By default, Linux supports and use ext3 or ext4 file systems.

</details>

<details>
<summary><b>What are some common things between Linux and UNIX?</b></summary><br>

- GUI, file, and windows managers (KDE, Gnome)<br>
- Shells (ksh, csh, bash)<br>
- Various office applications such as OpenOffice.org<br>
- Development tools like perl, php, python, GNU c/c++ compilers<br>
- Posix interface<br>

</details>

<details>
<summary><b>What is Linux and also explain the basic components of this?</b></summary><br>

Linux operating system is consist of 3 components which are as below:<br>

- <b>Kernel</b>: Linux is a monolithic kernel that is free and open source <br>software that is responsible for managing hardware resources for the users.
- <b>System Library</b>: System Library plays a vital role because application programs access Kernels feature using system library.<br>
- <b>System Utility</b>: System Utility performs specific and individual level tasks.

</details>

<details>
<summary><b>What do you understand by CLI?</b></summary><br>

CLI is an acronym for Command Line Interface. We have to provide the information to the computer so that it can perform the function accordingly. In Linux, CLI is the interface that provides the user an interface so that user can type the commands and it complete the tasks. CLI is very easy to use, but it should be typed very precisely.

</details>

<details>
<summary><b>What is your favourite shell and why?</b></summary><br>

BASH as my favorite. It’s really a preferential kind of thing, where I love the syntax and it just "clicks" for me. The input/output redirection syntax (<code>>></code>, <code><< 2>&1</code>, <code>2></code>, <code>1></code>, etc) is similar to C++ which makes it click even easier in my mind.<br>

I also like ZSH shell because is much much more customizable than BASH. It has great Oh-My-Zsh framework, powerful context based tab completion, pattern matching/globbing on alien steroids, loadable modules and more.

</details>

<details>
<summary><b>What is the user ID?</b></summary><br>

Also called login name, logon name, sign-in name, sign-on name. a unique sequence of characters used to identify a user and allow access to a computer system, computer network, or online account. the part of an email address before the @ sign.

</details>

<details>
<summary><b>Describe the root account in Unix-like systems.</b></summary><br>

The root account is like a systems administrator account, and allows you full control of the system. Root always has a UID of zero.

</details>

<details>
<summary><b>How do you find who is logged in?</b></summary><br>

Use this command to find who logged in: <code>w</code>.

</details>

<details>
<summary><b>What is the UID and GID?</b></summary><br>

Unix-like operating systems identify a user within the kernel by a value called a user identifier, often abbreviated to user ID or UID. The UID, along with the group identifier (GID) and other access control criteria, is used to determine which system resources a user can access.

</details>

<details>
<summary><b>Which command is used to review boot messages?</b></summary><br>

<code>dmesg</code> command is used to review boot messages. This command will display system messages contained in the kernel ring buffer. We can use this command immediately after booting to see boot messages. A ring buffer is a buffer of fixed size for which any new data added to it overwrites the oldest data in it.

</details>

<details>
<summary><b>What is the swap space?</b></summary><br>

Swap space is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space. While swap space can help machines with a small amount of RAM, it should not be considered a replacement for more RAM. Swap space is located on hard drives, which have a slower access time than physical memory.

</details>

<details>
<summary><b>How to check memory stats and CPU stats?</b></summary><br>

Using <code>free</code> and <code>vmstat</code> command we can display the physical and virtual memory statistics respectively. With the help of <code>sar</code> command we see the CPU utilization & other stats.

</details>

<details>
<summary><b>What is load average?</b></summary><br>

Is the average system load calculated over a given period of time of 1, 5 and 15 minutes. Lower numbers are better. Higher numbers represent a problem or an overloaded machine.

</details>

<details>
<summary><b>How to create partition and filesystem?</b></summary><br>

1) <code>fdisk</code> or <code>gparted</code> - create a new partition<br>
2) <code>mkfs</code> - create a new filesystem

</details>

<details>
<summary><b>Where journaling is dedicated?</b></summary><br>

Journaling has a dedicated area in the file system, where all the changes are tracked. When the system crashes, the possibility of file  system corruption is less because of journaling.

</details>

<details>
<summary><b>What are the kinds of permissions under Unix-like?</b></summary><br>

- <b>Read</b>: users can read the files or list the directory<br>
- <b>Write</b>: users may write to the file or add new files to the directory<br>
- <b>Execute</b>: users may run the file or lookup a specific file within a directory

</details>

<details>
<summary><b>Where is password file located in Linux?</b></summary><br>

Linux passwords are stored in the <b>/etc/shadow</b> file. They are salted and the algorithm being used depends on the particular distribution and is configurable.

</details>

<details>
<summary><b>How do you change directory and subdirectory with file permissions in Linux/UNIX?</b></summary><br>

To change all the directories eg. to 755 (drwxr-xr-x):<br>

<code>
find /opt/data -type d -exec chmod 755 {} \;
</code><br><br>

To change all the files eg. to 644 (-rw-r--r--):<br>

<code>
find /opt/data -type f -exec chmod 644 {} \;
</code><br><br>

</details>

<details>
<summary><b>What is redirection?</b></summary><br>

It’s a fairly simple process, allowing you to direct data from one output to another. You can also use it to direct an output as an input to another process.

</details>

<details>
<summary><b>What is grep command?</b></summary><br>

<code>grep</code> searches file patterns. If you are looking for a specific pattern in the output of another command, grep highlights the relevant lines. Use this grep command for searching log files, specific processes, and more.<br>

</details>

<details>
<summary><b>Explain file content commands along with the description.</b></summary><br>

- <b>head</b>: to check the starting of a file.<br>
- <b>tail</b>: to check the ending of the file. It is the reverse of head command.<br>
- <b>cat</b>: used to view, create, concatenate the files.<br>
- <b>more</b>: used to display the text in the terminal window in pager form.<br>
- <b>less</b>: used to view the text in the backward direction and also provides single line movement.

</details>

<details>
<summary><b>Explain SIGHUP, SIGINT, SIGKILL and SIGTERM Posix signals.</b></summary><br>

- <b>SIGHUP</b> - the SIGHUP signal is sent to a process when its controlling terminal is closed. It was originally designed to notify the process of a serial line drop (a hangup). Many daemons will reload their configuration files and reopen their logfiles instead of exiting when receiving this signal.<br>
- <b>SIGINT</b> - the SIGINT signal is sent to a process by its controlling terminal when a user wishes to interrupt the process. This is typically initiated by pressing Ctrl+C, but on some systems, the "delete" character or "break" key can be used.<br>
- <b>SIGKILL</b> - the SIGKILL signal is sent to a process to cause it to terminate immediately (kill). In contrast to SIGTERM and SIGINT, this signal cannot be caught or ignored, and the receiving process cannot perform any clean-up upon receiving this signal.<br>
- <b>SIGTERM</b> - the SIGTERM signal is sent to a process to request its termination. Unlike the SIGKILL signal, it can be caught and interpreted or ignored by the process. This allows the process to perform nice termination releasing resources and saving state if appropriate. SIGINT is nearly identical to SIGTERM.

</details>

<details>
<summary><b>How do you terminate an ongoing process?</b></summary><br>

The <code>kill</code> command is used on Linux and other Unix-like operating systems. Explain how every process in the system is identified by a unique process id or pid.<br>

Using the <code>kill</code> command followed by pid terminates that process. You can add a line on how to terminate all processes at once, by using <code>kill 0</code>.

</details>

<details>
<summary><b>What is the difference between "rm" and "rm -r"?</b></summary><br>

<code>rm</code> removes files and <code>-rf</code> are to options:<br>

- <code>-r</code> remove directories and their contents recursively<br>
- <code>-f</code> ignore nonexistent files, never prompt

</details>

<details>
<summary><b>How do you list contents of archive.tgz and extract only one file?</b></summary><br>

<code>
tar tf archive.tgz
</code><br>
<code>
tar xf archive.tgz filename
</code><br>

</details>

###### Network Questions

<details>
<summary><b>What are the default ports used for SMTP, FTP, DNS, DHCP and SSH protocols?</b></summary><br>

<table style="width:100%">
  <tr>
    <th>SERVICE</th>
    <th>PORT</th>
  </tr>
  <tr>
    <td>SMTP</td>
    <td>25</td>
  </tr>
  <tr>
    <td>FTP</td>
    <td>20 for data transfer and 21 for connection established</td>
  </tr>
  <tr>
    <td>DNS</td>
    <td>53</td>
  </tr>
  <tr>
    <td>DHCP</td>
    <td>67/UDP for DHCP server, 68/UDP for DHCP client</td>
  </tr>
  <tr>
    <td>SSH</td>
    <td>22</td>
  </tr>
</table>

</details>

<details>
<summary><b>How to check default route and routing table?</b></summary><br>

Using the commands <code>netstat -nr</code>, <code>route -n</code> or <code>ip route show</code> we can see the default route and routing tables.

</details>

<details>
<summary><b>Why should you avoid telnet to administer a system remotely?</b></summary><br>

Telnet uses most insecure method for communication. It sends data across the network in plain text format and anybody can easily find out the password using the network tool. In the case of Telnet, these include the passing of login credentials in plain text, which means anyone running a sniffer on your network can find the information he needs to take control of a device in a few seconds by eavesdropping on a Telnet login session.

</details>

### :diamond_shape_with_a_dot_inside: <a name="regular-sysadmin">Regular Sysadmin</a>

28 Questions.

###### System Questions

<details>
<summary><b>Explain Linux Boot Sequence.</b></summary><br>

<b>BIOS</b>: Full form of BIOS is Basic Input or Output System that performs integrity checks and it will search and load and then it will execute the bootloader.<br>

<b>MBR</b>: MBR means Master Boot Record. MBR contains the information regarding GRUB and executes and loads this bootloader.<br>

<b>GRUB</b>: GRUB means Grand Unified Bootloader. In case, many kernel images are installed on your system then you can select which one you want to execute.<br>

<b>Kernel</b>: Root file system is mounted by Kernel and executes the <code>/sbin/init</code> program.<br>

<b>Init</b>: Init checks the file <code>/etc/inittab</code> and decides the run level. There are seven-run levels available from 0-6. It will identify the default init level and will load the program.<br>

<b>Runlevel programs</b>: As per your default settings for the run level, the system will execute the programs.

</details>

<details>
<summary><b>What is the name and path of the main system log?</b></summary><br>

By default, the main system log is <b>/var/log/messages</b>. This file contains all the messages and the script written by the user.

By default all scripts are saved in this file. This is the standard system log file, which contains messages from all system software, non-kernel boot issues, and messages that go to <code>dmesg</code> (is a system file that is written upon system boot).

</details>

<details>
<summary><b>Explain /proc filesystem.</b></summary><br>

<b>/proc</b> is a virtual file system that provides detailed information about kernel, hardware and running processes.

Since <b>/proc</b> contains virtual files, it is called virtual file system. These virtual files have unique qualities. Most of them are listed as zero bytes in size.<br>

Virtual files such as <b>/proc/interrupts</b>, <b>/proc/meminfo</b>, <b>/proc/mounts</b> and <b>/proc/partitions</b> provide an up-to-the-moment glimpse of the system’s hardware. Others: <b>/proc/filesystems</b> file and the <b>/proc/sys/</b> directory provide system configuration information and interfaces.

</details>

<details>
<summary><b>Why when load is 1.00 on one-core machine is not ideal?</b></summary><br>

The problem with a load of 1.00 is that you have no headroom. In practice, many sysadmins will draw a line at 0.70:<br>

The "Need to Look into it" Rule of Thumb: 0.70 If your load average is staying above > 0.70, it's time to investigate before things get worse.<br>

The "Fix this now" Rule of Thumb: 1.00. If your load average stays above 1.00, find the problem and fix it now. Otherwise, you're going to get woken up in the middle of the night, and it's not going to be fun.<br>

Rule of Thumb: 5.0. If your load average is above 5.00, you could be in serious trouble, your box is either hanging or slowing way down, and this will (inexplicably) happen in the worst possible time like in the middle of the night or when you're presenting at a conference. Don't let it get there.

</details>

<details>
<summary><b>What is umask? How to set it permanently for a user?</b></summary><br>

On Linux and other Unix-like operating systems, new files are created with a default set of permissions. Specifically, a new file's permissions may be restricted in a specific way by applying a permissions "mask" called the umask. The umask command is used to set this mask, or to show you its current value.<br>

Permanently change (set eg. <code>umask 02</code>):<br>

- <b>~/.profile</b><br>
- <b>~/.bashrc</b><br>
- <b>~/.zshrc</b><br>
- <b>~/.cshrc</b>

</details>

<details>
<summary><b>What are symbolic links?</b></summary><br>

A symbolic link, also termed a soft link, is a special kind of file that points to another file, much like a shortcut in Windows or a Macintosh alias. Unlike a hard link, a symbolic link does not contain the data in the target file. It simply points to another entry somewhere in the file system.

</details>

<details>
<summary><b>List out the differences between softlink and hardlink?</b></summary><br>

a) Hardlink cannot be created for directories. Hard link can only be created for a file.<br>

b) Softlink also termed a symbolic links or symlinks can link to a directory.

</details>

<details>
<summary><b>What is the sticky-bit?</b></summary><br>

A Sticky bit is a permission bit that is set on a file or a directory that lets only the owner of the file/directory or the root user to delete or rename the file. No other user is given privileges to delete the file created by some other user.

</details>

<details>
<summary><b>How to change the default run level in Linux?</b></summary><br>

To change the run level we have to edit the file <b>/etc/inittab</b> and change initdefault entry (<code>id:5:initdefault</code>:). Using <code>init</code> command we change the run level temporary like <code>init 3</code>, this command will move the system in runlevl 3.

</details>

<details>
<summary><b>How to add & change the Kernel parameters?</b></summary><br>

To set the kernel parameters in UNIX-like, first edit the file <code>/etc/sysctl.conf</code> after making the changes save the file and run the command <code>sysctl -p</code>, this command will make the changes permanently without rebooting the machine.

</details>

<details>
<summary><b>What is the difference between ext2, ext3 and ext4 file systems?</b></summary>
<br>

<b>ext2</b><br>

- ext2 stands for second extended file system.<br>
- ext2 does not have journaling feature.<br>
- on flash drives, usb drives, ext2 is recommended, as it doesn’t need to do the over head of journaling.<br>
- maximum individual file size can be from 16 GB to 2 TB.<br>
- overall ext2 file system size can be from 2 TB to 32 TB.<br>

<b>ext3</b><br>

- ext3 stands for third extended file system.<br>
- starting from Linux Kernel 2.4.15 ext3 was available.<br>
- the main benefit of ext3 is that it allows journaling.<br>
- maximum individual file size can be from 16 GB to 2 TB.<br>
- overall ext3 file system size can be from 2 TB to 32 TB.<br>
- you can convert a ext2 file system to ext3 file system directly (without backup/restore).<br>

<b>ext4</b><br>

- ext4 stands for fourth extended file system.<br>
- starting from Linux Kernel 2.6.19 ext4 was available.<br>
- supports huge individual file size and overall file system size.<br>
- maximum individual file size can be from 16 GB to 16 TB.<br>
- overall maximum ext4 file system size is 1 EB (exabyte). 1 EB = 1024 PB (petabyte). 1 PB = 1024 TB (terabyte).<br>
- directory can contain a maximum of 64,000 subdirectories (as opposed to 32,000 in ext3).<br>
- you can also mount an existing ext3 fs as ext4 fs (without having to upgrade it).<br>
- several other new features are introduced in ext4: multiblock  allocation, delayed allocation, journal checksum, fast fsck, etc.<br>
- in ext4, you also have the option of turning the journaling feature "off".

</details>

<details>
<summary><b>Explain three types of journaling in ext3/ext4.</b></summary><br>

There are three types of journaling available in ext3/ext4 file systems:

- <b>Journal</b> - metadata and content are saved in the journal.<br>
- <b>Ordered</b> - only metadata is saved in the journal. Metadata are  journaled only after writing the content to disk. This is the default.<br>
- <b>Writeback</b> - only metadata is saved in the journal. Metadata might be  journaled either before or after the content is written to the disk.

</details>

<details>
<summary><b>What is an Inode?</b></summary><br>

An inode is a data structure on a filesystem on Linux and other Unix-like operating systems that stores all the information about a file except its name and its actual data. A data structure is a way of storing data so that it can be used efficiently.<br>

A Unix file is "stored" in two different parts of the disk - the data blocks and the inodes. (I won't get into superblocks and other esoteric information.) The data blocks contain the "contents" of the file. The information about the file is stored elsewhere - in the inode.

</details>

<details>
<summary><b>How to increase the size of LVM partition?</b></summary><br>

Use the <code>lvextend</code> command for resize LVM partition.<br>

- extending the size by 500MB:<br>
<code>
lvextend -L +500M /dev/vgroup/lvolume
</code><br><br>

- extending all available free space:<br>
<code>
lvextend -l +100%FREE /dev/vgroup/lvolume
</code><br><br>

and `resize2fs` or `xfs_growfs` to resize filesystem:<br>

- for ext filesystems:<br>
<code>
resize2fs /dev/vgroup/lvolume
</code><br><br>

- for xfs filesystem:<br>
<code>
xfs_growfs mountpoint_for_/dev/vgroup/lvolume
</code><br><br>

</details>

<details>
<summary><b>Describe a process to create partition, lvm and filesystem.</b></summary><br>

1. Create partition<br>

<code>
fdisk /dev/sdb
</code><br><br>

2. Create LVM<br>

<code>
pvcreate /dev/sdb1
vgcreate vg0 /dev/sdb1
lvcreate --name datastore --size 50G vg0
</code><br><br>

3. Create filesystem<br>

<code>
mkfs -t xfs /dev/mapper/vg0-datastore
</code><br>

</details>

<details>
<summary><b>What is the advantage of executing the running processes in the background? How can you do that?</b></summary><br>

The most significant advantage of executing the running process in the background is that you can do any other task simultaneously while other processes are running in the background. So, more processes can be completed in the background while you are working on different processes. It can be achieved by adding a special character '&' at the end of the command.

</details>

<details>
<summary><b>What is a zombie/defunct process?</b></summary><br>

Is a process that has completed execution (via the <b>exit</b> system call) but still has an entry in the process table: it is a process in the "Terminated state".

</details>

<details>
<summary><b>Which algorithms are supported in passwd file?</b></summary><br>

The algorithms supported are MD5, Blowfish, SHA256 and SHA512.

</details>

<details>
<summary><b>What is key-based authentication? Explain.</b></summary><br>

Key-based authentication is a kind of authentication that may be used as an alternative to password authentication. Instead of requiring a user's password, it is possible to confirm the client's identity by using asymmetric cryptography algorithms, with public and private keys.

</details>

<details>
<summary><b>Which utility is used to make automate rotation of a log?</b></summary><br>

Logrotate command is used to make automate rotation of log. It allows automatic rotation, compression, removal, and mailing of log files.

</details>

<details>
<summary><b>What is the use of ulimit in Unix-like systems?</b></summary><br>

Most UNIX-like operating systems, including Linux and BSD, provide ways to limit and control the usage of system resources such as threads, files, and network connections on a per-process and per-user basis. These "ulimits" prevent single users from using too many system resources.

</details>

<details>
<summary><b>What are soft limits and hard limits?</b></summary><br>

Hard limit is the maximum allowed to a user, set by the superuser or root. This value is set in the file <code>/etc/security/limits.conf</code>. The user can increase the soft limit on their own in times of needing more resources, but cannot set the soft limit higher than the hard limit.

</details>

<details>
<summary><b>What is the difference between Cron and Anacron?</b></summary><br>

- one of the main difference between cron and anacron jobs is that cron works on the system that are running continuously that means it is designed for the system that is running24*7. While anacron is used for the systems that are not running continuously.<br>
- other difference between the two is cron jobs can run every minute, but anacron jobs can be run only once a day.<br>
- any normal user can do the scheduling of cron jobs, but the scheduling of anacron jobs can be done by the superuser only.<br>
- cron should be used when you need to execute the job at a specific time as per the given time in cron, but anacron should be used in when there is no any restriction for the timing and can be executed at any time.

</details>

###### Network Questions

<details>
<summary><b>How to check which ports are listening in my Linux Server?</b></summary><br>

Use the <code>netstat -tapn</code> or <code>lsof -i</code>.

</details>

<details>
<summary><b>What does curl command do in Linux?</b></summary><br>

</details>

### :diamond_shape_with_a_dot_inside: <a name="senior-sysadmin">Senior Sysadmin</a>

22 Questions.

###### System Questions

<details>
<summary><b>What are the different types of Kernels? Explain.</b></summary><br>

- <b>Microkernel</b>: This type of kernel only manages CPU, memory, and IPC. This kind of kernel provides portability, small memory footprint and also security.<br>
- <b>Monolithic Kernel</b>: Linux is a monolithic kernel. So, this type of kernel provides file management, system server calls, also manages CPU, IPC as well as device drivers. It provides easier access to the process to communicate and as there is not any queue for processor time, so processes react faster.<br>
- <b>Hybrid Kernel</b>: In this type of kernels, programmers can select what they want to run in user mode and what in supervisor mode. So, this kernel provides more flexibility than any other kernel but it can have some latency problems.

</details>

<details>
<summary><b>What is LD_LIBRARY_PATH?</b></summary><br>

Environment variable LD_LIBRARY_PATH is a colon-separated set of directories where libraries should be searched for first, before the standard set of directories; this is useful when debugging a new library or using a nonstandard library for special purposes.

</details>

<details>
<summary><b>How shadow passwords are given by in Linux?</b></summary><br>

<code>pwconv</code> command is used for giving shadow passwords. Shadow passwords are given for better system security. The <code>pwconv</code> command creates the file <code>/etc/shadow</code> and changes all passwords to 'x' in the <code>/etc/passwd</code> file.

</details>

<details>
<summary><b>Explain all the fields in the /etc/passwd file.</b></summary><br>

- <b>Username</b>: First field is the username that contains the username which is 1 to 32 length characters.<br>
- <b>Password</b>: This field does not show the actual password as the password is encrypted. Here, x character shows that password is encrypted that is located in <code>/etc/shadow</code> file.<br>
- <b>User ID (UID)</b>: All the users created in Linux is given a user ID whenever the user is created. UID 0 is fixed and reserved for the root user.<br>
- <b>Group ID (GID)</b>: This field specifies the name of the group to which the user belongs. The group information is also stored in a file <code>/etc/group</code>.<br>
- <b>User ID Info</b>: Here you can add comments and you can add any extra information related to the users like full name, contact number, etc.<br>
- <b>Home directory</b>: This field provides the path where the user is directed after the login. For example, <code>/home/smith</code>.<br>
- <b>Command/shell</b>: This field provides the path of a command/shell and denotes that user has access to this shell i.e. /bin/bash.

</details>

<details>
<summary><b>What does Sar provides and at which location Sar logs are stored?</b></summary><br>

Sar collect, report or save system activity information. The default version of the sar command (CPU utilization report) might be one of the first facilities the user runs to begin system activity investigation, because it monitors major system resources. If CPU utilization is near 100 percent (user + nice + system), the workload sampled is CPU-bound.

By default log files of Sar command is located at <code>/var/log/sa/sadd</code> file, where the dd parameter indicates the current day.

</details>

<details>
<summary><b>How to scan newly assigned luns on linux box without rebooting?</b></summary><br>

Run the command: <code>echo "---" >/sys/class/scsi_host/hostX/scan</code>.

</details>

<details>
<summary><b>Explain system calls used for process management?</b></summary><br>

There are some system calls used in Linux for process management. These are as follows:<br>

- <code>Fork()</code>: It is used to create a new process<br>
- <code>Exec()</code>: It is used to execute a new process<br>
- <code>Wait()</code>: It is used to make the process to wait<br>
- <code>Exit()</code>: It is used to exit or terminate the process<br>
- <code>Getpid()</code>: It is used to find the unique process ID<br>
- <code>Getppid()</code>: It is used to check the parent process ID<br>
- <code>Nice()</code>: It is used to bias the currently running process property

</details>

<details>
<summary><b>Explain interrupts in Linux and also explain interrupt handlers.</b></summary><br>

Interrupts means the processor is transferred temporarily to another program or function. When that program is completed, the processor will be given back to that program to complete the task.

Interrupt handler is the function that the kernel runs for a specific interrupt. It is also called Interrupt Service Routine. Interrupts handlers are the function that matches a particular prototype and enables the kernel to pass the handler information accurately.

</details>

<details>
<summary><b>How can we edit a file without opening in Linux?</b></summary><br>

For example:<br>

<code>
cat >> /path/to/file << __EOF__
How to Use the VI Editor.
__EOF__
</code><br><br>

</details>

<details>
<summary><b>What is the Pluggable Authentication Modules? Explain.</b></summary><br>

It provides a layer between applications and actual authentication mechanism. It is a library of loadable modules which are called by the application for authentication. It also allows the administrator to control when a user can log in. All PAM applications are configured in the directory <code>/etc/pam.d</code> or in a file <code>/etc/pam.conf</code>. PAM is controlled using the configuration file or the configuration directory.

</details>

<details>
<summary><b>What is strace command in Linux?</b></summary><br>

strace is a powerful command line tool for debugging and trouble shooting programs in Unix-like operating systems such as Linux. It captures and records all system calls made by a process and the signals received by the process.

</details>

<details>
<summary><b>How do you run command every time a file is modified?</b></summary><br>

For example:<br>

<code>
while inotifywait -e close_write filename ; do

  echo "changed" >> /var/log/changed

done
</code><br><br>

</details>

<details>
<summary><b>What is the Superblock?</b></summary><br>

A superblock is a record of the characteristics of a filesystem, including its size, the block size, the empty and the filled blocks and their respective counts, the size and location of the inode tables, the disk block map and usage information, and the size of the block groups.

</details>

<details>
<summary><b>What is the use of Suid?</b></summary><br>

An "s" in the first position means that the SETUID (or SUID) bit was set (the GUID bit is the same thing, at the group level). Linux runs an executable file with the SETUID bit set with the User ID (that is, the privileges!) of the owner of that file, not the one of the user who launched it.

</details>

<details>
<summary><b>What does a kill command do?</b></summary><br>

In Unix and Unix-like operating systems, kill is a command used to send a signal to a process. By default, the message sent is the termination signal, which requests that the process exit. But kill is something of a misnomer; the signal sent may have nothing to do with process killing.

</details>

<details>
<summary><b>Describe exceptions for which the use of SIGKILL is insufficient.</b></summary><br>

- Zombie processes cannot be killed since they are already dead and waiting for their parent processes to reap them.<br>
- Processes that are in the blocked state will not die until they wake up again.<br>
- The init process is special: It does not get signals that it does not want to handle, and thus it can ignore SIGKILL. An exception from this exception is while init is ptraced on Linux.<br>
- An uninterruptibly sleeping process may not terminate (and free its resources) even when sent SIGKILL. This is one of the few cases in which a UNIX system may have to be rebooted to solve a temporary software problem.

</details>

<details>
<summary><b>What was getfacl and setfacl commands do?</b></summary><br>

The command "setfacl" refers to Set File Access Control Lists and "getfacl" refers to Get File Access Control List. Each file and directory in a Linux filesystem is created with a specific set of file permissions for its access. In order to know the access permissions of a file or directory we use getfacl.

</details>

<details>
<summary><b>What is a file descriptor in Linux?</b></summary><br>

In Unix and related computer operating systems, a file descriptor (FD, less frequently fildes) is an abstract indicator (handle) used to access a file or other input/output resource, such as a pipe or network socket. File descriptors form part of the POSIX application programming interface.

</details>

<details>
<summary><b>What is an open file table?</b></summary><br>

The process table entry (aka process control block) contains a table, the file descriptor table that gives the mapping between the descriptor the process uses to refer to a file connection and the data structure inside the kernel that represents the actual file connection.

</details>

<details>
<summary><b>What's the difference between /sbin/nologin, /bin/false and /bin/true?
</b></summary><br>

When <code>/sbin/nologin</code> is set as the shell, if user with that shell logs in, they'll get a polite message saying 'This account is currently not available.'

<code>/bin/false</code> is just a binary that immediately exits, returning false, when it's called, so when someone who has false as shell logs in, they're immediately logged out when false exits. Setting the shell to <code>/bin/true</code> has the same effect of not allowing someone to log in but false is probably used as a convention over true since it's much better at conveying the concept that person doesn't have a shell.

nologin is the more user-friendly option, with a customizable message given to the user trying to log in, so you would theoretically want to use that; but both nologin and false will have the same end result of someone not having a shell and not being able to ssh in.

</details>

###### Network Questions

<details>
<summary><b>How do you kill program using one port in Linux?</b></summary><br>

To list any process listening to the port 8080:<br>

<code>lsof -i:8080</code>

To kill any process listening to the port 8080:<br>

<code>kill $(lsof -t -i:8080)</code>

or more violently:<br>

<code>kill -9 $(lsof -t -i:8080)</code><br><br>

</details>

## <a name="secret-knowledge">Secret Knowledge</a>

### :diamond_shape_with_a_dot_inside: Guru Sysadmin

0 Questions.
