<p align="center">
    <img src="./sysadmin_preview.png" alt="sysadmin logo">
</p>

<br>

<p align="center">:star:</p>

<p align="center">"<i>A great Admin doesn't need to know everything, but they should be able to come up with amazing solutions to impossible projects.</i>" - cwheeler33 (ServerFault)</p>

<p align="center">:star:</p>

<p align="center">"<i>Systems Administration... [is about] acting as a force multiplier to optimize the effectiveness of other employees.</i>" <br>- Unknown</p>

<br>

<p align="center">
  <a href="https://github.com/dfuentes87/test-your-sysadmin-skills/pulls">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?longCache=true" alt="Pull Requests">
  </a>
  <a href="LICENSE.md">
    <img src="https://img.shields.io/badge/License-MIT-lightgrey.svg?longCache=true" alt="MIT License">
  </a>
</p>

<div align="center">
  <sub>Forked from <a href="https://github.com/trimstray/test-your-sysadmin-skills">trimstray</a>; Brought back to life and updated by <a href="https://github.com/dfuentes87/linux-sysadmin-questions">dfuentes87</a>
</div>

<br>

****

<br>

:information_source: &nbsp;This project contains over **200** questions and answers that can be used to test your general knowledge as a **Linux System Administrator**, or to ask someone interviewing for such a position.

These questions are not meant to be a list of arbitrary facts, such as port numbers that you'll maybe deal with once a year, situations or commands that are rarely encountered, or issues specific to a certain application. Instead these are geared towards real world situations that are common and good to know in general, however not knowing all these does not mean you are not a good Linux SysAdmin.

:heavy_check_mark: &nbsp;The answers are only **examples** and do not exhaust the whole topic. Most of them contains **useful resources** for a deeper understanding.

:warning: &nbsp;Questions marked **`***`** don't have answer yet or answer the is incomplete - **make a pull request to add them**!

:traffic_light: &nbsp;If you find something which doesn't make sense, or something doesn't seem right, **please make a pull request** and please add valid and well-reasoned explanations about your changes or comments.

<br>

### Contributing

If you would like to answer questions or you found an error - fork the repo, add your fixes, and submit a pull request.

#### Using the issue tracker

* Please **do not** use the issue tracker for personal tech support requests.

* Please **do not** derail or troll issues. Keep the discussion on topic and
  respect the opinions of others.

#### Pull requests

When creating a pull request, please heed the following:

- For new answers: try to give an objective, clear, and concise response, including an example if appropriate.
- For changes to answers: explain why you believe the current answer is incorrect and a better response and/or solution. 

<br>

***

<br>

## Table of Contents

| <b><u>The type of chapter</u></b>    | <b><u>Short description</u></b> |
| :---         | :---         |
| <b>[General Knowledge](#general-knowledge)</b> ||
| :small_orange_diamond: [Junior SysAdmin](#junior-sysadmin) | Reasonably simple questions based on basic knowledge. |
| :small_orange_diamond: [Proficient SysAdmin](#proficient-sysadmin) | Mid-level questions that you will probably come across during your first 5 years. |
| :small_orange_diamond: [Senior SysAdmin](#senior-sysadmin) | Advanced questions which may be open-ended, require actual experience to<br> fully understand, or are unique scenarios. |
| <b>[Extra Knowledge](#extra-knowledge)</b> |

<br>

## <a name="general-knowledge">General Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="junior-sysadmin">Junior Sysadmin</a>

###### System Questions

<details>
<summary><b>Give some examples of Unix or Linux distributions. Describe what makes them unique.</b></summary><br>

- Red Hat Enterprise Linux

- AlmaLinux

- Debian

- Ubuntu

- Arch

- Kali

- OpenBSD

- **Arch Linux** offers a minimalist base system on which one can build a custom operating system. The beauty of it is that it has the Arch User Repository (AUR), which when combined with its official binary repositories allows it to probably have the largest repositories of any distribution. Its packaging process is also very simple, which means if one wants a package not in its official repositories or the AUR, it should be easy to make it for oneself.

- **Kali Linux** is a Debian-based Linux distribution aimed at advanced Penetration Testing and Security Auditing. Kali contains several hundred tools which are geared towards various information security tasks, such as Penetration Testing, Security research, Computer Forensics and Reverse Engineering.

- **OpenBSD** is a security-focused OS which emphasizes adherence to strictly open source licensing, sane initial settings, and excellent documentation for everything. It is known for it's superior packet filter firewall and much of the OpenSSH codebase.

Useful resources:

- [List of Linux distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions)
- [Distro Watch](https://distrowatch.com/)

</details>

<details>
<summary><b>In SQL, what is a Primary key? What implicit constraint does it have? ***</b></summary><br>

A primary key is a combination of fields which uniquely specify a row. A Unique key constraint uniquely identified each record in the database. This provides uniqueness for the column or set of columns. This is a special kind of unique key, and it has implicit NOT NULL constraint. It means, Primary key values cannot be NULL.

</details>

<details>
<summary><b>What is BASH? ***</b></summary><br>

*Pending rewrite*

Useful resources:

- [Comparison of command shells](https://en.wikipedia.org/wiki/Comparison_of_command_shells)

</details>

<details>
<summary><b>How do you get help on the command line?</b></summary><br>

- `man` [commandname] can be used to see a description of a command (ex.: `man less`, `man cat`)

- `-h` or `--help` some programs will implement printing instructions when passed this parameter (ex.: `python -h` and `python --help`)

</details>

<details>
<summary><b>What do the fields in <code>ls -al</code> output mean?</b></summary><br>

In the order of output:

```bash
-rwxrw-r--    1    root   root 2048    Jan 13 07:11 db.dump
```

- file permissions,
- number of links,
- owner name,
- owner group,
- file size,
- time of last modification,
- file/directory name

File permissions is displayed as following:

- first character is `-` or `l` or `d`, `d` indicates a directory, a `-` represents a file, `l` is a symlink (or soft link) - special type of file
- three sets of characters, three times, indicating permissions for owner, group and other:
  - `r` = readable
  - `w` = writable
  - `x` = executable

In your example `-rwxrw-r--`, this means the line displayed is:

- a regular file (displayed as `-`)
- readable, writable and executable by owner (`rwx`)
- readable, writable, but not executable by group (`rw-`)
- readable but not writable or executable by other (`r--`)

Useful resources:

- [What do the fields in ls -al output mean? (original)](https://unix.stackexchange.com/questions/103114/what-do-the-fields-in-ls-al-output-mean)

</details>

<details>
<summary><b>In SQL, how do you restrict your query to a certain number of rows, aside from using specific <code>where</code> clauses? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the advantage of executing a process in the background? How can you do that?</b></summary><br>

The advantage of executing processes in the background is that you can do any other task simultaneously. You can do this by adding the special character `&` at the end of the command.

Generally applications that take too long to execute and doesn't require user interaction are sent to background so that we can continue our work in terminal.

For example if you want to download something in background, you can:

```bash
wget https://url-to-download.com/download.tar.gz &
```

When you run the above command you get the following output:

```bash
[1] 2203
```

Here 1 is the serial number of job and 2203 is PID of the job.

You can see the jobs running in background using the following command:

```bash
jobs
```

When you execute job in background it give you a PID of job, you can kill the job running in background using the following command:

```bash
kill PID
```

Replace the PID with the PID of the job. If you have only one job running you can bring it to foreground using:

```bash
fg
```

If you have multiple jobs running in background you can bring any job in foreground using:

```bash
fg %#
```

Replace the `#` with serial number of the job.

Useful resources:

- [How do I run a Unix process in the background?](https://kb.iu.edu/d/afnz)
- [Job Control Commands](http://tldp.org/LDP/abs/html/x9644.html)
- [What is/are the advantage(s) of running applications in background?](https://unix.stackexchange.com/questions/162186/what-is-are-the-advantages-of-running-applications-in-backgound)

</details>

<details>
<summary><b>How can you reduce load time of a dynamic website?</b></summary><br>

- website optimization
- compressed files
- Apache/Nginx tuning
- server-side "caching" (Squid, Varnish, Redis)
- external caching (e.g. Cloudflare)

</details>

<details>
<summary><b>Is running processes as root a good or bad practice?</b></summary><br>

Running (everything) as root is bad because:

- **Stupidity**: nothing prevents you from making a careless mistake. If you try to change the system in any potentially harmful way, you need to use sudo, which ensures a pause (while you're entering the password) to ensure that you aren't about to make a mistake.

- **Security**: harder to hack if you don't know the admin user's login account. root means you already have one half of the working set of admin credentials.

- **You don't really need it**: if you need to run several commands as root, and you're annoyed by having to enter your password several times when `sudo` has expired, all you need to do is `sudo -i` and you are now root. Want to run some commands using pipes? Then use `sudo sh -c "command1 | command2"`.

- **You can always use it in the recovery console**: the recovery console allows you to recover from a major mistake, or fix a problem caused by an app (which you still had to run as `sudo`). Ubuntu doesn't have a password for the root account in this case, but you can search online for changing that - this will make it harder for anyone that has physical access to your box to be able to do harm.

Useful resources:

- [Why is it bad to log in as root? (original)](https://askubuntu.com/questions/16178/why-is-it-bad-to-log-in-as-root)
- [What's wrong with always being root?](https://serverfault.com/questions/57962/whats-wrong-with-always-being-root)
- [Why you should avoid running applications as root](https://bencane.com/2012/02/20/why-you-should-avoid-running-applications-as-root/)

</details>

<details>
<summary><b>How can you check memory and CPU resource usage? ***</b></summary><br>

*Answer needs more details*

You can use `top` for both. Using `free` and `vmstat` command we can display the physical and virtual memory statistics respectively. With the help of `sar` command we see the CPU utilization & other stats (but `sar` isn't even installed in most systems).

Useful resources:

- [How do I Find Out Linux CPU Utilization?](https://www.cyberciti.biz/tips/how-do-i-find-out-linux-cpu-utilization.html)
- [16 Linux server monitoring commands you really need to know](https://www.hpe.com/us/en/insights/articles/16-linux-server-monitoring-commands-you-really-need-to-know-1703.html)

</details>

<details>
<summary><b>What is load average?</b></summary><br>

Linux **load averages** are "system load averages" that show the running thread (task) demand on the system as an average number of running plus waiting threads. This measures demand, which can be greater than what the system is currently processing. Most tools show three averages, for 1, 5, and 15 minutes.

These 3 numbers are not the numbers for the different CPUs. These numbers are mean values of the load number for a given period of time (of the last 1, 5 and 15 minutes).

**Load average** is usually described as "average length of run queue". So few CPU-consuming processes or threads can raise **load average** above 1. There is no problem if **load average** is less than total number of CPU cores. But if it gets higher than number of CPUs, this means some threads/processes will stay in queue, ready to run, but waiting for free CPU.

It is meant to give you an idea of the state of the system, averaged over several periods of time. Since it is averaged, it takes time for it to go back to 0 after a heavy load was placed on the system.

Some interpretations:

- if the averages are 0.0, then your system is idle
- if the 1 minute average is higher than the 5 or 15 minute averages, then load is increasing
- if the 1 minute average is lower than the 5 or 15 minute averages, then load is decreasing
- if they are higher than your CPU count, then you might have a performance problem (it depends)

Useful resources:

- [Linux Load Averages: Solving the Mystery (original)](http://www.brendangregg.com/blog/2017-08-08/linux-load-averages.html)
- [Linux load average - the definitive summary](http://blog.angulosolido.pt/2015/04/linux-load-average-definitive-summary.html)
- [How CPU load averages work (and using them to triage webserver performance!)](https://jvns.ca/blog/2016/02/07/cpu-load-averages/)

</details>

<details>
<summary><b>Where are user passwords stored on Linux/Unix systems?</b></summary><br>

The passwords are not stored anywhere on the system at all. What is stored in `/etc/shadow` are so called hashes of the passwords.

A hash of some text is created by performing a so called one way function on the text (password), thus creating a string to check against. By design it is "impossible" (computationally infeasible) to reverse that process.

Older Unix variants stored the encrypted passwords in `/etc/passwd` along with other information about each account.

Newer ones simply have a `*` in the relevant field in `/etc/passwd` and use `/etc/shadow` to store the password, in part to ensure nobody gets read access to the passwords when they only need the other stuff (`shadow` is usually protected more strongly than `passwd`).

For more info consult `man crypt`, `man shadow`, `man passwd`.

Useful resources:

- [Where is my password stored on Linux?](https://security.stackexchange.com/questions/37050/where-is-my-password-stored-on-linux)
- [Where are the passwords of the users located in Linux?](https://www.cyberciti.biz/faq/where-are-the-passwords-of-the-users-located-in-linux/)
- [Linux Password & Shadow File Formats](https://www.tldp.org/LDP/lame/LAME/linux-admin-made-easy/shadow-file-formats.html)

</details>

<details>
<summary><b>You type <code>CTRL + C</code> but your script still running. How do you stop it? ***</b></summary><br>

To be completed.

Useful resources:

- [How to kill a script running in terminal, without closing terminal (Ctrl + C doesn't work)? (original)](https://askubuntu.com/questions/520107/how-to-kill-a-script-running-in-terminal-without-closing-terminal-ctrl-c-doe)
- [What's the difference between ^C and ^D for Unix/Mac OS X terminal?](https://superuser.com/questions/169051/whats-the-difference-between-c-and-d-for-unix-mac-os-x-terminal)

</details>

<details>
<summary><b>What is <code>grep</code> command? How do you match multiple strings in the same line?</b></summary><br>

The `grep` utilities are a family of Unix tools, including `egrep` and `fgrep`.

`grep` searches file patterns. If you are looking for a specific pattern in the output of another command, `grep` highlights the relevant lines. Use this grep command for searching log files, specific processes, and more.

For match multiple strings:

```bash
grep -E "string1|string2" filename
```

or

```bash
grep -e "string1" -e "string2" filename
```

Useful resources:

- [What is grep, and how do I use it? (original)](https://kb.iu.edu/d/afiy)

</details>

<details>
<summary><b>Explain a few commands to read files without editing them.</b></summary><br>

- `head`: to check the starting of a file.
- `tail`: to check the ending of the file. It is the reverse of head command.
- `cat`: used to view, create, concatenate the files.
- `tac`: same as `cat` but the contents are shown starting from the bottom
- `more`: used to display the text in the terminal window in pager form.
- `less`: used to view the text in the backward direction and also provides single line movement.

Useful resources:

- [5 Commands to View the Content of a File in Linux Command Line](https://linuxhandbook.com/view-file-linux/)

</details>

<details>
<summary><b>Explain the SIGHUP, SIGINT, SIGKILL, and SIGTERM signals.</b></summary><br>

- **SIGHUP** - is sent to a process when its controlling terminal is closed. It was originally designed to notify the process of a serial line drop (a hangup). Many daemons will reload their configuration files and reopen their logfiles instead of exiting when receiving this signal.
- **SIGINT** - is sent to a process by its controlling terminal when a user wishes to interrupt the process. This is typically initiated by pressing `Ctrl+C`, but on some systems, the "delete" character or "break" key can be used.
- **SIGKILL** - is sent to a process to cause it to terminate immediately (kill). In contrast to **SIGTERM** and **SIGINT**, this signal cannot be caught or ignored, and the receiving process cannot perform any clean-up upon receiving this signal.
- **SIGTERM** - is sent to a process to request its termination. Unlike the **SIGKILL** signal, it can be caught and interpreted or ignored by the process. This allows the process to perform nice termination releasing resources and saving state if appropriate. **SIGINT** is nearly identical to **SIGTERM**.

Useful resources:

- [A list of signals and what they mean](https://www-uxsup.csx.cam.ac.uk/courses/moved.Building/signals.pdf)

</details>

<details>
<summary><b>What does <code>kill</code> command do?</b></summary><br>

In Unix and Unix-like operating systems, `kill` is a command used to send a signal to a process. By default, the message sent is the termination signal, which requests that the process exit. But `kill` is something of a misnomer; the signal sent may have nothing to do with process killing.

Useful resources:

- [Mastering the "Kill" Command in Linux](https://www.maketecheasier.com/kill-command-in-linux/)

</details>

<details>
<summary><b>When would you want to use <code>-f</code> for <code>rm</code>? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How can I chmod files using the <code>find</code> command? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Combine multiple shell commands in one line.</b></summary><br>

If you want to execute each command only if the previous one succeeded, then combine them using the `&&` operator:

```bash
cd /my_folder && rm *.jar && svn co path to repo && mvn compile package install
```

If one of the commands fails, then all other commands following it won't be executed.

If you want to execute all commands regardless of whether the previous ones failed or not, separate them with semicolons:

```bash
cd /my_folder; rm *.jar; svn co path to repo; mvn compile package install
```

In your case, I think you want the first case where execution of the next command depends on the success of the previous one.

You can also put all commands in a script and execute that instead:

```bash
#! /bin/sh
cd /my_folder \
&& rm *.jar \
&& svn co path to repo \
&& mvn compile package install
```

Useful resources:

- [Execute combine multiple linux commands in one line (original)](https://stackoverflow.com/questions/13077241/execute-combine-multiple-linux-commands-in-one-line)

</details>

<details>
<summary><b>What symbolic representation can you pass to <code>chmod</code> to give all users execute access to a file without affecting other permissions?</b></summary><br>

```bash
chmod a+x /path/to/file
```

- `a` - for all users
- `x` - for execution permission
- `r` - for read permission
- `w` - for write permission

Useful resources:
- [How to Set File Permissions Using chmod](https://www.washington.edu/computing/unix/permissions.html)
- [What does "chmod +x your_file_name" do and how do I use it?](https://askubuntu.com/questions/443789/what-does-chmod-x-filename-do-and-how-do-i-use-it)

</details>

<details>
<summary><b>How can you mirror the contents of two directories?</b></summary><br>

To sync the contents of **dir1** to **dir2** on the same system, type:

```bash
rsync -av --progress --delete dir1/ dir2
```

- `-a`, `--archive` - archive mode
- `--delete` - delete extraneous files from dest dirs
- `-v`, `--verbose` - verbose mode (increase verbosity)
- `--progress` - show progress during transfer

Useful resources:

- [How can I sync two local directories? (original](https://unix.stackexchange.com/questions/392536/how-can-i-sync-two-local-directories)
- [Synchronizing folders with rsync](https://www.jveweb.net/en/archives/2010/11/synchronizing-folders-with-rsync.html)

</details>

<details>
<summary><b>Many basic maintenance or troubleshooting tasks require you to edit config files. Explain ways to undo the changes you make.</b></summary><br>

- manually make a copy of the file or entire directory before editing using tools such as cp or tar
- for more permanent changes, the best solution is to use version control such as git to keep track of changes

Useful resources:

- [Backup file with .bak before filename extension](https://unix.stackexchange.com/questions/66376/backup-file-with-bak-before-filename-extension)
- [Is it a good idea to use git for configuration file version controlling?](https://superuser.com/questions/1037211/is-it-a-good-idea-to-use-git-for-configuration-file-version-controlling)

</details>

<details>
<summary><b>You have to find all files larger than 20MB. How you do it?</b></summary><br>

```bash
find / -type f -size +20M
```

Useful resources:

- [How can I find files that are bigger/smaller than x bytes?](https://superuser.com/questions/204564/how-can-i-find-files-that-are-bigger-smaller-than-x-bytes)

</details>

<details>
<summary><b>Why do we use <code>sudo su -</code> and not just <code>sudo su</code>?</b></summary><br>

`su` switches the user providing a normal shell with an environment nearly the same as with the user invoking the command.

`su -` invokes a login shell after switching the user. A login shell resets most environment variables, providing a clean base. This is a safer method because it prevents a malicious enviornment from being brought to the new user during the temporary session. It also allows the use of the new enviornment variables.

Useful resources:

- [su vs sudo -s vs sudo -i vs sudo bash](https://unix.stackexchange.com/questions/35338/su-vs-sudo-s-vs-sudo-i-vs-sudo-bash)
- [Why do we use su - and not just su? (original)](https://unix.stackexchange.com/questions/7013/why-do-we-use-su-and-not-just-su)

</details>

<details>
<summary><b>What are the main reasons for keeping old log files?</b></summary><br>

They are essential to investigate issues on the system. **Log management** is absolutely critical for IT security.

Servers, firewalls, and other IT equipment keep log files that record important events and transactions. This information can provide important clues about hostile activity affecting your network from within and without. Log data can also provide information for identifying and troubleshooting equipment problems including configuration problems and hardware failure.

It’s your server’s record of who’s come to your site, when, and exactly what they looked at. It’s incredibly detailed, showing:

- where folks came from
- what browser they were using
- exactly which files they looked at
- how long it took to load each file
- and a whole bunch of other nerdy stuff

Factors to consider:

- legal requirements for retention or destruction
- company policies for retention and destruction
- how long the logs are useful
- what questions you're hoping to answer from the logs
- how much space they take up

By collecting and analyzing logs, you can understand what transpires within your network. Each log file contains many pieces of information that can be invaluable, especially if you know how to read them and analyze them.

Useful resources:

- [How long do you keep log files?](https://serverfault.com/questions/135365/how-long-do-you-keep-log-files)

</details>

<details>
<summary><b>What is an incremental backup?</b></summary><br>

An incremental backup is a type of backup that only copies files that have changed since the previous backup.

Useful resources:

- [What Is Incremental Backup?](https://www.nakivo.com/blog/what-is-incremental-backup/)

</details>

<details>
<summary><b>What is RAID? What is RAID0, RAID1, RAID5, RAID6, RAID10? </b></summary><br>

A **RAID** (Redundant Array of Inexpensive Disks) is a technology that is used to increase the performance and/or reliability of data storage.

- **RAID0**: Also known as disk **striping**, is a technique that breaks up a file and spreads the data across all the disk drives in a RAID group. There are no safeguards against failure
- **RAID1**: A popular disk subsystem that increases safety by writing the same data on two drives. Called "**mirroring**," RAID 1 does not increase write performance, but read performance may equal up to the sum of each disks' performance. However, if one drive fails, the second drive is used, and the failed drive is manually replaced. After replacement, the RAID controller duplicates the contents of the working drive onto the new one
- **RAID5**: It is disk subsystem that increases safety by computing parity data and increasing speed by interleaving data across three or more drives (**striping**). Upon failure of a single drive, subsequent reads can be calculated from the distributed parity such that no data is lost
- **RAID6**: RAID 6 extends RAID 5 by adding another parity block. It requires a minimum of four disks and can continue to execute read and write of any two concurrent disk failures. RAID 6 does not have a performance penalty for read operations, but it does have a performance penalty on write operations because of the overhead associated with parity calculations
- **RAID10**: Also known as **RAID 1+0**, is a RAID configuration that combines disk mirroring and disk striping to protect data. It requires a minimum of four disks, and stripes data across mirrored pairs. As long as one disk in each mirrored pair is functional, data can be retrieved. If two disks in the same mirrored pair fail, all data will be lost because there is no parity in the striped sets

Useful resources:

- [RAID](https://www.prepressure.com/library/technology/raid)

</details>

<details>
<summary><b>Why would you want to mount servers in a rack?</b></summary><br>

- Protecting Hardware
- Proper Cooling
- Organized Workspace
- Better Power Management
- Cleaner Environment

Useful resources:

- [5 Reasons to Rackmount Your PC](https://www.racksolutions.com/news/custom-projects/5-reasons-to-rackmount-pc/)

</details>

###### Network Questions

<details>
<summary><b>Describe the steps for a successful DHCP handshake process.</b></summary><br>

1. Discover - The DHCP client broadcasts a DHCPDISCOVER message on the network subnet using the destination address 255.255.255.255 (limited broadcast) or the specific subnet broadcast address (directed broadcast). A DHCP client may also request its last known IP address.

2. Offer - When a DHCP server receives a DHCPDISCOVER message from a client, the DHCP server reserves an IP address for the client and makes a lease offer by sending a DHCPOFFER message to the client.

3. Request - In response to the DHCP offer, the client replies with a DHCPREQUEST message, broadcast to the server, requesting the offered address. Before claiming an IP address, the client will broadcast an ARP request, in order to find if there is another host present in the network with the proposed IP address. If there is no reply, this address does not conflict with that of another host, so it is free to be used. 

4. Acknowledge - The DHCP server sends a DHCPACK packet to the client. This packet includes the lease duration and any other configuration information that the client might have requested. At this point, the IP configuration process is completed. 

Useful resources:

- [DHCP Operation](https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol#Operation)

</details>

<details>
<summary><b>What are the most important things to understand about the OSI model?</b></summary><br>

The most important things to understand about the **OSI** model are:

- we can divide up protocols into layers
- layers provide encapsulation
- layers provide abstraction
- layers decouple functions from others

Useful resources:

- [OSI Model and Networking Protocols Relationship](https://networkengineering.stackexchange.com/questions/6380/osi-model-and-networking-protocols-relationship)

</details>

<details>
<summary><b>What is the difference between TCP and UDP? When is one better used than the other? ***</b></summary><br>

| TCP | UDP |
| :--- | :--- |
| TCP stands for Transmission Control Protocol | UDP is stands for User Datagram Protocol or Universal Datagram Protocol |
| Once the connection is setup, data can be sent bi-directional, i.e. TCP is a connection oriented protocol | UDP is connectionless, simple protocol. Using UDP, messages are sent as packets |
| TCP is slower than UDP | UDP is faster compared to TCP |
| TCP is used for applications where time is not critical part of data transmission | UDP is suitable for the applications which require fast transmission of data and time is crucial in this case. |
| TCP transmission occurs in a sequential manner | UDP does not guarantee data is received in the same order when it reaches the destination |
| TCP tracks the data sent to ensure no data loss during data transmission | UDP does not ensure whether receiver receives packets are not. If packets are misses then they are just lost |

</details>

<details>
<summary><b>What is a Proxy Server? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How do you check default route and routing table?</b></summary><br>

Using the commands `netstat -nr`, `route -n` or `ip route show` we can see the default route and routing tables.

Useful resources:

- [How to check routes (routing table) in linux](https://howto.lintel.in/how-to-check-routes-routing-table-in-linux/)

</details>

<details>
<summary><b>What are 127.0.0.1 and localhost?</b></summary><br>

127.0.0.1 is the loopback connection on your network interface card (NIC); pinging this address will see if it is responding. If the ping is successful, then the hardware is good. If the ping isn't successful, the NIC may have issues.

127.0.0.1 and localhost mean the same thing in most cases, but can be treated differently in some situations. The main difference is that you still have to do an actual lookup of localhost somewhere. If you use `127.0.0.1`, the request is directly against the IP address. Otherwise, the name has to be resolved.

Useful resources:

- [What is the difference between 127.0.0.1 and localhost?](https://stackoverflow.com/questions/7382602/what-is-the-difference-between-127-0-0-1-and-localhost)
- [localhost vs. 127.0.0.1](https://stackoverflow.com/questions/3715925/localhost-vs-127-0-0-1)

</details>

<details>
<summary><b>Server A can't talk to Server B. Describe possible reasons in a few steps.</b></summary><br>

To troubleshoot communication problems between servers, it is better to ideally follow the TCP/IP stack:

1. **Application Layer**: are the services up and running on both servers? Are they correctly configured (eg. bind the correct IP and correct port)? Do application and system logs show meaningful errors?

2. **Transport Layer**: are the ports used by the application open (try telnet!)? Is it possible to ping the server?

3. **Network Layer**: is there a firewall on the network or on the OS correctly configured? Is the IP stack correctly configured (IP, routes, dns, etc.)? Are switches and routers working (check the ARP table!)?

4. **Physical Layer**: are the servers connected to a network? Are packets being lost?

</details>

<details>
<summary><b>How can you resolve a domain name, using external dns, with CLI? Can IPs be resolved to domain names?</b></summary><br>

Examples to a resolve an IP address from a domain name:

```bash
# with host command:
host domain.com 8.8.8.8

# with dig command:
dig @9.9.9.9 google.com

# with nslookup command:
nslookup domain.com 8.8.8.8
```

You can resolve an IP Address back to a hostname if the IP Address is stored in a **PTR** DNS record.

```bash
dig -x 1.2.3.4
```

To lookup the IPv6 address for a host:

```bash
dig AAAA domain.com
```

Useful resources:

- [How can I resolve a hostname to an IP address in a Bash script?](https://unix.stackexchange.com/questions/20784/how-can-i-resolve-a-hostname-to-an-ip-address-in-a-bash-script)
- [How To Resolve IP Addresses To Domain Names?](https://superuser.com/questions/315687/how-to-resolve-ip-addresses-to-domain-names)

</details>

<details>
<summary><b>How do you test port connectivity with <code>telnet</code> or <code>nc</code>?</b></summary><br>

```bash
# with telnet command:
telnet code42.example.com 5432

# with nc (netcat) command:
nc -vz code42.example.com 5432
```

</details>

<details>
<summary><b>What are the ports used for FTP and SFTP, and how is each used? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between Hub, Switch, and Router? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is SSH and how does it work?</b></summary><br>

**SSH** stands for **Secure Shell**. It is a protocol that lets you access another machine through a shell session.

An **SSH** connection to be established, the remote machine (server A) must be running an **SSH** daemon and the user's computer must have an **SSH** client.

The **SSH** daemon and **SSH** client listen for connections on a specific network port (default 22), authenticates connection requests, and spawns the appropriate environment if the user provides the correct credentials.

Useful resources:

- [Understanding the SSH Encryption and Connection Process](https://www.digitalocean.com/community/tutorials/understanding-the-ssh-encryption-and-connection-process)

</details>

<details>
<summary><b>What are IP classes? How is it different from CIDR (classless)?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explain the function of each of the following DNS records: SOA, PTR, A, MX, and CNAME.</b></summary><br>

**DNS records** are basically mapping files that tell the DNS server which IP address each domain is associated with, and how to handle requests sent to each domain. Some **DNS records** syntax that are commonly used in nearly all DNS record configurations are `A`, `AAAA`, `CNAME`, `MX`, `PTR`, `NS`, `SOA`, `SRV`, `TXT`, and `NAPTR`.

- **SOA** - A Start Of Authority
- **A** - Address Mapping records
- **AAAA** - IP Version 6 Address records
- **CNAME** - Canonical Name records
- **MX** - Mail exchanger record
- **NS** - Name Server records
- **PTR** - Reverse-lookup Pointer records

Useful resources:

- [List of DNS record types](https://en.wikipedia.org/wiki/List_of_DNS_record_types)

</details>

<details>
<summary><b>What is a MAC address and how is it determined? ***</b></summary><br>

To be completed.

- [How is the MAC address on a computer determined?](https://superuser.com/questions/504770/how-is-the-mac-address-on-a-computer-determined)

</details>

<details>
<summary><b>What is the smallest IPv4 subnet that can be applied to a network containing up to 200 devices? ***</b></summary><br>

To be completed.

Useful resources:

- [How do you calculate the prefix, network, subnet, and host numbers?](https://networkengineering.stackexchange.com/questions/7106/how-do-you-calculate-the-prefix-network-subnet-and-host-numbers)
- [The slash after an IP Address - CIDR Notation](https://networkengineering.stackexchange.com/questions/3697/the-slash-after-an-ip-address-cidr-notation)
- [IP Calculator](http://jodies.de/ipcalc)

</details>

<details>
<summary><b>What are some common HTTP status codes?</b></summary><br>

- **1xx** - Informational responses - communicates transfer protocol-level information
- **2xx** - Success - indicates that the client’s request was accepted successfully
- **3xx** - Redirection - indicates that the client must take some additional action in order to complete their request
- **4xx** - Client side error - this category of error status codes points the finger at clients
- **5xx** - Server side error - the server takes responsibility for these error status codes

Useful resources:

- [HTTP Status Codes](https://httpstatuses.com/)

</details>

###### DevOps Questions

<details>
<summary><b>What is DevOps?</b></summary><br>

**DevOps** is a cohesive team that engages in both Development and Operations tasks, or it's individual Operations and Development teams that work very closely together. It's more of a "way" of working collaboratively with other departments to achieve common goals.

</details>

<details>
<summary><b>What is a version control? What are atomic commits? ***</b></summary><br>

It is a system that records changes to a file or set of files over time so that you can recall specific versions later. Version control systems consist of a central shared repository where teammates can commit changes to a file or set of file. Then you can mention the uses of version control.

Version control allows you to:

- revert files back to a previous state
- revert the entire project back to a previous state
- compare changes over time
- see who last modified something that might be causing a problem
- who introduced an issue and when

*Answer atomic commits question*

Useful resources:

- [Getting Started - About Version Control (original)](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)

</details>

<details>
<summary><b>Explain some basic <code>git</code> commands.</b></summary><br>

- `git init` - create a new local repository
- `git commit -m "message"` - commit changes to head
- `git status` - list the files you've added with `git add` and also commit any files you've changed since then
- `git push origin master` - send changes to the master branch of your remote repository

</details>

<details>
<summary><b>Explain a simple Continuous Integration pipeline.</b></summary><br>

- clone repository
- deploy stage (QA)
- testing environment (QA)
- deploy stage (PROD)

</details>

<details>
<summary><b>Explain some basic <code>Docker</code> commands.</b></summary><br>

- `docker ps` - show running containers
- `docker ps -a` - show all containers
- `docker images` - show docker images
- `docker logs <container-id|container-name>` - get logs from container
- `docker network ls` - show all docker networks
- `docker volumes ls` - show all docker volumes
- `docker exec -it <container-id|container-name> bash` - execute bash in container with interactive shell

</details>

###### Cyber Security Questions

<details>
<summary><b>What makes a password very strong? ***</b></summary><br>

To be completed.

Useful resources:
- [Password Strength](https://xkcd.com/936/)
- [Short complex password, or long dictionary passphrase?](https://security.stackexchange.com/questions/6095/xkcd-936-short-complex-password-or-long-dictionary-passphrase)

</details>

<details>
<summary><b>What is a Security Misconfiguration?</b></summary><br>

**Security misconfiguration** is a vulnerability when a device/application/network is configured in a way which can be exploited by an attacker to take advantage of it. This can be as simple as leaving the default username/password unchanged or too simple for device accounts etc.

</details>

<details>
<summary><b>Most tutorials suggest using SSH key authentication rather than password authentication. Why is it considered more secure?</b></summary><br>

An **SSH key** is an access credential in the SSH protocol. Its function is similar to that of user names and passwords, but the keys are primarily used for automated processes and for implementing single sign-on by system administrators and power users.

Instead of requiring a user's password, it is possible to confirm the client's identity by using asymmetric cryptography algorithms, with public and private keys.

If your SSH service only allows public-key authentication, an attacker needs a copy of a private key corresponding to a public key stored on the server.

If your SSH service allows password based authentication, then your Internet connected SSH server will be hammered day and night by bot-nets trying to guess user-names and passwords. The bot net needs no information, it can just try popular names and popular passwords. Apart from anything else this clogs your logs.

Useful resources:

- [Key-Based Authentication (Public Key Authentication)](http://www.crypto-it.net/eng/tools/key-based-authentication.html)
- [SSH password vs. key authentication](https://security.stackexchange.com/questions/33381/ssh-password-vs-key-authentication)

</details>

<details>
<summary><b>Define the three major terms in cybersecurity (Confidentiality, Integrity, and Availability). ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between threats, vulnerabilities, and attacks? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Describe Threat Modeling. ***</b></summary><br>

To be completed.

</details>

<br>

### :diamond_shape_with_a_dot_inside: <a name="proficient-sysadmin">Proficient Sysadmin</a>

###### System Questions

<details>
<summary><b>Explain briefly how Linux allows most of it's software to be updated without needing to reboot? Is it possible to update the kernel without rebooting?</b></summary><br>

To be completed.

Useful resources:

- [How does Linux update without a reboot? - Quora ](https://www.quora.com/How-does-Linux-update-without-a-reboot)
- [Updating Linux Kernel Without Reboots](https://blog.kernelcare.com/updating-linux-kernel-without-reboots-live-patching-tools-overview)

</details>

<details>
<summary><b>Difference between <code>nohup</code>, <code>disown</code>, and <code>&</code>. What happens when using all together?</b></summary><br>

- `&` puts the job in the background, that is, makes it block on attempting to read input, and makes the shell not wait for its completion
- `disown` removes the process from the shell's job control, but it still leaves it connected to the terminal. One of the results is that the shell won't send it a **SIGHUP**. Obviously, it can only be applied to background jobs, because you cannot enter it when a foreground job is running
- `nohup` disconnects the process from the terminal, redirects its output to `nohup.out` and shields it from **SIGHUP**. One of the effects (the naming one) is that the process won't receive any sent **SIGHUP**. It is completely independent from job control and could in principle be used also for foreground jobs (although that's not very useful)

If you use all three together, the process is running in the background, is removed from the shell's job control and is effectively disconnected from the terminal.

Useful resources:

- [Difference between nohup, disown and & (original)](https://unix.stackexchange.com/questions/3886/difference-between-nohup-disown-and)

</details>

<details>
<summary><b>Pick two different computer languages. Describe when you would use one over the other. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Why is the <code>mktemp</code> command useful? Present an example of use.</b></summary><br>

<code>mktemp</code> randomizes the name. It is very important from the security point of view.

Just imagine that you do something like:

```bash
echo "random_string" > /tmp/temp-file
```

in your root-running script. And someone (who has read your script) does

```bash
ln -s /etc/passwd /tmp/temp-file
```

The <code>mktemp</code> command could help you in this situation:

```bash
TEMP=$(mktemp /tmp/temp-file.XXXXXXXX)
echo "random_string" > ${TEMP}
```

Now this <code>ln /etc/passwd</code> attack will not work.

</details>

<details>
<summary><b>In what circumstance can <code>df</code> and <code>du</code> disagree on available disk space? How do you solve it?</b></summary><br>

`du` checks usage of directories, but `df` checks free'd inodes, and files can be held open and take space after they're deleted.

**Solution 1**

Check for files on located under mount points. Frequently if you mount a directory (say a sambafs) onto a filesystem that already had a file or directories under it, you lose the ability to see those files, but they're still consuming space on the underlying disk.

I've had file copies while in single user mode dump files into directories that I couldn't see except in single usermode (due to other directory systems being mounted on top of them).

**Solution 2**

On the other hand `df -h` and `du -sh` could mismatched by about 50% of the hard disk size. This was caused by e.g. Apache (httpd) keeping large log files in memory which had been deleted from disk.

This was tracked down by running `lsof | grep "/var" | grep deleted` where `/var` was the partition I needed to clean up.

The output showed lines like this:

```
httpd     32617    nobody  106w      REG        9,4 1835222944     688166 /var/log/apache/awstats_log (deleted)
```

The situation was then resolved by restarting Apache (`service httpd restart`) and cleared of disk space, by allowing the locks on deleted files to be cleared.

Useful resources:

- [Why du and df display different values in Linux and Unix](https://linuxshellaccount.blogspot.com/2008/12/why-du-and-df-display-different-values.html)

</details>

<details>
<summary><b>Every command fails with <code>command not found</code>. How can you trace the source of the error and resolve it?</b></summary><br>

It looks that at one point or another are overwriting the default `PATH` environment variable. The type of errors you have, indicates that `PATH` does not contain e.g. `/bin`, where the commands (including bash) reside.

One way to begin debugging your bash script or command would be to start a subshell with the `-x` option:

```bash
bash --login -x
```

This will show you every command, and its arguments, which is executed when starting that shell.

Also very helpful is show `PATH` variable values:

```bash
echo $PATH
```

If you run this:

```bash
PATH=/bin:/sbin:/usr/bin:/usr/sbin
```

most commands should start working - and then you can edit `~/.bash_profile` instead of `~/.bashrc` and fix whatever is resetting `PATH` there. Default `PATH` variable values for **root** and other users is in `/etc/profile` file.

Useful resource:

- [How to correctly add a path to PATH?](https://unix.stackexchange.com/questions/26047/how-to-correctly-add-a-path-to-path)

</details>

<details>
<summary><b>How are different production enviornments used and why? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Provide a general explanation of how SSL works. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explain in a few points the boot process of the Linux system.</b></summary><br>

**BIOS**: Full form of BIOS is Basic Input or Output System that performs integrity checks and it will search and load and then it will execute the bootloader.

**Bootloader**: Since the earlier phases are not specific to the operating system, the BIOS-based boot process for x86 and x86-64 architectures is considered to start when the master boot record (MBR) code is executed in real mode and the first-stage boot loader is loaded. In UEFI systems, a payload, such as the Linux kernel, can be executed directly. Thus no boot loader is necessary. Some popular bootloaders: **GRUB**, **Syslinux/Isolinux** or **Lilo**.

**Kernel**: The kernel in Linux handles all operating system processes, such as memory management, task scheduling, I/O, interprocess communication, and overall system control. This is loaded in two stages - in the first stage, the kernel (as a compressed image file) is loaded into memory and decompressed, and a few fundamental functions such as basic memory management are set up.

**Init**: Is the parent of all processes on the system, it is executed by the kernel and is responsible for starting all other processes.

- `SysV init` - init's job is "to get everything running the way it should be once the kernel is fully running. Essentially it establishes and operates the entire user space. This includes checking and mounting file systems, starting up necessary user services, and ultimately switching to a user-environment when system startup is completed.
- `systemd` - the developers of systemd aimed to replace the Linux init system inherited from Unix System V. Like init, systemd is a daemon that manages other daemons. All daemons, including systemd, are background processes. Systemd is the first daemon to start (during booting) and the last daemon to terminate (during shutdown).
- `runinit` - runinit is an init scheme for Unix-like operating systems that initializes, supervises, and ends processes throughout the operating system. It is a reimplementation of the daemontools process supervision toolkit that runs on the Linux, Mac OS X, \*BSD, and Solaris operating systems.

Useful resources:

- [Analyzing the Linux boot process](https://opensource.com/article/18/1/analyzing-linux-boot-process)
- [Systemd Boot Process a Close Look in Linux](https://linoxide.com/linux-how-to/systemd-boot-process/)

</details>

<details>
<summary><b>What is SELinux and how does it work? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Is 1.00 CPU load on a four-core processor a bad thing?</b></summary><br>

To be completed.

Useful resources:

- [Proper way of interpreting system load on a 4 core 8 thread processor](https://serverfault.com/questions/618130/proper-way-of-interpreting-system-load-on-a-4-core-8-thread-processor)
- [Understanding Linux CPU Load - when should you be worried?](http://blog.scoutapp.com/articles/2009/07/31/understanding-load-averages)

</details>

<details>
<summary><b>What does it mean when the effective user is root, but the real user ID is still your username?</b></summary><br>

The **real user ID** is who you really are (the user who owns the process), and the **effective user ID** is what the operating system looks at to make a decision whether or not you are allowed to do something (most of the time, there are some exceptions).

When you log in, the login shell sets both the **real and effective user ID** to the same value (your **real user ID**) as supplied by the password file.

If, for instance, you execute setuid, and besides running as another user (e.g. **root**) the setuid program is also supposed to do something on your behalf.

After executing setuid, it will have your **real ID** (since you're the process owner) and the effective user id of the file owner (for example **root**) since it is setuid.

Let's use the case of `passwd`:

```bash
-rwsr-xr-x 1 root root 45396 may 25  2012 /usr/bin/passwd
```

When user2 wants to change their password, they execute `/usr/bin/passwd`.

The **RUID** will be user2 but the **EUID** of that process will be root.

user2 can use only passwd to change their own password, because internally passwd checks the **RUID** and, if it is not root, its actions will be limited to real user's password.

It's necessary that the **EUID** becomes root in the case of passwd because the process needs to write to `/etc/passwd` and/or `/etc/shadow`.

Useful resources:

- [Difference between Real User ID, Effective User ID and Saved User ID? (original)](https://stackoverflow.com/questions/30493424/what-is-the-difference-between-a-process-pid-ppid-uid-euid-gid-and-egid)
- [What is the difference between a pid, ppid, uid, euid, gid and egid?](https://stackoverflow.com/questions/30493424/what-is-the-difference-between-a-process-pid-ppid-uid-euid-gid-and-egid)

</details>

<details>
<summary><b>How do you prevent logs from getting too big?</b></summary><br>

Using `logrotate` is the usual way of dealing with logfiles. But instead of adding content to `/etc/logrotate.conf` you should add your own job to `/etc/logrotate.d/`, to avoid issues between release upgrades and to better organize different tasks rather than searching through a large logrotate.conf file.

Useful resources:

- [How to Use logrotate to Manage Log Files](https://www.linode.com/docs/uptime/logs/use-logrotate-to-manage-log-files/)
- [System logging](https://www.ibm.com/developerworks/library/l-lpic1-108-2/index.html)

</details>

<details>
<summary><b>How can you see what files are associated with a running process? What is one example of why you would use this command? ***</b></summary><br>

To be completed.

Useful resources:

- [Linux Processes](https://www.tldp.org/LDP/tlk/kernel/processes.html)

</details>

<details>
<summary><b>What kind of information can you see with the <code>top</code> command and how is it they useful? ***</b></summary><br>

To be completed.

Useful resources:

- [top explained visually](https://svennd.be/top-explained-visually/)

</details>

<details>
<summary><b>You need to upgrade <code>ntpd</code> service at 200 servers. What is the best way to go about upgrading all of these to the latest?</b></summary><br>

By using **Infrastructure as a Code** approach, there are multiple good ways:

1. **Configuration Synchronization Change Management Model**:

There are Configuration Management Tools (Ansible, Chef, Puppet, Saltstack, ...), that can be used to automatically update `ntpd` service on all servers. To keep systems stable, system packages on servers are usually auto-updated with only security updates. Major or minor versions of packages are usually version locked in configuration definitions to prevent misconfiguration of the service. Change is then deployed by changing `ntpd` version in configuration definition.

With this approach, it is important to be careful when deploying changes into infrastructure massively. The pipeline of deployment should include Unit, Integration and System tests, and eventually be first deployed into Staging environment to prove configuration. If tests prove configuration correctness, deployment should be done by incremental rollout with ability to rollback in case of errors or failure.

2. **Immutable Servers Model**:

In Immutable Server model, whole unit (server, container) is replaced by new updated image rather than making changes to running server (this eliminates configuration drift). With this approach you usually build server image with tools like Packer or Docker with Dockerfile. This image is then tested and deployed similarly as in option above (1.), but now using techniques such as Canary Release, which also has ability to incremental rollout and rollback.

Useful resources:

- [Infrastructure as a Code - Chapter 8: Patterns for Updating and Changing Servers](http://shop.oreilly.com/product/0636920039297.do)

</details>

<details>
<summary><b>How do you permanently set <code>$PATH</code> on Linux/Unix? Why is this variable so important? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>When your server is booting up some errors appears on the console. How do you examine the system boot log and where are they stored?</b></summary><br>

Your console has two types of messages:

- **generated by the kernel** (via printk)
- **generated by userspace** (usually your init system)

Kernel messages are always stored in the **kmsg** buffer, visible via `dmesg` command. They're also often copied to your **syslog**. This also applies to userspace messages written to `/dev/kmsg`, but those are fairly rare.

Meanwhile, when userspace writes its fancy boot status text to `/dev/console` or `/dev/tty1`, it's not stored anywhere at all. It just goes to the screen and that's it.

`dmesg` is used to review boot messages contained in the kernel ring buffer. A ring buffer is a buffer of fixed size for which any new data added to it overwrites the oldest data in it.

It shows operations once the boot process has completed, such as command line options passed to the kernel; hardware components detected, events when a new USB device is added, or errors like NIC (Network Interface Card) failure and the drivers report no link activity detected on the network and so much more.

If system logging is done via the journal component you should use `journalctl`. It shows messages include kernel and boot messages; messages from syslog or various services.

Boot issues/errors calls for a system administrator to look into certain important files in conjunction with particular commands (handled differently by different versions of Linux):

- `/var/log/boot.log` - system boot log, it contains all that unfolded during the system boot
- `/var/log/messages` - stores global system messages, including the messages that are logged during system boot
- `/var/log/dmesg` - contains kernel ring buffer information

Useful resources:

- [How to view all boot messages in Linux after booting? (original)](https://superuser.com/questions/1188407/how-to-view-all-boot-messages-in-linux-after-booting)
- [Differences in /var/log/{syslog,dmesg,messages} log files](https://superuser.com/questions/565927/differences-in-var-log-syslog-dmesg-messages-log-files)
- [How can the messages that scroll by when booting a Debian system be reviewed later?](https://serverfault.com/questions/516411/all-debian-boot-messages)

</details>

<details>
<summary><b>Swap usage too high. What are the reasons for this and how do you resolve swapping problems?</b></summary><br>

**Swap** space is a restricted amount of physical memory that is allocated for use by the operating system when available memory has been fully utilized. It is memory management that involves swapping sections of memory to and from physical storage.

If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space. While swap space can help machines with a small amount of RAM, it should not be considered a replacement for more RAM. **Swap** space is located on hard drives, which have a slower access time than physical memory.

Workload increases your RAM demand. You are running a workload that requires more memory. Usage of the entire swap indicates that. Also, changing `swappiness` to **1** might not be a wise decision. Setting `swappiness` to **1** does not indicate that swapping will not be done. It just indicates how aggressive kernel will be in respect of swapping, it does not eliminate swapping. Swapping will happen if needs to be done.

- **Increasing the size of the swap space** - firstly, you'd have increased disk use. If your disks aren't fast enough to keep up, then your system might end up thrashing, and you'd experience slowdowns as data is swapped in and out of memory. This would result in a bottleneck.

- **Adding more RAM** - the real solution is to add more memory. There's no substitute for RAM, and if you have enough memory, you'll swap less.

For monitoring swap space usage:

- `cat /proc/swaps` - to see total and used swap size
- `grep SwapTotal /proc/meminfo` - to show total swap space
- `free` - to display the amount of free and used system memory (also swap)
- `vmstat` - to check swapping statistics
- `top`, `htop`- to check swap space usage
- `atop` - to show is that your system is overcommitting memory
- or use one-liner shell command to list all applications with how much swap space search is using in kilobytes:
```bash
for _fd in /proc/*/status ; do
  awk '/VmSwap|Name/{printf $2 " " $3}END{ print ""}' $_fd
done | sort -k 2 -n -r | less
```

Useful resources:

- [Linux ate my ram!](https://www.linuxatemyram.com/)
- [How to find out which processes are using swap space in Linux?](https://stackoverflow.com/questions/479953/how-to-find-out-which-processes-are-using-swap-space-in-linux)
- [8 Useful Commands to Monitor Swap Space Usage in Linux](https://www.tecmint.com/commands-to-monitor-swap-space-usage-in-linux/)
- [What is the danger in having a fully used SWAP in an Ubuntu server?](https://serverfault.com/questions/499301/what-is-the-danger-in-having-a-fully-used-swap-in-an-ubuntu-server)
- [How to empty swap if there is free RAM?](https://askubuntu.com/questions/1357/how-to-empty-swap-if-there-is-free-ram)

</details>

<details>
<summary><b>What is umask? Describe a scenario where you might need to change it for a user. ***</b></summary><br>

On Linux and other Unix-like operating systems, new files are created with a default set of permissions. Specifically, a new file's permissions may be restricted in a specific way by applying a permissions "mask" called the `umask`. The `umask` command is used to set this mask, or to show you its current value.

To be completed.

Useful resources:

- [What is Umask and How To Setup Default umask Under Linux?](https://www.cyberciti.biz/tips/understanding-linux-unix-umask-value-usage.html)

</details>

<details>
<summary><b>In SQL, how can you combine rows from two or more tables, based on a related column between them? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between a symbolic link and a hard link?</b></summary><br>

Underneath the file system files are represented by inodes (or is it multiple inodes not sure)

- a file in the file system is basically a link to an inode
- a hard link then just creates another file with a link to the same underlying inode

When you delete a file it removes one link to the underlying inode. The inode is only deleted (or deletable/over-writable) when all links to the inode have been deleted.

- a symbolic link is a link to another name in the file system

Once a hard link has been made the link is to the inode. deleting renaming or moving the original file will not affect the hard link as it links to the underlying inode. Any changes to the data on the inode is reflected in all files that refer to that inode.

Note: Hard links are only valid within the same file system. Symbolic links can span file systems as they are simply the name of another file.

Differences:

- **Hardlink** cannot be created for directories. Hard link can only be created for a file
- **Softlink** also termed a symbolic links or symlinks can link to a directory

Useful resources:

- [What is the difference between a hard link and a symbolic link?](https://medium.com/@wendymayorgasegura/what-is-the-difference-between-a-hard-link-and-a-symbolic-link-8c0493041b62)

</details>

<details>
<summary><b>How does the sticky bit work? Is <code>SUID/GUID</code> is the same?</b></summary><br>

The **SUID/GUID** bit and the **sticky-bit** are 2 completely different things.

**SUID/GUID**

The position that the x bit takes in the rwxrwxrwx for the user octal (1st group of rwx) and the group octal (2nd group of rwx) can take an additional state where the x becomes an s. When this occurs this file when executed (if it's a program and not just a shell script) will run with the permissions of the owner or the group of the file.

So if the file is owned by root and the **SUID** bit is turned on, the program will run as root. Even if you execute it as a regular user. The same thing applies to the **GUID** bit.

Examples:

**no suid/guid** - just the bits `rwxr-xr-x` are set.

```bash
ls -lt b.pl
-rwxr-xr-x 1 root root 179 Jan  9 01:01 b.pl
```

**suid & user's executable bit enabled (lowercase s)** - the bits `rwsr-x-r-x` are set.

```bash
chmod u+s b.pl
ls -lt b.pl
-rwsr-xr-x 1 root root 179 Jan  9 01:01 b.pl
```

**suid enabled & executable bit disabled (uppercase S)** - the bits `rwSr-xr-x` are set.

```bash
chmod u-x b.pl
ls -lt b.pl
-rwSr-xr-x 1 root root 179 Jan  9 01:01 b.pl
```

**guid & group's executable bit enabled (lowercase s)** - the bits `rwxr-sr-x` are set.

```bash
chmod g+s b.pl
ls -lt b.pl
-rwxr-sr-x 1 root root 179 Jan  9 01:01 b.pl
```

**guid enabled & executable bit disabled (uppercase S)** - the bits `rwxr-Sr-x` are set.

```bash
chmod g-x b.pl
ls -lt b.pl
-rwxr-Sr-x 1 root root 179 Jan  9 01:01 b.pl
```

**sticky bit**

The sticky bit on the other hand is denoted as `t`, such as with the `/tmp` directory:

```bash
ls -l /|grep tmp
drwxrwxrwt. 168 root root 28672 Jun 14 08:36 tmp
```

This bit should have always been called the _restricted deletion bit_ given that's what it really connotes. When this mode bit is enabled, it makes a directory such that users can only delete files & directories within it that they are the owners of.

Useful resources:

- [How does the sticky bit work? (original)](https://unix.stackexchange.com/questions/79395/how-does-the-sticky-bit-work)

</details>

<details>
<summary><b>In SQL, what is the difference between <code>REPLACE</code> and <code>INSERT</code>? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How do you make a server or application high availabile? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>You are configuring a new server. One of the steps is setting the permissions to the app directories. What steps will you take and what mistakes to avoid?</b></summary><br>

**1) Main requirements - remember about this**

- which users have access to the app filesystem
- permissions for web servers, e.g. Apache and app servers e.g. uwsgi
- permissions for specific directories like a **uploads**, **cache** and main app directory like a `/var/www/app01/html`
- correct `umask` value for users and **suid**/**sgid** (only for specific situations)
- permissions for all future files and directories
- permissions for cron jobs and scripts

**2) Application directories**

`/var/www` contains a directory for each website (isolation of the apps), e.g. `/var/www/app01`, `/var/www/app02`

```bash
mkdir /var/www/{app01,app02}
```

**3) Application owner and group**

Each application has a designated **owner** (e.g. **u01-prod**, **u02-prod**) and **group** (e.g. **g01-prod**, **g02-prod**) which are set as the owner of all files and directories in the website's directory:

```bash
chown -R u01-prod:g01-prod /var/www/app01
chown -R u02-prod:g02-prod /var/www/app02
```

**4) Developers owner and group**

All of the users that maintain the website have own groups and they're attach to application group:

```bash
id alice
uid=2000(alice) gid=4000(alice) groups=8000(g01-prod)
id bob
uid=2001(bob) gid=4001(bob) groups=8000(g01-prod),8001(g02-prod)
```

So **alice** user has standard privileges for `/var/www/app01` and **bob** user has standard privileges for `/var/www/app01` and `/var/www/app02`.

**5) Web server owner and group**

Any files or directories that need to be written by the webserver have their owner. If the web servers is Apache, default owner/group are **apache:apache** or **www-data:www-data** and for Nginx it will be **nginx:nginx**. Don't change these settings.

If applications works with app servers like a **uwsgi** or **php-fpm** should set the appropriate user and group (e.g. for **app01** it will be **u01-prod:g01-prod**) in specific config files.

**6) Permissions**

Set properly permissions with **Access Control Lists**:

```bash
# For web server
setfacl -Rdm "g:apache:rwx" /var/www/app01
setfacl -Rm "g:apache:rwx" /var/www/app01

# For developers
setfacl -Rdm "g:g01-prod:rwx" /var/www/app01
setfacl -Rm "g:g01-prod:rwx" /var/www/app01
```

If you use **SELinux** remember about security context:

```bash
chcon -R system_u:object_r:httpd_sys_content_t /var/www/app01
```

**7) Security mistakes**

- **root** owner for files and directories
- **root** never executes any files in website directory, and shouldn't be creating files in there
- to wide permissions like a **777** so some critical files may be world-writable and world-readable
- avoid creating maintenance scripts or other critical files with suid root

If you allow your site to modify the files which form the code running your site, you make it much easier for someone to take over your server.

A file upload tool allows users to upload a file with any name and any contents. This allows a user to upload a mail relay PHP script to your site, which they can place wherever they want to turn your server into a machine to forward unsolicited commercial email. This script could also be used to read every email address out of your database, or other personal information.

If the malicious user can upload a file with any name but not control the contents, then they could easily upload a file which overwrites your `index.php` (or another critical file) and breaks your site.

Useful resources:

- [How to setup linux permissions for the WWW folder?](https://serverfault.com/questions/124800/how-to-setup-linux-permissions-for-the-www-folder)
- [What permissions should my website files/folders have on a Linux webserver?](https://serverfault.com/questions/357108/what-permissions-should-my-website-files-folders-have-on-a-linux-webserver)
- [Security Pitfalls of setgid Programs](https://www.agwa.name/blog/post/security_pitfalls_of_setgid_programs)

</details>

<details>
<summary><b>How do you change system runlevels? What are some reasons you would need to? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>The root password has been forgotten and you are locked out of the system. How can you reset the root password?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How could you modify a text file without invoking a text editor?</b></summary><br>

For example:<br>

```bash
# cat  >filename ... - overwrite file
# cat >>filename ... - append to file
cat > filename << __EOF__
data
__EOF__
```

</details>

<details>
<summary><b>How do you change kernel parameters? What kernel options might you need to tune? ***</b></summary><br>

To set the kernel parameters in Unix-like, first edit the file `/etc/sysctl.conf` after making the changes save the file and run the command `sysctl -p`, this command will make the changes permanently without rebooting the machine.

Useful resources:

- [How to Change Kernel Runtime Parameters in a Persistent and Non-Persistent Way](https://www.tecmint.com/change-modify-linux-kernel-runtime-parameters/)

</details>

<details>
<summary><b>What is the best way to remove a directory named<code>-rf</code>? Explain the issue. ***</b></summary><br>

- <code>rm -- -fr</code>
- <code>rm ./-rf</code>
- <code>perl -le 'unlink("-fr");'</code>

</details>

<details>
<summary><b>Explain the <code>/proc</code> filesystem.</b></summary><br>

`/proc` is a virtual file system that provides detailed information about kernel, hardware and running processes.

Since `/proc` contains virtual files, it is called virtual file system. These virtual files have unique qualities. Most of them are listed as zero bytes in size.

Virtual files such as `/proc/interrupts`, `/proc/meminfo`, `/proc/mounts` and `/proc/partitions` provide an up-to-the-moment glimpse of the system’s hardware. Others: `/proc/filesystems` file and the `/proc/sys/` directory provide system configuration information and interfaces.

Useful resources:

- [Linux Filesystem Hierarchy - /proc](https://www.tldp.org/LDP/Linux-Filesystem-Hierarchy/html/proc.html)

</details>

<details>
<summary><b>Describe your data backup process. How often should you test your backups? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explain three types of journaling in ext3/ext4.</b></summary><br>

There are three types of journaling available in **ext3/ext4** file systems:

- **Journal** - metadata and content are saved in the journal
- **Ordered** - only metadata is saved in the journal. Metadata are  journaled only after writing the content to disk. This is the default
- **Writeback** - only metadata is saved in the journal. Metadata might be  journaled either before or after the content is written to the disk

</details>

<details>
<summary><b>What is an inode? How do you find a file's inode number and how can you use it?</b></summary><br>

An **inode** is a data structure on a filesystem on Linux and other Unix-like operating systems that stores all the information about a file except its name and its actual data. A data structure is a way of storing data so that it can be used efficiently.

A Unix file is stored in two different parts of the disk - the data blocks and the inodes. I won't get into superblocks and other esoteric information. The data blocks contain the "contents" of the file. The information about the file is stored elsewhere - in the inode.

A file's inode number can easily be found by using the `ls` command, which by default lists the objects (i.e. files, links and directories) in the current directory (i.e. the directory in which the user is currently working), with its `-i` option. Thus, for example, the following will show the name of each object in the current directory together with its inode number:

```bash
ls -i
```

`df's` `-i` option instructs it to supply information about inodes on each filesystem rather than about available space. Specifically, it tells df to return for each mounted filesystem the total number of inodes, the number of free inodes, the number of used inodes and the percentage of inodes used. This option can be used together with the `-h` option as follows to make the output easier to read:

```bash
df -hi
```

**Finding files by inodes**

If you know the inode, you can find it using the find command:

```bash
find . -inum 435304 -print
```

**Deleting files with strange names**

Sometimes files are created with strange characters in the filename. The Unix file system will allow any character as part of a filename except for a null (ASCII 000) or a "/". Every other character is allowed.

Users can create files with characters that make it difficult to see the directory or file. They can create the directory ".. " with a space at the end, or create a file that has a backspace in the name, using:

```bash
touch `printf "aa\bb"`
```

Now what what happens when you use the `ls` command:

```bash
ls
aa?b
ls | grep 'a'
ab
```

Note that when `ls` sends the result to a terminal, it places a "**?**" in the filename to show an unprintable character.

You can get rid of this file by using `rm -i *` and it will prompt you before it deletes each file. But you can also use `find` to remove the file, once you know the inode number.

```bash
ls -i
435304 aa?b
find . -inum 435304 -delete
```

Useful resources:

- [Understand UNIX/Linux Inodes Basics with Examples](https://www.thegeekstuff.com/2012/01/linux-inodes/)
- [What is an inode as defined by POSIX?](https://unix.stackexchange.com/questions/387087/what-is-an-inode-as-defined-by-posix/387093)

</details>

<details>
<summary><b><code>ls -l</code> shows file attributes as question marks. What this means and what steps will you take to remove unused "zombie" files?</b></summary><br>

This problem may be more difficult to solve because several steps may be required - sometimes you have get `test/file: Permission denied`, `test/file: No such file or directory` or `test/file: Input/output error`.

That happens when the user can't do a `stat()` on the files (which requires execute permissions), but can read the directory entries (which requires read access on the directory). So you get a list of files in the directory, but can't get any information on the files because they can't be read. If you have a directory which has read permission but not execute, you'll see this.

Some processes like a `rsync` generates temporary files that get created and dropped fast which will cause errors if you try to call other simple file management commands like `rm`, `mv` etc.

Example of output:

```bash
?????????? ? ?        ?               ?            ? sess_kee6fu9ag7tiph2jae
```

1) change permissions: `chmod 0777 sess_kee6fu9ag7tiph2jae` and try remove
2) change owner: `chown root:root sess_kee6fu9ag7tiph2jae` and try remove
3) change permissions and owner for directory: `chmod -R 0777 dir/ && chown -R root:root dir/` and try remove
4) recreate file: `touch sess_kee6fu9ag7tiph2jae` and try remove
5) watch out for other running processes on the server for example `rsync`, sometimes you can see this as a transient error when an NFS server is heavily overloaded
6) find file inode: `ls -i`, and try remove: `find . -inum <inode_num> -delete`
7) remount (if possible) your filesystem
8) boot system into single-user mode and repair your filesystem with `fsck`

Useful resources:

- [Question marks showing in ls of directory. IO errors too.](https://serverfault.com/questions/65616/question-marks-showing-in-ls-of-directory-io-errors-too)

</details>

<details>
<summary><b>What benefits does LVM provide?</b></summary><br>

- LVM makes it quite easy to move file systems around
- you can extend a volume group onto a new physical volume
- move any number of logical volumes of an old physical one
- remove that volume from the volume group without needing to unmount any partitions
- you can also make snapshots of logical volumes for making backups
- LVM has built in mirroring support so you can have a logical volume mirrored across multiple physical volumes
- LVM even supports TRIM

Useful resources:

- [What is LVM and what is it used for?](https://askubuntu.com/questions/3596/what-is-lvm-and-what-is-it-used-for)

</details>

<details>
<summary><b>How do you increase the size of LVM partition?</b></summary><br>

Use the `lvextend` command for resize LVM partition.

- extending the size by 500MB:

```bash
lvextend -L +500M /dev/vgroup/lvolume
```

- extending all available free space:

```bash
lvextend -l +100%FREE /dev/vgroup/lvolume
```

and `resize2fs` or `xfs_growfs` to resize filesystem:

- for ext filesystems:

```bash
resize2fs /dev/vgroup/lvolume
```

- for xfs filesystem:

```bash
xfs_growfs mountpoint_for_/dev/vgroup/lvolume
```

Useful resources:

- [Extending a logical volume](https://www.tldp.org/HOWTO/LVM-HOWTO/extendlv.html)

</details>

<details>
<summary><b>What is a zombie/defunct process?</b></summary><br>

Is a process that has completed execution (via the `exit` system call) but still has an entry in the process table: it is a process in the "**Terminated state**".

Processes marked **defunct** are dead processes (so-called "zombies") that remain because their parent has not destroyed them properly. These processes will be destroyed by init if the parent process exits.

Useful resources:

- [What is a <defunct> process, and why doesn't it get killed?](https://askubuntu.com/questions/201303/what-is-a-defunct-process-and-why-doesnt-it-get-killed)

</details>

<details>
<summary><b>What is the proper way to upgrade/update a system in production? Do you automate these processes? Do you set downtime for them? Write recommendations. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Present and explain the good ways of using the <code>kill</code> command.</b></summary><br>

Speaking of killing processes never use `kill -9/SIGKILL` unless absolutely mandatory. This kill can cause problems because of its brute force.

Always try to use the following simple procedure:

- first, send **SIGTERM** (`kill -15`) signal first which tells the process to shutdown and is generally accepted as the signal to use when shutting down cleanly (but remember that this signal can be ignored).
- next try to send **SIGHUP** (`kill -1`) signal which is commonly used to tell a process to shutdown and restart, this signal can also be caught and ignored by a process.

The far majority of the time, this is all you need - and is much cleaner.

Useful resources:

- [When should I not kill -9 a process?](https://unix.stackexchange.com/questions/8916/when-should-i-not-kill-9-a-process)
- [SIGTERM vs. SIGKILL](https://major.io/2010/03/18/sigterm-vs-sigkill/)

</details>

<details>
<summary><b>What is <code>strace</code> command and how should be used? Explain example of connect to an already running process.</b></summary><br>

`strace` is a powerful command line tool for debugging and troubleshooting programs in Unix-like operating systems such as Linux. It captures and records all system calls made by a process and the signals received by the process.

**Strace Overview**

`strace` can be seen as a light weight debugger. It allows a programmer/user to quickly find out how a program is interacting with the OS. It does this by monitoring system calls and signals.

**Uses**

Good for when you don't have source code or don't want to be bothered to really go through it. Also, useful for your own code if you don't feel like opening up **GDB**, but are just interested in understanding external interaction.

**Example of attach to the process**

`strace -p <PID>` - to attach a process to strace.

`strace -e trace=read,write -p <PID>` - by this you can also trace a process/program for an event, like read and write (in this example). So here it will print all such events that include read and write system calls by the process.

Other such examples

- `-e trace=network` - trace all the network related system calls.
- `-e trace=signal` - trace all signal related system calls.
- `-e trace=ipc` - trace all IPC related system calls.
- `-e trace=desc` - trace all file descriptor related system calls.
- `-e trace=memory` - trace all memory mapping related system calls.

Useful resources:

- [How should strace be used? (original)](https://stackoverflow.com/questions/174942/how-should-strace-be-used)
- [How does strace connect to an already running process? (original)](https://stackoverflow.com/questions/7482076/how-does-strace-connect-to-an-already-running-process)
- [strace: for fun, profit, and debugging](http://timetobleed.com/hello-world/)

</details>

<details>
<summary><b>When would you use access control lists instead of or in conjunction with the <code>chmod</code> command? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Which algorithms are supported in <code>/etc/shadow</code> file?</b></summary><br>

Typical current algorithms are:

- MD5
- SHA-1 (also called SHA)

both should not be used for cryptographic/security purposes any more!!

- SHA-256
- SHA-512
- SHA-3 (KECCAK was announced the winner in the competition for a new federal approved hash algorithm in October 2012)

Useful resources:

- [What is the algorithm used to encrypt Linux passwords?](https://crypto.stackexchange.com/questions/40841/what-is-the-algorithm-used-to-encrypt-linux-passwords)
- [How to find the hashing algorithm used to obfuscate passwords?](https://unix.stackexchange.com/questions/430141/how-to-find-the-hashing-algorithm-used-to-obfuscate-passwords)

</details>

<details>
<summary><b>What is the use of ulimit in Unix-like systems?</b></summary><br>

Most Unix-like operating systems, including Linux and BSD, provide ways to limit and control the usage of system resources such as threads, files, and network connections on a per-process and per-user basis. These "**ulimits**" prevent single users from using too many system resources.

</details>

<details>
<summary><b>What are soft limits and hard limits?</b></summary><br>

**Hard limit** is the maximum allowed to a user, set by the superuser or root. This value is set in the file `/etc/security/limits.conf`. The user can increase the **soft limit** on their own in times of needing more resources, but cannot set the **soft limit** higher than the **hard limit**.

</details>

<details>
<summary><b>You have configured an RSA key login but your server show <code>Server refused our key</code> as expected. Where will you look for the cause of the problem?</b></summary><br>

**Server side**

Setting `LogLevel VERBOSE` in file `/etc/ssh/sshd_config` is probably what you need, although there are higher levels:

SSH auth failures are logged in `/var/log/auth.log`, `/var/log/secure` or `/var/log/audit/audit.log`.

The following should give you only ssh related log lines (for example):

```bash
grep 'sshd' /var/log/auth.log
```

Next, the most simple command to list all failed SSH logins is the one shown below:

```bash
grep "Failed password" /var/log/auth.log
```

also useful is:

```bash
grep "Failed\|Failure" /var/log/auth.log
```

On newer Linux distributions you can query the runtime log file maintained by Systemd daemon via `journalctl` command (`ssh.service` or `sshd.service`). For example:

```bash
journalctl _SYSTEMD_UNIT=ssh.service | egrep "Failed|Failure"
```

**Client side**

Also you should run SSH client with `-v|--verbose` - it is in first level of verbosity. Next, you can enable additional (level 2 and 3) verbosity for even more debugging messages as shown with e.g. `-vv`.

Useful resources:

- [Enable Debugging Mode in SSH to Troubleshoot Connectivity Issues](https://www.tecmint.com/enable-debugging-mode-in-ssh/)

</details>

<details>
<summary><b>Why do most distros use ext4, as opposed to XFS or other filesystems? Why are there so many of them? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>A project manager needs a new SQL Server. What do you ask her/his? ***</b></summary><br>

I want the DBA to ask questions like:

- How big will the database be? (whether we can add the database to an existing server)
- How critical is the database? (about clustering, disaster recovery, high availability)

</details>

<details>
<summary><b>Create a file with 100 lines with random values.</b></summary><br>

For example:

```bash
cat /dev/urandom | tr -dc 'a-zA-Z0-9' | fold -w 32 | head -n 100 > /path/to/file
```

</details>

<details>
<summary><b>How do you run a script as another user without password?</b></summary><br>

For example (with `visudo` command):

```bash
user1 ALL=(user2) NOPASSWD: /opt/scripts/bin/generate.sh
```

The command paths must be absolute! Then call `sudo -u user2 /opt/scripts/bin/generate.sh` from a user1 shell.

</details>

<details>
<summary><b>Can you give a particular example when is indicated to use <code>nobody</code> account? Tell me the differences running httpd service as a <code>nobody</code> and <code>www-data</code> accounts.</b></summary><br>

In many Unix variants, `nobody` is the conventional name of a user account which owns no files, is in no privileged groups, and has no abilities except those which every other user has.

It is common to run daemons as `nobody`, especially servers, in order to limit the damage that could be done by a malicious user who gained control of them.

However, the usefulness of this technique is reduced if more than one daemon is run like this, because then gaining control of one daemon would provide control of them all. The reason is that `nobody`-owned processes have the ability to send signals to each other and even debug each other, allowing them to read or even modify each other's memory.

**When should I use `nobody` account?**

When permissions aren't required for a program's operations. This is most notable when there isn't ever going to be any disk activity.

A real world example of this is **memcached** (a key-value in-memory cache/database/thing), sitting on my computer and my server running under the `nobody` account. Why? Because it just doesn't need any permissions and to give it an account that did have write access to files would just be a needless risk.

A good example are also web servers. Imagine if Apache ran as root and someone found a way to send custom commands to the console through Apache would have access to your entire system.

`nobody` account also is used as a restricted shell for giving users filesystem access without an actual shell like bash. This should prevent them from being able to execute things.

**`nobody` or `www-data` for httpd (Apache)**

Upon starting Apache needs root access, but it quickly drops this and assumes the identity of a non privileged user. This user can either be `nobody` or `apache`, or `www-data`.

Several applications use the user `nobody` as a default. For example you probably never really want say the Apache service to be overwriting files that belong to bind. Having a per-service account tends to be a very good idea.

Getting Apache to run as `nobody:nobody` is pretty easy, just update the user and group settings. But as I mentioned above I don't really recommend that particular user/group. It is entirely possible that you may be tempted to add a service to the system at some time in the future that also runs as `nobody`, and you will forget that have given write access on the filesystem to the user `nobody`.

 If somehow, `nobody` were to become compromised they could potentially have more impact than if an application isolate user, such as `www-data`. Of course a lot of this will depend on the file and group permissions. `nobody` uses the permissions of others, while an application specific user could be configured to allow file read access, but other could still be denied.

Useful resources:

- [What is nobody user and group?](https://unix.stackexchange.com/questions/186568/what-is-nobody-user-and-group)
- [The Linux and Unix Nobody User](http://linuxg.net/the-linux-and-unix-nobody-user/)
- [What is the purpose of the 'nobody' user?](https://askubuntu.com/questions/329714/what-is-the-purpose-of-the-nobody-user)

</details>

<details>
<summary><b>Is there a way to redirect output to a file and have it display on stdout?</b></summary><br>

The command you want is named tee:

`foo | tee output.file`

For example, if you only care about stdout:

`ls -a | tee output.file`

If you want to include stderr, do:

`program [arguments...] 2>&1 | tee outfile`

`2>&1` redirects channel 2 (stderr/standard error) into channel 1 (stdout/standard output), such that both is written as stdout. It is also directed to the given output file as of the tee command.

Furthermore, if you want to append to the log file, use `tee -a` as:

`program [arguments...] 2>&1 | tee -a outfile`

</details>

<details>
<summary><b>What is the preferred bash shebang and why? What is the difference between executing a file using <code>./script</code> or <code>bash script</code>?</b></summary><br>

You should use `#!/usr/bin/env bash` for portability: different \*nixes put bash in different places, and using `/usr/bin/env` is a workaround to run the first bash found on the `PATH`.

Running `./script` does exactly that, and requires execute permission on the file, but is agnostic to what type of a program it is. It might be a **bash script**, an **sh script**, or a **Perl**, **Python**, **awk**, or **expect script**, or an actual **binary executable**. Running `bash script` would force it to be run under `sh`, instead of anything else.

Useful resources:

- [What is the preferred Bash shebang? (original)](https://stackoverflow.com/questions/10376206/what-is-the-preferred-bash-shebang)

</details>

<details>
<summary><b>You must run command that will be performed for a very long time. How do you prevent killing this process after the ssh session drops?</b></summary><br>

Use `nohup` to make your process ignore the hangup signal:

```bash
nohup long-running-process &
exit
```

or you want to be using **GNU Screen**:

```bash
screen -d -m long-running-process
exit
```

Useful resources:

- [5 Ways to Keep Remote SSH Sessions and Processes Running After Disconnection](https://www.tecmint.com/keep-remote-ssh-sessions-running-after-disconnection/)

</details>

<details>
<summary><b>What is the main purpose of the intermediate certification authorities?</b></summary><br>

To find out the main purpose of an intermediate CA, you should first learn about **Root CAs**, **Intermediate CAs**, and the **SSL Certificate Chain Trust**.

**Root CAs** are primary CAs which typically don’t directly sign end entity/server certificates. They issue Root certificates which are usually pre-installed within all browsers, mobiles, and applications. The private key of these certificates is used to sign other subsequent certificates called intermediate certificates. Root CAs are usually kept "offline” and in a highly secure environment with stringently limited access.

**Intermediates CAs** are CAs that subordinate to the Root CA by one or more levels, being trusted by these to sign certificates on their behalf. The purpose of creating and using Intermediate CAs is primarily for security because if the intermediate private key is compromised, then the Root CA can revoke the intermediate certificate and create a new one with a new cryptographic key pair.

**SSL Certificate Chain Trust** is the list of SSL certificates, from the root certificate to the end entity/server certificate. For an SSL Certificate to be trusted, it must be issued by a trusted CAs which is included in the trusted CA list of the connecting device (browser, mobile, and application). Therefore, the connecting device will test the trustworthiness of each SSL Certificate in the Chain Trust until it matches the one issued by a trusted CA.

The **Root-Intermediate CA** structure is created by each major CA to protect against the disastrous effects of a root key compromise. If a root key is compromised, it would render the root and all subordinated certificates untrustworthy. For this reason, creating an Intermediate CA is a best practice to ensure a rigorous protection of the primary root key.

Useful resources:

- [How certificate chains work](https://knowledge.digicert.com/solution/SO16297.html)

</details>

<details>
<summary><b>You have added several aliases to <code>.bash_profile</code>. How can you reload shell without exiting?</b></summary><br>

The best way is `exec $SHELL -l` because `exec` replaces the current process with a new one. Another solution is to simply source the file `. ~/.profile`.

Useful resources:

- [How to reload .bash_profile from the command line?](https://stackoverflow.com/questions/4608187/how-to-reload-bash-profile-from-the-command-line)

</details>

<details>
<summary><b>What are the advantages of using a reverse proxy server?</b></summary><br>

**Hide the topology and characteristics of your back-end servers**

The **reverse proxy server** can hide the presence and characteristics of the origin server. It acts as an intermediate between internet cloud and web server. It is good for security reason especially when you are using web hosting services.

**Allows transparent maintenance of backend servers**

Changes you make to servers running behind a reverse proxy are going to be completely transparent to your end users.

**Load Balancing**

The reverse proxy will then enforce a load balancing algorithm like round robin, weighted round robin, least connections, weighted least connections, or random, to distribute the load among the servers in the cluster.

When a server goes down, the system will automatically failover to the next server up and users can continue with their secure file transfer activities.

**SSL offloading/termination**

Handles incoming HTTPS connections, decrypting the requests and passing unencrypted requests on to the web servers.

**IP masking**

Using a single ip but different URLs to route to different back end servers.

Useful resources:

- [The Benefits of a Reverse Proxy](https://dzone.com/articles/benefits-reverse-proxy)

</details>

<details>
<summary><b>Is there an easy way to search inside 1000s of files in a complex directory structure to find files which contain a specific string?</b></summary><br>

For example use `fgrep`:

```bash
fgrep * -R "string"
```

or:

```bash
grep -insr "pattern" *
```

- `-i` ignore case distinctions in both the **PATTERN** and the input files
- `-n`  prefix each line of output with the 1-based line number within its input file
- `-s` suppress error messages about nonexistent or unreadable files.
- `-r` read all files under each directory, recursively.

Useful resources:

- [How to grep a string in a directory and all its subdirectories files in LINUX?](https://stackoverflow.com/questions/15622328/how-to-grep-a-string-in-a-directory-and-all-its-subdirectories-files-in-linux)

</details>

<details>
<summary><b>How do you find out what dynamic libraries executables load when run?</b></summary><br>

You can do this with `ldd` command:

```bash
ldd /bin/ls
```

</details>

<details>
<summary><b>What is the difference between a container and a VM? Mention some benefits of each. ***</b></summary><br>

To be completed.

Below are the advantages of containerization over virtualization:

containers provide real-time provisioning and scalability but VMs provide slow provisioning
containers are lightweight when compared to VMs
VMs have limited performance when compared to containers
containers have better resource utilization compared to VMs

Useful resources:

- [RedHat: Containers vs VMs](https://www.redhat.com/en/topics/containers/containers-vs-vms)

</details>

<details>
<summary><b>Why wouldn't hostnames resolve on your server and how would you troubleshoot the issue? ***</b></summary><br>

To be completed.

</details>

###### Network Questions

<details>
<summary><b>What is Boot to LAN?</b></summary><br>

Boot to LAN is most often used when you are doing a fresh install on a system. What you would do is setup a network-based installer capable of network-booting via PXE. Boot to LAN enables this by allowing a pre-boot environment to look for a DHCP server and connect to the broadcasting network installation server. Environments that have very large numbers of systems more often than not have the capability of pushing out images via the network. This reduces the amount of hands-on time that is required on each system, and keeps the installs more consistent.

</details>

<details>
<summary><b>What is the difference between the Internet, Intranet, and Extranet?</b></summary><br>

The terminologies Internet, Intranet, and Extranet are used to define how the applications in the network can be accessed. They use similar TCP/IP technology but differ in terms of access levels for each user inside the network and outside the network.

- Internet: Applications are accessed by anyone from any location using the web.
- Intranet: It allows limited access to users in the same organization.
- Extranet: External users are allowed or provided with access to use the network application of the organization.

</details>

<details>
<summary><b>What is a packet filter and how does it work?</b></summary><br>

**Packet filtering** is a firewall technique used to control network access by monitoring outgoing and incoming packets and allowing them to pass or halt based on the source and destination Internet Protocol (IP) addresses, protocols and ports.

Packet filtering is appropriate where there are modest security requirements. The internal (private) networks of many organizations are not highly segmented. Highly sophisticated firewalls are not necessary for isolating one part of the organization from another.

However it is prudent to provide some sort of protection of the production network from a lab or experimental network. A packet filtering device is a very appropriate measure for providing isolation of one subnet from another.

Operating at the network layer and transport layer of the TCP/IP protocol stack, every packet is examined as it enters the protocol stack. The network and transport headers are examined closely for the following information:

- **protocol (IP header, network layer)** - in the IP header, byte 9 (remember the byte count begins with zero) identifies the protocol of the packet. Most filter devices have the capability to differentiate between TCP, UPD, and ICMP.
- **source address (IP header, network layer)** - the source address is the 32-bit IP address of the host which created the packet.
- **destination address (IP header, network layer)** - the destination address is the 32-bit IP address of the host the packet is destined for.
- **source port (TCP or UDP header, transport layer)** - each end of a TCP or UDP network connection is bound to a port. TCP ports are separate and distinct from UDP ports. Ports numbered below 1024 are reserved – they have a specifically defined use. Ports numbered above 1024 (inclusive) are known as ephemeral ports. They can be used however a vendor chooses. For a list of "well known" ports, refer to RFP1700. The source port is a pseudo-randomly assigned ephemeral port number. Thus it is often not very useful to filter on the source port.
- **destination port (TCP or UDP header, transport layer)** - the destination port number indicates a port that the packet is sent to. Each service on the destination host listens to a port. Some well-known ports that might be filtered are 20/TCP and 21/TCP - ftp connection/data, 23/TCP - telnet, 80/TCP - http, and 53/TCP - DNS zone transfers.
- **connection status (TCP header, transport layer)** - the connection status tells whether the packet is the first packet of the network session. The ACK bit in the TCP header is set to “false” or 0 if this is the first packet in the session. It is simple to disallow a host from establishing a connection by rejecting or discarding any packets which have the ACK bit set to "false" or 0.

Useful resources:

- [How does a packet filters work?](https://www.tutorialspoint.com/how-does-a-packet-filters-work)

</details>

<details>
<summary><b>What is a VPN? Describe briefly how it works. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>According to an HTTP monitor, a website is down. You're able to telnet to the port, so how do you resolve it?</b></summary><br>

If you can telnet to the port, this means that the service listening on the port is running and you can connect to it (it's not a networking problem). It is good to check this way for the IP address to which the domain is resolved and using the same domain to test connection.

First of all check if your site is online from a other location. It then lets you know if the site is down everywhere, or if only your network is unable to view it. It is also a good idea to check what the web browser returns.

**If only IP connection working**

- you can use whois to see what DNS servers serve up the hostname to the site: `whois www.example.com`
- you can use tools like `dig` or `host` to test DNS to see if the host name is resolving: `host www.example.org dns.example.org`
- you can also check global public dns servers: `host www.example.com 9.9.9.9`

If domain not resolved it's probably problem with DNS servers.

**If domain resolved properly**

- investigate the log files and resolve the issue regarding to the logs, it's the best way to show what's wrong
- check the http status code, usually it will be the response with the 5xx, maybe server is overload because clients making lot's of connection to the website or specific url? maybe your caching rules not working properly?
- check web/proxy server configuration (e.g. `nginx -t -c </path/to/nginx.conf>`), maybe another sysadmin has made some changes to the domain configuration?
- maybe something on the server has crashed? maybe run out of space or run out of memory?
- maybe it's a programming error on the website?

</details>

<details>
<summary><b>Load balancing can dramatically impact server performance. Discuss several load balancing mechanisms. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>List examples of network troubleshooting tools that can degrade during DNS issues. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explain difference between HTTP 1.1 and HTTP 2.0.</b></summary><br>

<b>HTTP/2</b> supports queries multiplexing, headers compression, priority and more intelligent packet streaming management. This results in reduced latency and accelerates content download on modern web pages.

Key differences with **HTTP/1.1**:

- it is binary, instead of textual
- fully multiplexed, instead of ordered and blocking
- can therefore use one connection for parallelism
- uses header compression to reduce overhead
- allows servers to "push" responses proactively into client caches

Useful resources:

- [What is HTTP/2 - The Ultimate Guide](https://kinsta.com/learn/what-is-http2/)

</details>

<details>
<summary><b>What is handshake mechanism and why do we need 3 way handshake?</b></summary><br>

**Handshaking** begins when one device sends a message to another device indicating that it wants to establish a communications channel. The two devices then send several messages back and forth that enable them to agree on a communications protocol.

A **three-way handshake** is a method used in a TCP/IP network to create a connection between a local host/client and server. It is a three-step method that requires both the client and server to exchange `SYN` and `ACK` (`SYN`, `SYN-ACK`, `ACK`) packets before actual data communication begins.

Useful resources:

- [Why do we need a 3-way handshake? Why not just 2-way?](https://networkengineering.stackexchange.com/questions/24068/why-do-we-need-a-3-way-handshake-why-not-just-2-way)

</details>

<details>
<summary><b>Why is UDP faster than TCP?</b></summary><br>

**UDP** is faster than **TCP**, and the simple reason is because its nonexistent acknowledge packet (`ACK`) that permits a continuous packet stream, instead of TCP that acknowledges a set of packets, calculated by using the TCP window size and round-trip time (`RTT`).

Useful resources:

- [UDP vs TCP, how much faster is it?](https://stackoverflow.com/questions/47903/udp-vs-tcp-how-much-faster-is-it)

</details>

<details>
<summary><b>Which, in your opinion, are the 5 most important OpenSSH parameters that improve the security? ***</b></summary><br>

To be completed.

Useful resources:

- [OpenSSH security and hardening](https://linux-audit.com/audit-and-harden-your-ssh-configuration/)

</details>

<details>
<summary><b>What is NAT? What is it used for?</b></summary><br>

It enables private IP networks that use unregistered IP addresses to connect to the Internet. **NAT** operates on a router, usually connecting two networks together, and translates the private (not globally unique) addresses in the internal network into legal addresses, before packets are forwarded to another network.

Workstations or other computers requiring special access outside the network can be assigned specific external IPs using **NAT**, allowing them to communicate with computers and applications that require a unique public IP address. **NAT** is also a very important aspect of firewall security.

Useful resources:

- [Network Address Translation (NAT) Concepts](http://www.firewall.cx/networking-topics/network-address-translation-nat/227-nat-concepts.html)

</details>

<details>
<summary><b>What is the purpose of Spanning Tree?</b></summary><br>

This protocol operates at layer 2 of the OSI model with the purpose of preventing loops on the network. Without **STP**, a redundant switch deployment would create broadcast storms that cripple even the most robust networks. There are several iterations based on the original IEEE 802.1D standard; each operates slightly different than the others while largely accomplishing the same loop-free goal.

</details>

<details>
<summary><b>How do you check which ports are listening?</b></summary><br>

Use the:

- `lsof -i`
- `ss -l`
- `netstat -atn` (for tcp)
- `netstat -aun` (for udp)
- `netstat -tulapn`

</details>

<details>
<summary><b>What mean <code>Host key verification failed</code> when you connect to the remote host? Do you accept it automatically?</b></summary><br>

`Host key verification failed` means that the host key of the remote host was changed. This can easily happen when connecting to a computer who's host keys in `/etc/ssh` have changed if that computer was upgraded without copying its old host keys. The host keys here are proof when you reconnect to a remote computer with ssh that you are talking to the same computer you connected to the first time you accessed it.

Whenever you connect to a server via SSH, that server's public key is stored in your home directory (or possibly in your local account settings if using a Mac or Windows desktop) file called **known_hosts**. When you reconnect to the same server, the SSH connection will verify the current public key matches the one you have saved in your **known_hosts** file. If the server's key has changed since the last time you connected to it, you will receive the above error.

Don't delete the entire **known_hosts** file as recommended by some people, this totally voids the point of the warning. It's a security feature to warn you that a man in the middle attack may have happened.

Before accepting the new host key, contact your/other system administrator for verification.

Useful resources:

- [Git error: "Host Key Verification Failed" when connecting to remote repository](https://stackoverflow.com/questions/13363553/git-error-host-key-verification-failed-when-connecting-to-remote-repository)

</details>

<details>
<summary><b>How do you connect to a mail server using <code>telnet</code>? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How do you kill program using e.g. 80 port in Linux?</b></summary><br>

To list any process listening to the port 80:

```bash
# with lsof
lsof -i:80

# with fuser
fuser 80/tcp
```

To kill any process listening to the port 80:

```bash
kill $(lsof -t -i:80)
```

or more violently:

```bash
kill -9 $(lsof -t -i:80)
```

or with `fuser` command:

```bash
fuser -k 80/tcp
```

Useful resources:

- [How to kill a process running on particular port in Linux?](https://stackoverflow.com/questions/11583562/how-to-kill-a-process-running-on-particular-port-in-linux/32592965)
- [Finding the PID of the process using a specific port?](https://unix.stackexchange.com/questions/106561/finding-the-pid-of-the-process-using-a-specific-port)

</details>

<details>
<summary><b>You get <code>curl: (56) TCP connection reset by peer</code>. What steps will you take to solve this problem?</b></summary><br>

- check if the URL is correct, maybe you should add `www` or set correctly `Host:` header? Check also scheme (http or https)
- check the domain is resolving into a correct IP address
- enable debug tracing with `--trace-ascii curl.dump`. `Recv failure` is a really generic error so its hard for more info
- use external proxy with `--proxy` for debug connection from external ip
- use network sniffer (e.g. `tcpdump`) for debug connection in the lower TCP/IP layers
- check firewall rules on the production environment and on the exit point of your network, also check your NAT rules
- check MTU size of packets traveling over your network
- check SSL version with ssl/tls `curl` params if you connecting to https protocol
- it may be a problem on the client side e.g. the netfilter drop or limit  connections from your IP address to the domain

Useful resources:

- [CURL ERROR: Recv failure: Connection reset by peer - PHP Curl](https://stackoverflow.com/questions/10285700/curl-error-recv-failure-connection-reset-by-peer-php-curl)

</details>

<details>
<summary><b>How do you allow traffic to/from specific IP with iptables?</b></summary><br>

For example:

```bash
/sbin/iptables -A INPUT -p tcp -s XXX.XXX.XXX.XXX -j ACCEPT
/sbin/iptables -A OUTPUT -p tcp -d  XXX.XXX.XXX.XXX -j ACCEPT
```

</details>

<details>
<summary><b>Explain four types of responses from firewall when scanning with <code>nmap</code>.</b></summary><br>

There might be four types of responses:

- **Open port** - few ports in the case of the firewall
- **Closed port** - most ports are closed because of the firewall
- **Filtered** - `nmap` is not sure whether the port is open or not
- **Unfiltered** - `nmap` can access the port but is still confused about the open status of the port

Useful resources:

- [NMAP - Closed vs Filtered](https://security.stackexchange.com/questions/182504/nmap-closed-vs-filtered)

</details>

<details>
<summary><b>What does <code>tcpdump</code> do and what are some examples for its use? ***</b></summary><br>

`tcpdump` is a powerful and widely used command-line packets sniffer or package analyzer tool which is used to capture or filter TCP/IP packets that received or transferred over a network on a specific interface.

`tcpdump` puts your network card into promiscuous mode, which basically tells it to accept every packet it receives. It allows the user to see all traffic being passed over the network. Wireshark uses pcap to capture packets.

</details>

###### Devops Questions

<details>
<summary><b>What some of the top DevOps tools? How do all these tools work together?</b></summary><br>

The most popular DevOps tools are mentioned below:

- **Git** : Version Control System tool
- **Jenkins** : Continuous Integration tool
- **Selenium** : Continuous Testing tool
- **Puppet**, **Chef**, **Ansible** : Configuration Management and Deployment tools
- **Nagios**, **Zabbix** : Continuous Monitoring tool
- **Docker** : Containerization tool

- Developers develop the code and this source code is managed by Version Control System tools like Git etc.
- Developers send this code to the Git repository and any changes made in the code is committed to this Repository
- Jenkins pulls this code from the repository using the Git plugin and build it using tools like Ant or Maven
- Configuration management tools like puppet deploys & provisions testing environment and then Jenkins releases this code on the test environment on which testing is done using tools like selenium
- Once the code is tested, Jenkins send it for deployment on the production server (even production server is provisioned & maintained by tools like puppet)
- After deployment It is continuously monitored by tools like Nagios
- Docker containers provides testing environment to test the build features

</details>

<details>
<summary><b>What is Agile and how is it beneficial?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is Continuous Integration and Continous Deployment?</b></summary><br>

To be completed.

</details>

###### Cyber Security Questions

<details>
<summary><b>What are salted hashes?</b></summary><br>

**Salt** at its most fundamental level is random data. When a properly protected password system receives a new password, it will create a hashed value for that password, create a new random salt value, and then store that combined value in its database. This helps defend against dictionary attacks and known hash attacks.

For example, if a user uses the same password on two different systems, if they used the same hashing algorithm, they could end up with the same hash value. However, if even one of the systems uses salt with its hashes, the values will be different.

The encrypted passwords in `/etc/shadow` file are stored in the following format:

```bash
$ID$SALT$ENCRYPTED
```

The `$ID` indicates the type of encryption, the `$SALT` is a random string (up to 16 characters) and `$ENCRYPTED` is a password’s hash.

</details>

<details>
<summary><b>Explain the four types of access control. ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What are some golden rules for reducing the impact of hacked system.</b></summary><br>

1) **The principle of least privilege**

You should configure services to run as a user with the least possible rights necessary to complete the service's tasks. This can contain a hacker even after they break in to a machine.

As an example, a hacker breaking into a system using a zero-day exploit of the Apache webserver service is highly likely to be limited to just the system memory and file resources that can be accessed by that process. The hacker would be able to download your html and php source files, and probably look into your mysql database, but they should not be able to get root or extend their intrusion beyond apache-accessible files.

Many default Apache webserver installations create the 'apache' user and group by default and you can easily configure the main Apache configuration file (`httpd.conf`) to run apache using those groups.

2) **The principle of separation of privileges**

If your web site only needs read-only access to the database, then create an account that only has read-only permissions, and only to that database.

**SElinux** is a good choice for creating context for security, `app-armor` is another tool. **Bastille** was a previous choice for hardening.

Reduce the consequence of any attack, by separating the power of the service that has been compromised into it own "Box".

3) **Whitelist, don't blacklist**

You're describing a blacklist approach. A whitelist approach would be much safer.

An exclusive club will never try to list everyone who can't come in; they will list everyone who can come in and exclude those not on the list.

Similarly, trying to list everything that shouldn't access a machine is doomed. Restricting access to a short list of programs/IP addresses/users would be more effective.

Of course, like anything else, this involves some trade-offs. Specifically, a whitelist is massively inconvenient and requires constant maintenance.

To go even further in the tradeoff, you can get great security by disconnecting the machine from the network.

**Also interesting are**:

Use the tools available. It's highly unlikely that you can do as well as the guys who are security experts, so use their talents to protect yourself.

- public key encryption provides excellent security
- enforce password complexity
- understand why you are making exceptions to the rules above - review your exceptions regularly
- hold someone to account for failure, it keeps you on your toes

Useful resources:

- [How to prevent zero day attacks (original)](https://serverfault.com/questions/391370/how-to-prevent-zero-day-attacks)

</details>

<details>
<summary><b>Developer uses private key on the server to deploy app through ssh. Why is this a security risk and what is the better, but not ideal, solution in such situations?</b></summary><br>

You have the private key for your personal account. The server needs your public key so that it can verify that your private key for the account you are trying to use is authorized.

The whole point with private keys is that they are private, meaning only you have your private key. If someone takes over your private key, it will be able to impersonate you any time he wants.

A better solutions is the use of ssh key forwarding. An essence, you need to create a `~/.ssh/config` file, if it doesn't exist. Then, add the hosts (either domain name or IP address in the file and set `ForwardAgent yes`). Example:

```bash
Host git.example.com
    User john
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa.git.example.com
    ForwardAgent yes
```

Your remote server must allow SSH agent forwarding on inbound connections and your local `ssh-agent` must be running.

Forwarding an ssh agent carries its own security risk. If someone on the remote machine can gain access to your forwarded ssh agent connection, they can still make use of your keys. However, this is better than storing keys on remote machines: the attacker can only use the ssh agent connection, not the key itself. Thus, only while you're logged into the remote machine can they do anything. If you store the key on the remote machine, they can make a copy of it and use it whenever they want.

If you use ssh keys remember about passphrases which is strongly recommended to reduce risk of keys accidentally leaking.

Useful resources:

- [How to forward local keypair in a SSH session?](https://stackoverflow.com/questions/12257968/how-to-forward-local-keypair-in-a-ssh-session)
- [Using SSH agent forwarding](https://developer.github.com/v3/guides/using-ssh-agent-forwarding/)
- [SSH Agent Forwarding considered harmful](https://heipei.github.io/2015/02/26/SSH-Agent-Forwarding-considered-harmful/)
- [Security Consideration while using ssh-agent](https://www.commandprompt.com/blog/security_considerations_while_using_ssh-agent/)

</details>

<details>
<summary><b>How would you secure a newly provisioned server?</b></summary><br>

- if machine is a new install, protect it from hostile network traffic, until the operating system is installed and hardened
- create a separate partition with the `nodev`, `nosuid`, and `noexec` options set for `/tmp`
- create separate partitions for `/var`, `/var/log`, `/var/log/audit`, and `/home`
- enable randomized virtual memory region placement
- remove legacy services (e.g. `telnet-server`, `rsh`, `rlogin`, `rcp`, `ypserv`, `ypbind`, `tftp`, `tftp-server`, `talk`, `talk-server`).
- limit connections to services running on the host to authorized users of the service via firewalls and other access control technologies
- disable source routed packet acceptance
- enable **TCP/SYN** cookies
- disable SSH root login
- install and configure **AIDE**
- install and configure **OSsec HIDS**
- configure **SELinux**
- all administrator or root access must be logged
- integrity checking of system accounts, group memberships, and their associated privileges should be enabled and tested
- set password creation requirements (e.g. with PAM)

Useful resources:

- [Security Harden CentOS 7](https://highon.coffee/blog/security-harden-centos-7/)
- [CentOS 7 Server Hardening Guide](https://www.lisenet.com/2017/centos-7-server-hardening-guide/)

</details>

<details>
<summary><b>What is the difference between Host Intrusion Detection and Network Intrusion Detection? Is one better than the other?</b></summary><br>

Host Intrusion Detection system runs on individual hosts, such as an anti-virus, while Network Intrusion Detection system oversees the network. One is not "better" than the other as they have similar but different functions. A **HIDS** is important to monitor and protect individual hosts generally from user actions, while a **NIDS** is important to monitor and protect hosts from each other as well as from outside networks.

</details>

<details>
<summary><b>What is Compliance?</b></summary><br>

Abiding by a set of standards set by a government/Independent party/organisation, e.g. an industry which stores, processes or transmits Payment related information needs to be complied with PCI DSS (Payment card Industry Data Security Standard). Other compliance examples can be an organisation complying with its own policies.

</details>

<details>
<summary><b>What is the difference between hashing and encryption?</b></summary><br>

**Hashing** is a form of cryptographic security which differs from **encryption** whereas **encryption** is a two step process used to first encrypt and then decrypt a message, **hashing** condenses a message into an irreversible fixed-length value, or hash.

</details>

<br>

### :diamond_shape_with_a_dot_inside: <a name="senior-sysadmin">Senior Sysadmin</a>

<details>
<summary><b>In the context of computing, what is Split-Brain and why is it a problem?</b></summary><br>

To be completed.

Useful resources:

- [What is Split brain and why do you need to worry about it?](https://www.45drives.com/community/articles/what-is-split-brain/)

</details>

<details>
<summary><b>What is Split-horizon DNS and how do you implement it?</b></summary><br>

To be completed.

Useful resources:

- [What is Split-Horizon DNS?](https://splitdns.net/)

</details>

###### System Questions

<details>
<summary><b>What are some keep elements to keep in mind when writing good documentation?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How would you remotely provision a blank server in a datacenter to be a LAMP stack web server with predefined users and configurations? Assume all datacenter hardware has been setup and networking side of things is also ready (e.g. VLAN tag). ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between EXT4, XFS, and ZFS? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>The Junior dev accidentally destroyed production database. How can you prevent such situations?</b></summary><br>

**Create disaster recovery plan**

Disaster recovery and business continuity planning are integral parts of the overall risk management for an organization. Is a documented process or set of procedures to recover and protect a business IT infrastructure.

If you don’t have a recovery solution, then your restoration efforts will become rebuilding efforts, starting from scratch to recreate whatever was lost.

You should use commonly occurring real life data disaster scenarios to simulate what your backups will and won’t do in a crisis.

**Create disaster recovery center**

As a result, in the event of unplanned interruptions in the functioning of the primary location, service and all operational activities are switched to the backup center and therefore the unavailability of services is limited to the absolute minimum.

Does the facility have sufficient bandwidth options and power to scale and deal with the increased load during a major disaster? Are resources available to periodically test failover?

**Create regular backups and tested it!**

Backups are a way to protect the investment in data. By having several copies of the data, it does not matter as much if one is destroyed (the cost is only that of the restoration of the lost data from the backup).

When you lose data, one thing is certain: downtime.

To assure the validity and integrity of any backup, it's essential to carry out regular restoration tests. Ideally, a test should be conducted after every backup completes to ensure data can be successfully secured and recovered. However, this often isn't practical due to a lack of available resources or time constraints.

Make backups of entire virtual machines and important components in the middle of them.

**Create snapshots: vm, disks or lvm**

Snapshots are perfect if you want to recover a server from a previous state but it's only a "quick method", it cannot restore the system after too many items changed.

Create them always before making changes on production environments (and not only).

Disk snapshots are used to generate a snapshot of an entire disk. These snapshots don't make it easy to restore individual chunks of data (e.g. a lost user account), though it's possible. The primary purpose is to restore entire disks in case of disk failure.

The LVM snapshots can be primarily used to easily copy data from production environment to staging environment.

Remember: Snapshots are not backups!

**Development and testing environments**

A production environment is the real instance of the application and its database used by the company or the clients. The production database has all the real data.

Setting up development environments based directly on the production database, instead of using a backup for this (removing the need for the above). Dev and test environment that your engineers can get to and a prod environment that only a few people can push updates to following an approved change.

All environments such as prod, dev and test should have one major difference: authorization data for services. For example postgres database instance on testing environment should be consistent (if possible) with the production base, however, in order to eliminate errors of database names and logins and passwords for authorization should be different.

**Single point of failure**

The general method to avoid single points of failures is to provide redundant components for each necessary resource, so service can continue if a component fails.

**Synchronization and replication process for databases**

The replication procedure is super fragile and prone to error.

A good idea is also slightly longer delay of data replication (e.g. for DRC). As in replicas, the data changes will usually be replicated within minutes, so the lost data won’t be on the replica database either once that happens.

**Create database model with users, roles and rights, use different methods of protection**

Only very advanced devs have permissions for db admin access. The other really don't need write access to clone a database. On the other hand just don't give a developer write access to prod.

The production database should refuse connections from any server and pc which isn't the one running the production application, even if it provides a valid username/password.

How the hell development machines can access a production database right like that? How about a simple firewall rule to just let the servers needing the DB data access the database?

**Create summary/postmortem documents after failures**

The post-mortem audience includes customers, direct reports, peers, the company's executive team and often investors.

Explain what caused the outage on a timeline. Every incident begins with a specific trigger at a specific time, which often causes some unexpected behavior. For example, our servers were rebooted and we expected them to come back up intact, which didn't happen.

Furthermore, every incident has a root cause: the reboot itself was trigger, however a bug in the driver caused the actual outage. Finally, there are consequences to every incident, the most obvious one is that the site goes down.

The post-mortem answers the single most important question of what could have prevented the outage.

Despite how painful an outage may have been, the worst thing you can do is to bury it and never properly close the incident in a clear and transparent way.

**If you also made a big mistake...**

  > "*Humans are just apes with bigger computers.*" - african_cheetah (Reddit)
  >
  > "*I've come to appreciate not having access to things I don't absolutely need.*" - warm_vanilla_sugar (Reddit)
  >
  > Document whatever happened somewhere. Write setup guides. Failure is instructive.

Useful resources:

- [Accidentally destroyed production database on first day of a job...](https://www.reddit.com/r/cscareerquestions/comments/6ez8ag/accidentally_destroyed_production_database_on/)
- [Postmortem of database outage of January 31](https://about.gitlab.com/2017/02/10/postmortem-of-database-outage-of-january-31/)
- [How to write an Incident Report/Postmortem](https://sysadmincasts.com/episodes/20-how-to-write-an-incident-report-postmortem)

</details>

<details>
<summary><b>How do you add new disk in Linux server without rebooting? How do you rescan and add it in LVM?</b></summary><br>

To be completed.

Useful resources:

- [How to Add New Disk in Linux CentOS 7 Without Rebooting](https://linoxide.com/linux-how-to/add-new-disk-centos-7-without-rebooting/)

</details>

<details>
<summary><b>What does it mean to mount the root file system? ***</b></summary><br>

To be completed.

Useful resources:

- [What does "mounting a root file system" mean exactly?](https://superuser.com/questions/193918/what-does-mounting-a-root-file-system-mean-exactly)
- [How does a kernel mount the root partition?](https://unix.stackexchange.com/questions/9944/how-does-a-kernel-mount-the-root-partition)

</details>

<details>
<summary><b>A bare metal server's root partition is full and will not boot. How do you troubleshoot and fix the issue? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What considerations come into play when designing a highly available application, both at the architecture level and the application level? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explain the risks and caveats of LVM. ***</b></summary><br>

**Risks of using LVM**

- Vulnerable to write caching issues with SSD or VM hypervisor
- Harder to recover data due to more complex on-disk structures
- Harder to resize filesystems correctly
- Snapshots are hard to use, slow and buggy
- Requires some skill to configure correctly given these issues

Useful resources:

- [LVM dangers and caveats (original)](https://serverfault.com/questions/279571/lvm-dangers-and-caveats)

</details>

<details>
<summary><b>What if <code>kill -9</code> does not work? Describe exceptions for which the use of SIGKILL is insufficient.</b></summary><br>

`kill -9` (`SIGKILL`) always works, provided you have the permission to kill the process. Basically either the process must be started by you and not be setuid or setgid, or you must be root. There is one exception: even root cannot send a fatal signal to PID 1 (the init process).

However `kill -9` is not guaranteed to work immediately. All signals, including `SIGKILL`, are delivered asynchronously: the kernel may take its time to deliver them. Usually, delivering a signal takes at most a few microseconds, just the time it takes for the target to get a time slice. However, if the target has blocked the signal, the signal will be queued until the target unblocks it.

Normally, processes cannot block `SIGKILL`. But kernel code can, and processes execute kernel code when they call system calls.

A process blocked in a system call is in uninterruptible sleep. The `ps` or `top` command will (on most unices) show it in state **D**.

To remove a **D** State Process, since it is uninterruptible, only a machine reboot can solve the problem in case its not automatically handled by the system.

Usually there is a very few chance that a process stays in **D** State for long. And if it does then there is something not properly being handled in the system. This can be a potential bug as well.

A classical case of long uninterruptible sleep is processes accessing files over NFS when the server is not responding; modern implementations tend not to impose uninterruptible sleep (e.g. under Linux, the intr mount option allows a signal to interrupt NFS file accesses).

You may sometimes see entries marked **Z** (or **H** under Linux) in the `ps` or `top` output. These are technically not processes, they are zombie processes, which are nothing more than an entry in the process table, kept around so that the parent process can be notified of the death of its child. They will go away when the parent process pays attention (or dies).

Summary exceptions:

- Zombie processes cannot be killed since they are already dead and waiting for their parent processes to reap them
- Processes that are in the blocked state will not die until they wake up again
- The init process is special: It does not get signals that it does not want to handle, and thus it can ignore **SIGKILL**. An exception from this exception is while init is ptraced on Linux
- An uninterruptibly sleeping process may not terminate (and free its resources) even when sent **SIGKILL**. This is one of the few cases in which a Unix system may have to be rebooted to solve a temporary software problem

Useful resources:

- [What if kill -9 does not work? (original)](https://unix.stackexchange.com/questions/5642/what-if-kill-9-does-not-work)
- [How to kill a process in Linux if kill -9 has no effect](https://serverfault.com/questions/458261/how-to-kill-a-process-in-linux-if-kill-9-has-no-effect)
- [When should I not kill -9 a process?](https://unix.stackexchange.com/questions/8916/when-should-i-not-kill-9-a-process)
- [SIGTERM vs. SIGKILL](https://major.io/2010/03/18/sigterm-vs-sigkill/)

</details>

<details>
<summary><b>What is the main advantage of using <code>chroot</code>? When and why do we use it? What is the purpose of the mount dev, proc, sys in a chroot environment?</b></summary><br>

An advantage of having a chroot environment is the file-system is totally isolated from the physical host. `chroot` has a separate file-system inside the file-system, the difference is its uses a newly created root(/) as its root directory.

A chroot jail is a way to isolate a process and its children from the rest of the system. It should only be used for processes that don't run as root, as root users can break out of the jail very easily.

The idea is that you create a directory tree where you copy or link in all the system files needed for a process to run. You then use the `chroot()` system call to change the root directory to be at the base of this new tree and start the process running in that chroot'd environment. Since it can't actually reference paths outside the modified root, it can't perform operations (read/write etc.) maliciously on those locations.

On Linux, using a bind mounts is a great way to populate the chroot tree. Using that, you can pull in folders like `/lib` and `/usr/lib` while not pulling in `/usr`, for example. Just bind the directory trees you want to directories you create in the jail directory.

Chroot environment is useful for:

- reinstall bootloader
- reset a forgotten password
- perform a kernel upgrade (or downgrade)
- rebuild your initramdisk
- fix your **/etc/fstab**
- reinstall packages using your package manager
- whatever

When working in a chrooted environment, there is a few special file systems that needs to be mounted so all programs behave properly.

Limitation is that `/dev`, `/sys` and `/proc` are not mounted by default but needed for many tasks.

Useful resources:

- [Its all about Chroot](https://medium.com/@itseranga/chroot-316dc3c89584)
- [Best Practices for UNIX chroot() Operations](http://www.unixwiz.net/techtips/chroot-practices.html)
- [Is there an easier way to chroot than bind-mounting?](https://askubuntu.com/questions/32418/is-there-an-easier-way-to-chroot-than-bind-mounting)
- [What's the proper way to prepare chroot to recover a broken Linux installation?](https://superuser.com/questions/111152/whats-the-proper-way-to-prepare-chroot-to-recover-a-broken-linux-installation)

</details>

<details>
<summary><b>What are segmentation faults (segfaults), and how can identify what's causing them?</b></summary><br>

A **segmentation fault** (aka _segfault_) is a common condition that causes programs to crash. Segfaults are caused by a program trying to read or write an illegal memory location.

Program memory is divided into different segments:

- a text segment for program instructions
- a data segment for variables and arrays defined at compile time
- a stack segment for temporary (or automatic) variables defined in subroutines and functions
- a heap segment for variables allocated during runtime by functions, such as `malloc` (in C)

In practice, segfaults are almost always due to trying to read or write a non-existent array element, not properly defining a pointer before using it, or (in C programs) accidentally using a variable's value as an address. Thus, when Process A reads memory location 0x877, it reads information residing at a different physical location in RAM than when Process B reads its own 0x877.

All modern operating systems support and use segmentation, and so all can produce a segmentation fault.

Segmentation fault can also occur under following circumstances:

- a buggy program/command, which can be only fixed by applying patch
- it can also appear when you try to access an array beyond the end of an array under C programming
- inside a chrooted jail this can occur when critical shared libs, config file or `/dev/` entry missing
- sometime hardware or faulty memory or driver can also create problem
- maintain suggested environment for all computer equipment (overheating can also generate this problem)

To debug this kind of error try one or all of the following techniques:

- enable core files: `$ ulimit -c unlimited`
- reproduce the crash: `$ ./<program>`
- debug crash with gdb: `$ gdb <program> [core file]`
- or run `LD_PRELOAD=...path-to.../libSegFault.so <program>` to get a report with backtrace, loaded libs, etc

Also:

- make sure correct hardware installed and configured
- always apply all patches and use updated system
- make sure all dependencies installed inside jail
- turn on core dumping for supported services such as Apache
- use `strace` which is a useful diagnostic, instructional, and debugging tool

Sometimes segmentation faults are not caused by bugs in the program but are caused instead by system memory limits being set too low. Usually it is the limit on stack size that causes this kind of problem (stack overflows). To check memory limits, use the `ulimit` command in bash.

Useful resources:

- [What are segmentation faults (segfaults), and how can I identify what's causing them? (original)](https://kb.iu.edu/d/aqsj)
- [What is a segmentation fault on Linux?](https://stackoverflow.com/questions/3200526/what-is-a-segmentation-fault-on-linux)
- [Segmentation fault when calling a recursive bash function](https://unix.stackexchange.com/questions/296641/segmentation-fault-when-calling-a-recursive-bash-function)
- [Troubleshooting Segmentation Violations/Faults](http://web.mit.edu/10.001/Web/Tips/tips_on_segmentation.html)
- [Can one use libSegFault.so to get backtraces for SIGABRT?](https://stackoverflow.com/questions/18706496/can-one-use-libsegfault-so-to-get-backtraces-for-sigabrt)

</details>

<details>
<summary><b>In terms of *nix systems, what does it mean when we say everything is a file?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between /dev/random and /dev/urandom ?</b></summary><br>

You should use `/dev/urandom`, not `/dev/random`. The differences between `/dev/random` and `/dev/urandom` are:

 - `/dev/random` might be theoretically better _in the context of an information-theoretically secure algorithm_. This is the kind of algorithm which is secure against today's technology, and also tomorrow's technology, and technology used by aliens.

 - `/dev/urandom` will not block, while `/dev/random` may do so. `/dev/random` maintains a counter of "how much entropy it still has" under the assumption that any bits it has produced is a lost entropy bit. Blocking induces very real issues, e.g. a server which fails to boot after an automated install because it is stalling on its SSH server key creation.

So you want to use `/dev/urandom` and stop to worry about this entropy business.

The trick is that `/dev/urandom` never blocks, ever, even when it should: `/dev/urandom` is secure as long as it has received enough bytes of "initial entropy" since the last boot (32 random bytes are enough). A normal Linux installation will create a random seed (from `/dev/random`) upon installation, and save it on the disk. Upon each reboot, the seed will be read, fed into `/dev/urandom`, and a new seed immediately generated (from `/dev/urandom`) to replace it. Thus, this guarantees that `/dev/urandom` will always have enough initial entropy to produce cryptographically strong alea, perfectly sufficient for any mundane cryptographic job, including password generation.

Should any of these daemons require randomness when all available entropy has been exhausted, they may pause to wait for more, which can cause excessive delays in your application. Even worse, since most modern applications will either resort to using its own random seed created at program initialization, or to using `/dev/urandom` to avoid blocking, your applications will suffer from lower quality random data. This can affect the integrity of your secure communications, and can increase the chance of cryptoanalysis on your private data.

Useful resources:

- [When to use /dev/random vs /dev/urandom](https://unix.stackexchange.com/questions/324209/when-to-use-dev-random-vs-dev-urandom)

</details>

<details>
<summary><b>What is the difference between <code>/sbin/nologin</code>, <code>/bin/false</code>, and <code>/bin/true</code>?</b></summary><br>

When `/sbin/nologin` is set as the shell, if user with that shell logs in, they'll get a polite message saying 'This account is currently not available'.

`/bin/false` is just a binary that immediately exits, returning false, when it's called, so when someone who has false as shell logs in, they're immediately logged out when false exits. Setting the shell to `/bin/true` has the same effect of not allowing someone to log in but false is probably used as a convention over true since it's much better at conveying the concept that person doesn't have a shell.

`/bin/nologin` is the more user-friendly option, with a customizable message given to the user trying to log in, so you would theoretically want to use that; but both nologin and false will have the same end result of someone not having a shell and not being able to ssh in.

Useful resources:

- [What's the difference between /sbin/nologin and /bin/false](https://unix.stackexchange.com/questions/10852/whats-the-difference-between-sbin-nologin-and-bin-false)
- [Why do some system users have /usr/bin/false as their shell?](https://superuser.com/questions/1183311/why-do-some-system-users-have-usr-bin-false-as-their-shell)

</details>

<details>
<summary><b>Which symptoms might be suffering from a disk bottleneck? ***</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Load averages are above 30.00 on a server with 24 cores but CPU shows around 70 percent idle. One of the common causes of this condition is? How can this be debugged and fixed?</b></summary><br>

Requests which involve disk I/O can be slowed greatly if cpu(s) needs to wait on the disk to read or write data. I/O Wait, is the percentage of time the CPU has to wait on disk.

First, attempt to confirm if disk I/O is slowing down application performance by using a few terminal command line tools (`top`, `atop` and `iotop`).

Example of debug:

- answering whether or not I/O is causing system slowness
- finding which disk is being written to
- finding the processes that are causing high I/O
- process list **state**
- finding what files are being written too heavily
- do you see your copy process put in **D** state waiting for I/O work to be done by pdflush?
- do you see heavy synchronous write activity on your disks?

also:

- using `top` command - load averages and wa (wait time)
- using `atop` command to monitor DSK (disk) I/O stats
- using `iotop` command for real-time insight on disk read/writes

For improvement performance:

- check drive array configuration
- check disk queuing algorithms and tuning them
- tuning general block I/O parameters
- tuning virtual memory management to improve I/O performance
- check and tuning mount options and filesystem params (also responsible for cache)

Useful resources:

- [Linux server performance: Is disk I/O slowing your application? (original)](https://haydenjames.io/linux-server-performance-disk-io-slowing-application/)
- [Troubleshooting High I/O Wait in Linux](https://bencane.com/2012/08/06/troubleshooting-high-io-wait-in-linux/)
- [Debugging Linux I/O latency](https://superuser.com/questions/396696/debugging-linux-i-o-latency)
- [How do pdflush, kjournald, swapd, etc interoperate?](https://unix.stackexchange.com/questions/76970/how-do-pdflush-kjournald-swapd-etc-interoperate)
- [5 ways to improve HDD speed on Linux](https://thecodeartist.blogspot.com/2012/06/improving-hdd-performance-linux.html)

</details>

<details>
<summary><b>You have just discovered a server you manage for the company you work at has been hacked. Go through the steps of what you do and recover from this.</b></summary><br>

To be completed.

</details>

<details>
<summary><b>You have a LAMP stack with Nginx as a reverse proxy. Going to the site served by this web server results in a 500 Internal Server Error. List the possible causes for this issue.</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Is it safe to attach the <code>strace</code> to a running process on the production? What are the consequences?</b></summary><br>

`strace` is the system call tracer for Linux. It currently uses the arcane `ptrace()` (process trace) debugging interface, which operates in a violent manner: **pausing the target process** for each syscall so that the debugger can read state. And doing this twice: when the syscall begins, and when it ends.

This means `strace` pauses your application twice for each syscall, and context-switches each time between the application and `strace`. It's like putting traffic metering lights on your application.

Cons:

- can cause significant and sometimes massive performance overhead, in the worst case, slowing the target application by over 100x. This may not only make it unsuitable for production use, but any timing information may also be so distorted as to be misleading
- can't trace multiple processes simultaneously (with the exception of followed children)
- visibility is limited to the system call interface

Useful resources:

- [strace Wow Much Syscall (original)](http://www.brendangregg.com/blog/2014-05-11/strace-wow-much-syscall.html)

</details>

<details>
<summary><b>MySQL replication for one Slave is failing. How do you troubleshoot the issue? ***</b></summary><br>

Useful resources:

- [MySQL: Troubleshooting Replication](https://dev.mysql.com/doc/mysql-replication-excerpt/8.0/en/replication-problems.html)

</details>

###### Network Questions

<details>
<summary><b>Is it better to set <code>-j REJECT</code> or <code>-j DROP</code> in iptables? ***</b></summary><br>

To be completed.

Useful resources:
- [https://unix.stackexchange.com/questions/109459/is-it-better-to-set-j-reject-or-j-drop-in-iptables](https://unix.stackexchange.com/questions/109459/is-it-better-to-set-j-reject-or-j-drop-in-iptables)
- [Drop versus Reject](https://www.chiark.greenend.org.uk/~peterb/network/drop-vs-reject)

</details>

<details>
<summary><b>What is ARP?</b></summary><br>

ARP, or Address Resolution Protocol can be likened to DNS for MAC Addresses. Standard DNS allows for the mapping of human-friendly URLs to IP addresses, while ARP allows for the mapping of IP addresses to MAC addresses. In this way it lets systems go from a regular domain name down to the actual piece of hardware it resides upon.

</details>

<details>
<summary><b>If you try resolve hostname you get <code>NXDOMAIN</code> from <code>host</code> command. Your <code>resolv.conf</code> stores two nameservers but only second of this store this domain name. Why did not the local resolver check the second nameserver?</b></summary><br>

**NXDOMAIN** is nothing but non-existent Internet or Intranet domain name. If domain name is unable to resolved using the DNS, a condition called the **NXDOMAIN** occurred.

The default behavior for `resolv.conf` and the `resolver` is to try the servers in the order listed. The resolver will only try the next nameserver if the first nameserver times out.

The algorithm used is to try a name server, and if the query times out, try the next, until out of name servers, then repeat trying all the name servers until a maximum number of retries are made.

If a nameserver responds with **SERVFAIL** or a referral (**nofail**) or terminate query (**fail**) also only the first dns server will be used.

Example:

```
nameserver 192.168.250.20   # it's not a dns
nameserver 8.8.8.8          # not store gate.test.int
nameserver 127.0.0.1        # store gate.test.int
```

so if you check:

```
host -v -t a gate.test.int
Trying "gate.test.int"                        # trying first dns (192.168.250.20) but response is time out, so try the next nameserver
Host gate.test.int not found: 3(NXDOMAIN)     # ok but response is NXDOMAIN (not found this domain name)
Received 88 bytes from 8.8.8.8#53 in 43 ms
Received 88 bytes from 8.8.8.8#53 in 43 ms
                                              # so the last server in the list was not asked
```

To avoid this you can use e.g. `nslookup` command which will use the second nameserver if it receives a **SERVFAIL** from the first nameserver.

Useful resources:

- [Second nameserver in /etc/resolv.conf not picked up by wget](https://serverfault.com/questions/398837/second-nameserver-in-etc-resolv-conf-not-picked-up-by-wget)

</details>

<details>
<summary><b>A client of the company you work at reports their server has stopped receiving data from your server. Go through the steps of troubleshooting the issue both on your end and your communications with them.</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is SNI SSL and in which cases it is useful?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>In the context of mail servers, is :fail: or :blackhole: better? ***</b></summary><br>

To be completed.

Useful resources:

- [Why you should use :fail:](https://www.configserver.com/free/fail.html)
- [Should I let email bounce or send it to a blackhole?](https://serverfault.com/questions/607568/should-i-let-email-bounce-or-send-it-to-a-blackhole)

</details>

<details>
<summary><b>What types of DNS cache are being checked when you type example.com in your browser and press return?</b></summary><br>

Browser checks if the domain is in its cache. When this cache fails, it simply asks the OS to resolve the domain.

The OS resolver has it's own cache which it will check. If it fails this, it resorts to asking the OS configured DNS servers.

The OS configured DNS servers will typically be configured by DHCP from the router where the DNS servers are likely to be the ISP's DNS servers configured by DHCP from the internet gateway to the router.

In the event the router has it's own DNS servers, it may have it's own cache otherwise you should be directed straight to your ISP's DNS servers most typically as soon as the OS cache was found to be empty.

Useful resources:

- [What happens when...](https://github.com/alex/what-happens-when)
- [DNS Explained - How Your Browser Finds Websites](https://scotch.io/tutorials/dns-explained-how-your-browser-finds-websites)
- [Firefox invalidate dns cache](https://stackoverflow.com/questions/13063496/firefox-invalidate-dns-cache)

</details>

<details>
<summary><b>What are the layers in OSI Reference Models? Describe each layer briefly.</b></summary><br>

a) <b>Physical Layer (Layer 1)</b>: It converts data bits into electrical impulses or radio signals. Example: Ethernet.

b) <b>Data Link Layer (Layer 2)</b>: At the Data Link layer, data packets are encoded and decoded into bits and it provides a node to node data transfer. This layer also detects the errors that occurred at Layer 1.

c) <b>Network Layer (Layer 3)</b>: This layer transfers variable length data sequence from one node to another node in the same network. This variable-length data sequence is also known as “Datagrams”.

d) <b>Transport Layer (Layer 4)</b>: It transfers data between nodes and also provides acknowledgment of successful data transmission. It keeps track of transmission and sends the segments again if the transmission fails.

e) <b>Session Layer (Layer 5)</b>: This layer manages and controls the connections between computers. It establishes, coordinates, exchange and terminates the connections between local and remote applications.

f) <b>Presentation Layer (Layer 6)</b>: It is also called as “Syntax Layer”. Layer 6 transforms the data into the form in which the application layer accepts.

g) <b>Application Layer (Layer 7)</b>: This is the last layer of the OSI Reference Model and is the one that is close to the end-user. Both end-user and application layer interacts with the software application. This layer provides services for email, file transfer, etc.

</details>

###### Devops Questions

<details>
<summary><b>In what situations is Docker and Kubernetes viable for production? When are they not the proper solutions for production? ***</b></summary><br>

To be completed.

</details>

###### Cyber Security Questions

<details>
<summary><b>Explain briefly how the Spectre vulnerability works.</b></summary><br>

To be completed.

Useful resources:

- [Spectre (security vulnerability)](https://en.wikipedia.org/wiki/Spectre_(security_vulnerability))

</details>

<details>
<summary><b>How would you break into a system? How would you prevent these attacks?</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between policies, processes and guidelines?</b></summary><br>

As **security policy** defines the security objectives and the security framework of an organisation. A **process** is a detailed step by step how to document that specifies the exact action which will be necessary to implement important security mechanism. **Guidelines** are recommendations which can be customized and used in the creation of procedures.

</details>

<br>

## <a name="extra-knowledge">Extra Knowledge</a>

<details>
<summary><b>Explain what is Event-Driven architecture and how it improves performance?</b></summary><br>

An event-driven architecture uses events to trigger and communicate between decoupled services; an event being a change in state. Event-driven architecture allows for proper and easier decoupling of services, less resource usage by being push-based, and easier to add consumers to scale.

</details>

<details>
<summary><b>Explain <code>:(){ :|:& };:</code> and how stop this code if you are already logged into a system?</b></summary><br>

It's a **fork bomb**.

- `:()` - this defines the function. `:` is the function name and the empty parenthesis shows that it will not accept any arguments
- `{ }` - these characters shows the beginning and end of function definition
- `:|:` - it loads a copy of the function `:` into memory and pipe its output to another copy of the `:` function, which has to be loaded into memory
- `&` - this will make the process as a background process, so that the child processes will not get killed even though the parent gets auto-killed
- `:` - final `:` will execute the function again and hence the chain reaction begins

The best way to protect a multi-user system is to use **PAM** to limit the number of processes a user can use. We know the biggest problem with a fork bomb is the fact it takes up so many processes.

So we have two ways of attempting to fix this, if you are already logged into the system:
- execute a **SIGSTOP** command to stop the process: `killall -STOP -u user1`
- if you can't run at the command line you will have to use `exec` to force it to run (due to processes all being used): `exec killall -STOP -u user1`

With fork bombs, the best thing to do is preventing it from being an issue in the first place.

</details>

<details>
<summary><b>How do you recover a deleted file still held open, e.g. by Apache?</b></summary><br>

If a file has been deleted but is still open, that means the file still exists in the filesystem (it has an inode) but has a hard link count of 0. Since there is no link to the file, you cannot open it by name. There is no facility to open a file by inode either.

Linux exposes open files through special symbolic links under `/proc`. These links are called `/proc/12345/fd/42` where 12345 is the **PID** of a process and 42 is the number of a file descriptor in that process. A program running as the same user as that process can access the file (the read/write/execute permissions are the same you had as when the file was deleted).

The name under which the file was opened is still visible in the target of the symbolic link: if the file was `/var/log/apache/foo.log`, then the target of the link is `/var/log/apache/foo.log (deleted)`.

Thus you can recover the content of an open deleted file given the **PID** of a process that has it open and the descriptor that it's opened on like this:

```bash
recover_open_deleted_file () {
  old_name=$(readlink "$1")
  case "$old_name" in
    *' (deleted)')
      old_name=${old_name%' (deleted)'}
      if [ -e "$old_name" ]; then
        new_name=$(TMPDIR=${old_name%/*} mktemp)
        echo "$oldname has been replaced, recovering content to $new_name"
      else
        new_name="$old_name"
      fi
      cat <"$1" >"$new_name";;
    *) echo "File is not deleted, doing nothing";;
  esac
}
recover_open_deleted_file "/proc/$pid/fd/$fd"
```

If you only know the process **ID** but not the descriptor, you can recover all files with:

```bash
for x in /proc/$pid/fd/* ; do
  recover_open_deleted_file "$x"
done
```

If you don't know the process **ID** either, you can search among all processes:

```bash
for x in /proc/[1-9]*/fd/* ; do
  case $(readlink "$x") in
    /var/log/apache/*) recover_open_deleted_file "$x";;
  esac
done
```

You can also obtain this list by parsing the output of `lsof`, but it isn't simpler nor more reliable nor more portable (this is Linux-specific anyhow).

</details>

<details>
<summary><b>Rsync triggered the Linux OOM killer on a single 50 GB file. How does the OOM killer decide which process to kill first? How to control this?</b></summary><br>

Major distribution kernels set the default value of `/proc/sys/vm/overcommit_memory` to zero, which means that processes can request more memory than is currently free in the system.

If memory is exhaustively used up by processes, to the extent which can possibly threaten the stability of the system, then the **OOM killer** comes into the picture.

NOTE: It is the task of the **OOM Killer** to continue killing processes until enough memory is freed for the smooth functioning of the rest of the process that the Kernel is attempting to run.

The **OOM Killer** has to select the best process(es) to kill. Best here refers to that process which will free up the maximum memory upon killing and is also the least important to the system.

The primary goal is to kill the least number of processes that minimizes the damage done and at the same time maximizing the amount of memory freed.

To facilitate this, the kernel maintains an `oom_score` for each of the processes. You can see the oom_score of each of the processes in the `/proc` filesystem under the pid directory.

  > When analyzing OOM killer logs, it is important to look at what triggered it.

```bash
cat /proc/10292/oom_score
```

The higher the value of `oom_score` of any process, the higher is its likelihood of getting killed by the **OOM Killer** in an out-of-memory situation.

If you want to create a special control group containing the list of processes which should be the first to receive the **OOM killer's** attention, create a directory under `/mnt/oom-killer` to represent it:

```bash
mkdir lambs
```

Set `oom.priority` to a value high enough:

```bash
echo 256 > /mnt/oom-killer/lambs/oom.priority
```

`oom.priority` is a 64-bit unsigned integer, and can have a maximum value an unsigned 64-bit number can hold. While scanning for the process to be killed, the **OOM-killer** selects a process from the list of tasks with the highest `oom.priority` value.

Add the PID of the process to be added to the list of tasks:

```bash
echo <pid> > /mnt/oom-killer/lambs/tasks
```

To create a list of processes, which will not be killed by the **OOM-killer**, make a directory to contain the processes:

```bash
mkdir invincibles
```

Setting `oom.priority` to zero makes all the process in this cgroup to be excluded from the list of target processes to be killed.

```bash
echo 0 > /mnt/oom-killer/invincibles/oom.priority
```

To add more processes to this group, add the pid of the task to the list of tasks in the invincible group:

```bash
echo <pid> > /mnt/oom-killer/invincibles/tasks
```

Useful resources:

- [Rsync triggered Linux OOM killer on a single 50 GB file](https://serverfault.com/questions/724469/rsync-triggered-linux-oom-killer-on-a-single-50-gb-file)
- [Taming the OOM killer](https://lwn.net/Articles/317814/)

</details>

<details>
<summary><b>You have a lot of sockets hanging in <code>TIME_WAIT</code>. Your http service behind proxy serve a lot of small http requests. How to check and reduce <code>TIME_WAIT</code> sockets? ***</b></summary><br>

To be completed.

Useful resources:

- [How to reduce number of sockets in TIME_WAIT?](https://serverfault.com/questions/212093/how-to-reduce-number-of-sockets-in-time-wait)

</details>

<details>
<summary><b>In context of an Operating System, what are Protection Rings? ***</b></summary><br>

- [What are Rings in Operating Systems?](https://www.baeldung.com/cs/os-rings)
- [Protecting Ring](https://en.wikipedia.org/wiki/Protection_ring)

</details>

<details>
<summary><b>Is it possible to have SSL certificate for IP address, not domain name?</b></summary><br>

It is possible (but rarely used) as long as it is a public IP address.

An SSL certificate is typically issued to a Fully Qualified Domain Name (FQDN) such as `https://www.domain.com`. However, some organizations need an SSL certificate issued to a public IP address. This option allows you to specify a public IP address as the Common Name in your Certificate Signing Request (CSR). The issued certificate can then be used to secure connections directly with the public IP address (e.g. `https://1.1.1.1`.).

According to the CA Browser forum, there may be compatibility issues with certificates for IP addresses unless the IP address is in both the commonName and subjectAltName fields. This is due to legacy SSL implementations which are not aligned with RFC 5280, notably, Windows OS prior to Windows 10.

Useful resources:

- [Are SSL certificates bound to the servers ip address?](https://stackoverflow.com/questions/1095780/are-ssl-certificates-bound-to-the-servers-ip-address)
- [SSL certificate for a public IP address?](https://serverfault.com/questions/193775/ssl-certificate-for-a-public-ip-address)

</details>

