<p align="center">
    <img src="https://github.com/trimstray/sysadmin-test-questions/blob/master/doc/img/sysadmin_preview.png"
        alt="Master">
</p>

<br>

<p align="center">"<i>A great Admin doesn't need to know everything, but they should be able to come up with amazing solutions to impossible projects.</i>" - cwheeler33 (ServerFault)</p>

<p align="center">"<i>My skills are making things work, not knowing a billion facts. [...] If I need to fix a system I’ll identify the problem, check the logs and look up the errors. If I need to implement a solution I’ll research the right solution, implement and document it, the later on only really have a general idea of how it works unless I interact with it frequently... it’s why it’s documented.</i>" - Sparcrypt (Reddit)</p>

<br>

<p align="center">
  <a href="https://github.com/trimstray/sysadmin-test-questions/tree/master">
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
  <a href="https://github.com/trimstray/sysadmin-test-questions/graphs/contributors">
    contributors
  </a>
</div>


<br>

****

:information_source: This project contains **examples** of test questions and answers that can be used during an interview or exam for positions such as **\*nix System Administrator**.

:warning: Questions marked '<b>*</b>' don't have answers yet - make a pull request to add them!

:bangbang: The answers are only examples and do not exhaust the whole topic.

:traffic_light: If you find a question which doesn't make sense, or one of the answers doesn't seem right; please make a pull request! Feedback and advice is welcome.

## Table of Contents

- <b>[Introduction](#introduction)</b>
  * [Simple Questions](#simple-questions) - 11 questions.
- <b>[General Knowledge](#general-knowledge)</b>
  * [Junior Sysadmin](#junior-sysadmin) - 51 questions.
  * [Regular Sysadmin](#regular-sysadmin) - 73 questions.
  * [Senior Sysadmin](#senior-sysadmin) - 78 questions.
- <b>[Secret Knowledge](#secret-knowledge)</b>
  * [Guru Sysadmin](#guru-sysadmin) - 12 questions.

## <a name="general-knowledge">Introduction</a>

### :diamond_shape_with_a_dot_inside: <a name="simple-questions">Simple Questions</a>

- <b>What did you learn this week?</b>
- <b>What excites or interests you about the Sysadmin world?</b>
- <b>What is a recent technical challenge you experienced and how did you solve it?</b>
- <b>Tell me about the last major project you finished.</b>
- <b>Do you contribute to any open source projects?</b>
- <b>Describe the setup of your homelab.</b>
- <b>What personal achievement are you most proud of?</b>
- <b>Tell me about the biggest mistake you've made.</b>
- <b>Tell me about your favorite UNIX-like system.</b>
- <b>Tell me about how you manage your knowledge database (e.g. wikis).</b>
- <b>What news sources do you check daily? (Sysadmin or security-related)</b>

## <a name="general-knowledge">General Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="junior-sysadmin">Junior Sysadmin</a>

###### System Questions

<details>
<summary><b>Give some examples of Linux distribution names.</b></summary><br>

- Red Hat Enterprise Linux
- Fedora
- CentOS
- Debian
- Ubuntu
- SUSE Linux Enterprise Server (SLES)
- SUSE Linux Enterprise Desktop (SLED)
- Slackware

Useful resources:

- [List of Linux distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions)

</details>

<details>
<summary><b>What are the differences between Unix, Linux, BSD and GNU?</b></summary><br>

GNU isn't really an OS. It's more of a set of rules or philosophies that govern free software, that at the same time gave birth to a bunch of tools while trying to create an OS. So GNU tools are basically open versions of tools that already existed, but were reimplemented to conform to principals of open software. GNU/Linux is a mesh of those tools and the Linux kernel to form a complete OS, but there are other "GNU"s, e.g. GNU/Hurd.

Unix and BSD are "older" implementations of POSIX that are various levels of "closed source". Unix is usually totally closed source, but there are as many flavors of Unix as there are Linux (if not more). BSD is not usually considered "open", but it was considered to be very open when it was released. Its licensing also allowed for commercial use with far fewer restrictions than the more "open" licenses of the time allowed.

Linux is the newest of the four. Strictly speaking, it's "just a kernel"; however, in general, it's thought of as a full OS when combined with GNU Tools and several other core components.

The main governing differences between these are their ideals. Unix, Linux, and BSD have different ideals that they implement. They are all POSIX, and are all basically interchangeable. They do solve some of the same problems in different ways. So other then ideals and how they choose to implement POSIX standards, there is little difference.

For more info I suggest your read a brief article on the creation of GNU, OSS, Linux, BSD, and UNIX. They will be slanted towards their individual ideas, but those articles should give you a better idea of the differences.

Useful resources:

- [What is the difference between Unix, Linux, BSD and GNU? (original)](https://unix.stackexchange.com/questions/104714/what-is-the-difference-between-unix-linux-bsd-and-gnu)
- [The Great Debate: Is it Linux or GNU/Linux?](https://www.howtogeek.com/139287/the-great-debate-is-it-linux-or-gnulinux/)

</details>

<details>
<summary><b>What is a CLI?</b></summary><br>

<b>CLI</b> is an acronym for Command Line Interface or Command Language Interpreter. The command line is one of the most powerful ways to control your system/computer.

In Linux, CLI is the interface by which a user can type commands for the system to execute. The CLI is very powerful, but is not very error-tolerant.

Useful resources:

- [Command Line Interface Definition](http://www.linfo.org/command_line_interface.html)

</details>

<details>
<summary><b>What is your favourite shell and why?</b></summary><br>

BASH is my favorite. It’s really a preferential kind of thing, where I love the syntax and it just "clicks" for me. The input/output redirection syntax (<code>>></code>, <code><< 2>&1</code>, <code>2></code>, <code>1></code>, etc) is similar to C++ which makes it easier for me to recognize.

I also like the ZSH shell, because is much more customizable than BASH. It has the Oh-My-Zsh framework, powerful context based tab completion, pattern matching/globbing on steroids, loadable modules and more.

Useful resources:

- [Comparison of command shells](https://en.wikipedia.org/wiki/Comparison_of_command_shells)

</details>

<details>
<summary><b>How do you get a list of logged-in users?</b></summary><br>

For a summary of logged-in users, including each login of a username, the terminal users are attached to, the date/time they logged in, and possibly the computer from which they are making the connection, enter:

```bash
who
```

For extensive information, including username, terminal, IP number of the source computer, the time the login began, any idle time, process CPU cycles, job CPU cycles, and the currently running command, enter:

```bash
w
```

<details>
<summary><b>How do you run commands in the background? *</b></summary><br>

To be completed.

</details>

</details>

<details>
<summary><b>What does it mean when the effective user is "root", but the real user ID is still your name?</b></summary><br>

The real user ID is who you really are (the user who owns the process), and the effective user ID is what the operating system looks at to make a decision whether or not you are allowed to do something (most of the time, there are some exceptions).

When you log in, the login shell sets both the real and effective user ID to the same value (your real user id) as supplied by the password file.

If, for instance, you execute setuid, and besides running as another user (e.g. root) the setuid program is also supposed to do something on your behalf:

After executing setuid, it will have your real id (since you're the process owner) and the effective user id of the file owner (for example root) since it is setuid.

Let's use the case of passwd:

```bash
-rwsr-xr-x 1 root root 45396 may 25  2012 /usr/bin/passwd
```

When user2 wants to change their password, they execute `/usr/bin/passwd`.

The **RUID** will be user2 but the **EUID** of that process will be root.

user2 can use only passwd to change their own password, because internally passwd checks the **RUID** and, if it is not root, its actions will be limited to real user's password.

It's neccesary that the **EUID** becomes root in the case of passwd because the process needs to write to `/etc/passwd` and/or `/etc/shadow`.

Useful resources:

- [Difference between Real User ID, Effective User ID and Saved User ID? (original)](https://stackoverflow.com/questions/30493424/what-is-the-difference-between-a-process-pid-ppid-uid-euid-gid-and-egid)
- [What is the difference between a pid, ppid, uid, euid, gid and egid?](https://stackoverflow.com/questions/30493424/what-is-the-difference-between-a-process-pid-ppid-uid-euid-gid-and-egid)

</details>

<details>
<summary><b>Another admin is running all commands as root. Why is this a bad idea?</b></summary><br>

Running everything as root is bad because:

- **Stupidity**: nothing prevents you from making a careless mistake. If you try to change the system in any potentially harmful way, you need to use sudo, which ensures a pause (while you're entering the password) to ensure that you aren't about to make a mistake.

- **Security**: harder to hack if you dont know the admin user's login account. root means you already have one half of the working set of admin credentials.

- **You don't really need it**: if you need to run several commands as root, and you're annoyed by having to enter your password several times when `sudo` has expired, all you need to do is `sudo -i` and you are now root. Want to run some commands using pipes? Then use `sudo sh -c "command1 | command2"`.

- **You can always use it in the recovery console**: the recovery console allows you to recover from a major mistake, or fix a problem caused by an app (which you still had to run as `sudo`). Ubuntu doesn't have a password for the root account in this case, but you can search online for changing that - this will make it harder for anyone that has physical access to your box to be able to do harm.

Useful resources:

- [Why is it bad to log in as root? (original)](https://askubuntu.com/questions/16178/why-is-it-bad-to-log-in-as-root)

</details>

<details>
<summary><b>Which command is used to review boot messages?</b></summary><br>

<code>dmesg</code> is used to review boot messages. This command will display system messages contained in the kernel ring buffer. We can use this command immediately after booting to see boot messages. A ring buffer is a buffer of fixed size for which any new data added to it overwrites the oldest data in it.

</details>

<details>
<summary><b>What is the swap space?</b></summary><br>

Swap space is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space. While swap space can help machines with a small amount of RAM, it should not be considered a replacement for more RAM. Swap space is located on hard drives, which have a slower access time than physical memory.

</details>

<details>
<summary><b>How to check memory stats and CPU stats?</b></summary><br>

You'd use `top/htop` for both. Using <code>free</code> and <code>vmstat</code> command we can display the physical and virtual memory statistics respectively. With the help of <code>sar</code> command we see the CPU utilization & other stats (but `sar` isn't even installed in most systems).

</details>

<details>
<summary><b>What is load average?</b></summary><br>

Linux load averages are "system load averages" that show the running thread (task) demand on the system as an average number of running plus waiting threads. This measures demand, which can be greater than what the system is currently processing. Most tools show three averages, for 1, 5, and 15 minutes.

Some interpretations:

- If the averages are 0.0, then your system is idle.
- If the 1 minute average is higher than the 5 or 15 minute averages, then load is increasing.
- If the 1 minute average is lower than the 5 or 15 minute averages, then load is decreasing.
- If they are higher than your CPU count, then you might have a performance problem (it depends).

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

To change all the directories e.g. to 755 (drwxr-xr-x):<br>

<code>
find /opt/data -type d -exec chmod 755 {} \;
</code><br><br>

To change all the files e.g. to 644 (-rw-r--r--):<br>

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
<summary><b>What is the difference between <code>rm</code> and <code>rm -rf</code>?</b></summary><br>

<code>rm</code> removes files and <code>-rf</code> are two options:<br>

- <code>-r</code> remove directories and their contents recursively<br>
- <code>-f</code> ignore nonexistent files, never prompt

</details>

<details>
<summary><b>How do you list contents of archive.tgz and extract only one file?</b></summary><br>

```bash
tar tf archive.tgz
tar xf archive.tgz filename
```

</details>

<details>
<summary><b>How to sync two local directories?</b></summary><br>

To sync the contents of dir1 to dir2 on the same system, type:

```bash
rsync -av --progress --delete dir1/ dir2
```

- <code>-a, --archive</code> - archive mode
- <code>--delete</code> - delete extraneous files from dest dirs
- <code>-v, --verbose</code> - verbose mode (increase verbosity)
- <code>--progress</code> - show progress during transfer

</details>

<details>
<summary><b>How to quickly backup a file?</b></summary><br>

```bash
cp filename{,.orig}
```

</details>

<details>
<summary><b>How to find all files larger than 20M?</b></summary><br>

```bash
find / -type f -size +20M
```

</details>

<details>
<summary><b>Why do we use <code>sudo su -</code> and not just <code>sudo su</code>?</b></summary><br>

<code>su -</code> invokes a login shell after switching the user. A login shell resets most environment variables, providing a clean base.

<code>su</code> just switches the user, providing a normal shell with an environment nearly the same as with the old user.

</details>

<details>
<summary><b>How to find files that have been modified on your system in the past 60 minutes?</b></summary><br>

```bash
find / -mmin 60 -type f
```

</details>

<details>
<summary><b>What are the main reasons for keeping old log files? </b></summary><br>

They are essential to investigate issue on the system.

</details>

<details>
<summary><b>What is an incremental backup? </b></summary><br>

An incremental backup is a type of backup that only copies files that have changed since the previous backup.

</details>

<details>
<summary><b>What is RAID? What is RAID0, RAID1, RAID5, RAID6, RAID10? </b></summary><br>

A <b>RAID</b> (Redundant Array of Inexpensive Disks) is a technology that is used to increase the performance and/or reliability of data storage.
- <b>RAID0</b>: Also known as disk <b>striping</b>, is a technique that breaks up a file and spreads the data across all the disk drives in a RAID group. There are no safeguards against failure.
- <b>RAID1</b>: A popular disk subsystem that increases safety by writing the same data on two drives. Called "<b>mirroring</b>," RAID 1 does not increase write performance, but read performance may equal up to the sum of each disks' performance. However, if one drive fails, the second drive is used, and the failed drive is manually replaced. After replacement, the RAID controller duplicates the contents of the working drive onto the new one.
- <b>RAID5</b>: It is disk subsystem that increases safety by computing parity data and increasing speed by interleaving data across three or more drives (striping). Upon failure of a single drive, subsequent reads can be calculated from the distributed parity such that no data is lost.
- <b>RAID6</b>: RAID 6 extends RAID 5 by adding another parity block. It requires a minimum of four disks and can continue to execute read and write of any two concurrent disk failures. RAID 6 does not have a performance penalty for read operations, but it does have a performance penalty on write operations because of the overhead associated with parity calculations.
- <b>RAID10</b>: Also known as <b>RAID 1+0</b>, is a RAID configuration that combines disk mirroring and disk striping to protect data. It requires a minimum of four disks, and stripes data across mirrored pairs. As long as one disk in each mirrored pair is functional, data can be retrieved. If two disks in the same mirrored pair fail, all data will be lost because there is no parity in the striped sets.

</details>

<details>
<summary><b>How is a user’s default group determined? How would you change it? </b></summary><br>

<code>useradd -m -g initial_group username</code>

<b>-g/--gid:</b>
  defines the group name or number of the user's initial login group. If specified, the group name must exist; if a group number is provided, it must refer to an already existing group. If not specified, the behaviour of useradd will depend on the USERGROUPS_ENAB variable contained in /etc/login.defs. The default behaviour (USERGROUPS_ENAB yes) is to create a group with the same name as the username, with GID equal to UID.


</details>

<details>
<summary><b>Why would you want to mount servers in a rack? </b></summary><br>

- Protecting Hardware
- Organized Workspace
- Better Power Management
- Cleaner Environment

</details>

###### Network Questions

<details>
<summary><b>According to an HTTP monitor, a website is down. You're able to telnet to the port, so how do you resolve it? </b></summary><br>

I would connect to my web server via telnet to investigate the log files and resolve the issue regarding to the logs.

</details>

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
<summary><b>What happens when you type api.example.com in your browser and press return?</b></summary><br>

1. You type api.example.com into the address bar of your browser.
2. The browser checks the cache for a DNS record to find the corresponding IP address of api.example.com.

- first, it checks the browser cache. The browser maintains a repository of DNS records for a fixed duration for websites you have previously visited. So, it is the first place to run a DNS query.
- second, the browser checks the OS cache. If it is not found in the browser cache, the browser would make a system call to your underlying computer OS to fetch the record since the OS also maintains a cache of DNS records.
- third, it checks the router cache. If it’s not found on your computer, the browser would communicate with the router that maintains its’ own cache of DNS records.
- fourth, it checks the ISP cache. If all steps fail, the browser would move on to the ISP. Your ISP maintains its’ own DNS server which includes a cache of DNS records which the browser would check with the last hope of finding your requested URL.

3.  If the requested URL is not in the cache, ISP’s DNS server initiates a DNS query to find the IP address of the server that hosts api.example.com.

- the purpose of a DNS query is to search multiple DNS servers on the internet until it finds the correct IP address for the website. This type of search is called a recursive search since the search will continue repeatedly from DNS server to DNS server until it either finds the IP address we need or returns an error response saying it was unable to find it.
- for api.example.com, first, the DNS recursor will contact the root name server. The root name server will redirect it to .com domain name server. .com name server will redirect it to google.com name server. google.com name server will find the matching IP address for api.example.com in its’ DNS records and return it to your DNS recursor which will send it back to your browser.

4.  Browser initiates a TCP connection with the server.

- once the browser receives the correct IP address it will build a connection with the server that matches IP address to transfer information. Browsers use internet protocols to build such connections.
- in order to transfer data packets between your computer(client) and the server, it is important to have a TCP connection established. This connection is established using a process called the TCP/IP three-way handshake.

5. The browser sends an HTTP request to the web server.

- this request will also contain additional information such as browser identification (User-Agent header), types of requests that it will accept (Accept header), and connection headers asking it to keep the TCP connection alive for additional requests. It will also pass information taken from cookies the browser has in store for this domain.

6. The server handles the request and sends back a response.

- the server contains a web server (i.e Apache, IIS) which receives the request from the browser and passes it to a request handler to read and generate a response.

7. The server sends out an HTTP response.

- the server response contains the web page you requested as well as the status code, compression type (Content-Encoding), how to cache the page (Cache-Control), any cookies to set, privacy information, etc.

8. The browser displays the HTML content (for HTML responses which is the most common).

</details>

<details>
<summary><b>How to check default route and routing table?</b></summary><br>

Using the commands <code>netstat -nr</code>, <code>route -n</code> or <code>ip route show</code> we can see the default route and routing tables.

</details>

<details>
<summary><b>What is the difference between 127.0.0.1 and localhost?</b></summary><br>

Well, the most likely difference is that you still have to do an actual lookup of localhost somewhere.

If you use <code>127.0.0.1</code>, then (intelligent) software will just turn that directly into an IP address and use it. Some implementations of <code>gethostbyname</code> will detect the dotted format (and presumably the equivalent IPv6 format) and not do a lookup at all.

Otherwise, the name has to be resolved. And there's no guarantee that your hosts file will actually be used for that resolution (first, or at all) so <code>localhost</code> may become a totally different IP address.

By that I mean that, on some systems, a local hosts file can be bypassed. The <code>host.conf</code> file controls this on Linux (and many other Unices).

If you use a unix domain socket it'll be slightly faster than using TCP/IP (because of the less overhead you have).
Windows is using TCP/IP as a default, whereas Linux tries to use a Unix Domain Socket if you choose localhost and TCP/IP if you take <code>127.0.0.1</code>.

Useful resources:

- **[What is the difference between 127.0.0.1 and localhost?](https://stackoverflow.com/questions/7382602/what-is-the-difference-between-127-0-0-1-and-localhost)**
- **[localhost vs. 127.0.0.1](https://stackoverflow.com/questions/3715925/localhost-vs-127-0-0-1)**

</details>

<details>
<summary><b>How to resolves the domain name (using external dns server) with CLI commands?</b></summary><br>

```bash
# with host command:
host domain.com 8.8.8.8
# with dig command:
dig @9.9.9.9 google.com
# with nslookup command:
nslookup domain.com 8.8.8.8
```

</details>

<details>
<summary><b>How to test port connectivity with <code>telnet</code> or <code>nc</code>?</b></summary><br>

```bash
# with telnet command:
telnet code42.example.com 5432
# with nc (netcat) command:
nc -vz code42.example.com 5432
```

</details>

<details>
<summary><b>Why should you avoid telnet to administer a system remotely?</b></summary><br>

Telnet uses most insecure method for communication. It sends data across the network in plain text format and anybody can easily find out the password using the network tool.

In the case of Telnet, these include the passing of login credentials in plain text, which means anyone running a sniffer on your network can find the information he needs to take control of a device in a few seconds by eavesdropping on a Telnet login session.

</details>

<details>
<summary><b>What is the difference between <code>wget</code> and <code>curl</code>?</b></summary><br>

The main differences are: wget's major strong side compared to curl is its ability to download recursively. Wget is command line only. Curl supports FTP, FTPS, HTTP, HTTPS, SCP, SFTP, TFTP, TELNET, DICT, LDAP, LDAPS, FILE, POP3, IMAP, SMTP, RTMP and RTSP.

</details>

<details>
<summary><b>How do SSH keys work?</b></summary><br>

SSH stands for Secure Shell. It is a protocol that lets you drop from a server "A" into a shell session to a server "B". It allows you interact with your server "B".
An SSH connection to be established, the remote machine (server A) must be running a piece of software called an SSH daemon and the user's computer (server B) must have an SSH client.
The SSH daemon and SSH client listen for connections on a specific network port (default 22), authenticates connection requests, and spawns the appropriate environment if the user provides the correct credentials.

</details>

<details>
<summary><b>What is a packet filter and how does it work?</b></summary><br>

Packet filtering is a firewall technique used to control network access by monitoring outgoing and incoming packets and allowing them to pass or halt based on the source and destination Internet Protocol (IP) addresses, protocols and ports.

</details>

<details>
<summary><b>What is a proxy and how does it work?</b></summary><br>

A proxy server is a dedicated computer or a software system running on a computer that acts as an intermediary between an endpoint device, such as a computer, and another server from which a user or client is requesting a service.

</details>

<details>
<summary><b>What is the difference between a router and a gateway? What is the default gateway?</b></summary><br>

Routers and Gateways are used to regulate network traffic between two or more separate networks. Gateways regulate traffic between two dissimilar networks, while routers regulate traffic between similar networks.

A default gateway serves as an access point or IP router that a networked computer uses to send information to a computer in another network or the internet. Default simply means that this gateway is used by default, unless an application specifies another gateway.

A gateway is a node (router) in a computer network, a key stopping point for data on its way to or from other networks. Thanks to gateways, we are able to communicate and send data back and forth.

</details>

<details>
<summary><b>Explain the function of each of the following DNS records: SOA, PTR, A, MX, and CNAME.</b></summary><br>

DNS records are basically mapping files that tell the DNS server which IP address each domain is associated with, and how to handle requests sent to each domain. Some DNS records syntax that are commonly used in nearly all DNS record configurations are A, AAAA, CNAME, MX, PTR, NS, SOA, SRV, TXT, and NAPTR.

- <b>SOA</b> - A Start Of Authority
- <b>A</b> - Address Mapping records
- <b>AAAA</b> - IP Version 6 Address records
- <b>CNAME</b> - Canonical Name records
- <b>MX</b> - Mail exchanger record
- <b>NS</b> - Name Server records
- <b>PTR</b> - Reverse-lookup Pointer records

</details>

<details>
<summary><b>What is the smallest IPv4 subnet mask that can be applied to a network containing up to 30 devices?</b></summary><br>

Whether you have a standard /24 VLAN for end users, a /30 for point-to-point links, or something in between and subnet that must contain up to 30 devices works out to be a /27 - or a subnet mask of <code>255.255.255.224</code>.

</details>

<details>
<summary><b>Various response codes from a web application?</b></summary><br>

- <b>1xx</b> - Informational responses - communicates transfer protocol-level information
- <b>2xx</b> - Success - indicates that the client’s request was accepted successfully
- <b>3xx</b> - Redirection - indicates that the client must take some additional action in order to complete their request
- <b>4xx</b> - Client side error - this category of error status codes points the finger at clients
- <b>5xx</b> - Server side error - the server takes responsibility for these error status codes

</details>

###### Devops Questions

<details>
<summary><b>What is Version Control?</b></summary><br>

It is a system that records changes to a file or set of files over time so that you can recall specific versions later. Version control systems consist of a central shared repository where teammates can commit changes to a file or set of file. Then you can mention the uses of version control.

Version control allows you to:

- revert files back to a previous state
- revert the entire project back to a previous state
- compare changes over time
- see who last modified something that might be causing a problem
- who introduced an issue and when

</details>

<details>
<summary><b>Explain some basic Git commands?</b></summary><br>

- <code>git init</code> - create a new local repository
- <code>git commit -m "message"</code> - commit changes to head
- <code>git status</code> - list the files you've added with <code>git add</code> and also commit any files you've changed since then
- <code>git push origin master</code> - send changes to the master branch of your remote repository

</details>

###### Cyber Security Questions

<details>
<summary><b>What is a Security Misconfiguration?</b></summary><br>

Security misconfiguration is a vulnerability when a device/application/network is configured in a way which can be exploited by an attacker to take advantage of it. This can be as simple as leaving the default username/password unchanged or too simple for device accounts etc.

</details>

### :diamond_shape_with_a_dot_inside: <a name="regular-sysadmin">Regular Sysadmin</a>

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
<summary><b>What is this UID 0 <code>toor</code> account? Have I been compromised?</b></summary><br>

<code>toor</code> is an "alternative" superuser account, where toor is root spelled backwards. It is intended to be used with a non-standard shell so the default shell for root does not need to change.

This is important as shells which are not part of the base distribution, but are instead installed from ports or packages, are installed in <code>/usr/local/bin</code> which, by default, resides on a different file system. If root's shell is located in <code>/usr/local/bin</code> and the file system containing <code>/usr/local/bin</code>) is not mounted, root will not be able to log in to fix a problem and will have to reboot into single-user mode in order to enter the path to a shell.

Some people use toor for day-to-day root tasks with a non-standard shell, leaving root, with a standard shell, for single-user mode or emergencies. By default, a user cannot log in using toor as it does not have a password, so log in as root and set a password for toor before using it to login.

</details>

<details>
<summary><b>What is the name and path of the main system log?</b></summary><br>

By default, the main system log is <b>/var/log/messages</b>. This file contains all the messages and the script written by the user.

By default all scripts are saved in this file. This is the standard system log file, which contains messages from all system software, non-kernel boot issues, and messages that go to <code>dmesg</code> (is a system file that is written upon system boot).

</details>

<details>
<summary><b>Explain <code>/proc</code> filesystem.</b></summary><br>

<code>/proc</code> is a virtual file system that provides detailed information about kernel, hardware and running processes.

Since <code>/proc</code> contains virtual files, it is called virtual file system. These virtual files have unique qualities. Most of them are listed as zero bytes in size.<br>

Virtual files such as <code>/proc/interrupts</code>, <code>/proc/meminfo</code>, <code>/proc/mounts</code> and <code>/proc/partitions</code> provide an up-to-the-moment glimpse of the system’s hardware. Others: <code>/proc/filesystems</code> file and the <code>/proc/sys/</code> directory provide system configuration information and interfaces.

</details>

<details>
<summary><b>Why is a load of 1.00 not ideal on a single-core machine?</b></summary><br>

The problem with a load of 1.00 is that you have no headroom. In practice, many sysadmins will draw a line at 0.70:<br>

The "Need to Look into it" Rule of Thumb: 0.70 If your load average is staying above > 0.70, it's time to investigate before things get worse.<br>

The "Fix this now" Rule of Thumb: 1.00. If your load average stays above 1.00, find the problem and fix it now. Otherwise, you're going to get woken up in the middle of the night, and it's not going to be fun.<br>

Rule of Thumb: 5.0. If your load average is above 5.00, you could be in serious trouble, your box is either hanging or slowing way down, and this will (inexplicably) happen in the worst possible time like in the middle of the night or when you're presenting at a conference. Don't let it get there.

</details>

<details>
<summary><b>How the Linux kernel creates, manages and deletes the processes in the system? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How would you recognize a process that is hogging resources? </b></summary><br>

<b><code>top</code></b> works reasonably well, as long as you look at the right numbers.
- <b>M</b> Sorts by current resident memory usage
- <b>T</b> Sorts by total ( or cummulaative) CPU usage
- <b>p</b> Sorts by current CPU usage (this is the default refresh)
- <b>?</b> Displays a usage summary for all top commands

This is very important information to obtain when problem solving why a computer process is running slowly and making decisions on what processes to kill / software to uninstall.


</details>

<details>
<summary><b>What is umask? How to set it permanently for a user?</b></summary><br>

On Linux and other Unix-like operating systems, new files are created with a default set of permissions. Specifically, a new file's permissions may be restricted in a specific way by applying a permissions "mask" called the umask. The umask command is used to set this mask, or to show you its current value.<br>

Permanently change (set e.g. <code>umask 02</code>):<br>

- <b>~/.profile</b><br>
- <b>~/.bashrc</b><br>
- <b>~/.zshrc</b><br>
- <b>~/.cshrc</b>

</details>

<details>
<summary><b>Explain the differences among the following umask values: 000, 002, 022, 027, 077 and 277.</b></summary><br>

<table style="width:100%">
  <tr>
    <th>Umask</th>
    <th>FIle result</th>
    <th>Directory result</th>
  </tr>
  <tr>
    <td>000</td>
    <td>666 rw- rw- rw-</td>
    <td>777 rwx rwx rwx</td>
  </tr>
 <tr>
    <td>002</td>
    <td>664 rw- rw- r--</td>
    <td>775 rwx rwx r-x</td>
  </tr>
  <tr>
    <td>022</td>
    <td>644 rw- r-- r--</td>
    <td>755 rwx r-x r-x</td>
  </tr>
<tr>
    <td>027</td>
    <td>640 rw- r-- ---</td>
    <td>750 rwx r-x ---</td>
  </tr>
<tr>
    <td>077</td>
    <td>600 rw---- ---</td>
    <td>700 rwx --- ---</td>
  </tr>
<tr>
    <td>277</td>
    <td>400 r-- --- ---</td>
    <td>500 r-x --- ---</td>
  </tr>
</table>

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
<summary><b>What steps will be taken by init when you run <code>telinit 1</code> from run level 3? What will be the final result of this? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>I have forgotten the root password! What do I do in BSD?</b></summary><br>

Restart the system, type <code>boot -s</code> at the <code>Boot:</code> prompt to enter single-user mode.

At the question about the shell to use, hit Enter which will display a # prompt.

Enter <code>mount -urw /</code> to remount the root file system read/write, then run <code>mount -a</code> to remount all the file systems.

Run <code>passwd root</code> to change the root password then run <code>exit</code> to continue booting.

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
<summary><b>What is an inode?</b></summary><br>

An inode is a data structure on a filesystem on Linux and other Unix-like operating systems that stores all the information about a file except its name and its actual data. A data structure is a way of storing data so that it can be used efficiently.<br>

A Unix file is "stored" in two different parts of the disk - the data blocks and the inodes. (I won't get into superblocks and other esoteric information.) The data blocks contain the "contents" of the file. The information about the file is stored elsewhere - in the inode.

</details>

<details>
<summary><b>How to increase the size of LVM partition?</b></summary><br>

Use the <code>lvextend</code> command for resize LVM partition.<br>

- extending the size by 500MB:

```bash
lvextend -L +500M /dev/vgroup/lvolume
```

- extending all available free space:

```bash
lvextend -l +100%FREE /dev/vgroup/lvolume
```

and `resize2fs` or `xfs_growfs` to resize filesystem:<br>

- for ext filesystems:

```bash
resize2fs /dev/vgroup/lvolume
```

- for xfs filesystem:

```bash
xfs_growfs mountpoint_for_/dev/vgroup/lvolume
```

</details>

<details>
<summary><b>Describe a process to create partition, lvm partition and filesystem.</b></summary><br>

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

</details>

<details>
<summary><b>What is the advantage of executing the running processes in the background? How can you do that?</b></summary><br>

The most significant advantage of executing the running process in the background is that you can do any other task simultaneously while other processes are running in the background. So, more processes can be completed in the background while you are working on different processes. It can be achieved by adding a special character `&` at the end of the command.

</details>

<details>
<summary><b>What is a zombie/defunct process?</b></summary><br>

Is a process that has completed execution (via the <b>exit</b> system call) but still has an entry in the process table: it is a process in the "Terminated state".

</details>

<details>
<summary><b>What if <code>kill -9</code> does not work?</b></summary><br>

<code>kill -9</code> (SIGKILL) always works, provided you have the permission to kill the process. Basically either the process must be started by you and not be setuid or setgid, or you must be root. There is one exception: even root cannot send a fatal signal to PID 1 (the init process).

However <code>kill -9</code> is not guaranteed to work immediately. All signals, including SIGKILL, are delivered asynchronously: the kernel may take its time to deliver them. Usually, delivering a signal takes at most a few microseconds, just the time it takes for the target to get a time slice. However, if the target has blocked the signal, the signal will be queued until the target unblocks it.

Normally, processes cannot block SIGKILL. But kernel code can, and processes execute kernel code when they call system calls.

A process blocked in a system call is in uninterruptible sleep. The <code>ps</code> or <code>top</code> command will (on most unices) show it in state <b>D</b>.

A classical case of long uninterruptible sleep is processes accessing files over NFS when the server is not responding; modern implementations tend not to impose uninterruptible sleep (e.g. under Linux, the intr mount option allows a signal to interrupt NFS file accesses).

You may sometimes see entries marked <b>Z</b> (or <b>H</b> under Linux) in the <code>ps</code> or <code>top</code> output. These are technically not processes, they are zombie processes, which are nothing more than an entry in the process table, kept around so that the parent process can be notified of the death of its child. They will go away when the parent process pays attention (or dies).

</details>

<details>
<summary><b>What is strace command in Linux?</b></summary><br>

<code>strace</code> is a powerful command line tool for debugging and trouble shooting programs in Unix-like operating systems such as Linux. It captures and records all system calls made by a process and the signals received by the process.

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

<code>logrotate</code> command is used to make automate rotation of log. It allows automatic rotation, compression, removal, and mailing of log files.

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

<details>
<summary><b>Create a file with 100 lines with random values.</b></summary><br>

For example:

```bash
cat /dev/urandom | tr -dc 'a-zA-Z0-9' | fold -w 32 | head -n 100 > /path/to/file
```

</details>

<details>
<summary><b>How to run script as another user without password?</b></summary><br>

For example (with <code>visudo</code> command):

```bash
user1 ALL=(user2) NOPASSWD: /opt/scripts/bin/generate.sh
```

The command paths must be absolute! Then call <code>sudo -u user2 /opt/scripts/bin/generate.sh</code> from a user1 shell.

</details>

<details>
<summary><b>How to check if running as root in a bash script?</b></summary><br>

In a bash script, you have several ways to check if the running user is root.

As a warning, do not check if a user is root by using the root username. Nothing guarantees that the user with ID 0 is called root. It's a very strong convention that is broadly followed but anybody could rename the superuser another name.

I think the best way when using bash is to use $EUID because $UID could be changed and not reflect the real user running the script.

```bash
if (( $EUID != 0 )); then
  echo "Please run as root"
  exit
fi
```
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

Furthermore, if you want to append to the log file, use tee -a as:

`program [arguments...] 2>&1 | tee -a outfile`

</details>

<details>
<summary><b>What is the preferred Bash shebang?</b></summary><br>

You should use <code>#!/usr/bin/env bash</code> for portability: different *nixes put bash in different places, and using <code>/usr/bin/env</code> is a workaround to run the first bash found on the PATH.

</details>

<details>
<summary><b>What is root certificate and intermediate certificate?</b></summary><br>

A "root" authority is a certificate issuer that parties choose to trust (explicitly). It is usually self-signed (self-issued) and very highly protected. An intermediate authority is a certificate issuer that has itself been issued by a root or another higher level intermediate authority.

</details>

<details>
<summary><b>Should the root certificate go on the server?</b></summary><br>

Self-signed root certificates need not/should not be included in web server configuration. They serve no purpose (clients will always ignore them) and they incur a slight performance (latency) penalty because they increase the size of the SSL handshake.

If the client does not have the root in their trust store, then it won't trust the web site, and there is no way to work around that problem. Having the web server send the root certificate will not help - the root certificate has to come from a trusted 3rd party (in most cases the browser vendor).

</details>

<details>
<summary><b>How to reload PostgreSQL after configuration changes?</b></summary><br>

Solution 1:

```
systemctl reload postgresql
```

Solution 2:

```
su - postgres
/usr/bin/pg_ctl reload
```

Solution 3:

```
SELECT pg_reload_conf();
```

</details>

<details>
<summary><b>How to restore config file in Debian GNU/Linux?</b></summary><br>

Will recreate any missing configuration files, e.g. <code>/etc/mysql/my.cnf</code> in your case:

```
dpkg -i --force-confmiss mysql-common.deb
```

</details>

<details>
<summary><b>How reload shell without exit?</b></summary><br>

The best way is: `exec $SHELL -l`

</details>

<details>
<summary><b>How to exit without saving shell history?</b></summary><br>

```bash
kill -9 $$
unset HISTFILE && exit
```

</details>

<details>
<summary><b>How do I find all files containing specific string?</b></summary><br>

For example use <code>fgrep</code>:

```bash
fgrep * -R "string"
```

or:

```bash
grep -insr "pattern" *
```

- <code>-i</code> ignore case distinctions in both the PATTERN and the input files
- <code>-n</code>  prefix each line of output with the 1-based line number within its input file
- <code>-s</code> suppress error messages about nonexistent or unreadable files.
- <code>-r</code> read all files under each directory, recursively.

</details>

<details>
<summary><b>How to find out the dynamic libraries executables loads when run?</b></summary><br>

You can do this with <code>ldd</code> command:

```bash
ldd /bin/ls
```

</details>

###### Network Questions

<details>
<summary><b>Configure a virtual interface on your workstation. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Load balancing can dramatically impact server performance. Discuss several load balancing mechanisms. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Server A can't talk to Server B. Describe possible reasons in a few steps. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>List examples of network troubleshooting tools that can degrade during DNS issues. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Why won’t the hostnames resolve on your server? Resolve this problem. *</b></summary><br>

To be completed.

</details>


<details>
<summary><b>What is handshake mechanism and why do we need 3 way handshake?</b></summary><br>

<b>Handshaking</b> begins when one device sends a message to another device indicating that it wants to establish a communications channel. The two devices then send several messages back and forth that enable them to agree on a communications protocol.

A <b>three-way handshake</b> is a method used in a TCP/IP network to create a connection between a local host/client and server. It is a three-step method that requires both the client and server to exchange SYN and ACK (SYN, SYN-ACK, ACK) packets before actual data communication begins.

</details>

<details>
<summary><b>Why is UDP faster than TCP?</b></summary><br>

UDP is faster than TCP, and the simple reason is because its nonexistent acknowledge packet (ACK) that permits a continuous packet stream, instead of TCP that acknowledges a set of packets, calculated by using the TCP window size and round-trip time (RTT).

</details>

<details>
<summary><b>What is NAT? What is it used for?</b></summary><br>

It enables private IP networks that use unregistered IP addresses to connect to the Internet. NAT operates on a router, usually connecting two networks together, and translates the private (not globally unique) addresses in the internal network into legal addresses, before packets are forwarded to another network.

Workstations or other computers requiring special access outside the network can be assigned specific external IPs using NAT, allowing them to communicate with computers and applications that require a unique public IP address. NAT is also a very important aspect of firewall security.

</details>

<details>
<summary><b>What's the purpose of Spanning Tree?</b></summary><br>

This protocol operates at layer 2 of the OSI model with the purpose of preventing loops on the network. Without STP, a redundant switch deployment would create broadcast storms that cripple even the most robust networks. There are several iterations based on the original IEEE 802.1D standard; each operates slightly different than the others while largely accomplishing the same loop-free goal.

</details>

<details>
<summary><b>How to check which ports are listening in my Linux Server?</b></summary><br>

Use the:

- <code>lsof -i</code>
- <code>ss -l</code>
- <code>netstat -atn</code> - for tcp
- <code>netstat -aun</code> - for udp
- <code>netstat -tulapn</code>

</details>

<details>
<summary><b>How to get fingerprint from SSH key?</b></summary><br>

```
ssh-keygen -lf ~/.ssh/id_rsa.pub
```

</details>

<details>
<summary><b>How to send an HTTP request using Telnet?</b></summary><br>

For example:

```bash
telnet example.com 80
Trying 192.168.252.10...
Connected to example.com.
Escape character is '^]'.
GET /questions HTTP/1.0
Host: example.com

HTTP/1.1 200 OK
Content-Type: text/html; charset=utf-8
...
```

</details>

<details>
<summary><b>How to allow traffic to/from specific IP with iptables?</b></summary><br>

For example:

```bash
/sbin/iptables -A INPUT -p tcp -s XXX.XXX.XXX.XXX -j ACCEPT
/sbin/iptables -A OUTPUT -p tcp -d  XXX.XXX.XXX.XXX -j ACCEPT
```

</details>

<details>
<summary><b>How to block abusive IP addresses with <code>pf</code> in OpenBSD?</b></summary><br>

The best way to do this is to define a table and create a rule to block the hosts, in <code>pf.conf</code>:

```bash
table <badhosts> persist
block on fxp0 from <badhosts> to any
```

And then dynamically add/delete IP addresses from it:

```bash
pfctl -t badhosts -T add 1.2.3.4
pfctl -t badhosts -T delete 1.2.3.4
```

</details>

<details>
<summary><b>How to disable cache for specific domain in Varnish?</b></summary><br>

For example:

```
sub vcl_recv {
   # dont cache foo.com or bar.com - optional www
   if (req.host ~ "(www)?(foo|bar).com") {
     return(pass);
   }
}
```

or:

```
sub vcl_recv {
  # dont cache foo.com or bar.com - optional www
   if (req.http.host ~ "(www\.)?(foo|bar)\.com") {
     return(pass);
   }
  # cache foobar.com - optional www
   if (req.http.host ~ "(www\.)?foobar\.com") {
     return(hash);
   }
}
```

</details>

<details>
<summary><b>Analyse web server log and show only 5xx http codes.</b></summary><br>

```bash
tail -n 100 -f /path/to/logfile | grep "HTTP/[1-2].[0-1]\" [5]"
```

</details>

<details>
<summary><b>Developer uses private key on the server to deploy app through ssh. Why it is incorrect behavior and what is the better (but not ideal) solution in such situations?</b></summary><br>

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
<summary><b>What is the difference between CORS and CSPs?</b></summary><br>

CORS allows the Same Origin Policy to be relaxed for a domain.

e.g. normally if the user logs into both example.com and <code>example.org</code>, the Same Origin Policy prevents <code>example.com</code> from making an AJAX request to <code>example.org/current_user/full_user_details</code> and gaining access to the response.

This is the default policy of the web and prevents the user's data from being leaked when logged into multiple sites at the same time.

Now with CORS, example.org could set a policy to say it will allow the origin <code>https://example.com</code> to read responses made by AJAX. This would be done if both example.com and example.org are ran by the same company and data sharing between the origins is to be allowed in the user's browser. It only affects the client-side of things, not the server-side.

CSPs on the other hand set a policy of what content can run on the current site. For example, if JavaScript can be executed inline, or which domains .js files can be loaded from. This can be beneficial to act as another line of defence against XSS attacks, where the attacker will try and inject script into the HTML page. Normally output would be encoded, however say the developer had forgotten only on one output field. Because the policy is preventing in-line script from executing, the attack is thwarted.

</details>

<details>
<summary><b>Explain four types of responses from firewall when scanning with Nmap.</b></summary><br>

There might be four types of responses:

- <b>Open port</b> - few ports in the case of the firewall
- <b>Closed port</b> - most ports are closed because of the firewall
- <b>Filtered</b> - Nmap is not sure whether the port is open or not
- <b>Unfiltered</b> - Nmap can access the port but is still confused about the open status of the port

</details>

###### Devops Questions

<details>
<summary><b>Which are the top DevOps tools? Which tools have you worked on?</b></summary><br>

The most popular DevOps tools are mentioned below:

- <b>Git</b> : Version Control System tool
- <b>Jenkins</b> : Continuous Integration tool
- <b>Selenium</b> : Continuous Testing tool
- <b>Puppet</b>, <b>Chef</b>, <b>Ansible</b> : Configuration Management and Deployment tools
- <b>Nagios</b> : Continuous Monitoring tool
- <b>Docker</b> : Containerization tool

</details>

<details>
<summary><b>How do all these tools work together?</b></summary><br>

The most popular DevOps tools are mentioned below:

- Developers develop the code and this source code is managed by Version Control System tools like Git etc.
- Developers send this code to the Git repository and any changes made in the code is committed to this Repository.
- Jenkins pulls this code from the repository using the Git plugin and build it using tools like Ant or Maven.
- Configuration management tools like puppet deploys & provisions testing environment and then Jenkins releases this code on the test environment on which testing is done using tools like selenium.
- Once the code is tested, Jenkins send it for deployment on the production server (even production server is provisioned & maintained by tools like puppet).
- After deployment It is continuously monitored by tools like Nagios.
- Docker containers provides testing environment to test the build features.

</details>

<details>
<summary><b>What are playbooks in Ansible?</b></summary><br>

Playbooks are Ansible’s configuration, deployment, and orchestration language.

They can describe a policy you want your remote systems to enforce, or a set of steps in a general IT process. Playbooks are designed to be human-readable and are developed in a basic text language.

At a basic level, playbooks can be used to manage configurations of and deployments to remote machines.

</details>

<details>
<summary><b>What is NRPE (Nagios Remote Plugin Executor) in Nagios?</b></summary><br>

The NRPE addon is designed to allow you to execute Nagios plugins on remote Linux/Unix machines. The main reason for doing this is to allow Nagios to monitor "local" resources (like CPU load, memory usage, etc.) on remote machines.

Since these public resources are not usually exposed to external machines, an agent like NRPE must be installed on the remote Linux/Unix machines.

</details>

<details>
<summary><b>What is the difference between Active and Passive check in Nagios?</b></summary><br>

The major difference between Active and Passive checks is that Active checks are initiated and performed by Nagios, while passive checks are performed by external applications.

Passive checks are useful for monitoring services that are:

- asynchronous in nature and cannot be monitored effectively by polling their status on a regularly scheduled basis.
- located behind a firewall and cannot be checked actively from the monitoring host.

The main features of Actives checks are as follows:

- active checks are initiated by the Nagios process.
- active checks are run on a regularly scheduled basis.

</details>

<details>
<summary><b>How to <code>git clone</code> including submodules?</b></summary><br>

For example:

```bash
# With -j8 - performance optimization
git clone --recurse-submodules -j8 git://github.com/foo/bar.git

# For already cloned repos or older Git versions
git clone git://github.com/foo/bar.git
cd bar
git submodule update --init --recursive
```

</details>

###### Cyber Security Questions

<details>
<summary><b>What is XSS, how will you mitigate it?</b></summary><br>

<b>Cross Site Scripting</b> is a JavaScript vulnerability in the web applications. The easiest way to explain this is a case when a user enters a script in the client side input fields and that input gets processed without getting validated. This leads to untrusted data getting saved and executed on the client side.

Countermeasures of XSS are input validation, implementing a CSP (Content security policy) etc.

</details>

<details>
<summary><b>HIDS vs NIDS and which one is better and why?</b></summary><br>

<b>HIDS</b> is host intrusion detection system and <b>NIDS</b> is network intrusion detection system. Both the systems work on the similar lines. It’s just that the placement in different. HIDS is placed on each host whereas NIDS is placed in the network. For an enterprise, NIDS is preferred as HIDS is difficult to manage, plus it consumes processing power of the host as well.

</details>

<details>
<summary><b>What is compliance?</b></summary><br>

Abiding by a set of standards set by a government/Independent party/organisation. E.g. An industry which stores, processes or transmits Payment related information needs to be complied with PCI DSS (Payment card Industry Data Security Standard). Other compliance examples can be an organisation complying with its own policies.

</details>

<details>
<summary><b>What is a WAF and what are its types?</b></summary><br>

<b>WAF</b> stands for web application firewall. It is used to protect the application by filtering legitimate traffic from malicious traffic. WAF can be either a box type or cloud based.

</details>

### :diamond_shape_with_a_dot_inside: <a name="senior-sysadmin">Senior Sysadmin</a>

###### Introduction Questions

<details>
<summary><b>Explain the current architecture you’re responsible for and point out where it’s scalable or fault-tolerant. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Tell me how code gets deployed in your current production. *</b></summary><br>

To be completed.

</details>

###### System Questions

<details>
<summary><b>What are the different types of Kernels? Explain.</b></summary><br>

- <b>Microkernel</b>: This type of kernel only manages CPU, memory, and IPC. This kind of kernel provides portability, small memory footprint and also security.<br>
- <b>Monolithic Kernel</b>: Linux is a monolithic kernel. So, this type of kernel provides file management, system server calls, also manages CPU, IPC as well as device drivers. It provides easier access to the process to communicate and as there is not any queue for processor time, so processes react faster.<br>
- <b>Hybrid Kernel</b>: In this type of kernels, programmers can select what they want to run in user mode and what in supervisor mode. So, this kernel provides more flexibility than any other kernel but it can have some latency problems.

</details>

<details>
<summary><b>What is LD_LIBRARY_PATH?</b></summary><br>

Environment variable <code>LD_LIBRARY_PATH</code> is a colon-separated set of directories where libraries should be searched for first, before the standard set of directories; this is useful when debugging a new library or using a nonstandard library for special purposes.

</details>

<details>
<summary><b>How shadow passwords are given by in Linux?</b></summary><br>

<code>pwconv</code> command is used for giving shadow passwords. Shadow passwords are given for better system security. The <code>pwconv</code> command creates the file <code>/etc/shadow</code> and changes all passwords to 'x' in the <code>/etc/passwd</code> file.

</details>

<details>
<summary><b>Explain all the fields in the <code>/etc/passwd</code> file.</b></summary><br>

- <b>Username</b>: First field is the username that contains the username which is 1 to 32 length characters.<br>
- <b>Password</b>: This field does not show the actual password as the password is encrypted. Here, x character shows that password is encrypted that is located in <code>/etc/shadow</code> file.<br>
- <b>User ID (UID)</b>: All the users created in Linux is given a user ID whenever the user is created. UID 0 is fixed and reserved for the root user.<br>
- <b>Group ID (GID)</b>: This field specifies the name of the group to which the user belongs. The group information is also stored in a file <code>/etc/group</code>.<br>
- <b>User ID Info</b>: Here you can add comments and you can add any extra information related to the users like full name, contact number, etc.<br>
- <b>Home directory</b>: This field provides the path where the user is directed after the login. For example, <code>/home/smith</code>.<br>
- <b>Command/shell</b>: This field provides the path of a command/shell and denotes that user has access to this shell i.e. <code>/bin/bash</code>.

</details>

<details>
<summary><b>What principles to follow for successful system performance tuning? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Describe start-up configuration files and directory in BSD systems.</b></summary><br>

In BSD the primary start-up configuration file is <code>/etc/defaults/rc.conf</code>. System startup scripts such as <code>/etc/rc</code> and <code>/etc/rc.d</code> just include this file.

If you want to add other programs to system startup you need to change <code>/etc/rc.conf</code> file instead of <code>/etc/defaults/rc.conf</code>.

</details>

<details>
<summary><b>What does Sar provides and at which location Sar logs are stored?</b></summary><br>

Sar collect, report or save system activity information. The default version of the sar command (CPU utilization report) might be one of the first facilities the user runs to begin system activity investigation, because it monitors major system resources. If CPU utilization is near 100 percent (user + nice + system), the workload sampled is CPU-bound.

By default log files of Sar command is located at <code>/var/log/sa/sadd</code> file, where the dd parameter indicates the current day.

</details>

<details>
<summary><b>How to scan newly assigned luns on Linux box without rebooting?</b></summary><br>

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
<summary><b>Can’t mount the root file system. Why? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the purpose of a process’s effective UID? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explain interrupts and interrupt handlers in Linux.</b></summary><br>

Interrupts means the processor is transferred temporarily to another program or function. When that program is completed, the processor will be given back to that program to complete the task.

Interrupt handler is the function that the kernel runs for a specific interrupt. It is also called Interrupt Service Routine. Interrupts handlers are the function that matches a particular prototype and enables the kernel to pass the handler information accurately.

</details>

<details>
<summary><b>How could you modify a text file without invoking a text editor?</b></summary><br>

For example:<br>

```bash
# cat  >filename ... - overwrite file
# cat >>filename ... - append to file
cat > filename << __EOF__
data data data
__EOF__
```

</details>

<details>
<summary><b>What fields are stored in an inode?</b></summary><br>

Within a POSIX system, a file has the following attributes which may be retrieved by the stat system call:

- <b>Device ID</b> (this identifies the device containing the file; that is, the scope of uniqueness of the serial number).
File serial numbers
- The <b>file mode</b> which determines the file type and how the file's owner, its group, and others can access the file
- A <b>link count</b> telling how many hard links point to the inode
- The <b>User ID</b> of the file's owner
- The <b>Group ID</b> of the file
- The <b>device ID</b> of the file if it is a device file.
- The <b>size of the file</b> in bytes
- <b>Timestamps</b> telling when the inode itself was last modified (ctime, inode change time), the file content last modified (mtime, modification time), and last accessed (atime, access time)
- The preferred <b>I/O block size</b>
- The <b>number of blocks</b> allocated to this file

</details>

<details>
<summary><b>What is the Pluggable Authentication Modules? Explain.</b></summary><br>

It provides a layer between applications and actual authentication mechanism. It is a library of loadable modules which are called by the application for authentication. It also allows the administrator to control when a user can log in. All PAM applications are configured in the directory <code>/etc/pam.d</code> or in a file <code>/etc/pam.conf</code>. PAM is controlled using the configuration file or the configuration directory.

</details>

<details>
<summary><b>How do you run command every time a file is modified?</b></summary><br>

For example:<br>

```bash
while inotifywait -e close_write filename ; do

  echo "changed" >> /var/log/changed

done
```

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
<summary><b>What does a <code>kill</code> command do?</b></summary><br>

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
<summary><b>Present and explain the correct process path using the <code>kill</code> command.</b></summary><br>

Speaking of killing processes never use <code>kill -9/SIGKILL</code> unless absolutely mandatory. This kill can cause problems because of its brute force.

Always try to use the following simple procedure:

- first, send <b>SIGTERM</b> (<code>kill -15</code>) signal first which tells the process to shutdown and is generally accepted as the signal to use when shutting down cleanly (but remember that this signal can be ignored).
- next try to send <b>SIGHUP</b> (<code>kill -1</code>) signal which is commonly used to tell a process to shutdown and restart, this signal can also be caught and ignored by a process.

The far majority of the time, this is all you need - and is much cleaner.

</details>

<details>
<summary><b>What was <code>getfacl</code> and <code>setfacl</code> commands do?</b></summary><br>

The command <code>setfacl</code> refers to Set File Access Control Lists and <code>getfacl</code> refers to Get File Access Control List. Each file and directory in a Linux filesystem is created with a specific set of file permissions for its access. In order to know the access permissions of a file or directory we use getfacl.

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
<summary><b>What's the difference between <code>/sbin/nologin</code>, <code>/bin/false</code> and <code>/bin/true</code>?
</b></summary><br>

When <code>/sbin/nologin</code> is set as the shell, if user with that shell logs in, they'll get a polite message saying 'This account is currently not available.'

<code>/bin/false</code> is just a binary that immediately exits, returning false, when it's called, so when someone who has false as shell logs in, they're immediately logged out when false exits. Setting the shell to <code>/bin/true</code> has the same effect of not allowing someone to log in but false is probably used as a convention over true since it's much better at conveying the concept that person doesn't have a shell.

nologin is the more user-friendly option, with a customizable message given to the user trying to log in, so you would theoretically want to use that; but both nologin and false will have the same end result of someone not having a shell and not being able to ssh in.

</details>

<details>
<summary><b>What is the meaning of the error <code>maxproc limit exceeded by uid %i ...</code> in FreeBSD?
</b></summary><br>

The FreeBSD kernel will only allow a certain number of processes to exist at one time. The number is based on the <code>kern.maxusers</code> variable.

<code>kern.maxusers</code> also affects various other in-kernel limits, such as network buffers. If the machine is heavily loaded, increase <code>kern.maxusers</code>. This will increase these other system limits in addition to the maximum number of processes.

To adjust the <code>kern.maxusers</code> value, see the File/Process Limits section of the Handbook. While that section refers to open files, the same limits apply to processes.

If the machine is lightly loaded but running a very large number of processes, adjust the <code>kern.maxproc</code> tunable by defining it in <code>/boot/loader.conf</code>.

</details>

<details>
<summary><b>How to read a file line by line and assigning the value to a variable.</b></summary><br>

For example:

```bash
while IFS='' read -r line || [[ -n "$line" ]] ; do
  echo "Text read from file: $line"
done < "/path/to/filename"
```

Explanation:

- <code>IFS=''</code> (or <code>IFS=</code>) prevents leading/trailing whitespace from being trimmed.
- <code>-r</code> prevents backslash escapes from being interpreted.
- <code>|| [[ -n $line ]]</code> prevents the last line from being ignored if it doesn't end with a <code>\n</code> (since  read returns a non-zero exit code when it encounters EOF).

</details>

<details>
<summary><b>How to rebuild Initial Ramdisk Image in Debian/CentOS?</b></summary><br>

Debian GNU/Linux:

```bash
update-initramfs -m -k all
update-grub
```

CentOS Linux:

```bash
dracut -f
grub2-mkconfig -o /boot/grub/grub.cfg
```

</details>

<details>
<summary><b>What does "CPU jumps" mean?</b></summary><br>

An OS is a very busy thing, particularly so when you have it doing something (and even when you aren't). And when we are looking at an active enterprise environment, something is always going on.

Most of this activity is "bursty", meaning processes are typically quiescent with short periods of intense activity. This is certainly true of any type of network-based activity (e.g. processing PHP requests), but also applies to OS maintenance (e.g. file system maintenance, page reclamation, disk I/O requests).

If you take a situation where you have a lot of such bursty processes, you get a very irregular and spiky CPU usage plot.

As "500 - Internal Server Error" says, the high number of context switches are going to make the situation even worse.

</details>

<details>
<summary><b>How does <code>strace</code> connect to an already running process?</b></summary><br>

`strace -p <PID>` - to attach a process to strace.

`strace -e trace=read,write -p <PID>` - by this you can also trace a process/program for an event, like read and write (in this example). So here it will print all such events that include read and write system calls by the process.

Other such examples

- `-e trace= network` - trace all the network related system calls.
- `-e trace=signal` - trace all signal related system calls.
- `-e trace=ipc` - trace all IPC related system calls.
- `-e trace=desc` - trace all file descriptor related system calls.
- `-e trace=memory` - trace all memory mapping related system calls.

</details>

<details>
<summary><b>How to remove all files except some from a directory?</b></summary><br>

Solution 1 - with <b>extglob</b>:

```
shopt -s extglob
rm !(textfile.txt|backup.tar.gz|script.php|database.sql|info.txt)
```

Solution 2 - with <b>find</b>:

```
find . -type f -not -name '*txt' -print0 | xargs -0 rm --
```

</details>

<details>
<summary><b>How to check if a string contains a substring in Bash?</b></summary><br>

You can use * (wildcards) outside a case statement, too, if you use double brackets:

```bash
string='some text'
if [[ $string = *"My long"* ]] ; then
  true
fi
```

</details>

<details>
<summary><b>How to redirect stderr and stdout to different files in the same line?</b></summary><br>

Just add them in one line <code>command 2>> error 1>> output</code>.

However, note that <code>>></code> is for appending if the file already has data. Whereas, <code>></code> will overwrite any existing data in the file.

So, <code>command 2> error 1> output</code> if you do not want to append.

Just for completion's sake, you can write <code>1></code> as just <code>></code> since the default file descriptor is the output. so <code>1></code> and <code>></code> is the same thing.

So, <code>command 2> error 1> output</code> becomes, <code>command 2> error > output</code>.

</details>

<details>
<summary><b>How to remove leading whitespace from each line in a file?</b></summary><br>

Warning: this will overwrite the original file:

```bash
sed -i "s/^[ \t]*//" filename
```

or:

```bash
sed 's/^[ \t]+//g' < input > output
```

</details>

<details>
<summary><b>How to enforce authorization methods in SSH?</b></summary><br>

Force login with a password:

```bash
ssh -o PreferredAuthentications=password -o PubkeyAuthentication=no user@remote_host
```

Force login using the key:

```bash
ssh -o PreferredAuthentications=publickey -o PubkeyAuthentication=yes -i id_rsa user@remote_host
```

</details>

<details>
<summary><b>Getting <code>Too many Open files</code> error for Postgres. How to resolve it?</b></summary><br>

Fixed the issue by reducing <code>max_files_per_process</code> e.g. to 200 from default 1000. This parameter is in <code>postgresql.conf</code> file and this sets the maximum number of simultaneously open files allowed to each server subprocess.

Usually people start to edit <code>/etc/security/limits.conf</code> file, but forget that this file only apply to the actively logged in users through the pam system.

</details>

<details>
<summary><b>In what circumstance can <code>df</code> and <code>du</code> disagree on available disk space? How do you solve it?</b></summary><br>

Solution 1:

Check for files on located under mount points. Frequently if you mount a directory (say a sambafs) onto a filesystem that already had a file or directories under it, you lose the ability to see those files, but they're still consuming space on the underlying disk.

I've had file copies while in single user mode dump files into directories that I couldn't see except in single usermode (due to other directory systems being mounted on top of them).

Solution 2:

On the other hand <code>df -h</code> and <code>du -sh</code> could mismatched by about 50% of the hard disk size. This was caused by e.g. apache (httpd) keeping large log files in memory which had been deleted from disk.

This was tracked down by running <code>lsof | grep "/var" | grep deleted</code> where <code>/var</code> was the partition I needed to clean up.

The output showed lines like this:

```
httpd     32617    nobody  106w      REG        9,4 1835222944     688166 /var/log/apache/awstats_log (deleted)
```

The situation was then resolved by restarting apache (<code>service httpd restart</code>) and cleared of disk space, by allowing the locks on deleted files to be cleared.

</details>

<details>
<summary><b>What is the difference between encryption and hashing?</b></summary><br>

<b>Hashing</b>: Finally, hashing is a form of cryptographic security which differs from <b>encryption</b>. Whereas <b>encryption</b> is a two step process used to first encrypt and then decrypt a message, <b>hashing</b> condenses a message into an irreversible fixed-length value, or hash.

</details>

<details>
<summary><b>How to log all commands run by root on production servers?</b></summary><br>

<code>auditd</code> is the correct tool for the job here:

1. Add these 2 lines to <code>/etc/audit/audit.rules</code>:

```bash
-a exit,always -F arch=b64 -F euid=0 -S execve
-a exit,always -F arch=b32 -F euid=0 -S execve
```

These will track all commands run by root (euid=0). Why two rules? The execve syscall must be tracked in both 32 and 64 bit code.

2. To get rid of <code>auid=4294967295</code> messages in logs, add <code>audit=1</code> to the kernel's cmdline (by editing <code>/etc/default/grub</code>)

3. Place the line

```bash
session  required                pam_loginuid.so
```

in all PAM config files that are relevant to login (<code>/etc/pam.d/{login,kdm,sshd}</code>), but not in the files that are relevant to su or sudo. This will allow auditd to get the calling user's uid correctly when calling sudo or su.

Restart your system now.

Let's login and run some commands:

```bash
$ id -u
1000
$ sudo ls /
bin  boot  data  dev  etc  home  initrd.img  initrd.img.old  lib  lib32  lib64  lost+found  media  mnt  opt  proc  root  run  sbin  scratch  seLinux  srv  sys  tmp  usr  var  vmlinuz  vmlinuz.old
$ sudo su -
# ls /etc
[...]
```

Now read <code>/var/log/audit/auditd.log</code> for show what has been logged in.

</details>

<details>
<summary><b>How to prevent <code>dd</code> from freezing system?</b></summary><br>

Try using ionice:

```bash
ionice -c3 dd if=/dev/zero of=z
```

This start the <code>dd</code> process with the "idle" IO priority: it only gets disk time when no other process is using disk IO for a certain amount of time.

Of course this can still flood the buffer cache and cause freezes while the system flushes out the cache to disk. There are tunables under <code>/proc/sys/vm/</code> to influence this, particularly the dirty_* entries.

</details>

<details>
<summary><b>How to limit processes to not exceed more than X% of CPU usage?</b></summary><br>

- <b>nice/renice</b>

nice is a great tool for 'one off' tweaks to a system:

`nice COMMAND`

- <b>cpulimit</b>

cpulimit if you need to run a CPU intensive job and having free CPU time is essential for the responsiveness of a system:

`cpulimit -l 50 COMMAND`

- <b>cgroups</b>

cgroups apply limits to a set of processes, rather than to just one:

```
cgcreate -g cpu:/cpulimited
cgset -r cpu.shares=512 cpulimited
cgexec -g cpu:cpulimited COMMAND_1
cgexec -g cpu:cpulimited COMMAND_2
cgexec -g cpu:cpulimited COMMAND_3
```

</details>

<details>
<summary><b>How mount a temporary ram partition?</b></summary><br>

```bash
# -t - filesystem type
# -o - mount options
mount -t tmpfs tmpfs /mnt -o size=64M
```

</details>

<details>
<summary><b>How to kills a process that is locking a file?</b></summary><br>

```bash
fuser -k filename
```

</details>

<details>
<summary><b>How to restore permission for <code>/bin/chmod</code>?</b></summary><br>

```bash
# 1:
cp /bin/ls chmod.01
cp /bin/chmod chmod.01
./chmod.01 700 file

# 2:
/bin/busybox chmod 0700 /bin/chmod

# 3:
setfacl --set u::rwx,g::---,o::--- /bin/chmod

# 4:
/usr/lib/ld*.so /bin/chmod 0700 /bin/chmod
```

</details>

<details>
<summary><b><code>grub></code> vs <code>grub-rescue></code>. Explain.</b></summary><br>

- <code>grub></code> - this is the mode to which it passes if you find everything you need to run the system in addition to the configuration file. With this mode, we have access to most (if not all) modules and commands. This mode can be called from the menu by pressing the 'c' key
- <code>grub-rescue></code> - this is the mode to which it passes if it is impossible to find its own directory (especially the directory with modules and additional commands, e.g. directory <code>/boot/grub/i386-pc</code>), if its contents are damaged or if no normal module is found, contains only basic commands

</details>

<details>
<summary><b>How to check whether the private key and the certificate match?</b></summary><br>

```bash
(openssl rsa -noout -modulus -in private.key | openssl md5 ; openssl x509 -noout -modulus -in certificate.crt | openssl md5) | uniq
```

</details>

<details>
<summary><b>How to create user without useradd command in Linux?</b></summary><br>

1. Add an entry of user details in <code>/etc/passwd</code>

```bash
# username:password:UID:GID:Comments:Home_Directory:Login Shell
user:x:501:501:test user:/home/user:/bin/bash
```

2. You will have to create a group with same name in <code>/etc/group</code>

```bash
user:x:501:
```

3. Assign a password to the user

```bash
passwd user
```

</details>

<details>
<summary><b>How profile app in Linux environment?</b></summary><br>

> Ideally, I need an app that will attach to a process and log periodic snapshots of: memory usage number of threads CPU usage.

1. You can use <code>top</code> in batch mode. It runs in the batch mode either until it is killed or until N iterations is done:

```bash
top -b -p `pidof a.out`
```

or

```bash
top -b -p `pidof a.out` -n 100
```

2. You can use ps (for instance in a shell script):

```bash
ps --format pid,pcpu,cputime,etime,size,vsz,cmd -p `pidof a.out`
```

> I need some means of recording the performance of an application on a Linux machine.

1. To record performance data:

```bash
perf record -p `pidof a.out`
```

or to record for 10 secs:

```bash
perf record -p `pidof a.out` sleep 10
```

or to record with call graph ():

```bash
perf record -g -p `pidof a.out`
```

2) To analyze the recorded data

```bash
perf report --stdio
perf report --stdio --sort=dso -g none
perf report --stdio -g none
perf report --stdio -g
```

<b>This is an example of profiling a test program</b>

1. I run my test program (c++):

```bash
./my_test 100000000
```

2. Then I record performance data of a running process:

```bash
perf record -g  -p `pidof my_test` -o ./my_test.perf.data sleep 30
```

3. Then I analyze load per module:

```bash
perf report --stdio -g none --sort comm,dso -i ./my_test.perf.data

# Overhead  Command                 Shared Object
# ........  .......  ............................
#
    70.06%  my_test  my_test
    28.33%  my_test  libtcmalloc_minimal.so.0.1.0
     1.61%  my_test  [kernel.kallsyms]
```

4. Then load per function is analyzed:

```bash
perf report --stdio -g none -i ./my_test.perf.data | c++filt

# Overhead  Command                 Shared Object                       Symbol
# ........  .......  ............................  ...........................
#
    29.30%  my_test  my_test                       [.] f2(long)
    29.14%  my_test  my_test                       [.] f1(long)
    15.17%  my_test  libtcmalloc_minimal.so.0.1.0  [.] operator new(unsigned long)
    13.16%  my_test  libtcmalloc_minimal.so.0.1.0  [.] operator delete(void*)
     9.44%  my_test  my_test                       [.] process_request(long)
     1.01%  my_test  my_test                       [.] operator delete(void*)@plt
     0.97%  my_test  my_test                       [.] operator new(unsigned long)@plt
     0.20%  my_test  my_test                       [.] main
     0.19%  my_test  [kernel.kallsyms]             [k] apic_timer_interrupt
     0.16%  my_test  [kernel.kallsyms]             [k] _spin_lock
     0.13%  my_test  [kernel.kallsyms]             [k] native_write_msr_safe

  ...
```

5. Then call chains are analyzed:

```bash
perf report --stdio -g graph -i ./my_test.perf.data | c++filt

# Overhead  Command                 Shared Object                       Symbol
# ........  .......  ............................  ...........................
#
    29.30%  my_test  my_test                       [.] f2(long)
            |
            --- f2(long)
               |
                --29.01%-- process_request(long)
                          main
                          __libc_start_main

    29.14%  my_test  my_test                       [.] f1(long)
            |
            --- f1(long)
               |
               |--15.05%-- process_request(long)
               |          main
               |          __libc_start_main
               |
                --13.79%-- f2(long)
                          process_request(long)
                          main
                          __libc_start_main

  ...
```

So at this point you know where your program spends time.

Also the simple way to do app profile is to use the <code>pstack</code> utility or <code>lsstack</code>.

Other tool is Valgrind. So this is what I recommend. Run program first:

```bash
valgrind --tool=callgrind --dump-instr=yes -v --instr-atstart=no ./binary > tmp
```

Now when it works and we want to start profiling we should run in another window:

```bash
callgrind_control -i on
```

This turns profiling on. To turn it off and stop whole task we might use:

```bash
callgrind_control -k
```

Now we have some files named callgrind.out.* in current directory. To see profiling results use:

```bash
kcachegrind callgrind.out.*
```

I recommend in next window to click on "Self" column header, otherwise it shows that "main()" is most time consuming task.

</details>


<details>
<summary><b>What is the easiest, safest and most portable way to remove <code>-rf</code> directory entry?</b></summary><br>

They're effective but not optimally portable:

- <code>rm -- -fr</code>
- <code>perl -le 'unlink("-fr");'</code>

People who go on about shell command line quoting and character escaping are almost as dangerous as those who simply don't even recognize why a file name like that poses any problem at all.

The most portable solution:

```bash
rm ./-fr
```

</details>

<details>
<summary><b>Write a simple bash script (or pair of scripts) to backup and restore your system. *</b></summary><br>

To be completed.

</details>

###### Network Questions

<details>
<summary><b>Create SPF records for your site to help control spam. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is the difference between an authoritative and a nonauthorita-
tive answer to a DNS query? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Explore the current MTA configuration at your site. What are some of the special features of the MTA that are in use? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Use tcpdump to capture FTP traffic for both active and passive FTP
sessions. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>Does having Varnish in front of your website/app mean you don't need to care about load balancing or redundancy? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What are hits, misses, and hit-for-pass in Varnish Cache?</b></summary><br>

A hit is a request which is successfully served from the cache, a miss is a request that goes through the cache but finds an empty cache and therefore has to be fetched from the origin, the hit-for-pass comes in when Varnish Cache realizes that one of the objects it has requested is uncachable and will result in a pass.

Useful resources:

- [VCL rules for hits](https://book.varnish-software.com/4.0/chapters/VCL_Subroutines.html#vcl-vcl-hit)
- [VCL rules for hit-for-pass](https://book.varnish-software.com/4.0/chapters/VCL_Subroutines.html#hit-for-pass)
- [Example of the use](https://book.varnish-software.com/4.0/chapters/VCL_Basics.html#vcl-backend-response)

</details>

<details>
<summary><b>What's a reasonable TTL for cached content given the following parameters? *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>How do you kill program using one port in Linux?</b></summary><br>

To list any process listening to the port 8080:<br>

<code>lsof -i:8080</code>

To kill any process listening to the port 8080:<br>

<code>kill $(lsof -t -i:8080)</code>

or more violently:<br>

<code>kill -9 $(lsof -t -i:8080)</code><br><br>

</details>

<details>
<summary><b>How to test connection with OpenSSL to remote host (with and without SNI)?</b></summary><br>

With <b>OpenSSL</b>:

```bash
# Testing connection to remote host (with SNI support)
echo | openssl s_client -showcerts -servername google.com -connect google.com:443
# Testing connection to remote host (without SNI support)
echo | openssl s_client -connect google.com:443 -showcerts
```

With <b>GnuTLS</b>:

```bash
# Testing connection to remote host (with SNI support)
gnutls-cli -p 443 google.com
# Testing connection to remote host (without SNI support)
gnutls-cli --disable-sni -p 443 google.com
```

</details>

<details>
<summary><b>How are cookies passed in the HTTP protocol?</b></summary><br>

The server sends the following in its response header to set a cookie field:

`Set-Cookie:name=value`

If there is a cookie set, then the browser sends the following in its request header:

`Cookie:name=value`

</details>

<details>
<summary><b>What is the proper way to test NFS performance?
</b></summary><br>

The best benchmark is always "the application(s) that you normally use". The load on a NFS system when you have 20 people simultaneously compiling a Linux kernel is comletely different from a bunch of people logging in at the same time or the accounts uses as "home directories for the local web-server".

But we have some good tools for testing this.

- <b>boonie</b> - a classical performances evaluation tool tests. The main program tests database type access to a single file (or a set of files if you wish to test more than 1G of storage), and it tests creation, reading, and deleting of small files which can simulate the usage of programs such as Squid, INN, or Maildir format email.
- <b>DBench</b> - was written to allow independent developers to debug and test SAMBA. It is heavily inspired of the original SAMBA tool.
- <b>IOZone</b> - performance tests suite. POSIX and 64 bits compliant. This tests is the file system test from the L.S.E. Main features: POSIX async I/O, Mmap() file I/O, Normal file I/O Single stream measurement, Multiple stream measurement, Distributed file server measurements (Cluster) POSIX pthreads, Multi-process measurement Selectable measurements with fsync, O_SYNC Latency plots.

</details>

<details>
<summary><b>How to run <code>scp</code> with a second remote host?</b></summary><br>

With <b>ssh</b>:

```bash
ssh user1@remote1 'ssh user2@remote2 "cat file"' > file
```

With <b>tar</b> (with compression):

```bash
ssh user1@remote1 'ssh user2@remote2 "cd path2; tar cj file"' | tar xj
```

With <b>ssh</b> and port forwarding tunnel:

```bash
# First, open the tunnel
ssh -L 1234:remote2:22 -p 45678 user1@remote1
# Then, use the tunnel to copy the file directly from remote2
scp -P 1234 user2@localhost:file .
```

</details>

<details>
<summary><b>How can you reduce load time of a dynamic website?</b></summary><br>

- webpage optimization
- cached web pages
- quality web hosting
- compressed text files
- apache/nginx tuning

</details>

<details>
<summary><b>Explain difference between HTTP 1.1 and HTTP 2.0.</b></summary><br>

<b>HTTP/2</b> supports queries multiplexing, headers compression, priority and more intelligent packet streaming management. This results in reduced latency and accelerates content download on modern web pages.

Key differences with HTTP/1.1:

- it is binary, instead of textual
- fully multiplexed, instead of ordered and blocking
- can therefore use one connection for parallelism
- uses header compression to reduce overhead
- allows servers to “push” responses proactively into client caches

</details>

<details>
<summary><b>What's the difference between <code>Cache-Control: max-age=0</code> and <code>no-cache</code>?</b></summary><br>

When sent by the origin server:

<code>max-age=0</code> simply tells caches (and user agents) the response is stale from the get-go and so they SHOULD revalidate the response (e.g. with the If-Not-Modified header) before using a cached copy, whereas, <code>no-cache</code> tells them they MUST revalidate before using a cached copy.

In other words, caches may sometimes choose to use a stale response (although I believe they have to then add a Warning header), but <code>no-cache</code> says they're not allowed to use a stale response no matter what. Maybe you'd want the SHOULD-revalidate behavior when baseball stats are generated in a page, but you'd want the MUST-revalidate behavior when you've generated the response to an e-commerce purchase.

When sent by the user agent:

If a user agent sends a request with <code>Cache-Control: max-age=0</code> (aka. "end-to-end revalidation"), then each cache along the way will revalidate its cache entry (e.g. with the If-Not-Modified header) all the way to the origin server. If the reply is then 304 (Not Modified), the cached entity can be used.

On the other hand, sending a request with <code>Cache-Control: no-cache</code> (aka. "end-to-end reload") doesn't revalidate and the server MUST NOT use a cached copy when responding.

</details>

<details>
<summary><b>What are the security risks of setting <code>Access-Control-Allow-Origin</code>?</b></summary><br>

By responding with <code>Access-Control-Allow-Origin: *</code>, the requested resource allows sharing with every origin. This basically means that any site can send an XHR request to your site and access the server’s response which would not be the case if you hadn’t implemented this CORS response.

So any site can make a request to your site on behalf of their visitors and process its response. If you have something implemented like an authentication or authorization scheme that is based on something that is automatically provided by the browser (cookies, cookie-based sessions, etc.), the requests triggered by the third party sites will use them too.

</details>

<details>
<summary><b>Create a single-use TCP or UDP proxy with Netcat.</b></summary><br>

```bash
### TCP -> TCP
nc -l -p 2000 -c "nc [ip|hostname] 3000"

### TCP -> UDP
nc -l -p 2000 -c "nc -u [ip|hostname] 3000"

### UDP -> UDP
nc -l -u -p 2000 -c "nc -u [ip|hostname] 3000"

### UDP -> TCP
nc -l -u -p 2000 -c "nc [ip|hostname] 3000"
```

</details>

<details>
<summary><b>Explain 3 techniques for Avoiding Firewalls with Nmap.</b></summary><br>

1. Use Decoy addresses

```bash
# Generates a random number of decoys.
nmap -D RND:10 [target]
# Manually specify the IP addresses of the decoys.
nmap -D decoy1,decoy2,decoy3
```

In this type of scan you can instruct Nmap to spoof packets from other hosts.In the firewall logs it will be not only our IP address but also and the IP addresses of the decoys so it will be much harder to determine from which system the scan started.

2. Source port number specification

```bash
nmap --source-port 53 [target]
```

A common error that many administrators are doing when configuring firewalls is to set up a rule to allow all incoming traffic that comes from a specific port number.The <code>--source-port</code> option of Nmap can be used to exploit this misconfiguration.Common ports that you can use for this type of scan are: 20, 53 and 67.

3. Append Random Data

```bash
nmap --data-length 25 [target]
```

Many firewalls are inspecting packets by looking at their size in order to identify a potential port scan.This is because many scanners are sending packets that have specific size.In order to avoid that kind of detection you can use the command <code>--data-length</code> to add additional data and to send packets with different size than the default.

4. TCP ACK Scan

```bash
nmap -sA [target]
```

It is always good to send the ACK packets rather than the SYN packets because if there is any active firewall working on the remote computer then because of the ACK packets the firewall cannot create the log, since firewalls treat ACK packet as the response of the SYN packet.

</details>

<details>
<summary><b>What does a Tcpdump do? How to capture only incoming traffic to your interface?</b></summary><br>

<code>tcpdump</code> is a most powerful and widely used command-line packets sniffer or package analyzer tool which is used to capture or filter TCP/IP packets that received or transferred over a network on a specific interface.

<code>tcpdump</code> puts your network card into promiscuous mode, which basically tells it to accept every packet it receives. It allows the user to see all traffic being passed over the network. Wireshark uses pcap to capture packets.

If you want to view only packets that come to your interface you should:

- <code>-Q in</code> - for Linux <code>tcpdump</code> version
- <code>-D in</code> - for BSD <code>tcpdump</code> version

Both params set send/receive direction direction for which packets should be captured.

```bash
tcpdump -nei eth0 -Q in host 192.168.252.125 and port 8080
```

</details>

###### Devops Questions

<details>
<summary><b>Explain how Flap Detection works in Nagios?</b></summary><br>

Flapping occurs when a service or host changes state too frequently, this causes lot of problem and recovery notifications.

Once you have defined Flapping, explain how Nagios detects Flapping. Whenever Nagios checks the status of a host or service, it will check to see if it has started or stopped flapping.

Nagios follows the below given procedure to do that:

- storing the results of the last 21 checks of the host or service analyzing the historical check results and determine where state changes/transitions occur
- using the state transitions to determine a percent state change value (a measure of change) for the host or service
- comparing the percent state change value against low and high flapping thresholds

</details>

<details>
<summary><b>What are the advantages that Containerization provides over Virtualization?</b></summary><br>

Below are the advantages of containerization over virtualization:

- containers provide real-time provisioning and scalability but VMs provide slow provisioning
- containers are lightweight when compared to VMs
- VMs have limited performance when compared to containers
- containers have better resource utilization compared to VMs

</details>

###### Cyber Security Questions

<details>
<summary><b>What is OWASP Application Security Verification Standard? Explain in a few points. *</b></summary><br>

To be completed.

</details>

<details>
<summary><b>What is CSRF?</b></summary><br>

<b>Cross Site Request Forgery</b> is a web application vulnerability in which the server does not check whether the request came from a trusted client or not. The request is just processed directly. It can be further followed by the ways to detect this, examples and countermeasures.

</details>

<details>
<summary><b>What is the difference between policies, processes and guidelines?</b></summary><br>

As <b>security policy</b> defines the security objectives and the security framework of an organisation. A <b>process</b> is a detailed step by step how to document that specifies the exact action which will be necessary to implement important security mechanism. <b>Guidelines</b> are recommendations which can be customised and used in the creation of procedures.

</details>

<details>
<summary><b>What is a false positive and false negative in case of IDS?</b></summary><br>

When the device generated an alert for an intrusion which has actually not happened: this is <b>false positive</b> and if the device has not generated any alert and the intrusion has actually happened, this is the case of a <b>false negative</b>.

</details>

<details>
<summary><b>5 quick points on Web server hardening?</b></summary><br>

Web server hardening is filtering of unnecessary services running on various ports and removal of default test scripts from the servers. Although web server hardening is a lot more than this and usually organisations have a customised checklist for hardening the servers. Any server getting created has to be hardened and hardening has to be re-confirmed on a yearly basis. Even the hardening checklist has to be reviewed on a yearly basis for new add-ons.

Example:

- if machine is a new install, protect it from hostile network traffic, until the operating system is installed and hardened
- create a separate partition with the <code>nodev</code>, <code>nosuid</code>, and <code>noexec</code> options set for <code>/tmp</code>
- create separate partitions for <code>/var</code>, <code>/var/log</code>, <code>/var/log/audit</code>, and <code>/home</code>
- enable randomized virtual memory region placement
- remove legacy services (e.g., telnet-server; rsh, rlogin, rcp; ypserv, ypbind; tftp, tftp-server; talk, talk-server).
- limit connections to services running on the host to authorized users of the service via firewalls and other access control technologies
- disable source routed packet acceptance
- enable TCP/SYN cookies
- disable SSH root login
- install and configure AIDE
- install and configure OSsec HIDS
- configure SELinux
- all administrator or root access must be logged
- integrity checking of system accounts, group memberships, and their associated privileges should be enabled and tested
- set password creation requirements

</details>

## <a name="secret-knowledge">Secret Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="guru-sysadmin">Guru Sysadmin</a>

<details>
<summary><b>Why do we need <code>mktemp</code> command? Present an example of use.</b></summary><br>

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
<summary><b>Use sysfs virtual filesystem to test connection on all interfaces (without loopback).</b></summary><br>

For example:

```bash
#!/usr/bin/bash

for iface in $(ls /sys/class/net/ | grep -v lo) ; do

  if [[ $(cat /sys/class/net/$iface/carrier) = 1 ]] ; then state=1 ; fi

done

if [[ $state -ne 0 ]] ; then echo "not connection" > /dev/stderr ; exit ; fi
```

</details>

<details>
<summary><b>Explain Varnish Cache SHM Log (pooling mechanism).</b></summary><br>

Every poll is recorded in the shared memory log as follows:

```bash
0 Backend_health - b0 Still healthy 4--X-S-RH 9 8 10 0.029291 0.030875 HTTP/1.1 200 Ok
```

The fields are:

- 0 - Constant
- Backend_health - Log record tag
- '-' client/backend indication (XXX: wrong! should be 'b')
- b0 - Name of backend (XXX: needs qualifier)
- two words indicating state:
  - "Still healthy"
  - "Still sick"
  - "Back healthy"
  - "Went sick"

Notice that the second word indicates present state, and the first word == "Still" indicates unchanged state.

- 4--X-S-RH - Flags indicating how the latest poll went
  - 4 - IPv4 connection established
  - 6 - IPv6 connection established
  - x - Request transmit failed
  - X - Request transmit succeeded
  - s - TCP socket shutdown failed
  - S - TCP socket shutdown succeeded
  - r - Read response failed
  - R - Read response succeeded
  - H - Happy with result
- 9 - Number of good polls in the last .window polls
- 8 - .threshold (see above)
- 10 - .window (see above)
- 0.029291 - Response time this poll or zero if it failed
- 0.030875 - Exponential average (r=4) of responsetime for good polls.
- HTTP/1.1 200 Ok - The HTTP response from the backend.

</details>

<details>
<summary><b>How to rewrite POST data with Payload in Nginx?</b></summary><br>

You just need to write a Nginx rewrite rule with HTTP status code <b>307</b> or <b>308</b>:

```bash
location / {
    proxy_pass              http://localhost:80;
    client_max_body_size    10m;
}

location /api {
    # HTTP 307 only for POST method.
    if ($request_method = POST) {
        return 307 https://api.example.com?request_uri;
    }

    # You can keep this for non-POST requests.
    rewrite ^ https://api.example.com?request_uri permanent;

    client_max_body_size    10m;
}
```

HTTP Status code 307 or 308 should be used instead of 301 because it changes the request method from POST to GET.

</details>

<details>
<summary><b>Developer reports a problem with connectivity to the remote service. Use <code>/dev</code> for troubleshooting.</b></summary><br>

```bash
# <host> - set remote host
# <port> - set destination port

# 1
timeout 1 bash -c "</dev/tcp/<host>/<port>" >/dev/null 2>&1 ; echo $?

# 2
timeout 1 bash -c 'cat < /dev/null > </dev/tcp/<host>/<port>' ; echo $?

# 2
&> echo > "</dev/tcp/<host>/<port>"
```

Useful resources:

- [Advanced Bash-Scripting Guide - /dev](http://www.tldp.org/LDP/abs/html/devref1.html#DEVTCP)
- [/dev/tcp as a weapon](https://securityreliks.wordpress.com/2010/08/20/devtcp-as-a-weapon/)
- [Test from shell script if remote TCP port is open](https://stackoverflow.com/questions/4922943/test-from-shell-script-if-remote-tcp-port-is-open)

</details>

<details>
<summary><b>How do I measure request and response times at once using cURL?</b></summary><br>

cURL supports formatted output for the details of the request (see the cURL manpage for details, under <code>-w| -write-out 'format'</code>). For our purposes we’ll focus just on the timing details that are provided.

1. Create a new file, curl-format.txt, and paste in:

```bash
    time_namelookup:  %{time_namelookup}\n
       time_connect:  %{time_connect}\n
    time_appconnect:  %{time_appconnect}\n
   time_pretransfer:  %{time_pretransfer}\n
      time_redirect:  %{time_redirect}\n
 time_starttransfer:  %{time_starttransfer}\n
                    ----------\n
         time_total:  %{time_total}\n
```

2. Make a request:

```bash
curl -w "@curl-format.txt" -o /dev/null -s "http://example.com/"
```

What this does:

- <code>-w "@curl-format.txt"</code> - tells cURL to use our format file
- <code>-o /dev/null</code> - redirects the output of the request to /dev/null
- <code>-s</code> - tells cURL not to show a progress meter
<code>http://example.com/</code> is the URL we are requesting. Use quotes particularly if your URL has "&" query string parameters

</details>

<details>
<summary><b>Is there a way to allow multiple cross-domains using the Access-Control-Allow-Origin header in Nginx?</b></summary><br>

To match a list of domain and subdomain this regex make it ease to work with fonts:

```bash
location ~* \.(?:ttf|ttc|otf|eot|woff|woff2)$ {
   if ( $http_origin ~* (https?://(.+\.)?(domain1|domain2|domain3)\.(?:me|co|com)$) ) {
      add_header "Access-Control-Allow-Origin" "$http_origin";
   }
}
```

More sligtly configuration:

```bash
location / {

    if ($http_origin ~* (^https?://([^/]+\.)*(domainone|domaintwo)\.com$)) {
        set $cors "true";
    }

    # Nginx doesn't support nested If statements. This is where things get slightly nasty.
    # Determine the HTTP request method used
    if ($request_method = 'GET') {
        set $cors "${cors}get";
    }
    if ($request_method = 'POST') {
        set $cors "${cors}post";
    }

    if ($cors = "true") {
        # Catch all incase there's a request method we're not dealing with properly
        add_header 'Access-Control-Allow-Origin' "$http_origin";
    }

    if ($cors = "trueget") {
        add_header 'Access-Control-Allow-Origin' "$http_origin";
        add_header 'Access-Control-Allow-Credentials' 'true';
        add_header 'Access-Control-Allow-Methods' 'GET, POST, OPTIONS';
        add_header 'Access-Control-Allow-Headers' 'DNT,X-CustomHeader,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type';
    }

    if ($cors = "truepost") {
        add_header 'Access-Control-Allow-Origin' "$http_origin";
        add_header 'Access-Control-Allow-Credentials' 'true';
        add_header 'Access-Control-Allow-Methods' 'GET, POST, OPTIONS';
        add_header 'Access-Control-Allow-Headers' 'DNT,X-CustomHeader,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type';
    }

}
```

</details>

<details>
<summary><b>Explain <code>:(){ :|:& };:</code> and how stop this code if you are already logged into a system?</b></summary><br>

It's a fork bomb.

- <code>:()</code> - this defines the function. ":"" is the function name and the empty parenthesis shows that it will not accept any arguments
- <code>{ }</code> - these characters shows the beginning and end of function definition
- <code>:|:</code> - it loads a copy of the function ":: into memory and pipe its output to another copy of the ":" function, which has to be loaded into memory
- <code>&</code> - this will make the process as a background process, so that the child processes will not get killed eventhough the parent gets auto-killed
- <code>:</code> - final ":" will execute the function again and hence the chain reaction begins

The best way to protect a multi-user system is to use PAM to limit the number of processes a user can use. We know the biggest problem with a fork bomb is the fact it takes up so many processes.

So we have two ways of attempting to fix this, if you are already logged into the system:
- execute a SIGSTOP command to stop the process: <code>killall -STOP -u user1</code>
- if you can't run at the command line you will have to use <code>exec</code> to force it to run (due to processes all being used): <code>exec killall -STOP -u user1</code>

With fork bombs your best method for this is preventing from being to big of an issue in the first place.

</details>

<details>
<summary><b>How to recover deleted file held open by Apache?</b></summary><br>

If a file has been deleted but is still open, that means the file still exists in the filesystem (it has an inode) but has a hard link count of 0. Since there is no link to the file, you cannot open it by name. There is no facility to open a file by inode either.

Linux exposes open files through special symbolic links under <code>/proc</code>. These links are called <code>/proc/12345/fd/42</code> where 12345 is the PID of a process and 42 is the number of a file descriptor in that process. A program running as the same user as that process can access the file (the read/write/execute permissions are the same you had as when the file was deleted).

The name under which the file was opened is still visible in the target of the symbolic link: if the file was <code>/var/log/apache/foo.log</code>, then the target of the link is <code>/var/log/apache/foo.log (deleted)</code>.

Thus you can recover the content of an open deleted file given the PID of a process that has it open and the descriptor that it's opened on like this:

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

If you only know the process ID but not the descriptor, you can recover all files with:

```bash
for x in /proc/$pid/fd/* ; do
  recover_open_deleted_file "$x"
done
```

If you don't know the process ID either, you can search among all processes:

```bash
for x in /proc/[1-9]*/fd/* ; do
  case $(readlink "$x") in
    /var/log/apache/*) recover_open_deleted_file "$x";;
  esac
done
```

You can also obtain this list by parsing the output of lsof, but it isn't simpler nor more reliable nor more portable (this is Linux-specific anyhow).

</details>

<details>
<summary><b>How to install Linux on disk, from and where other Linux exist and running?</b></summary><br>

It is possible that the question should be: "<i>System installation from the level and in place of already other system working</i>".

On the example of the Debian GNU/Linux distribution.

1. Creating a working directory and downloading the system using the debootstrap tool.

```bash
_working_directory="/mnt/system"
mkdir $_working_directory
debootstrap --verbose --arch amd64 {wheezy|jessie} . http://ftp.en.debian.org/debian
```

2. Mounting sub-systems: <code>proc</code>, <code>sys</code>, <code>dev</code> and <code>dev/pts</code>.

```bash
for i in proc sys dev dev/pts ; do mount -o bind $i $_working_directory/$i ; done
```

3. Copy system backup for restore.

```bash
cp system_backup_22012015.tgz $_working_directory/mnt
```

However, it is better not to waste space and do it in a different way (assuming that the copy is in <code>/mnt/backup</code>):

```bash
_backup_directory="${_working_directory}/mnt/backup"
mkdir $_backup_directory && mount --bind /mnt/backup $_backup_directory
```

4. Chroot to "new" system.

```bash
chroot $_working_directory /bin/bash
```

5. Updating information about mounted devices.

```bash
grep -v rootfs /proc/mounts > /etc/mtab
```

6. In the "new" system, the next thing to do is mount the disk on which the "old" system is located (e.g. <code>/dev/sda1</code>).

```bash
_working_directory="/mnt/old_system"
_backup_directory="/mnt/backup"
mkdir $_working_directory && mount /dev/sda1 $_working_directory
```

7. Remove all files of the old system.

```bash
for i in $(ls | awk '!(/proc/ || /dev/ || /sys/ || /mnt/)') ; do rm -fr $i ; done
```

8. The next step is to restore the system from a backup.

```bash
tar xzvfp $_backup_directory/system_backup_22012015.tgz -C $_working_directory
```

9. And mount <code>proc</code>, <code>sys</code>, <code>dev</code> and <code>dev/pts</code> in a new working directory.

```bash
for i in proc sys dev dev/pts ; do mount -o bind $i $_working_directory/$i ; done
```

10. Install and update grub configuration.

```bash
chroot $_working_directory /bin/bash -c "grub-install --no-floppy --root-directory=/ /dev/sda"
chroot $_working_directory /bin/bash -c "update-grub"
```

11. Unmount <code>proc</code>, <code>sys</code>, <code>dev</code> and <code>dev/pts</code> filesystems.

```bash
cd
grep $_working_directory /proc/mounts | cut -f2 -d " " | sort -r | xargs umount -n
```

None of the available commands, i.e. <code>halt</code>, <code>shutdown</code> or <code>reboot</code>, will work. You need to reload the system configuration - to do this, use the <b>kernel debugger</b> (without the 'b' option):

```bash
echo 1 > /proc/sys/kernel/sysrq
echo reisu > /proc/sysrq-trigger
```

Of course, it is recommended to fully restart the machine in order to completely load the current system. To do this:

```bash
sync ; reboot -f
```

</details>

<details>
<summary><b>How does the OOM killer decide which process to kill first? How to control this?</b></summary><br>

Major distribution kernels set the default value of <code>/proc/sys/vm/overcommit_memory</code> to zero, which means that processes can request more memory than is currently free in the system.

If memory is exhaustively used up by processes, to the extent which can possibly threaten the stability of the system, then the <b>OOM killer</b> comes into the picture.

NOTE: It is the task of the OOM Killer to continue killing processes until enough memory is freed for the smooth functioning of the rest of the process that the Kernel is attempting to run.

The OOM Killer has to select the best process(es) to kill. Best here refers to that process which will free up the maximum memory upon killing and is also the least important to the system.

The primary goal is to kill the least number of processes that minimizes the damage done and at the same time maximizing the amount of memory freed.

To facilitate this, the kernel maintains an <code>oom_score</code> for each of the processes. You can see the oom_score of each of the processes in the /proc filesystem under the pid directory.

```bash
cat /proc/10292/oom_score
```

The higher the value of <code>oom_score</code> of any process, the higher is its likelihood of getting killed by the OOM Killer in an out-of-memory situation.

If you want to create a special control group containing the list of processes which should be the first to receive the OOM killer's attention, create a directory under <code>/mnt/oom-killer</code> to represent it:

```bash
mkdir lambs
```

Set <code>oom.priority</code> to a value high enough:

```bash
echo 256 > /mnt/oom-killer/lambs/oom.priority
```

<code>oom.priority</code> is a 64-bit unsigned integer, and can have a maximum value an nsigned 64-bit number can hold. While scanning for the process to be killed, the OOM-killer selects a process from the list of tasks with the highest <code>oom.priority</code> value.

Add the PID of the process to be added to the list of tasks:

```bash
echo <pid> > /mnt/oom-killer/lambs/tasks
```

To create a list of processes, which will not be killed by the OOM-killer, make a directory to contain the processes:

```bash
mkdir invincibles
```

Setting <code>oom.priority</code> to zero makes all the process in this cgroup to be excluded from the list of target processes to be killed.

```bash
echo 0 > /mnt/oom-killer/invincibles/oom.priority
```

To add more processes to this group, add the pid of the task to the list of tasks in the invincible group:

```bash
echo <pid> > /mnt/oom-killer/invincibles/tasks
```

</details>

<details>
<summary><b>What are salted hashes? Generate the password with salt for the <code>/etc/shadow</code> file.</b></summary><br>

<b>Salt</b> at its most fundamental level is random data. When a properly protected password system receives a new password, it will create a hashed value for that password, create a new random salt value, and then store that combined value in its database. This helps defend against dictionary attacks and known hash attacks.

For example, if a user uses the same password on two different systems, if they used the same hashing algorithm, they could end up with the same hash value. However, if even one of the systems uses salt with its hashes, the values will be different.

The encrypted passwords in <code>/etc/shadow</code> file are stored in the following format:

```bash
$ID$SALT$ENCRYPTED
```

The <code>$ID</code> indicates the type of encryption, the <code>$SALT</code> is a random (up to 16 characters) string and <code>$ENCRYPTED</code> is a password’s hash.

<table style="width:100%">
  <tr>
    <th>Hash Type</th>
    <th>ID</th>
    <th>Hash Length</th>
  </tr>
  <tr>
    <td>MD5</td>
    <td>$1</td>
    <td>22 characters</td>
  </tr>
  <tr>
    <td>SHA-256</td>
    <td>$5</td>
    <td>43 characters</td>
  </tr>
  <tr>
    <td>SHA-512</td>
    <td>$6</td>
    <td>86 characters</td>
  </tr>
</table>

Use the below commands from the Linux shell to generate hashed password for <code>/etc/shadow</code> with the random salt:

- Generate <b>MD5</b> password hash

```bash
python -c "import random,string,crypt; randomsalt = ''.join(random.sample(string.ascii_letters,8)); print crypt.crypt('MySecretPassword', '\$1\$%s\$' % randomsalt)"
```

- Generate <b>SHA-256</b> password hash

```bash
python -c "import random,string,crypt; randomsalt = ''.join(random.sample(string.ascii_letters,8)); print crypt.crypt('MySecretPassword', '\$5\$%s\$' % randomsalt)"
```

- Generate <b>SHA-512</b> password hash

```bash
python -c "import random,string,crypt; randomsalt = ''.join(random.sample(string.ascii_letters,8)); print crypt.crypt('MySecretPassword', '\$6\$%s\$' % randomsalt)"
```

</details>
